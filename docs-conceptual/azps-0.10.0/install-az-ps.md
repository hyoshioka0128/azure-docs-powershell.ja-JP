---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/26/2020
ms.openlocfilehash: 7a25270566f5e856ee44c4c191a47a3e7334508b
ms.sourcegitcommit: 4c61442a2df1cee633ce93cad9f6bc793803baa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2020
ms.locfileid: "81445698"
---
# <a name="install-azure-powershell"></a><span data-ttu-id="59846-103">Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="59846-103">Install Azure PowerShell</span></span>

<span data-ttu-id="59846-104">この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="59846-104">This article explains how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="59846-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="59846-105">These instructions work on Windows, macOS, and Linux platforms.</span></span>

<span data-ttu-id="59846-106">Azure PowerShell は Azure [Cloud Shell](/azure/cloud-shell/overview) でも利用でき、現在は [Docker イメージ](azureps-in-docker.md)にプレインストールされています。</span><span class="sxs-lookup"><span data-stu-id="59846-106">Azure PowerShell is also available in Azure [Cloud Shell](/azure/cloud-shell/overview) and is now preinstalled in [Docker images](azureps-in-docker.md).</span></span>

## <a name="requirements"></a><span data-ttu-id="59846-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="59846-107">Requirements</span></span>

<span data-ttu-id="59846-108">Azure PowerShell は、Windows 上の PowerShell 5.1 以降、またはすべてのプラットフォーム上の PowerShell Core 6.x 以降で動作します。</span><span class="sxs-lookup"><span data-stu-id="59846-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="59846-109">お使いのオペレーティング システムで利用できる[最新バージョンの PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core) をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-109">You should install the [latest version of PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core) available for your operating system.</span></span> <span data-ttu-id="59846-110">PowerShell Core 上で実行する場合、Azure PowerShell にその他の要件はありません。</span><span class="sxs-lookup"><span data-stu-id="59846-110">Azure PowerShell has no additional requirements when run on PowerShell Core.</span></span>

<span data-ttu-id="59846-111">PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="59846-111">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="59846-112">Windows 上の PowerShell 5.1 で Azure PowerShell を使用するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="59846-112">To use Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="59846-113">必要に応じて [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。</span><span class="sxs-lookup"><span data-stu-id="59846-113">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="59846-114">Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="59846-114">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="59846-115">[.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="59846-115">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>
3. <span data-ttu-id="59846-116">最新バージョンの PowerShellGet がインストールされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="59846-116">Make sure you have the latest version of PowerShellGet.</span></span> <span data-ttu-id="59846-117">`Update-Module PowerShellGet -Force` を実行します。</span><span class="sxs-lookup"><span data-stu-id="59846-117">Run `Update-Module PowerShellGet -Force`.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="59846-118">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="59846-118">Install the Azure PowerShell module</span></span>

<span data-ttu-id="59846-119">推奨されるインストール方法は、PowerShellGet コマンドレットを使用することです。</span><span class="sxs-lookup"><span data-stu-id="59846-119">Using the PowerShellGet cmdlets is the preferred installation method.</span></span> <span data-ttu-id="59846-120">この方法は、Windows、macOS、Linux プラットフォーム上で同じように利用できます。</span><span class="sxs-lookup"><span data-stu-id="59846-120">This method works the same on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="59846-121">PowerShell セッションから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="59846-121">Run the following command from a PowerShell session:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="59846-122">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="59846-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="59846-123">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="59846-123">The first time you use the PSGallery you see the following prompt:</span></span>

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the `Set-PSRepository` cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="59846-124">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="59846-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="59846-125">Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="59846-125">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="59846-126">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="59846-126">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

> [!WARNING]
> <span data-ttu-id="59846-127">Windows 用の PowerShell 5.1 に対して AzureRM と Az の両方のモジュールを同時にインストールすることはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59846-127">We do not support having both the AzureRM and Az modules installed for PowerShell 5.1 for Windows at the same time.</span></span> <span data-ttu-id="59846-128">AzureRM をシステムで引き続き使用できるようにしておく必要がある場合は、PowerShell Core 6.x 以降用の Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="59846-128">If you need to keep AzureRM available on your system, install the Az module for PowerShell Core 6.x or later.</span></span>

<span data-ttu-id="59846-129">まず、[PowerShell Core 6.x 以降をインストールします](/powershell/scripting/install/installing-powershell-core-on-windows)。</span><span class="sxs-lookup"><span data-stu-id="59846-129">First, [install PowerShell Core 6.x or later](/powershell/scripting/install/installing-powershell-core-on-windows)</span></span>

<span data-ttu-id="59846-130">次に、PowerShell Core セッションから、現在のユーザーに対してのみ Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="59846-130">Then, from a PowerShell Core session, install the Az module for the current user only.</span></span> <span data-ttu-id="59846-131">これが推奨されるインストール範囲です。</span><span class="sxs-lookup"><span data-stu-id="59846-131">This is the recommended installation scope.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="59846-132">システム上のすべてのユーザーに対してモジュールをインストールするには、管理者特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="59846-132">Installing the module for all users on a system requires elevated privileges.</span></span> <span data-ttu-id="59846-133">Windows で **[管理者として実行]** を使用するか、macOS または Linux 上で `sudo` コマンドを使用して、PowerShell セッションを開始します。</span><span class="sxs-lookup"><span data-stu-id="59846-133">Start the PowerShell session using **Run as administrator** in Windows or use the `sudo` command on macOS or Linux:</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope AllUsers
```

## <a name="install-offline"></a><span data-ttu-id="59846-134">オフラインでインストールする</span><span class="sxs-lookup"><span data-stu-id="59846-134">Install offline</span></span>

<span data-ttu-id="59846-135">環境によっては、PowerShell ギャラリーに接続できない場合があります。</span><span class="sxs-lookup"><span data-stu-id="59846-135">In some environments it's not possible to connect to the PowerShell Gallery.</span></span> <span data-ttu-id="59846-136">そのような場合でも、次のいずれかの方法を使用してオフラインでインストールできます。</span><span class="sxs-lookup"><span data-stu-id="59846-136">In those situations, you can still install offline using one of these methods:</span></span>

* <span data-ttu-id="59846-137">モジュールをネットワーク内の別の場所にダウンロードし、それをインストール ソースとして使用します。</span><span class="sxs-lookup"><span data-stu-id="59846-137">Download the modules to another location in your network and use that as an installation source.</span></span>
  <span data-ttu-id="59846-138">これにより、1 台のサーバーまたはファイル共有に PowerShell モジュールをキャッシュして、任意の接続されていないシステムに PowerShellGet でデプロイすることができます。</span><span class="sxs-lookup"><span data-stu-id="59846-138">This allows you to cache PowerShell modules on a single server or file share to be deployed with PowerShellGet to any disconnected systems.</span></span> <span data-ttu-id="59846-139">ローカル リポジトリを設定して、切断されたシステムにインストールする方法については、「[ローカルの PowerShellGet リポジトリの操作](/powershell/scripting/gallery/how-to/working-with-local-psrepositories)」で説明されています。</span><span class="sxs-lookup"><span data-stu-id="59846-139">Learn how to set up a local repository and install on disconnected systems with [Working with local PowerShellGet repositories](/powershell/scripting/gallery/how-to/working-with-local-psrepositories).</span></span>
* <span data-ttu-id="59846-140">ネットワークに接続されているコンピューターに [Azure PowerShell MSI をダウンロード](install-az-ps-msi.md)し、PowerShell ギャラリーにアクセスできないシステムにインストーラーをコピーします。</span><span class="sxs-lookup"><span data-stu-id="59846-140">[Download the Azure PowerShell MSI](install-az-ps-msi.md) to a machine connected to the network, and then copy the installer to systems without access to PowerShell Gallery.</span></span> <span data-ttu-id="59846-141">MSI インストーラーは、Windows 上の PowerShell 5.1 でのみ動作することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="59846-141">Keep in mind that the MSI installer only works for PowerShell 5.1 on Windows.</span></span>
* <span data-ttu-id="59846-142">モジュールを [Save-Module](/powershell/module/PowershellGet/Save-Module) を使用してファイル共有に保存するか、別のソースに保存して他のコンピューターに手動でコピーします。</span><span class="sxs-lookup"><span data-stu-id="59846-142">Save the module with [Save-Module](/powershell/module/PowershellGet/Save-Module) to a file share, or save it to another source and manually copy it to other machines:</span></span>

  ```powershell-interactive
  Save-Module -Name Az -Path '\\server\share\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a><span data-ttu-id="59846-143">トラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="59846-143">Troubleshooting</span></span>

<span data-ttu-id="59846-144">ここでは、Azure PowerShell モジュールのインストール時に発生する一般的な問題をいくつか示します。</span><span class="sxs-lookup"><span data-stu-id="59846-144">Here are some common problems seen when installing the Azure PowerShell module.</span></span> <span data-ttu-id="59846-145">ここに示されていない問題が発生した場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="59846-145">If you experience a problem not listed here, please [file an issue on GitHub](https://github.com/azure/azure-powershell/issues).</span></span>

### <a name="proxy-blocks-connection"></a><span data-ttu-id="59846-146">プロキシによる接続のブロック</span><span class="sxs-lookup"><span data-stu-id="59846-146">Proxy blocks connection</span></span>

<span data-ttu-id="59846-147">PowerShell ギャラリーにアクセスできないことを示すエラーが `Install-Module` から発生した場合は、プロキシの内側にいる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="59846-147">If you get errors from `Install-Module` that indicate the PowerShell Gallery is unreachable, you may be behind a proxy.</span></span> <span data-ttu-id="59846-148">システム全体のプロキシを構成するための要件は、オペレーティング システムとネットワーク環境によってさまざまに異なります。</span><span class="sxs-lookup"><span data-stu-id="59846-148">Different operating systems and network environment have different requirements for configuring a system-wide proxy.</span></span> <span data-ttu-id="59846-149">プロキシ設定と、ご使用の環境での構成方法については、システム管理者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="59846-149">Contact your system administrator for your proxy settings and how to configure them for your environment.</span></span>

<span data-ttu-id="59846-150">PowerShell 自体は、このプロキシを自動的に使用するように構成されていない場合があります。</span><span class="sxs-lookup"><span data-stu-id="59846-150">PowerShell itself may not be configured to use this proxy automatically.</span></span> <span data-ttu-id="59846-151">PowerShell 5.1 以降では、次のコマンドを使用して、プロキシを使用するように PowerShell セッションを構成します。</span><span class="sxs-lookup"><span data-stu-id="59846-151">With PowerShell 5.1 and later, configure the PowerShell session to use a proxy using the following commands:</span></span>

```powershell
$webClient = New-Object System.Net.WebClient
$webClient.Proxy.Credentials = [System.Net.CredentialCache]::DefaultNetworkCredentials
```

<span data-ttu-id="59846-152">オペレーティング システムの資格情報が正しく構成されている場合は、この構成により PowerShell 要求がプロキシ経由でルーティングされます。</span><span class="sxs-lookup"><span data-stu-id="59846-152">If your operating system credentials are configured correctly, this configuration routes PowerShell requests through the proxy.</span></span> <span data-ttu-id="59846-153">この設定をセッション間で保持するには、このコマンドを [PowerShell プロファイル](/powershell/module/microsoft.powershell.core/about/about_profiles)に追加します。</span><span class="sxs-lookup"><span data-stu-id="59846-153">To have this setting persist between sessions, add the commands to your [PowerShell profile](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>

<span data-ttu-id="59846-154">パッケージをインストールするには、プロキシで次のアドレスへの HTTPS 接続を許可する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-154">To install the package, your proxy needs to allow HTTPS connections to the following address:</span></span>

* `https://www.powershellgallery.com`

## <a name="sign-in"></a><span data-ttu-id="59846-155">サインイン</span><span class="sxs-lookup"><span data-stu-id="59846-155">Sign in</span></span>

<span data-ttu-id="59846-156">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="59846-156">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
> <span data-ttu-id="59846-157">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートします。</span><span class="sxs-lookup"><span data-stu-id="59846-157">If you've disabled module autoloading, manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="59846-158">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="59846-158">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="59846-159">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-159">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="59846-160">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="59846-160">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="59846-161">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="59846-161">Update the Azure PowerShell module</span></span>

<span data-ttu-id="59846-162">PowerShell モジュールを更新するには、モジュールのインストールに使用したのと同じ方法を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-162">To update any PowerShell module, you should use the same method used to install the module.</span></span> <span data-ttu-id="59846-163">たとえば、最初に `Install-Module` を使用した場合は、[Update-Module](/powershell/module/powershellget/update-module) を使用して最新バージョンを取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-163">For example, if you originally used `Install-Module`, then you should use [Update-Module](/powershell/module/powershellget/update-module) to get the latest version.</span></span> <span data-ttu-id="59846-164">最初に MSI パッケージを使用した場合は、新しい MSI をダウンロードしてインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-164">If you originally used the MSI package then you should download and install the new MSI package.</span></span>

<span data-ttu-id="59846-165">PowerShellGet コマンドレットは、MSI パッケージからインストールされたモジュールを更新できません。</span><span class="sxs-lookup"><span data-stu-id="59846-165">The PowerShellGet cmdlets cannot update modules that were installed from an MSI package.</span></span> <span data-ttu-id="59846-166">MSI パッケージは、PowerShellGet を使用してインストールされたモジュールを更新しません。</span><span class="sxs-lookup"><span data-stu-id="59846-166">MSI packages do not update modules that were installed using PowerShellGet.</span></span> <span data-ttu-id="59846-167">PowershellGet を使用した更新で問題が発生した場合は、**更新**ではなく**再インストール**を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-167">If you have any issues updating using PowershellGet then you should **reinstall**, rather than **update**.</span></span> <span data-ttu-id="59846-168">再インストールはインストールと同じ方法で行いますが、`-Force` パラメーターを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="59846-168">Reinstalling is done the same way as installing, but you need to add the `-Force` parameter:</span></span>

```powershell
Install-Module -Name Az -AllowClobber -Force
```

<span data-ttu-id="59846-169">MSI ベースのインストールとは異なり、PowerShellGet を使用してインストールまたは更新を行っても、システム上に存在する古いバージョンは削除されません。</span><span class="sxs-lookup"><span data-stu-id="59846-169">Unlike MSI-based installations, installing or updating using PowerShellGet does not remove older versions that may exist on your system.</span></span> <span data-ttu-id="59846-170">古いバージョンの Azure PowerShell をシステムから削除する方法については、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59846-170">To remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span> <span data-ttu-id="59846-171">MSI ベースのインストールの詳細については、「[MSI を使用して Azure PowerShell をインストールする](install-az-ps-msi.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59846-171">For more information about MSI-based installations, see [Install Azure PowerShell with an MSI](install-az-ps-msi.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="59846-172">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="59846-172">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="59846-173">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="59846-173">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="59846-174">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="59846-174">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="59846-175">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59846-175">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="59846-176">複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="59846-176">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

<span data-ttu-id="59846-177">特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` パラメーターを使用できます。</span><span class="sxs-lookup"><span data-stu-id="59846-177">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` parameter:</span></span>

```powershell-interactive
# Install Az version 3.6.1
Install-Module -Name Az -RequiredVersion 3.6.1
# Load Az version 3.6.1
Import-Module -Name Az -RequiredVersion 3.6.1
```

## <a name="provide-feedback"></a><span data-ttu-id="59846-178">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="59846-178">Provide feedback</span></span>

<span data-ttu-id="59846-179">Azure PowerShell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="59846-179">If you find a bug in Azure PowerShell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="59846-180">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="59846-180">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="59846-181">次の手順</span><span class="sxs-lookup"><span data-stu-id="59846-181">Next Steps</span></span>

<span data-ttu-id="59846-182">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="59846-182">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span> <span data-ttu-id="59846-183">Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="59846-183">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
