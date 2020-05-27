---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 10/22/2019
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 1bf94f4c7a27328b60b7f9369888f688541ba4a7
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386869"
---
# <a name="uninstall-the-azure-powershell-module"></a><span data-ttu-id="0771a-103">Azure PowerShell モジュールのアンインストール</span><span class="sxs-lookup"><span data-stu-id="0771a-103">Uninstall the Azure PowerShell module</span></span>

<span data-ttu-id="0771a-104">この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="0771a-104">This article tells you how to uninstall an older version of Azure PowerShell, or completely remove it from your system.</span></span> <span data-ttu-id="0771a-105">Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用してフィードバックをお送りください。</span><span class="sxs-lookup"><span data-stu-id="0771a-105">If you've decided to completely uninstall the Azure PowerShell, give us some feedback through the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>
<span data-ttu-id="0771a-106">バグが見つかった場合は、修正できるようにするため、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。</span><span class="sxs-lookup"><span data-stu-id="0771a-106">If you encountered a bug, we'd appreciate it if you [file a GitHub issue](https://github.com/azure/azure-powershell/issues) so that it can be fixed.</span></span>

## <a name="uninstall-azure-powershell-from-msi"></a><span data-ttu-id="0771a-107">MSI からの Azure PowerShell をアンインストールする</span><span class="sxs-lookup"><span data-stu-id="0771a-107">Uninstall Azure PowerShell from MSI</span></span>

<span data-ttu-id="0771a-108">MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0771a-108">If you installed Azure PowerShell using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="0771a-109">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="0771a-109">Platform</span></span> | <span data-ttu-id="0771a-110">Instructions</span><span class="sxs-lookup"><span data-stu-id="0771a-110">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="0771a-111">Windows 10</span><span class="sxs-lookup"><span data-stu-id="0771a-111">Windows 10</span></span> | <span data-ttu-id="0771a-112">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="0771a-112">Start > Settings > Apps</span></span> |
| <span data-ttu-id="0771a-113">Windows 7</span><span class="sxs-lookup"><span data-stu-id="0771a-113">Windows 7</span></span> </br><span data-ttu-id="0771a-114">Windows 8</span><span class="sxs-lookup"><span data-stu-id="0771a-114">Windows 8</span></span> | <span data-ttu-id="0771a-115">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="0771a-115">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="0771a-116">この画面のプログラムの一覧に [__Azure PowerShell__] が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0771a-116">Once on this screen you should see __Azure PowerShell__ in the program listing.</span></span> <span data-ttu-id="0771a-117">これが、アンインストール対象のアプリです。</span><span class="sxs-lookup"><span data-stu-id="0771a-117">This is the app to uninstall.</span></span> <span data-ttu-id="0771a-118">このプログラムが一覧に表示されていない場合は、PowerShellGet を介してインストールされています。この場合は、次の一連の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="0771a-118">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

## <a name="uninstall-azure-powershell-from-powershell-get"></a><span data-ttu-id="0771a-119">PowerShell Get からの Azure PowerShell をアンインストールする</span><span class="sxs-lookup"><span data-stu-id="0771a-119">Uninstall Azure PowerShell from PowerShell Get</span></span>

<span data-ttu-id="0771a-120">Az モジュールをアンインストールするには、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="0771a-120">To uninstall the Az modules, use the [Uninstall-Module](/powershell/module/powershellget/uninstall-module) cmdlet.</span></span> <span data-ttu-id="0771a-121">ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="0771a-121">However, `Uninstall-Module` only uninstalls one module.</span></span> <span data-ttu-id="0771a-122">Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0771a-122">To remove Azure PowerShell completely, you must uninstall each module individually.</span></span> <span data-ttu-id="0771a-123">複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。</span><span class="sxs-lookup"><span data-stu-id="0771a-123">Uninstallation can be complicated if you have more than one version of Azure PowerShell installed.</span></span>

<span data-ttu-id="0771a-124">現在インストールされている Azure PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="0771a-124">To check which versions of Azure PowerShell you currently have installed, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions
```

```output
Version             Name                           Repository           Description
-------             ----                           ----------           -----------
0.7.0               Az                             PSGallery            Azure Resource Manager Module
1.0.0               Az                             PSGallery            Azure Resource Manager Module
```

<a name="uninstall-script"/>

<span data-ttu-id="0771a-125">次のスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="0771a-125">The following script queries the PowerShell Gallery to get a list of dependent submodules.</span></span> <span data-ttu-id="0771a-126">次に、各サブモジュールの適切なバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="0771a-126">Then, the script uninstalls the correct version of each submodule.</span></span> <span data-ttu-id="0771a-127">`Process` または `CurrentUser` 以外のスコープでこのスクリプトを実行するには、管理者アクセス権が必要です。</span><span class="sxs-lookup"><span data-stu-id="0771a-127">You will need to have administrator access to run this script in a scope other than `Process` or `CurrentUser`.</span></span>

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

<span data-ttu-id="0771a-128">この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="0771a-128">To use this function, copy and paste the code into your PowerShell session.</span></span> <span data-ttu-id="0771a-129">次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0771a-129">The following example shows how to run the function to remove an older version of Azure PowerShell.</span></span>

```powershell-interactive
Uninstall-AllModules -TargetModule Az -Version 0.7.0 -Force
```

<span data-ttu-id="0771a-130">スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0771a-130">As the script runs, it will display the name and version of each submodule that is being uninstalled.</span></span> <span data-ttu-id="0771a-131">スクリプトを実行して削除対象を削除せずに表示のみを行うには、`-WhatIf` オプションを使用します。</span><span class="sxs-lookup"><span data-stu-id="0771a-131">To run the script to only see what would be deleted, without removing it, use the `-WhatIf` option.</span></span>

```output
Creating list of dependencies...
Uninstalling Az.Profile version 0.7.0
Uninstalling Az.Aks version 0.7.0
Uninstalling Az.AnalysisServices version 0.7.0
...
```

> [!NOTE]
> <span data-ttu-id="0771a-132">このスクリプトは、アンインストールするのと同じバージョンの依存関係を正確に突き合わせることができない場合、その依存関係の "_どの_" バージョンもアンインストールしません。</span><span class="sxs-lookup"><span data-stu-id="0771a-132">If this script can't match an exact dependency with the same version to uninstall, it won't uninstall _any_ version of that dependecy.</span></span> <span data-ttu-id="0771a-133">これは、これらの依存関係に依存する他のバージョンのターゲット モジュールがシステム上に存在する可能性があるためです。</span><span class="sxs-lookup"><span data-stu-id="0771a-133">This is because there may be other versions of the target module on your system which rely on these dependencies.</span></span> <span data-ttu-id="0771a-134">この場合、依存関係の使用可能なバージョンが一覧表示されます。</span><span class="sxs-lookup"><span data-stu-id="0771a-134">In this case, the available versions of the dependency are listed.</span></span>
> <span data-ttu-id="0771a-135">その後、`Uninstall-Module` を使用して任意の古いバージョンを手動で削除できます。</span><span class="sxs-lookup"><span data-stu-id="0771a-135">You can then remove any old versions manually with `Uninstall-Module`.</span></span>

<span data-ttu-id="0771a-136">アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="0771a-136">Run this command for every version of Azure PowerShell that you want to uninstall.</span></span> <span data-ttu-id="0771a-137">便宜上、次のスクリプトにより、最新バージョンを__除く__、Az のすべてのバージョンがアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="0771a-137">For convenience, the following script will uninstall all versions of Az __except__ for the latest.</span></span>

```powershell-interactive
$versions = (Get-InstalledModule Az -AllVersions | Select-Object Version)
$versions[0..($versions.Length-2)]  | foreach { Uninstall-AllModules -TargetModule Az -Version ($_.Version) -Force }
```

## <a name="uninstall-the-azurerm-module"></a><span data-ttu-id="0771a-138">AzureRM モジュールをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="0771a-138">Uninstall the AzureRM module</span></span>

<span data-ttu-id="0771a-139">Az モジュールがシステムにインストールされていて、AzureRM をアンインストールする場合は、上記の `Uninstall-AllModules` スクリプトを実行する必要のない方法が 2 つあります。</span><span class="sxs-lookup"><span data-stu-id="0771a-139">If you have the Az module installed on your system and would like to uninstall AzureRM, there are two options that don't require running the `Uninstall-AllModules` script above.</span></span> <span data-ttu-id="0771a-140">AzureRM モジュールをインストールした方法に応じて、実行する方法は異なります。</span><span class="sxs-lookup"><span data-stu-id="0771a-140">Which method you follow depends on how you installed the AzureRM module.</span></span>
<span data-ttu-id="0771a-141">元のインストール方法が不明な場合は、まず、MSI をアンインストールするための手順に従います。</span><span class="sxs-lookup"><span data-stu-id="0771a-141">If you're not sure of your original install method, follow the steps for uninstalling an MSI first.</span></span>

### <a name="uninstall-azure-powershell-msi"></a><span data-ttu-id="0771a-142">Azure PowerShell MSI のアンインストール</span><span class="sxs-lookup"><span data-stu-id="0771a-142">Uninstall Azure PowerShell MSI</span></span>

<span data-ttu-id="0771a-143">MSI パッケージを使用して Azure PowerShell AzureRM モジュールをインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0771a-143">If you installed the Azure PowerShell AzureRM modules using the MSI package, you must uninstall through the Windows system rather than PowerShell.</span></span>

| <span data-ttu-id="0771a-144">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="0771a-144">Platform</span></span> | <span data-ttu-id="0771a-145">Instructions</span><span class="sxs-lookup"><span data-stu-id="0771a-145">Instructions</span></span> |
|----------|--------------|
| <span data-ttu-id="0771a-146">Windows 10</span><span class="sxs-lookup"><span data-stu-id="0771a-146">Windows 10</span></span> | <span data-ttu-id="0771a-147">[スタート] > [設定] > [アプリ]</span><span class="sxs-lookup"><span data-stu-id="0771a-147">Start > Settings > Apps</span></span> |
| <span data-ttu-id="0771a-148">Windows 7</span><span class="sxs-lookup"><span data-stu-id="0771a-148">Windows 7</span></span> </br><span data-ttu-id="0771a-149">Windows 8</span><span class="sxs-lookup"><span data-stu-id="0771a-149">Windows 8</span></span> | <span data-ttu-id="0771a-150">[スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール]</span><span class="sxs-lookup"><span data-stu-id="0771a-150">Start > Control Panel > Programs > Uninstall a program</span></span> |

<span data-ttu-id="0771a-151">この画面のプログラムの一覧に __[Azure PowerShell]__ または __[Azure PowerShell - 月年]__ が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0771a-151">Once on this screen you should see __Azure PowerShell__ or __Microsoft Azure PowerShell - Month Year__ in the program listing.</span></span> <span data-ttu-id="0771a-152">これが、アンインストール対象のアプリです。</span><span class="sxs-lookup"><span data-stu-id="0771a-152">This is the app to uninstall.</span></span> <span data-ttu-id="0771a-153">このプログラムが一覧に表示されていない場合は、PowerShellGet を介してインストールされています。この場合は、次の一連の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="0771a-153">If you don't see this program listed, then you installed through PowerShellGet, and should follow the next set of instructions.</span></span>

### <a name="uninstall-from-powershell"></a><span data-ttu-id="0771a-154">PowerShell からのアンインストール</span><span class="sxs-lookup"><span data-stu-id="0771a-154">Uninstall from PowerShell</span></span>

<span data-ttu-id="0771a-155">PowerShellGet を使用して AzureRM をインストールした場合は、`Az.Accounts` モジュールの一部として使用可能な [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) コマンドでモジュールを削除します。</span><span class="sxs-lookup"><span data-stu-id="0771a-155">If you installed AzureRM with PowerShellGet, then you can remove the modules with the [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) command, available as part of the `Az.Accounts` module.</span></span> <span data-ttu-id="0771a-156">これによって、"_すべて_" の AzureRM モジュールがコンピューターから削除されます。ただし、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="0771a-156">This removes _all_ AzureRM modules from your machine, but requires administrator privileges.</span></span>

```powershell-interactive
Uninstall-AzureRm
```
<span data-ttu-id="0771a-157">or</span><span class="sxs-lookup"><span data-stu-id="0771a-157">or</span></span>
```powershell-interactive
Uninstall-Module AzureRm
```

<span data-ttu-id="0771a-158">`Uninstall-AzureRM` コマンドを正常に実行できない場合は、この記事で提供されている [`Uninstall-AllModules` スクリプト](#uninstall-script)を次の呼び出しで使用します。</span><span class="sxs-lookup"><span data-stu-id="0771a-158">If you can't successfully run the `Uninstall-AzureRM` command, use the [`Uninstall-AllModules` script](#uninstall-script) provided in this article with the following invocation:</span></span>

```powershell-interactive
$versions = (Get-InstalledModule AzureRM -AllVersions | Select-Object Version)
$versions | foreach { Uninstall-AllModules -TargetModule AzureRM -Version ($_.Version) -Force }
```
<span data-ttu-id="0771a-159">or</span><span class="sxs-lookup"><span data-stu-id="0771a-159">or</span></span>
```powershell-interactive
foreach ($module in (Get-Module -ListAvailable AzureRM*).Name |Get-Unique) {
   write-host "Removing Module $module"
   Uninstall-module $module
}
```
