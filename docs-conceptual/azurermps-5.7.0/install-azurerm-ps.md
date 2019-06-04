---
title: PowerShellGet を使用した Windows への Azure PowerShell のインストール
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.openlocfilehash: e05a519fabe41f3c23ffd63a8ceea69a0e58d5e1
ms.sourcegitcommit: bbd3f061cac3417ce588487c1ae4e0bc52c11d6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "65534671"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="e3c6f-103">PowerShellGet を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="e3c6f-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="e3c6f-104">この記事では、PowerShellGet を使用して、Windows 用 PowerShell 5.x の Azure PowerShell モジュールをインストールする手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-104">This article explains the steps to install the Azure PowerShell modules for PowerShell 5.x for Windows using PowerShellGet.</span></span> <span data-ttu-id="e3c6f-105">Azure PowerShell をインストールするときは、PowerShellGet およびモジュール管理を使用することをお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、[その他のインストール方法](other-install.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="e3c6f-106">このバージョンの Azure PowerShell では、Azure クラシック デプロイ モデルはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-106">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="e3c6f-107">クラシック デプロイのサポートについては、「[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)」の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-107">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e3c6f-108">AzureRM モジュールは、macOS または Linux ではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-108">The AzureRM module is not supported for macOS or Linux.</span></span> <span data-ttu-id="e3c6f-109">これらのプラットフォームで Azure PowerShell コマンドレットを使用するには、[Az モジュールをインストール](/powershell/azure/install-az-ps)します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-109">To use Azure PowerShell cmdlets on these platforms, [Install the Az module](/powershell/azure/install-az-ps).</span></span>

## <a name="requirements"></a><span data-ttu-id="e3c6f-110">必要条件</span><span class="sxs-lookup"><span data-stu-id="e3c6f-110">Requirements</span></span>

<span data-ttu-id="e3c6f-111">Azure PowerShell をインストールするには、PowerShellGet バージョン 1.1.2.0 以上が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-111">To install Azure PowerShell, you need PowerShellGet version 1.1.2.0 or higher.</span></span> <span data-ttu-id="e3c6f-112">お使いのシステムで使用できるかどうかを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-112">To check if it is available on your system, run the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name PowerShellGet -AllVersions | Select-Object -Property Name,Version,Path
```

<span data-ttu-id="e3c6f-113">次のような出力結果が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-113">You should see something similar to the following output:</span></span>

```output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="e3c6f-114">PowerShellGet のインストールを更新する必要がある場合は、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-114">If you need to update your installation of PowerShellGet, run the following command:</span></span>

```powershell-interactive
Install-Module PowerShellGet -Force
```

<span data-ttu-id="e3c6f-115">PowerShellGet がインストールされていない場合は、お使いのシステムで次の表の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-115">If you don't have PowerShellGet installed, follow the instructions in the table below for your system.</span></span>

|<span data-ttu-id="e3c6f-116">シナリオ</span><span class="sxs-lookup"><span data-stu-id="e3c6f-116">Scenario</span></span>|<span data-ttu-id="e3c6f-117">インストール手順</span><span class="sxs-lookup"><span data-stu-id="e3c6f-117">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="e3c6f-118">Windows 10</span><span class="sxs-lookup"><span data-stu-id="e3c6f-118">Windows 10</span></span><br/><span data-ttu-id="e3c6f-119">Windows Server 2016</span><span class="sxs-lookup"><span data-stu-id="e3c6f-119">Windows Server 2016</span></span>|<span data-ttu-id="e3c6f-120">OS 標準の Windows Management Framework (WMF) 5.0 に組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-120">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="e3c6f-121">PowerShell 5 にアップグレードする</span><span class="sxs-lookup"><span data-stu-id="e3c6f-121">Upgrade to PowerShell 5</span></span>| <ol><li><span data-ttu-id="e3c6f-122">[最新バージョンの WMF をインストール](https://www.microsoft.com/en-us/download/details.aspx?id=54616)します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-122">[Install the latest version of WMF](https://www.microsoft.com/en-us/download/details.aspx?id=54616)</span></span></li><li><span data-ttu-id="e3c6f-123">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-123">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|
|<span data-ttu-id="e3c6f-124">PowerShell 3 または PowerShell 4 がインストールされている Windows</span><span class="sxs-lookup"><span data-stu-id="e3c6f-124">Windows with PowerShell 3 or PowerShell 4</span></span>|<ol><span data-ttu-id="e3c6f-125"><il>[PackageManagement モジュールを入手します。](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span><span class="sxs-lookup"><span data-stu-id="e3c6f-125"><il>[Get the PackageManagement modules](http://go.microsoft.com/fwlink/?LinkID=746217)</il></span></span><li><span data-ttu-id="e3c6f-126">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-126">Run the following command:</span></span><br/>```Install-Module PowerShellGet -Force```</li></ol>|

> [!NOTE]
> <span data-ttu-id="e3c6f-127">PowerShellGet を使用するには、実行ポリシーでスクリプトの実行が許可されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-127">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="e3c6f-128">PowerShell の実行ポリシーについて詳しくは、「[About Execution Policies (実行ポリシーについて)](/powershell/module/microsoft.powershell.core/about/about_execution_policies)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-128">For more information about PowerShell's Execution Policy, see [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span></span>
>
> [!IMPORTANT]
> <span data-ttu-id="e3c6f-129">このドキュメントで説明するモジュール AzureRM では、.NET Framework を使用します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-129">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="e3c6f-130">そのため、.NET Core を使用する PowerShell 6.0 とは互換性がなくなります。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-130">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="e3c6f-131">PowerShell 6.0 を使用している場合は、[macOS および Linux のインストール手順](install-azurermps-maclinux.md)に従います。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-131">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="e3c6f-132">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="e3c6f-132">Install the Azure PowerShell module</span></span>

<span data-ttu-id="e3c6f-133">PowerShell ギャラリーからモジュールをインストールするには、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-133">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="e3c6f-134">Azure PowerShell をインストールするには、管理者特権のセッションで次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-134">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell-interactive
Install-Module -Name AzureRM
```

> [!NOTE]
> <span data-ttu-id="e3c6f-135">ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-135">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="e3c6f-136">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-136">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="e3c6f-137">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-137">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="e3c6f-138">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-138">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="e3c6f-139">`AzureRM` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-139">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="e3c6f-140">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-140">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="e3c6f-141">サインイン</span><span class="sxs-lookup"><span data-stu-id="e3c6f-141">Sign in</span></span>

<span data-ttu-id="e3c6f-142">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-142">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="e3c6f-143">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-143">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="e3c6f-144">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-144">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="e3c6f-145">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-145">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="e3c6f-146">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="e3c6f-146">Update the Azure PowerShell module</span></span>

<span data-ttu-id="e3c6f-147">Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-147">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="e3c6f-148">このコマンドでは、以前のバージョンはアンインストール__されません__。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-148">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name AzureRM
```

<span data-ttu-id="e3c6f-149">古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-149">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="e3c6f-150">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="e3c6f-150">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="e3c6f-151">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-151">It's possible to install multiple versions of Azure PowerShell.</span></span> <span data-ttu-id="e3c6f-152">オンプレミスの Azure Stack リソースを使用する場合、PowerShell 5.0 に更新できない古いバージョンの Windows を実行している場合、または Azure クラシック デプロイ モデルを使用している場合は、複数のバージョンが必要になります。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-152">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows that you can't update to PowerShell 5.0, or use the Azure classic deployment model.</span></span> <span data-ttu-id="e3c6f-153">古いバージョンをインストールするには、インストール時に `-RequiredVersion` 引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-153">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell-interactive
# Install version 2.3.0 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

<span data-ttu-id="e3c6f-154">Azure PowerShell モジュールの読み込み時には、最新バージョンが既定で読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-154">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="e3c6f-155">別のバージョンを読み込むには、`-RequiredVersion` 引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-155">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell-interactive
# Load version 2.3.0 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

## <a name="provide-feedback"></a><span data-ttu-id="e3c6f-156">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="e3c6f-156">Provide feedback</span></span>

<span data-ttu-id="e3c6f-157">Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-157">If you find a bug when using Azure Powershell, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="e3c6f-158">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-158">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e3c6f-159">次の手順</span><span class="sxs-lookup"><span data-stu-id="e3c6f-159">Next Steps</span></span>

<span data-ttu-id="e3c6f-160">Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e3c6f-160">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
