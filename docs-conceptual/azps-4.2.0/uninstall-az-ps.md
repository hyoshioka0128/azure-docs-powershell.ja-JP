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
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="23a9f-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="23a9f-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="23a9f-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="23a9f-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="23a9f-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="23a9f-105">If you've decided to completely uninstall Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span> <span data-ttu-id="23a9f-106">バグが見つかった場合は、修正できるようにするため、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="23a9f-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues) so that it can be fixed.</span></span>

## <a name="uninstall-azure-powershell-from-msi"></a><span data-ttu-id="23a9f-107">MSI からの Azure PowerShell をアンインストールする</span><span class="sxs-lookup"><span data-stu-id="23a9f-107">Uninstall Azure PowerShell from MSI</span></span>

<span data-ttu-id="23a9f-108">MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="23a9f-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

|         <span data-ttu-id="23a9f-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="23a9f-109">Platform</span></span>         |                      <span data-ttu-id="23a9f-110">Instructions</span><span class="sxs-lookup"><span data-stu-id="23a9f-110">Instructions</span></span>                      |
| ------------------------ | ------------------------------------------------------ |
| <span data-ttu-id="23a9f-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="23a9f-111">Windows 10</span></span>               | <span data-ttu-id="23a9f-112">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="23a9f-112">Start > Settings > Apps</span></span>                                |
| <span data-ttu-id="23a9f-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="23a9f-113">Windows 7</span></span> </br><span data-ttu-id="23a9f-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="23a9f-114">Windows 8</span></span> | <span data-ttu-id="23a9f-115">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="23a9f-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="23a9f-116">この画面のプログラムの一覧に **[Azure PowerShell]** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-116">Once on this screen, you should see **Azure PowerShell** in the program listing.</span></span> <span data-ttu-id="23a9f-117">これが、アンインストール対象のアプリです。</span><span class="sxs-lookup"><span data-stu-id="23a9f-117">This is the app to uninstall.</span></span> <span data-ttu-id="23a9f-118">このプログラムが一覧に表示されていない場合は、PowerShellGet を介してインストールされています。この場合は、次の一連の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="23a9f-118">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

## <a name="uninstall-azure-powershell-from-powershellget"></a><span data-ttu-id="23a9f-119">PowerShellGet から Azure PowerShell をアンインストールする</span><span class="sxs-lookup"><span data-stu-id="23a9f-119">Uninstall Azure PowerShell from PowerShellGet</span></span>

<span data-ttu-id="23a9f-120">Az モジュールをアンインストールするために、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用できます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-120">To uninstall the Az modules, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="23a9f-121">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="23a9f-121">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="23a9f-122">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="23a9f-122">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="23a9f-123">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="23a9f-123">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="23a9f-124">インストールされている Azure PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="23a9f-124">To check which versions of Azure PowerShell you've installed, run the following command:</span></span>

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

<span data-ttu-id="23a9f-125">次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="23a9f-125">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="23a9f-126">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-126">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="23a9f-127">**Process** または **CurrentUser**.以外のスコープでこのスクリプトを実行するには、管理者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="23a9f-127">You need to have administrator access to run this script in a scope other than **Process** or **CurrentUser**.</span></span>

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

<span data-ttu-id="23a9f-128">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-128">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="23a9f-129">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="23a9f-129">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AzModule -Name Az -Version 1.8.0
```

<span data-ttu-id="23a9f-130">スクリプトを実行すると、アンインストールされる各サブモジュールの**名前**、**バージョン**、および**状態**が表示されます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-130">As the script runs, it displays the **Name**, **Version**, and **State** of each submodule that is being uninstalled.</span></span> <span data-ttu-id="23a9f-131">スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` パラメーターを指定します。</span><span class="sxs-lookup"><span data-stu-id="23a9f-131">To run the script to only see what would be deleted, without removing it, specify the `-WhatIf` parameter.</span></span>

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
> <span data-ttu-id="23a9f-132">このスクリプトは、アンインストールするのと同じバージョンの依存関係を正確に突き合わせることができない場合、その依存関係の "_どの_" バージョンもアンインストールしません。</span><span class="sxs-lookup"><span data-stu-id="23a9f-132">If this script can't match an exact dependency with the same version to uninstall, it won't uninstall _any_ version of that dependency.</span></span> <span data-ttu-id="23a9f-133">これは、これらの依存関係に依存する他のバージョンのターゲット モジュールがシステム上に存在する可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="23a9f-133">This is because there may be other versions of the target module on your system which rely on these dependencies.</span></span>

<span data-ttu-id="23a9f-134">アンインストールする Azure PowerShell のすべてのバージョンに対して次の例を実行します。</span><span class="sxs-lookup"><span data-stu-id="23a9f-134">Run the following example for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="23a9f-135">便宜上、次のスクリプトにより、最新バージョンを**除く**、Az のすべてのバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-135">For convenience, the following script uninstalls all versions of Az **except** for the latest.</span></span>

```powershell-interactive
$Modules = Get-InstalledModule -Name Az -AllVersions | 
    Sort-Object -Property Version -Descending | 
        Select-Object -Skip 1
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```

## <a name="uninstall-the-azurerm-module"></a><span data-ttu-id="23a9f-136">AzureRM モジュールをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="23a9f-136">Uninstall the AzureRM module</span></span>

<span data-ttu-id="23a9f-137">Az モジュールがシステムにインストールされていて、AzureRM をアンインストールする場合は、上記の `Uninstall-AzModule` スクリプトを実行する必要のない方法が 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="23a9f-137">If you have the Az module installed on your system and would like to uninstall AzureRM, there are two options that don't require running the `Uninstall-AzModule` script above.</span></span> <span data-ttu-id="23a9f-138">AzureRM モジュールをインストールした方法に応じて、実行する方法は異なります。</span><span class="sxs-lookup"><span data-stu-id="23a9f-138">Which method you follow depends on how you installed the AzureRM module.</span></span> <span data-ttu-id="23a9f-139">元のインストール方法が不明な場合は、まず、MSI をアンインストールするための手順に従います。</span><span class="sxs-lookup"><span data-stu-id="23a9f-139">If you're not sure of your original install method, follow the steps for uninstalling an MSI first.</span></span>

### <a name="uninstall-azure-powershell-msi"></a><span data-ttu-id="23a9f-140">Azure PowerShell MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="23a9f-140">Uninstall Azure PowerShell MSI</span></span>

<span data-ttu-id="23a9f-141">MSI パッケージを使用して Azure PowerShell AzureRM モジュールをインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="23a9f-141">If you installed the Azure PowerShell AzureRM modules using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

|         <span data-ttu-id="23a9f-142">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="23a9f-142">Platform</span></span>         |                      <span data-ttu-id="23a9f-143">Instructions</span><span class="sxs-lookup"><span data-stu-id="23a9f-143">Instructions</span></span>                      |
| ------------------------ | ------------------------------------------------------ |
| <span data-ttu-id="23a9f-144">Windows 10</span><span class="sxs-lookup"><span data-stu-id="23a9f-144">Windows 10</span></span>               | <span data-ttu-id="23a9f-145">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="23a9f-145">Start > Settings > Apps</span></span>                                |
| <span data-ttu-id="23a9f-146">Windows 7</span><span class="sxs-lookup"><span data-stu-id="23a9f-146">Windows 7</span></span> </br><span data-ttu-id="23a9f-147">Windows 8</span><span class="sxs-lookup"><span data-stu-id="23a9f-147">Windows 8</span></span> | <span data-ttu-id="23a9f-148">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="23a9f-148">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="23a9f-149">この画面のプログラムの一覧に **[Azure PowerShell]** または **[Azure PowerShell - 月年]** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-149">Once on this screen, you should see **Azure PowerShell** or **Microsoft Azure PowerShell - Month Year** in the program listing.</span></span> <span data-ttu-id="23a9f-150">これが、アンインストール対象のアプリです。</span><span class="sxs-lookup"><span data-stu-id="23a9f-150">This is the app to uninstall.</span></span> <span data-ttu-id="23a9f-151">このプログラムが一覧に表示されていない場合は、PowerShellGet を介してインストールされています。この場合は、次の一連の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="23a9f-151">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

### <a name="uninstall-from-powershell"></a><span data-ttu-id="23a9f-152">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="23a9f-152">Uninstall from PowerShell</span></span>

<span data-ttu-id="23a9f-153">PowerShellGet を使用して AzureRM をインストールした場合は、`Az.Accounts` モジュールの一部として使用可能な [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) コマンドレットでモジュールを削除できます。</span><span class="sxs-lookup"><span data-stu-id="23a9f-153">If you installed AzureRM with PowerShellGet, then you can remove the modules with the [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) cmdlet, available as part of the `Az.Accounts` module.</span></span> <span data-ttu-id="23a9f-154">次の例では、"_すべて_" の AzureRM モジュールがマシンから削除されます。ただし、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="23a9f-154">The following example removes _all_ AzureRM modules from your machine but requires administrator privileges.</span></span>

```powershell-interactive
Uninstall-AzureRm
```

<span data-ttu-id="23a9f-155">`Uninstall-AzureRM` コマンドを正常に実行できない場合は、この記事で提供されている [`Uninstall-AzModule` スクリプト](#uninstall-script)を次の呼び出しで使用します。</span><span class="sxs-lookup"><span data-stu-id="23a9f-155">If you can't successfully run the `Uninstall-AzureRM` command, use the [`Uninstall-AzModule` script](#uninstall-script) provided in this article with the following invocation:</span></span>

```powershell-interactive
$Modules = Get-InstalledModule -Name AzureRM -AllVersions
$Modules | ForEach-Object {Uninstall-AzModule -Name $_.Name -Version $_.Version}
```
