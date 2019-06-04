---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 11/30/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 79c34ea74887113be3683e32ab9a03ed4c7daa7c
ms.sourcegitcommit: bbd3f061cac3417ce588487c1ae4e0bc52c11d6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "65534479"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="90292-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="90292-103">Uninstall the Azure PowerShell module</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="90292-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="90292-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="90292-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="90292-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="90292-106">バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="90292-106">If you encounter a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>


## <a name="uninstall-azure-powershell-msi"></a><span data-ttu-id="90292-107">Azure PowerShell MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="90292-107">Uninstall Azure PowerShell MSI</span></span>

<span data-ttu-id="90292-108">MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="90292-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="90292-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="90292-109">Platform</span></span> | <span data-ttu-id="90292-110">Instructions</span><span class="sxs-lookup"><span data-stu-id="90292-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="90292-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="90292-111">Windows 10</span></span> | <span data-ttu-id="90292-112">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="90292-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="90292-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="90292-113">Windows 7</span></span> </br><span data-ttu-id="90292-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="90292-114">Windows 8</span></span> | <span data-ttu-id="90292-115">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="90292-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="90292-116">この画面のプログラムの一覧に [__Azure PowerShell__] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="90292-116">Once on this screen you should see __Azure PowerShell__ in the program listing.</span></span> <span data-ttu-id="90292-117">これが、アンインストール対象のアプリです。</span><span class="sxs-lookup"><span data-stu-id="90292-117">This is the app to uninstall.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="90292-118">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="90292-118">Uninstall from PowerShell</span></span>

<span data-ttu-id="90292-119">PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="90292-119">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="90292-120">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="90292-120">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="90292-121">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="90292-121">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="90292-122">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="90292-122">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="90292-123">現在インストールされている Azure PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="90292-123">To check which versions of Azure PowerShell you currently have installed, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

```output
Version              Name                                Repository           Description
-------              ----                                ----------           -----------
6.11.0               AzureRM                             PSGallery            Azure Resource Manager Module
6.13.1               AzureRM                             PSGallery            Azure Resource Manager Module
```

<span data-ttu-id="90292-124">次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="90292-124">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="90292-125">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="90292-125">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="90292-126">`Process` または `CurrentUser` 以外のスコープでこのスクリプトを実行するには、管理者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="90292-126">You will need to have administrator access to run this script in a scope other than `Process` or `CurrentUser`.</span></span>

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

<span data-ttu-id="90292-127">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="90292-127">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="90292-128">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="90292-128">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="90292-129">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="90292-129">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="90292-130">スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="90292-130">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="90292-131">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="90292-131">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="90292-132">便宜上、次のスクリプトにより、最新バージョンを__除く__、AzureRM のすべてのバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="90292-132">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```
