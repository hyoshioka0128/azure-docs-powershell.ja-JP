---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 47611281f67d68c9fc2686e0c6156b060a225158
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217526"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="af9fd-103">macOS または Linux で Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="af9fd-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="af9fd-104">Windows 以外のプラットフォームについては、PowerShell Core v6 で Azure PowerShell を実行できます。</span><span class="sxs-lookup"><span data-stu-id="af9fd-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="af9fd-105">このバージョンの PowerShell は、.NET Core をサポートするプラットフォームで使用できるように構築されています。</span><span class="sxs-lookup"><span data-stu-id="af9fd-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="af9fd-106">これらのプラットフォームで使用するために、Azure PowerShell の特別な .NET Core バージョンが提供されています。</span><span class="sxs-lookup"><span data-stu-id="af9fd-106">To work with these platforms, there's a special .NET Core version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="af9fd-107">現時点では、PowerShell Core v6 と Azure PowerShell for .NET Core はどちらもベータ版で提供されており、</span><span class="sxs-lookup"><span data-stu-id="af9fd-107">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="af9fd-108">これらの製品のサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="af9fd-108">Support for these products is limited.</span></span> <span data-ttu-id="af9fd-109">問題やバグを見つけた場合は、GitHub で問題を登録してください。</span><span class="sxs-lookup"><span data-stu-id="af9fd-109">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="af9fd-110">PowerShell Core v6 の問題</span><span class="sxs-lookup"><span data-stu-id="af9fd-110">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="af9fd-111">Azure PowerShell の問題</span><span class="sxs-lookup"><span data-stu-id="af9fd-111">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="af9fd-112">PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="af9fd-112">Install PowerShell Core</span></span>

<span data-ttu-id="af9fd-113">PowerShell Core のインストール手順は、macOS とほとんどの Linux ディストリビューションで異なります。</span><span class="sxs-lookup"><span data-stu-id="af9fd-113">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="af9fd-114">詳細な手順については、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="af9fd-114">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="af9fd-115">macOS で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="af9fd-115">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="af9fd-116">Linux で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="af9fd-116">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="af9fd-117">Azure PowerShell for .NET Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="af9fd-117">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="af9fd-118">PowerShell Core には、インストール済みの PowerShellGet モジュールが付属しています。</span><span class="sxs-lookup"><span data-stu-id="af9fd-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="af9fd-119">PowerShell のモジュールをインストールするには、昇格された特権が必要であるため、スーパーユーザーとしてセッションを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="af9fd-119">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="af9fd-120">Azure PowerShell をインストールするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="af9fd-120">To install Azure PowerShell, run the following command:</span></span>

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> <span data-ttu-id="af9fd-121">他の記事で詳述されている `AzureRM` モジュールは、.NET Core 用に構築されておらず、PowerShell Core では動作しません。</span><span class="sxs-lookup"><span data-stu-id="af9fd-121">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="af9fd-122">`AzureRM` と `AzureRM.NetCore` では、同じコマンドレット名を使用します。唯一の違いは、ロールアップ モジュールの名前と対象とする .NET バージョンです。</span><span class="sxs-lookup"><span data-stu-id="af9fd-122">Both `AzureRM` and `AzureRM.NetCore` use the same cmdlet names, so the only difference is the name of the rollup module and which .NET version they are built against.</span></span>

<span data-ttu-id="af9fd-123">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="af9fd-123">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="af9fd-124">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="af9fd-124">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="af9fd-125">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="af9fd-125">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="af9fd-126">[サインイン]</span><span class="sxs-lookup"><span data-stu-id="af9fd-126">Sign in</span></span>

<span data-ttu-id="af9fd-127">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、PowerShell セッションに `AzureRM.Netcore` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="af9fd-127">To start working with Azure PowerShell, you need to load `AzureRM.Netcore` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="af9fd-128">モジュールのインポートには、昇格された特権は__不要__です。</span><span class="sxs-lookup"><span data-stu-id="af9fd-128">Importing a module does __not__ require elevated privileges.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="af9fd-129">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="af9fd-129">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="af9fd-130">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="af9fd-130">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="af9fd-131">macOS と Linux では、`$Profile` 環境変数を使用してプロファイルを操作する必要があります。</span><span class="sxs-lookup"><span data-stu-id="af9fd-131">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="af9fd-132">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="af9fd-132">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="af9fd-133">利用可能なコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af9fd-133">Available cmdlets</span></span>

<span data-ttu-id="af9fd-134">.NET Core 向けの Azure PowerShell モジュールはまだ開発途中です。</span><span class="sxs-lookup"><span data-stu-id="af9fd-134">The Azure PowerShell modules for .NET Core are still in development.</span></span> <span data-ttu-id="af9fd-135">これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。</span><span class="sxs-lookup"><span data-stu-id="af9fd-135">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="af9fd-136">AzureRM.Netcore モジュールには次の関数が実装されています。</span><span class="sxs-lookup"><span data-stu-id="af9fd-136">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="af9fd-137">アカウント管理</span><span class="sxs-lookup"><span data-stu-id="af9fd-137">Account management</span></span>
  * <span data-ttu-id="af9fd-138">Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでサインインする</span><span class="sxs-lookup"><span data-stu-id="af9fd-138">Sign in with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  * <span data-ttu-id="af9fd-139">Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む</span><span class="sxs-lookup"><span data-stu-id="af9fd-139">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="af9fd-140">環境</span><span class="sxs-lookup"><span data-stu-id="af9fd-140">Environment</span></span>
  * <span data-ttu-id="af9fd-141">すぐに使えるさまざまな Microsoft Azure 環境を取得する</span><span class="sxs-lookup"><span data-stu-id="af9fd-141">Get the different out-of-box Microsoft Azure environments</span></span>
  * <span data-ttu-id="af9fd-142">カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する</span><span class="sxs-lookup"><span data-stu-id="af9fd-142">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="af9fd-143">Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット</span><span class="sxs-lookup"><span data-stu-id="af9fd-143">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  * <span data-ttu-id="af9fd-144">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="af9fd-144">Virtual Machine</span></span>
  * <span data-ttu-id="af9fd-145">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="af9fd-145">App Service (Websites)</span></span>
  * <span data-ttu-id="af9fd-146">SQL Database</span><span class="sxs-lookup"><span data-stu-id="af9fd-146">SQL Database</span></span>
  * <span data-ttu-id="af9fd-147">Storage</span><span class="sxs-lookup"><span data-stu-id="af9fd-147">Storage</span></span>
  * <span data-ttu-id="af9fd-148">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="af9fd-148">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="af9fd-149">次の手順</span><span class="sxs-lookup"><span data-stu-id="af9fd-149">Next Steps</span></span>

<span data-ttu-id="af9fd-150">Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="af9fd-150">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
