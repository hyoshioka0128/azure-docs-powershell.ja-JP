---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: f60ea1c608be4b1c8319d53303713ba039276abc
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2018
ms.locfileid: "51576421"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="84482-103">macOS または Linux で Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="84482-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="84482-104">Windows 以外のプラットフォームについては、PowerShell Core v6 で Azure PowerShell を実行できます。</span><span class="sxs-lookup"><span data-stu-id="84482-104">For non-Windows platforms, it's possible to run Azure PowerShell in PowerShell Core v6.</span></span> <span data-ttu-id="84482-105">このバージョンの PowerShell は、.NET Core をサポートするプラットフォームで使用できるように構築されています。</span><span class="sxs-lookup"><span data-stu-id="84482-105">This version of PowerShell is built for use on any platform that supports .NET Core.</span></span> <span data-ttu-id="84482-106">これらのプラットフォームで使用するために、Azure PowerShell の .NET Standard バージョンが提供されています。</span><span class="sxs-lookup"><span data-stu-id="84482-106">To work with these platforms, there's a .NET Standard version of Azure PowerShell available.</span></span>

> [!NOTE]
> <span data-ttu-id="84482-107">現時点では、Azure PowerShell for .NET Standard はベータ版で提供されています。</span><span class="sxs-lookup"><span data-stu-id="84482-107">At this time, Azure PowerShell for .NET Standard is still in beta.</span></span>
> <span data-ttu-id="84482-108">問題やバグを見つけた場合は、GitHub で問題を登録してください。</span><span class="sxs-lookup"><span data-stu-id="84482-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="84482-109">Azure PowerShell の問題</span><span class="sxs-lookup"><span data-stu-id="84482-109">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a><span data-ttu-id="84482-110">PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="84482-110">Install PowerShell Core</span></span>

<span data-ttu-id="84482-111">PowerShell Core のインストール手順は、macOS とほとんどの Linux ディストリビューションで異なります。</span><span class="sxs-lookup"><span data-stu-id="84482-111">The installation instructions for PowerShell Core are different for macOS and most Linux distributions.</span></span>
<span data-ttu-id="84482-112">詳細な手順については、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="84482-112">Detailed instructions can be found in the following articles:</span></span>

* [<span data-ttu-id="84482-113">macOS で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="84482-113">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [<span data-ttu-id="84482-114">Linux で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="84482-114">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a><span data-ttu-id="84482-115">Azure PowerShell for .NET Standard をインストールする</span><span class="sxs-lookup"><span data-stu-id="84482-115">Install Azure PowerShell for .NET Standard</span></span>

> [!IMPORTANT]
> <span data-ttu-id="84482-116">他の記事で詳述されている `AzureRM` モジュールは、PowerShell Core では動作しません。</span><span class="sxs-lookup"><span data-stu-id="84482-116">The `AzureRM` module detailed in other articles does not work with PowerShell Core.</span></span>
> <span data-ttu-id="84482-117">PowerShell Core で Azure PowerShell の機能を使用するには、`Az` モジュールをインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="84482-117">You must install the `Az` module to get Azure PowerShell functionality in PowerShell Core.</span></span>

<span data-ttu-id="84482-118">PowerShell Core には、インストール済みの PowerShellGet モジュールが付属しています。</span><span class="sxs-lookup"><span data-stu-id="84482-118">PowerShell Core comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="84482-119">次のコマンドを使用して PowerShell を起動します。</span><span class="sxs-lookup"><span data-stu-id="84482-119">Start PowerShell with the command:</span></span>

```bash
pwsh
```

<span data-ttu-id="84482-120">Azure PowerShell をインストールするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="84482-120">To install Azure PowerShell, run the following command:</span></span>

```powershell-interactive
Install-Module Az
```

> [!NOTE]
> <span data-ttu-id="84482-121">モジュールをインストールするときにアクセス許可エラーが発生した場合は、スーパーユーザー モードで PowerShell を実行して、モジュールをインストールしなければならない可能性があります。</span><span class="sxs-lookup"><span data-stu-id="84482-121">If you encounter a permissions error when attempting to install the module, you may need to run PowerShell in superuser mode to install modules.</span></span>
>
> ```bash
> sudo pwsh
> ```

<span data-ttu-id="84482-122">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="84482-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="84482-123">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="84482-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="84482-124">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="84482-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

## <a name="enable-aliases"></a><span data-ttu-id="84482-125">エイリアスを有効にする</span><span class="sxs-lookup"><span data-stu-id="84482-125">Enable aliases</span></span>

<span data-ttu-id="84482-126">既存の `AzureRM` モジュールとの互換性のために、新しい `Az` モジュールでは、`AzureRM` コマンドレット用に下位互換性のあるエイリアスを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="84482-126">For compatibility with the existing `AzureRM` module, the new `Az` module has the ability to create backwards compatible aliases for the `AzureRM` cmdlets.</span></span> <span data-ttu-id="84482-127">初めてモジュールを使用する前に、次のコマンドでこれらのエイリアスを設定します。</span><span class="sxs-lookup"><span data-stu-id="84482-127">Before using the module for the first time, set up these aliases with the following command:</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="84482-128">これにより現在のユーザーに対してのみエイリアスが設定されます。</span><span class="sxs-lookup"><span data-stu-id="84482-128">This sets up aliases for the current user only.</span></span> <span data-ttu-id="84482-129">エイリアスを設定する際に `-Scope` に指定できる他の値については、コマンドレットのヘルプを確認してください。</span><span class="sxs-lookup"><span data-stu-id="84482-129">Check the cmdlet help for other values that can be provided to `-Scope` to set up the aliases.</span></span>

> [!NOTE]
> <span data-ttu-id="84482-130">パスの場所に関するエラーが発生した場合は、それがお使いのローカル システムに存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="84482-130">If you encounter an error about a path location, make sure that it exists on your local system.</span></span> <span data-ttu-id="84482-131">`CurrentUser` スコープの場合、このエラーは、`bash` で次のコマンドを実行することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="84482-131">For the `CurrentUser` scope, this error can be resolved by running the following command in `bash`:</span></span>
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a><span data-ttu-id="84482-132">[サインイン]</span><span class="sxs-lookup"><span data-stu-id="84482-132">Sign in</span></span>

<span data-ttu-id="84482-133">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、PowerShell セッションに `Az` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="84482-133">To start working with Azure PowerShell, you need to load `Az` into your PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span> <span data-ttu-id="84482-134">モジュールのインポートには、昇格された特権は__不要__です。</span><span class="sxs-lookup"><span data-stu-id="84482-134">Importing a module does __not__ require elevated privileges.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="84482-135">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="84482-135">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="84482-136">`Az` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="84482-136">Automatically importing the `Az` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="84482-137">macOS と Linux では、`$Profile` 環境変数を使用してプロファイルを操作する必要があります。</span><span class="sxs-lookup"><span data-stu-id="84482-137">On macOS and Linux, you should work with your profile through the `$Profile` environment variable.</span></span> <span data-ttu-id="84482-138">Azure サインインをセッション間で維持する方法については、「[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84482-138">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="84482-139">次の手順</span><span class="sxs-lookup"><span data-stu-id="84482-139">Next Steps</span></span>

<span data-ttu-id="84482-140">Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="84482-140">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
