---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 92af0fdd8db451e2f0f092d66a3e296ad8d6a09e
ms.sourcegitcommit: dca906e73e943aac207cee23b79915773419c673
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2018
ms.locfileid: "43250067"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="0394c-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="0394c-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="0394c-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="0394c-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="0394c-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="0394c-105">If you've decided to completely uninstall the Azure PowerShell, please give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="0394c-106">バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="0394c-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi"></a><span data-ttu-id="0394c-107">MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="0394c-107">Uninstall MSI</span></span>

<span data-ttu-id="0394c-108">MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0394c-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="0394c-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="0394c-109">Platform</span></span> | <span data-ttu-id="0394c-110">このサンプルについての指示</span><span class="sxs-lookup"><span data-stu-id="0394c-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="0394c-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="0394c-111">Windows 10</span></span> | <span data-ttu-id="0394c-112">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="0394c-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="0394c-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="0394c-113">Windows 7</span></span> </br><span data-ttu-id="0394c-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="0394c-114">Windows 8</span></span> | <span data-ttu-id="0394c-115">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="0394c-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="0394c-116">この画面のプログラムの一覧に [Azure PowerShell] が表示されたら、そこからアンインストールできます。</span><span class="sxs-lookup"><span data-stu-id="0394c-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="0394c-117">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="0394c-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="0394c-118">PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="0394c-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="0394c-119">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="0394c-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="0394c-120">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0394c-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="0394c-121">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="0394c-121">Uninstallation can be complicated if you have multiple versions of Azure PowerShell installed.</span></span>

<span data-ttu-id="0394c-122">次のスクリプトは、1 つのバージョンの Azure PowerShell を完全に削除するときに使用できます。</span><span class="sxs-lookup"><span data-stu-id="0394c-122">The following script can be used to completely remove a single version of Azure PowerShell.</span></span> <span data-ttu-id="0394c-123">このスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0394c-123">The script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="0394c-124">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="0394c-124">Then, the script uninstalls the correct version of each submodule.</span></span>

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

<span data-ttu-id="0394c-125">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="0394c-125">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="0394c-126">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0394c-126">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="0394c-127">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0394c-127">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

<span data-ttu-id="0394c-128">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="0394c-128">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span>