---
title: Azure PowerShell のインストールおよび構成 | Microsoft Docs
description: 初めて使う Azure PowerShell をインストールして構成する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/27/2018
ms.openlocfilehash: 7b099fead7cb985fc8f7e6fed55b8c1107caa0d9
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "75720380"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a><span data-ttu-id="0dae2-103">PowerShellGet を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="0dae2-103">Install Azure PowerShell on Windows with PowerShellGet</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="0dae2-104">この記事では、PowerShellGet を使用して、Windows 用 PowerShell 5.x の Azure PowerShell モジュールをインストールする手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-104">This article explains the steps to install the Azure PowerShell modules for PowerShell 5.x for Windows using PowerShellGet.</span></span> <span data-ttu-id="0dae2-105">Azure PowerShell をインストールするときは、PowerShellGet およびモジュール管理を使用することをお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、[その他のインストール方法](other-install.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-105">PowerShellGet and module management is the preferred way to install Azure PowerShell but if you would rather install with the Web Platform Installer or MSI package, see [Other installation methods](other-install.md).</span></span>

<span data-ttu-id="0dae2-106">このバージョンの Azure PowerShell では、Azure クラシック デプロイ モデルはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dae2-106">The Azure classic deployment model is not supported by this version of Azure PowerShell.</span></span> <span data-ttu-id="0dae2-107">クラシック デプロイのサポートについては、「[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)」の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-107">For support for classic deployments, follow the instructions in [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0dae2-108">AzureRM モジュールは、macOS または Linux ではサポートされません。</span><span class="sxs-lookup"><span data-stu-id="0dae2-108">The AzureRM module is not supported for macOS or Linux.</span></span> <span data-ttu-id="0dae2-109">これらのプラットフォームで Azure PowerShell コマンドレットを使用するには、[Az モジュールをインストール](/powershell/azure/install-az-ps)します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-109">To use Azure PowerShell cmdlets on these platforms, [Install the Az module](/powershell/azure/install-az-ps).</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="0dae2-110">手順 1: PowerShellGet をインストールする</span><span class="sxs-lookup"><span data-stu-id="0dae2-110">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="0dae2-111">PowerShell ギャラリーからソフトウェアをインストールするには、PowerShellGet モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="0dae2-111">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="0dae2-112">PowerShellGet のバージョンが適切であるかなど、システム要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-112">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="0dae2-113">ご使用のシステムに PowerShellGet がインストールされているかどうかを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-113">Run the following command to see if you have PowerShellGet installed on your system.</span></span>


```powershell-interactive
Get-InstalledModule -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

<span data-ttu-id="0dae2-114">次のような出力結果が表示されます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-114">You should see something similar to the following output:</span></span>

```Output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="0dae2-115">PowerShellGet バージョン 1.1.2.0 以降が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dae2-115">You need PowerShellGet version 1.1.2.0 or higher.</span></span> <span data-ttu-id="0dae2-116">PowerShellGet を更新するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-116">To update PowerShellGet, use the following command:</span></span>

```powershell-interactive
Install-Module PowerShellGet -Force
```

<span data-ttu-id="0dae2-117">PowerShellGet がインストールされていない場合は、この記事の「[PowerShellGet の入手方法](#how-to-get-powershellget)」のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-117">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget) section of this article.</span></span>

> [!NOTE]
> <span data-ttu-id="0dae2-118">PowerShellGet を使用するには、実行ポリシーでスクリプトの実行が許可されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-118">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="0dae2-119">PowerShell の実行ポリシーについて詳しくは、「[About Execution Policies (実行ポリシーについて)](/powershell/module/microsoft.powershell.core/about/about_execution_policies)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-119">For more information about PowerShell's Execution Policy, see [About Execution Policies](/powershell/module/microsoft.powershell.core/about/about_execution_policies).</span></span>
>
> [!IMPORTANT]
> <span data-ttu-id="0dae2-120">このドキュメントで説明するモジュール AzureRM では、.NET Framework を使用します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-120">The module described in this document, AzureRM, uses .NET Framework.</span></span> <span data-ttu-id="0dae2-121">そのため、.NET Core を使用する PowerShell 6.0 とは互換性がなくなります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-121">This makes it incompatible with PowerShell 6.0, which uses .NET Core.</span></span> <span data-ttu-id="0dae2-122">PowerShell 6.0 を使用している場合は、[macOS および Linux のインストール手順](install-azurermps-maclinux.md)に従います。</span><span class="sxs-lookup"><span data-stu-id="0dae2-122">If you are using PowerShell 6.0, follow the [installation instructions for macOS and Linux](install-azurermps-maclinux.md).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="0dae2-123">手順 2: Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="0dae2-123">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="0dae2-124">Azure PowerShell を PowerShell ギャラリーからインストールするためには、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dae2-124">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="0dae2-125">管理者特権の PowerShell セッションから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-125">Run the following command from an elevated PowerShell session:</span></span>

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

<span data-ttu-id="0dae2-126">既定では、PowerShell ギャラリーは PowerShellGet の信頼できるリポジトリとして構成されていません。</span><span class="sxs-lookup"><span data-stu-id="0dae2-126">By default, the PowerShell gallery is not configured as a Trusted repository for PowerShellGet.</span></span> <span data-ttu-id="0dae2-127">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-127">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

<span data-ttu-id="0dae2-128">インストールを続行するには、"Yes" または "Yes to All" と回答します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-128">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="0dae2-129">ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-129">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="0dae2-130">AzureRM モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="0dae2-130">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="0dae2-131">AzureRM モジュールをインストールすると、まだインストールしていない Azure PowerShell モジュールが PowerShell ギャラリーからダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-131">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded and from the PowerShell Gallery.</span></span>

<span data-ttu-id="0dae2-132">以前のバージョンの Azure PowerShell がインストールされている場合、エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-132">If you have a previous version of Azure PowerShell installed you may receive an error.</span></span> <span data-ttu-id="0dae2-133">この問題を解決するには、この記事の「[新しいバージョンの Azure PowerShell に更新する](#update-azps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-133">To resolve this issue, see the [Updating to a new version of Azure PowerShell](#update-azps) section of this article.</span></span>

## <a name="step-3-load-the-azurerm-module"></a><span data-ttu-id="0dae2-134">手順 3: AzureRM モジュールを読み込む</span><span class="sxs-lookup"><span data-stu-id="0dae2-134">Step 3: Load the AzureRM module</span></span>

<span data-ttu-id="0dae2-135">モジュールは、インストール後、PowerShell セッションに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-135">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="0dae2-136">これは通常の (管理者特権ではない) PowerShell セッションで実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-136">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="0dae2-137">モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="0dae2-137">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell-interactive
Import-Module -Name AzureRM
```

## <a name="next-steps"></a><span data-ttu-id="0dae2-138">次の手順</span><span class="sxs-lookup"><span data-stu-id="0dae2-138">Next Steps</span></span>

<span data-ttu-id="0dae2-139">Azure PowerShell の使用について詳しくは、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-139">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="0dae2-140">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="0dae2-140">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="0dae2-141">問題とフィードバックの報告</span><span class="sxs-lookup"><span data-stu-id="0dae2-141">Reporting issues and feedback</span></span>

<span data-ttu-id="0dae2-142">ツールにバグを発見した場合は、GitHub リポジトリの [[Issues (問題)]](https://github.com/Azure/azure-powershell/issues) セクションで問題を報告してください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-142">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-powershell/issues) section of our GitHub repo.</span></span> <span data-ttu-id="0dae2-143">コマンド ラインからフィードバックを送るには、`Send-Feedback` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-143">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="0dae2-144">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="0dae2-144">Frequently asked questions</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="0dae2-145">PowerShellGet の入手方法</span><span class="sxs-lookup"><span data-stu-id="0dae2-145">How to get PowerShellGet</span></span>

|<span data-ttu-id="0dae2-146">OS バージョン</span><span class="sxs-lookup"><span data-stu-id="0dae2-146">OS Version</span></span>|<span data-ttu-id="0dae2-147">インストール手順</span><span class="sxs-lookup"><span data-stu-id="0dae2-147">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="0dae2-148">Windows 10 または Windows Server 2016 を所有している</span><span class="sxs-lookup"><span data-stu-id="0dae2-148">I have Windows 10 or Windows Server 2016</span></span>|<span data-ttu-id="0dae2-149">OS 標準の Windows Management Framework (WMF) 5.0 に組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="0dae2-149">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="0dae2-150">PowerShell 5 にアップグレードしたい</span><span class="sxs-lookup"><span data-stu-id="0dae2-150">I want to upgrade to PowerShell 5</span></span>|<span data-ttu-id="0dae2-151">[最新バージョンの WMF をインストール](https://www.microsoft.com/download/details.aspx?id=54616)します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-151">[Install the latest version of WMF](https://www.microsoft.com/download/details.aspx?id=54616)</span></span>|
|<span data-ttu-id="0dae2-152">PowerShell 3 または PowerShell 4 が付属するバージョンの Windows を使っている</span><span class="sxs-lookup"><span data-stu-id="0dae2-152">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|<span data-ttu-id="0dae2-153">[PackageManagement モジュールを入手](https://go.microsoft.com/fwlink/?LinkID=746217)します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-153">[Get the PackageManagement modules](https://go.microsoft.com/fwlink/?LinkID=746217)</span></span>|

### <a name="div-idhelpmechoosechecking-the-version-of-azure-powershell"></a><div id="helpmechoose"/><span data-ttu-id="0dae2-154">Azure PowerShell のバージョン確認</span><span class="sxs-lookup"><span data-stu-id="0dae2-154">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="0dae2-155">Azure PowerShell は、できるだけ早く最新バージョンにアップグレードすることをお勧めしますが、いくつかのバージョンがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="0dae2-155">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="0dae2-156">インストールされている Azure PowerShell のバージョンを確認するには、コマンド ラインから `Get-InstalledModule AzureRM` を実行します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-156">To determine the version of Azure PowerShell you have installed, run `Get-InstalledModule AzureRM` from your command line.</span></span>

```powershell-interactive
Get-InstalledModule AzureRM -AllVersions | Select-Object -Property Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a><span data-ttu-id="0dae2-157">クラシック デプロイ方法のサポート</span><span class="sxs-lookup"><span data-stu-id="0dae2-157">Support for classic deployment methods</span></span>

<span data-ttu-id="0dae2-158">クラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-158">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="0dae2-159">詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-159">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="0dae2-160">Azure と AzureRM のモジュールは、依存するコンポーネントが共通しています。</span><span class="sxs-lookup"><span data-stu-id="0dae2-160">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="0dae2-161">Azure と AzureRM の両方のモジュールを使用する場合は、各パッケージの同じバージョンをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-161">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <a name="div-idupdate-azpsupdating-to-a-new-version-of-azure-powershell"></a><div id="update-azps"/><span data-ttu-id="0dae2-162">新しいバージョンの Azure PowerShell に更新する</span><span class="sxs-lookup"><span data-stu-id="0dae2-162">Updating to a new version of Azure PowerShell</span></span>

<span data-ttu-id="0dae2-163">Service Management モジュールを含む、以前のバージョンの Azure PowerShell がインストールされている場合は、次のエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-163">If you have a previous version of Azure PowerShell installed that includes the Service Management module, you may receive the following error:</span></span>

```Output
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

<span data-ttu-id="0dae2-164">エラー メッセージが示すように、AllowClobber パラメーターを使用してモジュールをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-164">As the error message states, you need to use the -AllowClobber parameter to install the module.</span></span> <span data-ttu-id="0dae2-165">次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="0dae2-165">Use the following command:</span></span>

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

<span data-ttu-id="0dae2-166">詳細については、[Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module) に関するヘルプ トピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-166">For more information, see the help topic for [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span></span>

### <a name="installing-module-versions-side-by-side"></a><span data-ttu-id="0dae2-167">サイド バイ サイド構成でのモジュール バージョンのインストール</span><span class="sxs-lookup"><span data-stu-id="0dae2-167">Installing module versions side by side</span></span>

<span data-ttu-id="0dae2-168">複数バージョンのインストールに対応しているのは、PowerShellGet を使ったインストール方法だけです。</span><span class="sxs-lookup"><span data-stu-id="0dae2-168">The PowerShellGet method of installation is the only method that supports the installation of multiple versions.</span></span> <span data-ttu-id="0dae2-169">たとえば、以前のバージョンの Azure PowerShell で記述されたスクリプトがあり、更新する時間も人材も確保できないことがあります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-169">For example, you may have scripts written using a previous version of Azure PowerShell that you don't have the time or resources to updated.</span></span> <span data-ttu-id="0dae2-170">次のコマンドで、複数バージョンの Azure PowerShell をインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-170">The following commands illustrate how to install multiple versions of Azure PowerShell:</span></span>

```powershell-interactive
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

<span data-ttu-id="0dae2-171">PowerShell セッションに読み込むことができるモジュールのバージョンは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="0dae2-171">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="0dae2-172">特定のバージョンの AzureRM コマンドレットをインポートするには、新たに PowerShell ウィンドウを開いて `Import-Module` を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dae2-172">You must open a new PowerShell window and use `Import-Module` to import a specific version of the AzureRM cmdlets:</span></span>

```powershell-interactive
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

> [!NOTE]
> <span data-ttu-id="0dae2-173">共存インストールでの使用が想定された最初のモジュール バージョンは、バージョン 2.1.0 とバージョン 1.2.6 です。</span><span class="sxs-lookup"><span data-stu-id="0dae2-173">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="0dae2-174">以前のバージョンの Azure PowerShell を読み込むと、互換性のないバージョンの **AzureRM.Profile** モジュールが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-174">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="0dae2-175">このため、コマンドレットでは、コマンドレットを実行するたびにサインインを要求されます。</span><span class="sxs-lookup"><span data-stu-id="0dae2-175">This results in the cmdlets prompting you to sign in whenever you execute a cmdlet.</span></span>

### <a name="other-installation-methods"></a><span data-ttu-id="0dae2-176">その他のインストール方法</span><span class="sxs-lookup"><span data-stu-id="0dae2-176">Other installation methods</span></span>

<span data-ttu-id="0dae2-177">Web プラットフォーム インストーラーまたは MSI パッケージを使ったインストールについては、「[Other installation methods (その他のインストール方法)](other-install.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0dae2-177">For information about installing using the Web Platform Installer or the MSI Package, see [Other installation methods](other-install.md)</span></span>
