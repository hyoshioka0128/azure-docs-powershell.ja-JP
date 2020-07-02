---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 05/28/2020
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 4b40a3aebab84176a48bcdb0ef818cfa05dea269
ms.sourcegitcommit: 5523170e571fbd1dc93bd0fa4223aba3b324d3b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2020
ms.locfileid: "85363364"
---
# <a name="uninstall-the-azure-powershell-module"></a>Azure PowerShell モジュールのアンインストール

この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。 Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用してフィードバックをお送りください。 バグが見つかった場合は、修正できるようにするため、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。

## <a name="uninstall-azure-powershell-from-msi"></a>MSI からの Azure PowerShell をアンインストールする

MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。

|         プラットフォーム         |                      Instructions                      |
| ------------------------ | ------------------------------------------------------ |
| Windows 10               | [スタート] > [設定] > [アプリ]                                |
| Windows 7 </br>Windows 8 | [スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール] |

この画面のプログラムの一覧に **[Azure PowerShell]** が表示されます。 これが、アンインストール対象のアプリです。 このプログラムが一覧に表示されていない場合は、PowerShellGet を介してインストールされています。この場合は、次の一連の手順に従います。

## <a name="uninstall-azure-powershell-from-powershellget"></a>PowerShellGet から Azure PowerShell をアンインストールする

Az モジュールをアンインストールするために、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用できます。 ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。 Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。 複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。

インストールされている Azure PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
3.8.0               Az                             PSGallery            Microsoft Azure PowerShell
4.1.0               Az                             PSGallery            Microsoft Azure PowerShell
```

<a name="uninstall-script"/>

次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。 次に、各サブモジュールの適切なバージョンがアンインストールされます。 **Process** または **CurrentUser**.以外のスコープでこのスクリプトを実行するには、管理者アクセス権が必要です。

```powershell-interactive
function Uninstall-AzModule {
  [CmdletBinding(SupportsShouldProcess)]
  param(
    [ValidateNotNullOrEmpty()]
    [ValidateSet('Az','AzureRM','Azure')]
    [string]$Name = 'Az',

    [Parameter(Mandatory)]
    [string]$Version,

    [switch]$AllowPrerelease
  )

  $Params = @{}

  if ($PSBoundParameters.AllowPrerelease) {
    $Params.AllowPrerelease = $true
  }

  $IsAdmin = ([Security.Principal.WindowsPrincipal] [Security.Principal.WindowsIdentity]::GetCurrent()).IsInRole([Security.Principal.WindowsBuiltInRole] 'Administrator')

  if (-not(Get-InstalledModule -Name $Name -RequiredVersion $Version -ErrorAction SilentlyContinue -OutVariable RootModule @Params)) {

    Write-Warning -Message "Uninstall aborted. $Name version $Version not found."

  } elseif (($RootModule.InstalledLocation -notlike "*$env:USERPROFILE*") -and ($IsAdmin -eq $false)) {

    Write-Warning -Message "Uninstall aborted. $Name version $Version exists in a system path. PowerShell must be run elevated as an admin to remove it."

  } elseif ((Get-Process -Name powershell, pwsh -OutVariable Sessions -ErrorAction SilentlyContinue).Count -gt 1) {

    Write-Warning -Message "Uninstall aborted. Please close all other PowerShell sessions before continuing. There are currently $($Sessions.Count) PowerShell sessions running."

  } else {
    Write-Verbose -Message 'Creating list of dependencies...'
    $target = Find-Module -Name $Name -RequiredVersion $Version @Params

    $AllModules = @([pscustomobject]@{
      Name = $Name
      Version = $Version
    })

    $AllModules += foreach ($dependency in $target.Dependencies) {
      switch ($dependency.keys) {
        {$_ -contains 'RequiredVersion'} {$UninstallVersion = $dependency.RequiredVersion; break}
        {$_ -contains 'MinimumVersion'} {$UninstallVersion = $dependency.MinimumVersion; break}
      }

      [pscustomobject]@{
        Name = $dependency.Name
        Version = $UninstallVersion
      }
    }

    [int]$i = 100 / $AllModules.Count

    foreach ($module in $AllModules) {
      Write-Progress -Activity 'Uninstallation in Progress' -Status "$i% Complete:" -PercentComplete $i
      $i++

      if (Get-InstalledModule -Name $module.Name -RequiredVersion $module.Version -ErrorAction SilentlyContinue @Params) {
        Write-Verbose -Message "Uninstalling $($module.Name) version $($module.Version)"

        Remove-Module -FullyQualifiedName @{ModuleName=$module.Name;ModuleVersion=$module.Version} -ErrorAction SilentlyContinue

        try {
          if ($PSCmdlet.ShouldProcess("$($module.Name) version $($module.Version)")) {
            Uninstall-Module -Name $module.Name -RequiredVersion $module.Version -Force -ErrorAction Stop @Params
          }
          $State = 'Uninstalled'
        } Catch {
          $State = 'Manual uninstall required'
          Write-Verbose -Message "$($module.Name) version: $($module.Version) may require manual uninstallation."
        }

      } else {
        $State = 'Not found'
        Write-Verbose -Message "$($module.Name) version: $($module.Version) not found."
      }

      if (-not $PSBoundParameters.WhatIf) {
        [pscustomobject]@{
          ModuleName = $module.Name
          Version = $module.Version
          State = $State
        }
      }

    }
  }
}
```

この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。 次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。

```powershell-interactive
Uninstall-AzModule -Name Az -Version 1.8.0
```

スクリプトを実行すると、アンインストールされる各サブモジュールの**名前**、**バージョン**、および**状態**が表示されます。 スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` パラメーターを指定します。

```output
ModuleName              Version  State
----------              -------  -----
Az.Accounts             1.5.1    Not found
Az.Aks                  1.0.1    Uninstalled
Az.AnalysisServices     1.1.0    Uninstalled
Az.ApiManagement        1.0.0    Uninstalled
Az.ApplicationInsights  1.0.0    Uninstalled
...
```

> [!IMPORTANT]
> このスクリプトは、アンインストールするのと同じバージョンの依存関係を正確に突き合わせることができない場合、その依存関係の "_どの_" バージョンもアンインストールしません。 これは、これらの依存関係に依存する他のバージョンのターゲット モジュールがシステム上に存在する可能性があるためです。

アンインストールする Azure PowerShell のすべてのバージョンに対して次の例を実行します。 便宜上、次のスクリプトにより、最新バージョンを**除く**、Az のすべてのバージョンがアンインストールされます。

```powershell-interactive
$Modules = Get-InstalledModule -Name Az -AllVersions | 
    Sort-Object -Property Version -Descending | 
        Select-Object -Skip 1
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```

## <a name="uninstall-the-azurerm-module"></a>AzureRM モジュールをアンインストールする

Az モジュールがシステムにインストールされていて、AzureRM をアンインストールする場合は、上記の `Uninstall-AzModule` スクリプトを実行する必要のない方法が 2 つあります。 AzureRM モジュールをインストールした方法に応じて、実行する方法は異なります。 元のインストール方法が不明な場合は、まず、MSI をアンインストールするための手順に従います。

### <a name="uninstall-azure-powershell-msi"></a>Azure PowerShell MSI のアンインストール

MSI パッケージを使用して Azure PowerShell AzureRM モジュールをインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。

|         プラットフォーム         |                      Instructions                      |
| ------------------------ | ------------------------------------------------------ |
| Windows 10               | [スタート] > [設定] > [アプリ]                                |
| Windows 7 </br>Windows 8 | [スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール] |

この画面のプログラムの一覧に **[Azure PowerShell]** または **[Azure PowerShell - 月年]** が表示されます。 これが、アンインストール対象のアプリです。 このプログラムが一覧に表示されていない場合は、PowerShellGet を介してインストールされています。この場合は、次の一連の手順に従います。

### <a name="uninstall-from-powershell"></a>PowerShell からのアンインストール

PowerShellGet を使用して AzureRM をインストールした場合は、`Az.Accounts` モジュールの一部として使用可能な [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) コマンドレットでモジュールを削除できます。 次の例では、"_すべて_" の AzureRM モジュールがマシンから削除されます。ただし、管理者特権が必要です。

```powershell-interactive
Uninstall-AzureRm
```

`Uninstall-AzureRM` コマンドを正常に実行できない場合は、この記事で提供されている [`Uninstall-AzModule` スクリプト](#uninstall-script)を次の呼び出しで使用します。

```powershell-interactive
$Modules = Get-InstalledModule -Name AzureRM -AllVersions
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```
