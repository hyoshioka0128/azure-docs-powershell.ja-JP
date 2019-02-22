---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 936bb24eecb4077080e172bf0d29fe57ec652187
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153690"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="3ad26-103">macOS または Linux で Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="3ad26-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="3ad26-104">Windows 以外のプラットフォームについては、PowerShell Core v6 で Azure PowerShell を実行できます。</span><span class="sxs-lookup"><span data-stu-id="3ad26-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="3ad26-105">このバージョンの PowerShell は、.NET Core をサポートするプラットフォームで使用できるように構築されています。</span><span class="sxs-lookup"><span data-stu-id="3ad26-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="3ad26-106">これらのプラットフォームで使用するために、Azure PowerShell の特別な .NET Core バージョンが提供されています。</span><span class="sxs-lookup"><span data-stu-id="3ad26-106">To work with these platforms, there's a special .NET Core version of Azure PowerShell available.</span></span>

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

## <a name="install-powershell-core"></a><span data-ttu-id="3ad26-107">PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="3ad26-107">Install PowerShell Core</span></span>

<span data-ttu-id="3ad26-108">PowerShell Core のインストール手順は、macOS とほとんどの Linux ディストリビューションで異なります。</span><span class="sxs-lookup"><span data-stu-id="3ad26-108">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="3ad26-109">詳細な手順については、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3ad26-109">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="3ad26-110">macOS で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="3ad26-110">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="3ad26-111">Linux で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="3ad26-111">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="3ad26-112">Azure PowerShell for .NET Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="3ad26-112">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="3ad26-113">PowerShell Core には、インストール済みの PowerShellGet モジュールが付属しています。</span><span class="sxs-lookup"><span data-stu-id="3ad26-113">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="3ad26-114">PowerShell のモジュールをインストールするには、昇格された特権が必要であるため、スーパーユーザーとしてセッションを開始する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ad26-114">Installation of modules in PowerShell requires elevated privileges, so you'll need to start your session as superuser:</span></span>

```bash
sudo pwsh
```

<span data-ttu-id="3ad26-115">Azure PowerShell をインストールするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="3ad26-115">To install Azure PowerShell, run the following command:</span></span>

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> <span data-ttu-id="3ad26-116">他の記事で詳述されている `AzureRM` モジュールは、.NET Core 用に構築されておらず、PowerShell Core では動作しません。</span><span class="sxs-lookup"><span data-stu-id="3ad26-116">The `AzureRM` module detailed in other articles is not built for .NET Core and will not work with PowerShell Core.</span></span> <span data-ttu-id="3ad26-117">`AzureRM` と `AzureRM.NetCore` では、同じコマンドレット名を使用します。唯一の違いは、ロールアップ モジュールの名前と対象とする .NET バージョンです。</span><span class="sxs-lookup"><span data-stu-id="3ad26-117">Both `AzureRM` and `AzureRM.NetCore` use the same cmdlet names, so the only difference is the name of the rollup module and which .NET version they are built against.</span></span>

<span data-ttu-id="3ad26-118">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="3ad26-118">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="3ad26-119">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="3ad26-119">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="3ad26-120">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="3ad26-120">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="sign-in"></a><span data-ttu-id="3ad26-121">サインイン</span><span class="sxs-lookup"><span data-stu-id="3ad26-121">Sign in</span></span>

<span data-ttu-id="3ad26-122">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、PowerShell セッションに `AzureRM.Netcore` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ad26-122">To start working with Azure PowerShell, you need to load `AzureRM.Netcore` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="3ad26-123">モジュールのインポートには、昇格された特権は__不要__です。</span><span class="sxs-lookup"><span data-stu-id="3ad26-123">Importing a module does __not__ require elevated privileges.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="3ad26-124">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ad26-124">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="3ad26-125">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3ad26-125">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="3ad26-126">macOS と Linux では、`$Profile` 環境変数を使用してプロファイルを操作する必要があります。</span><span class="sxs-lookup"><span data-stu-id="3ad26-126">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="3ad26-127">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3ad26-127">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="3ad26-128">利用可能なコマンドレット</span><span class="sxs-lookup"><span data-stu-id="3ad26-128">Available cmdlets</span></span>

<span data-ttu-id="3ad26-129">.NET Core 向けの Azure PowerShell モジュールはまだ開発途中です。</span><span class="sxs-lookup"><span data-stu-id="3ad26-129">The Azure PowerShell modules for .NET Core are still in development.</span></span> <span data-ttu-id="3ad26-130">これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。</span><span class="sxs-lookup"><span data-stu-id="3ad26-130">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="3ad26-131">AzureRM.Netcore モジュールには次の関数が実装されています。</span><span class="sxs-lookup"><span data-stu-id="3ad26-131">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="3ad26-132">アカウント管理</span><span class="sxs-lookup"><span data-stu-id="3ad26-132">Account management</span></span>
  * <span data-ttu-id="3ad26-133">Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでサインインする</span><span class="sxs-lookup"><span data-stu-id="3ad26-133">Sign in with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  * <span data-ttu-id="3ad26-134">Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む</span><span class="sxs-lookup"><span data-stu-id="3ad26-134">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="3ad26-135">環境</span><span class="sxs-lookup"><span data-stu-id="3ad26-135">Environment</span></span>
  * <span data-ttu-id="3ad26-136">すぐに使えるさまざまな Microsoft Azure 環境を取得する</span><span class="sxs-lookup"><span data-stu-id="3ad26-136">Get the different out-of-box Microsoft Azure environments</span></span>
  * <span data-ttu-id="3ad26-137">カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する</span><span class="sxs-lookup"><span data-stu-id="3ad26-137">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="3ad26-138">Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット</span><span class="sxs-lookup"><span data-stu-id="3ad26-138">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  * <span data-ttu-id="3ad26-139">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="3ad26-139">Virtual Machine</span></span>
  * <span data-ttu-id="3ad26-140">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="3ad26-140">App Service (Websites)</span></span>
  * <span data-ttu-id="3ad26-141">SQL Database</span><span class="sxs-lookup"><span data-stu-id="3ad26-141">SQL Database</span></span>
  * <span data-ttu-id="3ad26-142">Storage</span><span class="sxs-lookup"><span data-stu-id="3ad26-142">Storage</span></span>
  * <span data-ttu-id="3ad26-143">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="3ad26-143">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="3ad26-144">次の手順</span><span class="sxs-lookup"><span data-stu-id="3ad26-144">Next Steps</span></span>

<span data-ttu-id="3ad26-145">Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="3ad26-145">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
