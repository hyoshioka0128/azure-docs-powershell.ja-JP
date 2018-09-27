---
title: PowerShellGet を使用した Windows への Azure PowerShell のインストール
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 970742c91b327a1310ef5097edef40287ebf9f9b
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2018
ms.locfileid: "47178733"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="86839-103">PowerShellGet を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="86839-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

<span data-ttu-id="86839-104">この記事では、PowerShellGet を使用して、Windows 環境に Azure PowerShell モジュールをインストールする手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="86839-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span> <span data-ttu-id="86839-105">Azure PowerShell をインストールするときは、PowerShellGet およびモジュール管理を使用することをお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、[その他のインストール方法](other-install.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="86839-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="86839-106">Azure PowerShell を他のプラットフォームにインストールする手順については、[macOS および Linux への Azure PowerShell のインストールと構成](install-azurermps-maclinux.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="86839-106">For instructions to install Azure PowerShell on other platforms, see [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

<span data-ttu-id="86839-107">このバージョンの Azure PowerShell では、Azure クラシック デプロイ モデルはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="86839-107">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="86839-108">クラシック デプロイのサポートについては、「[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)」の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="86839-108">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

## <a name="requirements"></a><span data-ttu-id="86839-109">必要条件</span><span class="sxs-lookup"><span data-stu-id="86839-109">Requirements</span></span>

<span data-ttu-id="86839-110">Azure PowerShell バージョン 6.0 以降、Azure PowerShell では PowerShell バージョン 5.0 が必要です。</span><span class="sxs-lookup"><span data-stu-id="86839-110">Starting with Azure PowerShell version 6.0, Azure PowerShell requires PowerShell version 5.0.</span></span> <span data-ttu-id="86839-111">お使いのマシンで実行されている PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="86839-111">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell
$PSVersionTable.PSVersion
```

<span data-ttu-id="86839-112">バージョンが古い場合は、「[既存の Windows PowerShell をアップグレードする](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="86839-112">If you have an outdated version, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="86839-113">このドキュメントで説明するモジュール AzureRM では、.NET Framework を使用します。</span><span class="sxs-lookup"><span data-stu-id="86839-113">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="86839-114">そのため、.NET Core を使用する PowerShell 6.0 とは互換性がなくなります。</span><span class="sxs-lookup"><span data-stu-id="86839-114">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="86839-115">PowerShell 6.0 を使用している場合は、[macOS および Linux のインストール手順](install-azurermps-maclinux.md)に従います。</span><span class="sxs-lookup"><span data-stu-id="86839-115">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="86839-116">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="86839-116">Install the Azure PowerShell module</span></span>

<span data-ttu-id="86839-117">PowerShell ギャラリーからモジュールをインストールするには、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="86839-117">You need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="86839-118">Azure PowerShell をインストールするには、管理者特権のセッションで次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="86839-118">To install Azure PowerShell, run the following command in an elevated session:</span></span>

```powershell
Install-Module -Name AzureRM
```

> [!NOTE]
> <span data-ttu-id="86839-119">ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。</span><span class="sxs-lookup"><span data-stu-id="86839-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="86839-120">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="86839-120">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="86839-121">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="86839-121">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="86839-122">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="86839-122">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="86839-123">`AzureRM` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="86839-123">The `AzureRM` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="86839-124">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="86839-124">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="86839-125">[サインイン]</span><span class="sxs-lookup"><span data-stu-id="86839-125">Sign in</span></span>

<span data-ttu-id="86839-126">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="86839-126">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="86839-127">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="86839-127">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="86839-128">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="86839-128">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="86839-129">Azure サインインをセッション間で維持する方法については、「[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="86839-129">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="86839-130">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="86839-130">Update the Azure PowerShell module</span></span>

<span data-ttu-id="86839-131">Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。</span><span class="sxs-lookup"><span data-stu-id="86839-131">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="86839-132">このコマンドでは、以前のバージョンはアンインストール__されません__。</span><span class="sxs-lookup"><span data-stu-id="86839-132">This command does __not__ uninstall earlier versions.</span></span>

```powershell
Update-Module -Name AzureRM
```

<span data-ttu-id="86839-133">古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="86839-133">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="86839-134">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="86839-134">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="86839-135">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="86839-135">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="86839-136">オンプレミスの Azure Stack リソースを使用する場合、古いバージョンの Windows を実行している場合、または Azure クラシック デプロイ モデルを使用している場合は、複数のバージョンが必要になります。</span><span class="sxs-lookup"><span data-stu-id="86839-136">You might need more than one version if you work with on-premises Azure Stack resources, run an older version of Windows, or use the Azure classic deployment model.</span></span> <span data-ttu-id="86839-137">古いバージョンをインストールするには、インストール時に `-RequiredVersion` 引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="86839-137">To install an older version, provide the `-RequiredVersion` argument when installing.</span></span>

```powershell
# Install version 1.2.9 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="86839-138">Azure PowerShell モジュールの読み込み時には、最新バージョンが既定で読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="86839-138">When loading the Azure PowerShell module the latest version is loaded by default.</span></span> <span data-ttu-id="86839-139">別のバージョンを読み込むには、`-RequiredVersion` 引数を指定します。</span><span class="sxs-lookup"><span data-stu-id="86839-139">To load a different version, provide the `-RequiredVersion` argument.</span></span>

```powershell
# Load version 1.2.9 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

## <a name="provide-feedback"></a><span data-ttu-id="86839-140">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="86839-140">Provide feedback</span></span>

<span data-ttu-id="86839-141">Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="86839-141">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="86839-142">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="86839-142">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/azurerm.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="86839-143">次の手順</span><span class="sxs-lookup"><span data-stu-id="86839-143">Next Steps</span></span>

<span data-ttu-id="86839-144">Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="86839-144">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>