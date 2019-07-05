---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 06/10/2019
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: cc0b6a4369116e92b8200ffbc0838d6ee2991263
ms.sourcegitcommit: febbbd3f75c8dd1a296281d265289f015b6cb537
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2019
ms.locfileid: "67037698"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="1a64d-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="1a64d-103">Uninstall the Azure PowerShell module</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="1a64d-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="1a64d-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="1a64d-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="1a64d-105">If you've decided to completely uninstall the Azure PowerShell, please give us some feedback through the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>
<span data-ttu-id="1a64d-106">バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="1a64d-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues).</span></span>

## <a name="uninstall-msi-or-web-platform-installer"></a><span data-ttu-id="1a64d-107">MSI または Web Platform Installer のアンインストール</span><span class="sxs-lookup"><span data-stu-id="1a64d-107">Uninstall MSI or Web Platform Installer</span></span>

<span data-ttu-id="1a64d-108">MSI パッケージまたは Web Platform Installer を使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a64d-108">If you installed Azure PowerShell using the MSI package or the Web Platform Installer, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="1a64d-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="1a64d-109">Platform</span></span> | <span data-ttu-id="1a64d-110">Instructions</span><span class="sxs-lookup"><span data-stu-id="1a64d-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="1a64d-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="1a64d-111">Windows 10</span></span> | <span data-ttu-id="1a64d-112">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="1a64d-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="1a64d-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="1a64d-113">Windows 7</span></span> </br><span data-ttu-id="1a64d-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="1a64d-114">Windows 8</span></span> | <span data-ttu-id="1a64d-115">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="1a64d-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="1a64d-116">この画面のプログラムの一覧に [Azure PowerShell] が表示されたら、そこからアンインストールできます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-116">Once on this screen you should see "Azure PowerShell" in the program listing, and can uninstall from there.</span></span>

## <a name="uninstall-from-powershell"></a><span data-ttu-id="1a64d-117">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="1a64d-117">Uninstall from PowerShell</span></span>

<span data-ttu-id="1a64d-118">PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="1a64d-118">If you installed Azure PowerShell using PowerShellGet, you can use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="1a64d-119">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="1a64d-119">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="1a64d-120">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a64d-120">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="1a64d-121">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a64d-121">Uninstallation can be complicated if you have multiple versions of Azure PowerShell installed.</span></span>

<span data-ttu-id="1a64d-122">次のスクリプトを使用して、1 つのバージョンの Azure PowerShell を完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-122">You use the following script can be used to completely remove a single version of Azure PowerShell.</span></span> <span data-ttu-id="1a64d-123">このスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="1a64d-123">The script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="1a64d-124">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-124">Then, the script uninstalls the correct version of each submodule.</span></span>

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

<span data-ttu-id="1a64d-125">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-125">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="1a64d-126">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="1a64d-126">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

<span data-ttu-id="1a64d-127">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-127">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="1a64d-128">スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="1a64d-128">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

> [!NOTE]
> <span data-ttu-id="1a64d-129">このスクリプトは、アンインストールするのと同じバージョンの依存関係を正確に突き合わせることができない場合、その依存関係の_どの_バージョンもアンインストールしません。</span><span class="sxs-lookup"><span data-stu-id="1a64d-129">If this script can't match an exact dependency with the same version to uninstall, it won't uninstall _any_ version of that dependecy.</span></span> <span data-ttu-id="1a64d-130">これは、これらの依存関係に依存する他のバージョンのターゲット モジュールがシステム上に存在する可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="1a64d-130">This is because there may be other versions of the target module on your system which rely on these dependencies.</span></span> <span data-ttu-id="1a64d-131">この場合、依存関係の使用可能なバージョンが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-131">In this case, the available versions of the dependency are listed.</span></span>
> <span data-ttu-id="1a64d-132">その後、`Uninstall-Module` を使用して任意の古いバージョンを手動で削除できます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-132">You can then remove any old versions manually with `Uninstall-Module`.</span></span>


<span data-ttu-id="1a64d-133">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="1a64d-133">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="1a64d-134">便宜上、次のスクリプトにより、最新バージョンを__除く__、AzureRM のすべてのバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="1a64d-134">For convenience, the following script will uninstall all versions of AzureRM __except__ for the latest.</span></span>

```powershell-interactive
$versions = (get-installedmodule AzureRM -AllVersions | Select-Object Version)
$versions[0..($versions.Length-2)]  | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```
