---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 21345445efc89ab54bb7483cfe81f439f0a887a3
ms.sourcegitcommit: b02cbcd00748a4a9a4790a5fba229ce53c3bf973
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/09/2019
ms.locfileid: "68861207"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="cf205-103">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="cf205-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="cf205-104">この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="cf205-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="cf205-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="cf205-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="cf205-106">Az モジュールについては、現在他のインストール方法はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf205-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="cf205-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="cf205-107">Requirements</span></span>

<span data-ttu-id="cf205-108">Azure PowerShell は、Windows 上の PowerShell 5.1 以降、またはすべてのプラットフォーム上の PowerShell Core 6.x 以降で動作します。</span><span class="sxs-lookup"><span data-stu-id="cf205-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="cf205-109">PowerShell がインストールされているかどうか、または macOS または Linux かどうか不明な場合な場合は、[最新バージョンの PowerShell Core をインストール](/powershell/scripting/install/installing-powershell#powershell-core)してください。</span><span class="sxs-lookup"><span data-stu-id="cf205-109">If you aren't sure if you have PowerShell, or are on macOS or Linux, [install the latest version of PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span></span>

<span data-ttu-id="cf205-110">PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="cf205-110">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="cf205-111">Windows 上の PowerShell 5.1 で Azure PowerShell を実行するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="cf205-111">To run Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="cf205-112">必要に応じて [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。</span><span class="sxs-lookup"><span data-stu-id="cf205-112">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="cf205-113">Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="cf205-113">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="cf205-114">[.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="cf205-114">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

<span data-ttu-id="cf205-115">PowerShell Core を使用する場合、Azure PowerShell にその他の要件はありません。</span><span class="sxs-lookup"><span data-stu-id="cf205-115">There are no additional requirements for Azure PowerShell when using PowerShell Core.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="cf205-116">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="cf205-116">Install the Azure PowerShell module</span></span>

> [!WARNING]
> <span data-ttu-id="cf205-117">Windows 用の PowerShell 5.1 で AzureRM と Az の両方のモジュールを同時にインストールすることは__できません__。</span><span class="sxs-lookup"><span data-stu-id="cf205-117">You __can't__ have both the AzureRM and Az modules installed for PowerShell 5.1 for Windows at the same time.</span></span> <span data-ttu-id="cf205-118">AzureRM をシステムで引き続き使用できるようにしておく必要がある場合は、PowerShell Core 6.x 以降用の Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="cf205-118">If you need to keep AzureRM available on your system, install the Az module for PowerShell Core 6.x or later.</span></span> <span data-ttu-id="cf205-119">そのためには、[PowerShell Core 6.x 以降をインストール](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows)してから、PowerShell Core ターミナルで以下の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="cf205-119">To do this, [install PowerShell Core 6.x or later](https://docs.microsoft.com/powershell/scripting/install/installing-powershell-core-on-windows) and then follow these instructions in a PowerShell Core terminal.</span></span>

<span data-ttu-id="cf205-120">推奨されるインストール方法として、アクティブ ユーザーにのみインストールします。</span><span class="sxs-lookup"><span data-stu-id="cf205-120">The recommended install method is to only install for the active user:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="cf205-121">システム上のすべてのユーザーに対してインストールする場合は、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="cf205-121">If you want to install for all users on a system, this requires administrator privileges.</span></span> <span data-ttu-id="cf205-122">管理者特権での PowerShell セッションから、管理者として実行するか、macOS または Linux 上で `sudo` コマンドを使用して実行します。</span><span class="sxs-lookup"><span data-stu-id="cf205-122">From an elevated PowerShell session either run as administrator or with the `sudo` command on macOS or Linux:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope AllUsers
```

<span data-ttu-id="cf205-123">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="cf205-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="cf205-124">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="cf205-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="cf205-125">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="cf205-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="cf205-126">Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="cf205-126">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="cf205-127">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="cf205-127">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="cf205-128">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="cf205-128">Troubleshooting</span></span>

<span data-ttu-id="cf205-129">ここでは、Azure PowerShell モジュールのインストール時に発生する一般的な問題をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="cf205-129">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="cf205-130">ここに示されていない問題が発生した場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="cf205-130">If you experience a problem not listed here, please [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="cf205-131">プロキシによる接続のブロック</span><span class="sxs-lookup"><span data-stu-id="cf205-131">Proxy blocks connection</span></span>

<span data-ttu-id="cf205-132">PowerShell ギャラリーにアクセスできないことを示すエラーが `Install-Module` から発生した場合は、プロキシの内側にいる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-132">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="cf205-133">さまざまなオペレーティング システムにシステム全体のプロキシを構成するためのさまざまな要件がありますが、ここではそれについて詳しく説明しません。</span><span class="sxs-lookup"><span data-stu-id="cf205-133">Different operating systems will have different requirements for configuring a system-wide proxy, which are not covered in detail here.</span></span> <span data-ttu-id="cf205-134">プロキシ設定とお使いの OS 用に構成する方法については、システム管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="cf205-134">Contact your system administrator for your proxy settings and how to configure them for your OS.</span></span>

<span data-ttu-id="cf205-135">PowerShell 自体は、このプロキシを自動的に使用するように構成されていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-135">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="cf205-136">PowerShell 5.1 以降は、次のコマンドで PowerShell セッションに使用するプロキシを構成します。</span><span class="sxs-lookup"><span data-stu-id="cf205-136">With PowerShell 5.1 and later, configure the proxy to use for a PowerShell session with the following command:</span></span>

```powershell
(New-Object System.Net.WebClient).Proxy.Credentials = `
  [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="cf205-137">オペレーティング システムの資格情報が正しく構成されている場合は、これにより PowerShell 要求がプロキシ経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="cf205-137">If your operating system credentials are configured correctly, this will route PowerShell requests through the proxy.</span></span>
<span data-ttu-id="cf205-138">この設定をセッション間で保持するためには、このコマンドを [PowerShell プロファイル](/powershell/module/microsoft.powershell.core/about/about_profiles)に追加します。</span><span class="sxs-lookup"><span data-stu-id="cf205-138">In order to have this setting persist between sessions, add the command to a [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="cf205-139">パッケージをインストールするためには、プロキシで次のアドレスへの HTTPS 接続を許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-139">In order to install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="cf205-140">サインイン</span><span class="sxs-lookup"><span data-stu-id="cf205-140">Sign in</span></span>

<span data-ttu-id="cf205-141">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="cf205-141">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="cf205-142">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-142">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="cf205-143">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf205-143">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="cf205-144">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-144">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="cf205-145">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="cf205-145">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="cf205-146">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="cf205-146">Update the Azure PowerShell module</span></span>

<span data-ttu-id="cf205-147">Az モジュールのパッケージ方法のために、[Update-Module](/powershell/module/powershellget/update-module) コマンドではインストールは適切に更新されません。</span><span class="sxs-lookup"><span data-stu-id="cf205-147">Because of how the Az module is packaged, the [Update-Module](/powershell/module/powershellget/update-module) command won't update your installation correctly.</span></span> <span data-ttu-id="cf205-148">Az は技術的にはメタモジュールであり、Azure サービスを操作するためのコマンドレットを含むすべてのサブモジュールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf205-148">Az is technically a meta-module, encompassing all of the submodules that contain cmdlets to interact with Azure services.</span></span> <span data-ttu-id="cf205-149">つまり、Azure PowerShell モジュールを更新するには、__更新__するだけではなく__再インストール__する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-149">That means that to update the Azure PowerShell module, you will need to __reinstall__, rather than just __update__.</span></span> <span data-ttu-id="cf205-150">これはインストールと同じ方法で行いますが、`-Force` 引数を追加する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="cf205-150">This is done in the same way as installing, but you may need to add the `-Force` argument:</span></span>

```powershell
Install-Module -Name Az -AllowClobber -Force
```

<span data-ttu-id="cf205-151">これによりインストールされているモジュールを上書きできますが、システム上には以前のバージョンがそのまま残っていることがあります。</span><span class="sxs-lookup"><span data-stu-id="cf205-151">Although this can overwrite installed modules, you may still have older versions left on your system.</span></span>
<span data-ttu-id="cf205-152">以前のバージョンの Azure PowerShell をシステムから削除する方法については、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-az-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="cf205-152">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="cf205-153">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="cf205-153">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="cf205-154">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="cf205-154">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="cf205-155">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="cf205-155">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="cf205-156">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf205-156">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="cf205-157">特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` 引数を使用できます。</span><span class="sxs-lookup"><span data-stu-id="cf205-157">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="cf205-158">複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="cf205-158">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="cf205-159">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="cf205-159">Provide feedback</span></span>

<span data-ttu-id="cf205-160">Azure Powershell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="cf205-160">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="cf205-161">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="cf205-161">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="cf205-162">次の手順</span><span class="sxs-lookup"><span data-stu-id="cf205-162">Next Steps</span></span>

<span data-ttu-id="cf205-163">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="cf205-163">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="cf205-164">Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf205-164">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
