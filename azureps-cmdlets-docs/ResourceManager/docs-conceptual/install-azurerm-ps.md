---
title: "Azure PowerShell のインストールおよび構成 | Microsoft Docs"
description: "初めて使う Azure PowerShell をインストールして構成する方法について説明します。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/17/2017
ms.openlocfilehash: 8b82de3634a1492baf54ce4d2172af3e3287229c
ms.sourcegitcommit: db5c50de90764a9bdc7c1f1dbca3aed5bfeb05fa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2017
---
# <a name="install-and-configure-azure-powershell"></a><span data-ttu-id="35f20-103">Azure PowerShell のインストールおよび構成</span><span class="sxs-lookup"><span data-stu-id="35f20-103">Install and configure Azure PowerShell</span></span>

<span data-ttu-id="35f20-104">Azure PowerShell は、PowerShell ギャラリーからインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="35f20-104">Installing Azure PowerShell from the PowerShell Gallery is the preferred method of installation.</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="35f20-105">手順 1: PowerShellGet をインストールする</span><span class="sxs-lookup"><span data-stu-id="35f20-105">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="35f20-106">PowerShell ギャラリーからソフトウェアをインストールするには、PowerShellGet モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="35f20-106">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="35f20-107">PowerShellGet のバージョンが適切であるかなど、システム要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="35f20-107">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="35f20-108">ご使用のシステムに PowerShellGet がインストールされているかどうかを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="35f20-108">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

<span data-ttu-id="35f20-109">次のような出力結果が表示されます。</span><span class="sxs-lookup"><span data-stu-id="35f20-109">You should see something similar to the following output:</span></span>

```
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="35f20-110">PowerShellGet がインストールされていない場合は、この記事の「[PowerShellGet の入手方法](#how-to-get-powershellget)」のセクションをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="35f20-110">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget) section of this article.</span></span>

> [!NOTE]
> <span data-ttu-id="35f20-111">PowerShellGet を使用するには、実行ポリシーでスクリプトの実行が許可されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-111">Using PowerShellGet requires an Execution Policy that allows you to run scripts.</span></span> <span data-ttu-id="35f20-112">PowerShell の実行ポリシーについて詳しくは、「[About Execution Policies (実行ポリシーについて)](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.core/about/about_execution_policies)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="35f20-112">For more information about PowerShell's Execution Policy, see [About Execution Policies](https://msdn.microsoft.com/powershell/reference/5.1/microsoft.powershell.core/about/about_execution_policies).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="35f20-113">手順 2: Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="35f20-113">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="35f20-114">Azure PowerShell を PowerShell ギャラリーからインストールするためには、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="35f20-114">Installing Azure PowerShell from the PowerShell Gallery requires elevated privileges.</span></span> <span data-ttu-id="35f20-115">管理者特権の PowerShell セッションから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="35f20-115">Run the following command from an elevated PowerShell session:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module AzureRM
```

<span data-ttu-id="35f20-116">既定では、PowerShell ギャラリーは PowerShellGet の信頼できるリポジトリとして構成されていません。</span><span class="sxs-lookup"><span data-stu-id="35f20-116">By default, the PowerShell gallery is not configured as a Trusted repository for PowerShellGet.</span></span> <span data-ttu-id="35f20-117">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="35f20-117">The first time you use the PSGallery you see the following prompt:</span></span>

```
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

<span data-ttu-id="35f20-118">インストールを続行するには、"Yes" または "Yes to All" と回答します。</span><span class="sxs-lookup"><span data-stu-id="35f20-118">Answer 'Yes' or 'Yes to All' to continue with the installation.</span></span>

> [!NOTE]
> <span data-ttu-id="35f20-119">ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。</span><span class="sxs-lookup"><span data-stu-id="35f20-119">If you have a version older than 2.8.5.201 of NuGet, you are prompted to download and install the latest version of NuGet.</span></span>

<span data-ttu-id="35f20-120">AzureRM モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="35f20-120">The AzureRM module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="35f20-121">AzureRM モジュールをインストールすると、まだインストールしていない Azure PowerShell モジュールが PowerShell ギャラリーからダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="35f20-121">When you install the AzureRM module, any Azure PowerShell module not previously installed is downloaded and from the PowerShell Gallery.</span></span>

<span data-ttu-id="35f20-122">以前のバージョンの Azure PowerShell がインストールされている場合、エラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-122">If you have a previous version of Azure PowerShell installed you may receive an error.</span></span> <span data-ttu-id="35f20-123">この問題を解決するには、この記事の「[新しいバージョンの Azure PowerShell に更新する](#update-azps)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35f20-123">To resolve this issue, see the [Updating to a new version of Azure PowerShell](#update-azps) section of this article.</span></span>

## <a name="step-3-load-the-azurerm-module"></a><span data-ttu-id="35f20-124">手順 3: AzureRM モジュールを読み込む</span><span class="sxs-lookup"><span data-stu-id="35f20-124">Step 3: Load the AzureRM module</span></span>
<span data-ttu-id="35f20-125">モジュールは、インストール後、PowerShell セッションに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-125">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="35f20-126">これは通常の (管理者特権ではない) PowerShell セッションで実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-126">You should do this in a normal (non-elevated) PowerShell session.</span></span> <span data-ttu-id="35f20-127">モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="35f20-127">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM
```

## <a name="next-steps"></a><span data-ttu-id="35f20-128">次のステップ</span><span class="sxs-lookup"><span data-stu-id="35f20-128">Next Steps</span></span>

<span data-ttu-id="35f20-129">Azure PowerShell の使用について詳しくは、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="35f20-129">For more information about using Azure PowerShell, see the following articles:</span></span>

* [<span data-ttu-id="35f20-130">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="35f20-130">Get started with Azure PowerShell</span></span>](get-started-azureps.md)

## <a name="reporting-issues-and-feedback"></a><span data-ttu-id="35f20-131">問題とフィードバックの報告</span><span class="sxs-lookup"><span data-stu-id="35f20-131">Reporting issues and feedback</span></span>

<span data-ttu-id="35f20-132">ツールにバグを発見した場合は、GitHub リポジトリの [[Issues (問題)]](https://github.com/Azure/azure-powershell/issues) セクションで問題を報告してください。</span><span class="sxs-lookup"><span data-stu-id="35f20-132">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-powershell/issues) section of our GitHub repo.</span></span> <span data-ttu-id="35f20-133">コマンド ラインからフィードバックを送るには、`Send-Feedback` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="35f20-133">To provide feedback from the command line, use the `Send-Feedback` cmdlet.</span></span>

## <a name="frequently-asked-questions"></a><span data-ttu-id="35f20-134">よく寄せられる質問</span><span class="sxs-lookup"><span data-stu-id="35f20-134">Frequently asked questions</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="35f20-135">PowerShellGet の入手方法</span><span class="sxs-lookup"><span data-stu-id="35f20-135">How to get PowerShellGet</span></span>

|<span data-ttu-id="35f20-136">OS バージョン</span><span class="sxs-lookup"><span data-stu-id="35f20-136">OS Version</span></span>|<span data-ttu-id="35f20-137">インストール手順</span><span class="sxs-lookup"><span data-stu-id="35f20-137">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="35f20-138">Windows 10 または Windows Server 2016 を所有している</span><span class="sxs-lookup"><span data-stu-id="35f20-138">I have Windows 10 or Windows Server 2016</span></span>|<span data-ttu-id="35f20-139">OS 標準の Windows Management Framework (WMF) 5.0 に組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="35f20-139">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="35f20-140">PowerShell 5 にアップグレードしたい</span><span class="sxs-lookup"><span data-stu-id="35f20-140">I want to upgrade to PowerShell 5</span></span>|<span data-ttu-id="35f20-141">[最新バージョンの WMF をインストール](https://www.microsoft.com/en-us/download/details.aspx?id=54616)します。</span><span class="sxs-lookup"><span data-stu-id="35f20-141">[Install the latest version of WMF](https://www.microsoft.com/en-us/download/details.aspx?id=54616)</span></span>|
|<span data-ttu-id="35f20-142">PowerShell 3 または PowerShell 4 が付属するバージョンの Windows を使っている</span><span class="sxs-lookup"><span data-stu-id="35f20-142">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|<span data-ttu-id="35f20-143">[PackageManagement モジュールを入手](http://go.microsoft.com/fwlink/?LinkID=746217)します。</span><span class="sxs-lookup"><span data-stu-id="35f20-143">[Get the PackageManagement modules](http://go.microsoft.com/fwlink/?LinkID=746217)</span></span>|

<a id="helpmechoose"></a>
### <a name="checking-the-version-of-azure-powershell"></a><span data-ttu-id="35f20-144">Azure PowerShell のバージョン確認</span><span class="sxs-lookup"><span data-stu-id="35f20-144">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="35f20-145">Azure PowerShell は、できるだけ早く最新バージョンにアップグレードすることをお勧めしますが、いくつかのバージョンがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="35f20-145">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are supported.</span></span> <span data-ttu-id="35f20-146">インストールされている Azure PowerShell のバージョンを確認するには、コマンド ラインから `Get-Module AzureRM` を実行します。</span><span class="sxs-lookup"><span data-stu-id="35f20-146">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -list | Select-Object Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a><span data-ttu-id="35f20-147">クラシック デプロイ方法のサポート</span><span class="sxs-lookup"><span data-stu-id="35f20-147">Support for classic deployment methods</span></span>

<span data-ttu-id="35f20-148">クラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="35f20-148">If you have deployments that use the classic deployment model you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="35f20-149">詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="35f20-149">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span> <span data-ttu-id="35f20-150">Azure と AzureRM のモジュールは、依存するコンポーネントが共通しています。</span><span class="sxs-lookup"><span data-stu-id="35f20-150">The Azure and AzureRM modules share common dependencies.</span></span> <span data-ttu-id="35f20-151">Azure と AzureRM の両方のモジュールを使用する場合は、各パッケージの同じバージョンをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-151">If you use both the Azure and AzureRM modules, you should install the same version of each package.</span></span>

### <span data-ttu-id="35f20-152"><a id="update-azps"></a>新しいバージョンの Azure PowerShell への更新</span><span class="sxs-lookup"><span data-stu-id="35f20-152"><a id="update-azps"></a>Updating to a new version of Azure PowerShell</span></span>

<span data-ttu-id="35f20-153">Service Management モジュールを含む、以前のバージョンの Azure PowerShell がインストールされている場合は、次のエラーが発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-153">If you have a previous version of Azure PowerShell installed that includes the Service Management module, you may receive the following error:</span></span>

```
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

<span data-ttu-id="35f20-154">エラー メッセージが示すように、AllowClobber パラメーターを使用してモジュールをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-154">As the error message states, you need to use the -AllowClobber parameter to install the module.</span></span> <span data-ttu-id="35f20-155">次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="35f20-155">Use the following command:</span></span>

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module AzureRM -AllowClobber
```

<span data-ttu-id="35f20-156">詳細については、[Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module) に関するヘルプ トピックをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="35f20-156">For more information, see the help topic for [Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module).</span></span>

### <a name="installing-module-versions-side-by-side"></a><span data-ttu-id="35f20-157">サイド バイ サイド構成でのモジュール バージョンのインストール</span><span class="sxs-lookup"><span data-stu-id="35f20-157">Installing module versions side by side</span></span>

<span data-ttu-id="35f20-158">複数バージョンのインストールに対応しているのは、PowerShellGet を使ったインストール方法だけです。</span><span class="sxs-lookup"><span data-stu-id="35f20-158">The PowerShellGet method of installation is the only method that supports the installation of multiple versions.</span></span> <span data-ttu-id="35f20-159">たとえば、以前のバージョンの Azure PowerShell で記述されたスクリプトがあり、更新する時間も人材も確保できないことがあります。</span><span class="sxs-lookup"><span data-stu-id="35f20-159">For example, you may have scripts written using a previous version of Azure PowerShell that you don't have the time or resources to updated.</span></span> <span data-ttu-id="35f20-160">次のコマンドで、複数バージョンの Azure PowerShell をインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="35f20-160">The following commands illustrate how to install multiple versions of Azure PowerShell:</span></span>

```powershell
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

<span data-ttu-id="35f20-161">PowerShell セッションに読み込むことができるモジュールのバージョンは 1 つだけです。</span><span class="sxs-lookup"><span data-stu-id="35f20-161">Only one version of the module can be loaded in a PowerShell session.</span></span> <span data-ttu-id="35f20-162">特定のバージョンの AzureRM コマンドレットをインポートするには、新たに PowerShell ウィンドウを開いて `Import-Module` を実行する必要があります。</span><span class="sxs-lookup"><span data-stu-id="35f20-162">You must open a new PowerShell window and use `Import-Module` to import a specific version of the AzureRM cmdlets:</span></span>

```powershell
Import-Module AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> <span data-ttu-id="35f20-163">共存インストールでの使用が想定された最初のモジュール バージョンは、バージョン 2.1.0 とバージョン 1.2.6 です。</span><span class="sxs-lookup"><span data-stu-id="35f20-163">Version 2.1.0 and version 1.2.6 are the first module versions designed to be installed and used side by side.</span></span> <span data-ttu-id="35f20-164">以前のバージョンの Azure PowerShell を読み込むと、互換性のないバージョンの **AzureRM.Profile** モジュールが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="35f20-164">When loading an earlier version of the Azure PowerShell, incompatible versions of the **AzureRM.Profile** module are loaded.</span></span> <span data-ttu-id="35f20-165">このため、コマンドレットでは、コマンドレットを実行するたびにログインを要求されます。</span><span class="sxs-lookup"><span data-stu-id="35f20-165">This results in the cmdlets prompting you to log in whenever you execute a cmdlet.</span></span>

### <a name="other-installation-methods"></a><span data-ttu-id="35f20-166">その他のインストール方法</span><span class="sxs-lookup"><span data-stu-id="35f20-166">Other installation methods</span></span>

<span data-ttu-id="35f20-167">Web プラットフォーム インストーラーまたは MSI パッケージを使ったインストールについては、「[Other installation methods (その他のインストール方法)](other-install.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="35f20-167">For information about installing using the Web Platform Installer or the MSI Package, see [Other installation methods](other-install.md)</span></span>
