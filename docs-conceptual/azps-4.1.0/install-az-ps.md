---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/14/2020
ms.openlocfilehash: d3bed5a96af6bed16cda971a1a40b8416a1b115b
ms.sourcegitcommit: 10ec909100a70acec94d42f6084e7bf0342c6854
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "83630760"
---
# <a name="install-azure-powershell"></a><span data-ttu-id="98104-103">Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="98104-103">Install Azure PowerShell</span></span>

<span data-ttu-id="98104-104">この記事では、[PowerShellGet](/powershell/scripting/gallery/installing-psget) を使用して Azure PowerShell モジュールをインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="98104-104">This article explains how to install the Azure PowerShell modules using [PowerShellGet](/powershell/scripting/gallery/installing-psget).</span></span> <span data-ttu-id="98104-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="98104-105">These instructions work on Windows, macOS, and Linux platforms.</span></span>

<span data-ttu-id="98104-106">Azure PowerShell は Azure [Cloud Shell](/azure/cloud-shell/overview) でも利用でき、現在は [Docker イメージ](azureps-in-docker.md)にプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="98104-106">Azure PowerShell is also available in Azure [Cloud Shell](/azure/cloud-shell/overview) and is now preinstalled in [Docker images](azureps-in-docker.md).</span></span>

## <a name="requirements"></a><span data-ttu-id="98104-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="98104-107">Requirements</span></span>

> [!NOTE]
> <span data-ttu-id="98104-108">Powershell 7.x 以降が、すべてのプラットフォームで Azure PowerShell に使用できる PowerShell の推奨バージョンです。</span><span class="sxs-lookup"><span data-stu-id="98104-108">PowerShell 7.x and later is the recommended version of PowerShell for use with Azure PowerShell on all platforms.</span></span>

<span data-ttu-id="98104-109">Azure PowerShell は、どのプラットフォームでも PowerShell 6.2.4 以降で動作します。</span><span class="sxs-lookup"><span data-stu-id="98104-109">Azure PowerShell works with PowerShell 6.2.4 and later on all platforms.</span></span> <span data-ttu-id="98104-110">また、Windows 上では PowerShell 5.1 でもサポートされます。</span><span class="sxs-lookup"><span data-stu-id="98104-110">It is also supported with PowerShell 5.1 on Windows.</span></span> <span data-ttu-id="98104-111">お使いのオペレーティング システムで利用できる[最新バージョンの PowerShell](/powershell/scripting/install/installing-powershell) をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="98104-111">Install the [latest version of PowerShell](/powershell/scripting/install/installing-powershell) available for your operating system.</span></span> <span data-ttu-id="98104-112">PowerShell 6.2.4 上で実行する場合、Azure PowerShell にその他の要件はありません。</span><span class="sxs-lookup"><span data-stu-id="98104-112">Azure PowerShell has no additional requirements when run on PowerShell 6.2.4 and later.</span></span>

<span data-ttu-id="98104-113">PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="98104-113">To check your PowerShell version, run the command:</span></span>

```azurepowershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="98104-114">Windows 上の PowerShell 5.1 で Azure PowerShell を使用するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="98104-114">To use Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="98104-115">[Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。</span><span class="sxs-lookup"><span data-stu-id="98104-115">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell).</span></span>
   <span data-ttu-id="98104-116">Windows 10 バージョン 1607 以降の場合は、あらかじめ PowerShell 5.1 がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="98104-116">If you're on Windows 10 version 1607 or higher, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="98104-117">[.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="98104-117">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>
3. <span data-ttu-id="98104-118">最新バージョンの PowerShellGet がインストールされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="98104-118">Make sure you have the latest version of PowerShellGet.</span></span> <span data-ttu-id="98104-119">`Install-Module -Name PowerShellGet -Force` を実行します。</span><span class="sxs-lookup"><span data-stu-id="98104-119">Run `Install-Module -Name PowerShellGet -Force`.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="98104-120">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="98104-120">Install the Azure PowerShell module</span></span>

> [!WARNING]
> <span data-ttu-id="98104-121">Windows では PowerShell 5.1 に対して AzureRM と Az の両方のモジュールを同時にインストールすることはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="98104-121">We do not support having both the AzureRM and Az modules installed for PowerShell 5.1 on Windows at the same time.</span></span> <span data-ttu-id="98104-122">AzureRM をシステムで引き続き使用できるようにしておく必要がある場合は、PowerShell 6.2.4 以降用の Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="98104-122">If you need to keep AzureRM available on your system, install the Az module for PowerShell 6.2.4 or later.</span></span>

<span data-ttu-id="98104-123">推奨されるインストール方法は、PowerShellGet コマンドレットを使用することです。</span><span class="sxs-lookup"><span data-stu-id="98104-123">Using the PowerShellGet cmdlets is the preferred installation method.</span></span> <span data-ttu-id="98104-124">Az モジュールは現在のユーザーのみを対象としてインストールします。</span><span class="sxs-lookup"><span data-stu-id="98104-124">Install the Az module for the current user only.</span></span> <span data-ttu-id="98104-125">これが推奨されるインストール範囲です。</span><span class="sxs-lookup"><span data-stu-id="98104-125">This is the recommended installation scope.</span></span> <span data-ttu-id="98104-126">この方法は、Windows、macOS、Linux プラットフォーム上で同じように利用できます。</span><span class="sxs-lookup"><span data-stu-id="98104-126">This method works the same on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="98104-127">PowerShell セッションから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="98104-127">Run the following command from a PowerShell session:</span></span>

```powershell-interactive
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message 'Az module not installed. Having both the AzureRM and Az modules installed at the same time is not supported.'
} else {
    Install-Module -Name Az -AllowClobber -Scope CurrentUser
}
```

<span data-ttu-id="98104-128">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されていないため、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="98104-128">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet and you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the `Set-PSRepository` cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="98104-129">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="98104-129">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="98104-130">システム上のすべてのユーザーに対してモジュールをインストールするには、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="98104-130">Installing the module for all users on a system requires elevated privileges.</span></span> <span data-ttu-id="98104-131">Windows で **[管理者として実行]** を使用するか、macOS または Linux 上で `sudo` コマンドを使用して、PowerShell セッションを開始します。</span><span class="sxs-lookup"><span data-stu-id="98104-131">Start the PowerShell session using **Run as administrator** in Windows or use the `sudo` command on macOS or Linux:</span></span>

```powershell-interactive
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message 'Az module not installed. Having both the AzureRM and Az modules installed at the same time is not supported.'
} else {
    Install-Module -Name Az -AllowClobber -Scope AllUsers
}
```

<span data-ttu-id="98104-132">Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="98104-132">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="98104-133">これをインストールすると、一般公開されている Az PowerShell モジュールがすべてダウンロードされ、そのコマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="98104-133">Installing it downloads all of the generally available Az PowerShell modules, and makes their cmdlets available for use.</span></span>

## <a name="install-offline"></a><span data-ttu-id="98104-134">オフラインでインストールする</span><span class="sxs-lookup"><span data-stu-id="98104-134">Install offline</span></span>

<span data-ttu-id="98104-135">環境によっては、PowerShell ギャラリーに接続できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="98104-135">In some environments, it's not possible to connect to the PowerShell Gallery.</span></span> <span data-ttu-id="98104-136">そのような場合でも、次のいずれかの方法を使用してオフラインでインストールできます。</span><span class="sxs-lookup"><span data-stu-id="98104-136">In those situations, you can still install offline using one of these methods:</span></span>

* <span data-ttu-id="98104-137">モジュールをネットワーク内の別の場所にダウンロードし、それをインストール ソースとして使用します。</span><span class="sxs-lookup"><span data-stu-id="98104-137">Download the modules to another location in your network and use that as an installation source.</span></span>
  <span data-ttu-id="98104-138">この方法により、1 台のサーバーまたはファイル共有に PowerShell モジュールをキャッシュして、任意の接続されていないシステムに PowerShellGet でデプロイすることができます。</span><span class="sxs-lookup"><span data-stu-id="98104-138">This method allows you to cache PowerShell modules on a single server or file share to be deployed with PowerShellGet to any disconnected systems.</span></span> <span data-ttu-id="98104-139">ローカル リポジトリを設定して、切断されたシステムにインストールする方法については、「[ローカルの PowerShellGet リポジトリの操作](/powershell/scripting/gallery/how-to/working-with-local-psrepositories)」で説明されています。</span><span class="sxs-lookup"><span data-stu-id="98104-139">Learn how to set up a local repository and install on disconnected systems with [Working with local PowerShellGet repositories](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span></span>
* <span data-ttu-id="98104-140">ネットワークに接続されているコンピューターに [Azure PowerShell MSI をダウンロード](install-az-ps-msi.md)し、PowerShell ギャラリーにアクセスできないシステムにインストーラーをコピーします。</span><span class="sxs-lookup"><span data-stu-id="98104-140">[Download the Azure PowerShell MSI](install-az-ps-msi.md) to a machine connected to the network, and then copy the installer to systems without access to PowerShell Gallery.</span></span> <span data-ttu-id="98104-141">MSI インストーラーは、Windows 上の PowerShell 5.1 でのみ動作することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="98104-141">Keep in mind that the MSI installer only works for PowerShell 5.1 on Windows.</span></span>
* <span data-ttu-id="98104-142">モジュールを [Save-Module](/powershell/module/PowershellGet/Save-Module) を使用してファイル共有に保存するか、別のソースに保存して他のコンピューターに手動でコピーします。</span><span class="sxs-lookup"><span data-stu-id="98104-142">Save the module with [Save-Module](/powershell/module/PowershellGet/Save-Module) to a file share, or save it to another source and manually copy it to other machines:</span></span>

  ```powershell-interactive
  Save-Module -Name Az -Path '\\server\share\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a><span data-ttu-id="98104-143">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="98104-143">Troubleshooting</span></span>

<span data-ttu-id="98104-144">ここでは、Azure PowerShell モジュールのインストール時に発生する一般的な問題をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="98104-144">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="98104-145">ここに示されていない問題が発生した場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="98104-145">If you experience a problem not listed here, [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="98104-146">プロキシによる接続のブロック</span><span class="sxs-lookup"><span data-stu-id="98104-146">Proxy blocks connection</span></span>

<span data-ttu-id="98104-147">PowerShell ギャラリーにアクセスできないことを示すエラーが `Install-Module` から発生した場合は、プロキシの内側にいる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="98104-147">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="98104-148">システム全体のプロキシを構成するための要件は、オペレーティング システムとネットワーク環境によってさまざまに異なります。</span><span class="sxs-lookup"><span data-stu-id="98104-148">Different operating systems and network environment have different requirements for configuring a system-wide proxy.</span></span> <span data-ttu-id="98104-149">プロキシ設定と、ご使用の環境での構成方法については、システム管理者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="98104-149">Contact your system administrator for your proxy settings and how to configure them for your environment.</span></span>

<span data-ttu-id="98104-150">PowerShell 自体は、このプロキシを自動的に使用するように構成されていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="98104-150">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="98104-151">PowerShell 5.1 以降では、次のコマンドを使用して、プロキシを使用するように PowerShell セッションを構成します。</span><span class="sxs-lookup"><span data-stu-id="98104-151">With PowerShell 5.1 and later, configure the PowerShell session to use a proxy using the following commands:</span></span>

```powershell
$webClient = New-Object System.Net.WebClient
$webClient.Proxy.Credentials = [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="98104-152">オペレーティング システムの資格情報が正しく構成されている場合は、この構成により PowerShell 要求がプロキシ経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="98104-152">If your operating system credentials are configured correctly, this configuration routes PowerShell requests through the proxy.</span></span> <span data-ttu-id="98104-153">この設定をセッション間で保持するには、このコマンドを [PowerShell プロファイル](/powershell/module/microsoft.powershell.core/about/about_profiles)に追加します。</span><span class="sxs-lookup"><span data-stu-id="98104-153">To have this setting persist between sessions, add the commands to your [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="98104-154">パッケージをインストールするには、プロキシで次のアドレスへの HTTPS 接続を許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-154">To install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="98104-155">サインイン</span><span class="sxs-lookup"><span data-stu-id="98104-155">Sign in</span></span>

<span data-ttu-id="98104-156">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="98104-156">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
> <span data-ttu-id="98104-157">モジュールの自動読み込みを無効にしている場合は、`Import-Module -Name Az` を使用してモジュールを手動でインポートします。</span><span class="sxs-lookup"><span data-stu-id="98104-157">If you've disabled module autoloading, manually import the module with `Import-Module -Name Az`.</span></span>
> <span data-ttu-id="98104-158">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="98104-158">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="98104-159">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-159">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="98104-160">Azure サインインを PowerShell セッション間で維持する方法については、[PowerShell セッション間でのユーザー資格情報の保持](context-persistence.md)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="98104-160">To learn how to persist your Azure sign in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="98104-161">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="98104-161">Update the Azure PowerShell module</span></span>

<span data-ttu-id="98104-162">PowerShell モジュールを更新するには、モジュールのインストールに使用したのと同じ方法を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-162">To update any PowerShell module, you should use the same method used to install the module.</span></span> <span data-ttu-id="98104-163">たとえば、最初に `Install-Module` を使用した場合は、[Update-Module](/powershell/module/powershellget/update-module) を使用して最新バージョンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-163">For example, if you originally used `Install-Module`, then you should use [Update-Module](/powershell/module/powershellget/update-module) to get the latest version.</span></span> <span data-ttu-id="98104-164">最初に MSI パッケージを使用した場合は、新しい MSI をダウンロードしてインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-164">If you originally used the MSI package then you should download and install the new MSI package.</span></span>

<span data-ttu-id="98104-165">PowerShellGet コマンドレットは、MSI パッケージからインストールされたモジュールを更新できません。</span><span class="sxs-lookup"><span data-stu-id="98104-165">The PowerShellGet cmdlets cannot update modules that were installed from an MSI package.</span></span> <span data-ttu-id="98104-166">MSI パッケージは、PowerShellGet を使用してインストールされたモジュールを更新しません。</span><span class="sxs-lookup"><span data-stu-id="98104-166">MSI packages do not update modules that were installed using PowerShellGet.</span></span> <span data-ttu-id="98104-167">PowershellGet を使用した更新で問題が発生した場合は、**更新**ではなく**再インストール**を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-167">If you have any issues updating using PowershellGet, then you should **reinstall**, rather than **update**.</span></span> <span data-ttu-id="98104-168">再インストールはインストールと同じ方法で行いますが、`-Force` パラメーターを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="98104-168">Reinstalling is done the same way as installing, but you need to add the `-Force` parameter:</span></span>

```powershell
if (Get-Module -Name AzureRM -ListAvailable) {
    Write-Warning -Message 'Az module not installed. Having both the AzureRM and Az modules installed at the same time is not supported.'
} else {
    Install-Module -Name Az -AllowClobber -Force
}
```

<span data-ttu-id="98104-169">MSI ベースのインストールとは異なり、PowerShellGet を使用してインストールまたは更新を行っても、システム上に存在する古いバージョンは削除されません。</span><span class="sxs-lookup"><span data-stu-id="98104-169">Unlike MSI-based installations, installing or updating using PowerShellGet does not remove older versions that may exist on your system.</span></span> <span data-ttu-id="98104-170">古いバージョンの Azure PowerShell をシステムから削除する方法については、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98104-170">To remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span> <span data-ttu-id="98104-171">MSI ベースのインストールの詳細については、「[MSI を使用して Azure PowerShell をインストールする](install-az-ps-msi.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98104-171">For more information about MSI-based installations, see [Install Azure PowerShell with an MSI](install-az-ps-msi.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="98104-172">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="98104-172">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="98104-173">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="98104-173">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="98104-174">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="98104-174">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | Select-Object -Property Name, Version
```

<span data-ttu-id="98104-175">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="98104-175">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="98104-176">複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="98104-176">If you have more than one version of the module installed, module autoload, and `Import-Module` load the latest version by default.</span></span>

<span data-ttu-id="98104-177">特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` パラメーターを使用できます。</span><span class="sxs-lookup"><span data-stu-id="98104-177">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` parameter:</span></span>

```powershell-interactive
# Install Az version 3.6.1
Install-Module -Name Az -RequiredVersion 3.6.1
# Load Az version 3.6.1
Import-Module -Name Az -RequiredVersion 3.6.1
```

## <a name="provide-feedback"></a><span data-ttu-id="98104-178">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="98104-178">Provide feedback</span></span>

<span data-ttu-id="98104-179">Azure PowerShell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="98104-179">If you find a bug in Azure PowerShell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="98104-180">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="98104-180">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="98104-181">次の手順</span><span class="sxs-lookup"><span data-stu-id="98104-181">Next Steps</span></span>

<span data-ttu-id="98104-182">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="98104-182">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span> <span data-ttu-id="98104-183">Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="98104-183">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
