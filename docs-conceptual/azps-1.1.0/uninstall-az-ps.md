---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 9d1f1b6550c39b8c65662cf0150f477392747708
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342057"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="3cd8b-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="3cd8b-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="3cd8b-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="3cd8b-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>
<span data-ttu-id="3cd8b-106">バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-106">If you encounter a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-the-az-module"></a><span data-ttu-id="3cd8b-107">Az モジュールをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="3cd8b-107">Uninstall the Az module</span></span>

<span data-ttu-id="3cd8b-108">Az モジュールをアンインストールするには、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-108">To uninstall the Az modules, use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="3cd8b-109">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-109">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="3cd8b-110">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-110">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="3cd8b-111">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-111">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="3cd8b-112">現在インストールされている Azure PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-112">To check which versions of Azure PowerShell you currently have installed, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
0.7.0               Az                             PSGallery            Azure Resource Manager Module
1.0.0               Az                             PSGallery            Azure Resource Manager Module
```

<span data-ttu-id="3cd8b-113">次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-113">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="3cd8b-114">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-114">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="3cd8b-115">`Process` または `CurrentUser` 以外のスコープでこのスクリプトを実行するには、管理者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-115">You will need to have administrator access to run this script in a scope other than `Process` or `CurrentUser`.</span></span>

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
    if ($_.requiredVersion) {
      $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredVersion}
    }
    else { # Assume minimum version
      # Minimum version actually reports the installed dependency
      # which is used, not the actual "minimum dependency." Check to
      # see if the requested version was installed as a dependency earlier.
      $candidate = Get-InstalledModule $_.name -RequiredVersion $version
      if ($candidate) {
        $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$version}
      }
      else {
        Write-Warning ("Could not find uninstall candidate for {0}:{1} - module may require manual uninstall" -f $_.name,$version)
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

<span data-ttu-id="3cd8b-116">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-116">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="3cd8b-117">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-117">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule Az -Version 0.7.0 -Force
```

<span data-ttu-id="3cd8b-118">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-118">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="3cd8b-119">スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-119">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling Az.Profile version 0.7.0
Uninstalling Az.Aks version 0.7.0
Uninstalling Az.AnalysisServices version 0.7.0
...
```

<span data-ttu-id="3cd8b-120">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-120">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="3cd8b-121">便宜上、次のスクリプトにより、最新バージョンを__除く__、Az のすべてのバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-121">For convenience, the following script will uninstall all versions of Az __except__ for the latest.</span></span>

```powershell-interactive
$versions = (Get-InstalledModule Az -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule Az -Version ($_.Version) -Force }
```

## <a name="uninstall-the-azurerm-module"></a><span data-ttu-id="3cd8b-122">AzureRM モジュールをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="3cd8b-122">Uninstall the AzureRM module</span></span>

<span data-ttu-id="3cd8b-123">Az モジュールがシステムにインストールされていて、AzureRM をアンインストールする場合は、上記の `Uninstall-AllModules` スクリプトを実行する必要のない方法が 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-123">If you have the Az module installed on your system and would like to uninstall AzureRM, there are two simple options that don't require running the `Uninstall-AllModules` script above.</span></span> <span data-ttu-id="3cd8b-124">AzureRM をインストールした方法に応じて、実行する方法は異なります。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-124">Which method you follow depends on how you installed AzureRM.</span></span>
<span data-ttu-id="3cd8b-125">不明な場合は、まず、MSI をアンインストールするための手順を確認します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-125">If you're not sure, check the steps for uninstalling an MSI first.</span></span>

### <a name="uninstall-msi"></a><span data-ttu-id="3cd8b-126">MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="3cd8b-126">Uninstall MSI</span></span>

<span data-ttu-id="3cd8b-127">MSI パッケージを使用して Azure PowerShell AzureRM モジュールをインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-127">If you installed the Azure PowerShell AzureRM modules using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="3cd8b-128">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="3cd8b-128">Platform</span></span> | <span data-ttu-id="3cd8b-129">Instructions</span><span class="sxs-lookup"><span data-stu-id="3cd8b-129">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="3cd8b-130">Windows 10</span><span class="sxs-lookup"><span data-stu-id="3cd8b-130">Windows 10</span></span> | <span data-ttu-id="3cd8b-131">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="3cd8b-131">Start > Settings > Apps</span></span> |
| <span data-ttu-id="3cd8b-132">Windows 7</span><span class="sxs-lookup"><span data-stu-id="3cd8b-132">Windows 7</span></span> </br><span data-ttu-id="3cd8b-133">Windows 8</span><span class="sxs-lookup"><span data-stu-id="3cd8b-133">Windows 8</span></span> | <span data-ttu-id="3cd8b-134">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="3cd8b-134">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="3cd8b-135">この画面のプログラムの一覧に [Azure PowerShell] が表示されたら、そこからアンインストールできます。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-135">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

### <a name="uninstall-from-powershell"></a><span data-ttu-id="3cd8b-136">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="3cd8b-136">Uninstall from PowerShell</span></span>

<span data-ttu-id="3cd8b-137">PowerShellGet から AzureRM をインストールした場合は、新しい `Uninstall-AzureRM` コマンドを使用してモジュールを削除します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-137">If you installed AzureRM from PowerShellGet, then you can remove the modules with the new `Uninstall-AzureRM` command.</span></span> <span data-ttu-id="3cd8b-138">これによって、"_すべて_" の AzureRM モジュールがコンピューターから削除されます。ただし、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-138">This removes _all_ AzureRM modules from your machine, but requires administrator privileges.</span></span>

```powershell-interactive
Uninstall-AzureRm
```

<span data-ttu-id="3cd8b-139">`Uninstall-AzureRM` コマンドを正常に実行できない場合は、この記事で提供されている `Uninstall-AllModules` スクリプトを使用します。</span><span class="sxs-lookup"><span data-stu-id="3cd8b-139">If you can't successfully run the `Uninstall-AzureRM` command, use the `Uninstall-AllModules` script provided in this article instead.</span></span>