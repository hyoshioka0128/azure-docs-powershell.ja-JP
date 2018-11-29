---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: bf1f81b4929ec066eeb888da4ba1303430f026b4
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "52586583"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="53a8b-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="53a8b-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="53a8b-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="53a8b-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="53a8b-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="53a8b-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="53a8b-106">バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="53a8b-106">If you encounter a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="53a8b-107">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="53a8b-107">Uninstall from PowerShell</span></span>

<span data-ttu-id="53a8b-108">PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="53a8b-108">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="53a8b-109">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="53a8b-109">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="53a8b-110">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="53a8b-110">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="53a8b-111">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="53a8b-111">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="53a8b-112">次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="53a8b-112">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="53a8b-113">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="53a8b-113">Then, the script uninstalls the correct version of each submodule.</span></span>

```powershell-interactive
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force
  )

  $AllModules = @()

  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.minimumVersion}
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

<span data-ttu-id="53a8b-114">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="53a8b-114">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="53a8b-115">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="53a8b-115">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="53a8b-116">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="53a8b-116">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="53a8b-117">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="53a8b-117">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="53a8b-118">便宜上、次のスクリプトにより、最新バージョンを__除く__、AzureRM のすべてのバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="53a8b-118">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[1..($versions.Length-1)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```

## <a name="uninstall-msi"></a><span data-ttu-id="53a8b-119">MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="53a8b-119">Uninstall MSI</span></span>

<span data-ttu-id="53a8b-120">MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="53a8b-120">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="53a8b-121">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="53a8b-121">Platform</span></span> | <span data-ttu-id="53a8b-122">Instructions</span><span class="sxs-lookup"><span data-stu-id="53a8b-122">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="53a8b-123">Windows 10</span><span class="sxs-lookup"><span data-stu-id="53a8b-123">Windows 10</span></span> | <span data-ttu-id="53a8b-124">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="53a8b-124">Start > Settings > Apps</span></span> |
| <span data-ttu-id="53a8b-125">Windows 7</span><span class="sxs-lookup"><span data-stu-id="53a8b-125">Windows 7</span></span> </br><span data-ttu-id="53a8b-126">Windows 8</span><span class="sxs-lookup"><span data-stu-id="53a8b-126">Windows 8</span></span> | <span data-ttu-id="53a8b-127">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="53a8b-127">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="53a8b-128">この画面のプログラムの一覧に [Azure PowerShell] が表示されたら、そこからアンインストールできます。</span><span class="sxs-lookup"><span data-stu-id="53a8b-128">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>
