---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 09/11/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: bc017c40f955f2f4d99000bcde047d54eb3e155f
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/01/2018
ms.locfileid: "50738038"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="1d909-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="1d909-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="1d909-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d909-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="1d909-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="1d909-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="1d909-106">バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="1d909-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi"></a><span data-ttu-id="1d909-107">MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="1d909-107">Uninstall MSI</span></span>

<span data-ttu-id="1d909-108">MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d909-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="1d909-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="1d909-109">Platform</span></span> | <span data-ttu-id="1d909-110">このサンプルについての指示</span><span class="sxs-lookup"><span data-stu-id="1d909-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="1d909-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="1d909-111">Windows 10</span></span> | <span data-ttu-id="1d909-112">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="1d909-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="1d909-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="1d909-113">Windows 7</span></span> </br><span data-ttu-id="1d909-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="1d909-114">Windows 8</span></span> | <span data-ttu-id="1d909-115">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="1d909-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="1d909-116">この画面のプログラムの一覧に [Azure PowerShell] が表示されたら、そこからアンインストールできます。</span><span class="sxs-lookup"><span data-stu-id="1d909-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="1d909-117">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="1d909-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="1d909-118">PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="1d909-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="1d909-119">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="1d909-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="1d909-120">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1d909-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="1d909-121">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d909-121">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="1d909-122">次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1d909-122">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="1d909-123">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="1d909-123">Then, the script uninstalls the correct version of each submodule.</span></span>

```powershell
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
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredversion}
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

<span data-ttu-id="1d909-124">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="1d909-124">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="1d909-125">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1d909-125">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="1d909-126">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1d909-126">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="1d909-127">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="1d909-127">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span>
