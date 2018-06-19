---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323103"
---
# <a name="install-azure-powershell-with-powershellget"></a><span data-ttu-id="d09c7-103">PowerShellGet を使用して Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="d09c7-103">Install Azure PowerShell with PowerShellGet</span></span>

<span data-ttu-id="d09c7-104">この記事では、PowerShellGet を使用して、Windows 環境に Azure PowerShell モジュールをインストールする手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-104">This article explains the steps to install the Azure PowerShell modules in a Windows environment using PowerShellGet.</span></span>  <span data-ttu-id="d09c7-105">Azure PowerShell をインストールする場合は、この方法をお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、「[その他のインストール方法](other-install.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-105">This is the preferred way to install Azure PowerShell, but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="d09c7-106">macOS または Linux で Azure PowerShell を使用する場合は、「[macOS および Linux での Azure PowerShell のインストールおよび構成](install-azurermps-maclinux.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-106">If you want to use Azure PowerShell on macOS or Linux, see the following article: [Install and configure Azure PowerShell on macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="system-requirements"></a><span data-ttu-id="d09c7-107">システム要件</span><span class="sxs-lookup"><span data-stu-id="d09c7-107">System requirements</span></span>

<span data-ttu-id="d09c7-108">Azure PowerShell バージョン 6.1.0 には、PowerShell バージョン 5.0 (以降) が必要です。</span><span class="sxs-lookup"><span data-stu-id="d09c7-108">Azure PowerShell version 6.1.0 requires version 5.0 (or higher) of PowerShell.</span></span> <span data-ttu-id="d09c7-109">PowerShell 5.0 へのアップグレードについては、[既存の Windows PowerShell のアップグレード](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-109">For information on upgrading to PowerShell 5.0, see [Upgrading existing Windows PowerShell](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

<span data-ttu-id="d09c7-110">PowerShellGet は、PowerShell 5.0 に自動的に追加されます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-110">PowerShellGet is automatically included as part of PowerShell 5.0.</span></span>

## <a name="install-or-update-the-azure-powershell-module"></a><span data-ttu-id="d09c7-111">Azure PowerShell モジュールをインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="d09c7-111">Install or update the Azure PowerShell module</span></span>

<span data-ttu-id="d09c7-112">Azure PowerShell を PowerShell ギャラリーからインストールするためには、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="d09c7-112">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="d09c7-113">管理者特権の PowerShell セッションから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-113">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> <span data-ttu-id="d09c7-114">このコマンドにより、お使いのシステム上の Azure PowerShell の既存のインストールすべてが更新されます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-114">This command will update any existing installation of Azure PowerShell on your system.</span></span> <span data-ttu-id="d09c7-115">複数のバージョンをインストールする必要がある場合は、FAQ の「[複数のバージョンの Azure PowerShell をインストールできますか](#multiple-versions)」の回答を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-115">If you need to have more than one version installed, see the FAQ answer for [Can I install multiple versions of Azure PowerShell?](#multiple-versions)</span></span>

<span data-ttu-id="d09c7-116">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとして構成されていません。</span><span class="sxs-lookup"><span data-stu-id="d09c7-116">By default, the PowerShell gallery is not configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="d09c7-117">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-117">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="d09c7-118">インストールを続行するには、"Yes" または "Yes to All" と回答します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-118">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="d09c7-119">ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="d09c7-120">AzureRM モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="d09c7-120">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="d09c7-121">AzureRM モジュールをインストールすると、まだインストールしていない Azure PowerShell モジュールが PowerShell ギャラリーからダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-121">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded from the PowerShell Gallery.</span></span>

## <a name="load-the-azure-powershell-module"></a><span data-ttu-id="d09c7-122">Azure PowerShell モジュールを読み込む</span><span class="sxs-lookup"><span data-stu-id="d09c7-122">Load the Azure PowerShell module</span></span>

<span data-ttu-id="d09c7-123">モジュールは、インストール後、PowerShell セッションに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09c7-123">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="d09c7-124">これは通常の (管理者特権ではない) PowerShell セッションで実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09c7-124">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="d09c7-125">モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="d09c7-125">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="d09c7-126">問題とフィードバックの報告</span><span class="sxs-lookup"><span data-stu-id="d09c7-126">Reporting issues and feedback</span></span>

<span data-ttu-id="d09c7-127">ツールにバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-127">If you encounter any bugs with the tool, please [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="d09c7-128">コマンド ラインからフィードバックを送るには、`Send-Feedback` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-128">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="d09c7-129">次の手順</span><span class="sxs-lookup"><span data-stu-id="d09c7-129">Next Steps</span></span>

<span data-ttu-id="d09c7-130">Azure PowerShell の使用について詳しくは、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-130">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="d09c7-131">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="d09c7-131">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="frequently-asked-questions"></a><span data-ttu-id="d09c7-132">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="d09c7-132">Frequently asked questions</span></span>

### <a id="helpmechoose"></a><span data-ttu-id="d09c7-133">Azure PowerShell のバージョンを確認するには、どうすればよいですか。</span><span class="sxs-lookup"><span data-stu-id="d09c7-133">How do I check the version of Azure PowerShell?</span></span>

<span data-ttu-id="d09c7-134">Azure PowerShell は、できるだけ早く最新バージョンにアップグレードすることをお勧めしますが、いくつかのバージョンがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="d09c7-134">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="d09c7-135">インストールされている Azure PowerShell のバージョンを確認するには、コマンド ラインから `Get-Module AzureRM` を実行します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-135">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a><span data-ttu-id="d09c7-136">Azure クラシックのデプロイに Azure PowerShell を使用できますか。</span><span class="sxs-lookup"><span data-stu-id="d09c7-136">Can I use Azure PowerShell for Azure Classic deployments?</span></span>

<span data-ttu-id="d09c7-137">クラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-137">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="d09c7-138">詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d09c7-138">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="d09c7-139">Azure と AzureRM のモジュールは、依存するコンポーネントが共通しています。</span><span class="sxs-lookup"><span data-stu-id="d09c7-139">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="d09c7-140">Azure と AzureRM の両方のモジュールを使用する場合は、各パッケージの同じバージョンをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09c7-140">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><span data-ttu-id="d09c7-141"><a name="multiple-versions"/>複数のバージョンの Azure PowerShell をインストールできますか。</span><span class="sxs-lookup"><span data-stu-id="d09c7-141"><a name="multiple-versions"/>Can I install multiple versions of Azure PowerShell?</span></span>

<span data-ttu-id="d09c7-142">PowerShellGet を使用したインストールのみが、複数のバージョンのインストールに対応しています。</span><span class="sxs-lookup"><span data-stu-id="d09c7-142">PowerShellGet the only method of installation that supports multiple versions.</span></span> <span data-ttu-id="d09c7-143">複数のバージョンをインストールするには、`-RequiredVersion` パラメーターを `Install-Module` コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-143">To install multiple versions, you can add the `-RequiredVersion` parameter to the `Install-Module` cmdlet.</span></span> <span data-ttu-id="d09c7-144">たとえば、バージョン 6.1.0 と 1.2.9 の両方をインストールするには、次を実行します。</span><span class="sxs-lookup"><span data-stu-id="d09c7-144">For example, to install both versions 6.1.0 and 1.2.9:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="d09c7-145">PowerShell セッションに読み込むことができるモジュールのバージョンは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="d09c7-145">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="d09c7-146">特定のバージョンの Azure PowerShell モジュールをインポートするには、新しい PowerShell ウィンドウを開いて `Import-Module` を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d09c7-146">You must open a new PowerShell window and use `Import-Module` to import a specific version of the Azure PowerShell module.</span></span>

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="d09c7-147">共存インストールでの使用が想定された最初のモジュール バージョンは、バージョン 2.1.0 とバージョン 1.2.6 です。</span><span class="sxs-lookup"><span data-stu-id="d09c7-147">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="d09c7-148">以前のバージョンの Azure PowerShell を読み込むと、互換性のないバージョンの **AzureRM.Profile** モジュールが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-148">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="d09c7-149">このため、コマンドレットでは、コマンドレットを実行するたびにログインを要求されます。</span><span class="sxs-lookup"><span data-stu-id="d09c7-149">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>
