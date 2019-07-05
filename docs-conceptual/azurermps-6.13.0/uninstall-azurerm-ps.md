---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 06/10/2019
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 17197b77e26ccf0e41b5faf3cbbde34338b28167
ms.sourcegitcommit: febbbd3f75c8dd1a296281d265289f015b6cb537
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2019
ms.locfileid: "67037726"
---
# <a name="uninstall-the-azure-powershell-module"></a>Azure PowerShell モジュールのアンインストール

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。 Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。
バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。


## <a name="uninstall-azure-powershell-msi"></a>Azure PowerShell MSI のアンインストール

MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。

| プラットフォーム | Instructions |
|----------|--------------|
| Windows 10 | [スタート] > [設定] > [アプリ] |
| Windows 7 </br>Windows 8 | [スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール] |

この画面のプログラムの一覧に [__Azure PowerShell__] が表示されます。 これが、アンインストール対象のアプリです。

## <a name="uninstall-from-powershell"></a>PowerShell からのアンインストール

PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。 ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。 Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。 複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。

現在インストールされている Azure PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

```output
Version              Name                                Repository           Description
-------              ----                                ----------           -----------
6.11.0               AzureRM                             PSGallery            Azure Resource Manager Module
6.13.1               AzureRM                             PSGallery            Azure Resource Manager Module
```

次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。 次に、各サブモジュールの適切なバージョンがアンインストールされます。 `Process` または `CurrentUser` 以外のスコープでこのスクリプトを実行するには、管理者アクセス権が必要です。

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force,

    [switch]$WhatIf
  )
  
  $AllModules = @()
  
  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    if ($_.PSObject.Properties.Name -contains 'requiredVersion') {
      $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredVersion}
    }
    else { # Assume minimum version
      # Minimum version actually reports the installed dependency
      # which is used, not the actual "minimum dependency." Check to
      # see if the requested version was installed as a dependency earlier.
      $candidate = Get-InstalledModule $_.name -RequiredVersion $version -ErrorAction Ignore
      if ($candidate) {
        $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$version}
      }
      else {
        $availableModules = Get-InstalledModule $_.name -AllVersions
        Write-Warning ("Could not find uninstall candidate for {0}:{1} - module may require manual uninstall. Available versions are: {2}" -f $_.name,$version,($availableModules.Version -join ', '))
      }
    }
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}...' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop -WhatIf:$WhatIf
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。 次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。 スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` オプションを使用します。

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

> [!NOTE]
> このスクリプトは、アンインストールするのと同じバージョンの依存関係を正確に突き合わせることができない場合、その依存関係の_どの_バージョンもアンインストールしません。 これは、これらの依存関係に依存する他のバージョンのターゲット モジュールがシステム上に存在する可能性があるためです。 この場合、依存関係の使用可能なバージョンが一覧表示されます。
> その後、`Uninstall-Module` を使用して任意の古いバージョンを手動で削除できます。


アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。 便宜上、次のスクリプトにより、最新バージョンを__除く__、AzureRM のすべてのバージョンがアンインストールされます。

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[0..($versions.Length-2)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```
