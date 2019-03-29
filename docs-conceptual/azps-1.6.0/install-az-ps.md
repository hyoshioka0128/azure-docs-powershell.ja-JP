---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 269119333b2197a15ed7bb50e3e5d90588456174
ms.sourcegitcommit: 8f59e11e5c991543964154d63648aa1e6ae22512
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "58475535"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="6b1c6-103">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="6b1c6-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="6b1c6-104">この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="6b1c6-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="6b1c6-106">Az モジュールについては、現在他のインストール方法はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="6b1c6-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="6b1c6-107">Requirements</span></span>

<span data-ttu-id="6b1c6-108">Azure PowerShell は、Windows にインストールされている PowerShell 5.1 以降、または任意のプラットフォーム上の PowerShell 6 上で動作します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell 6 on any platform.</span></span>
<span data-ttu-id="6b1c6-109">PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-109">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="6b1c6-110">期限切れのバージョンをお使いの場合や PowerShell をインストールする必要がある場合は、「[PowerShell のさまざまなバージョンのインストール](/powershell/scripting/setup/installing-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](/powershell/scripting/setup/installing-powershell).</span></span> <span data-ttu-id="6b1c6-111">お使いのプラットフォームでのインストール情報については、そのページにリンクがあります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-111">Install information for your platform is linked from that page.</span></span>

<span data-ttu-id="6b1c6-112">Windows で PowerShell 5 を使用している場合は、.NET Framework 4.7.2 もインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-112">If you are using PowerShell 5 on Windows, you also need .NET Framework 4.7.2 installed.</span></span> <span data-ttu-id="6b1c6-113">新しいバージョンの .NET Framework を更新またはインストールする手順については、[.NET Framework のインストール ガイド](/dotnet/framework/install)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-113">For instructions on updating or installing a new version of .NET Framework, see the [.NET Framework installation guide](/dotnet/framework/install).</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="6b1c6-114">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="6b1c6-114">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="6b1c6-115">AzureRM と Az の両方のモジュールを同時にインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-115">You can have both the AzureRM and Az modules installed at the same time.</span></span> <span data-ttu-id="6b1c6-116">両方のモジュールをインストールした場合は、__別名を有効にしない__でください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-116">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="6b1c6-117">別名を有効にすると、AzureRM コマンドレットと Az コマンドの別名との間に競合が発生して、予期しない動作が起こる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-117">Enabling aliases will cause conflicts between AzureRM cmdlets and Az command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="6b1c6-118">Az モジュールをインストールする前に、AzureRM をアンインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-118">It's recommended that before installing the Az module, you uninstall AzureRM.</span></span> <span data-ttu-id="6b1c6-119">AzureRM のアンインストールや別名の有効化はいつでもできます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-119">You can always uninstall AzureRM or enable aliases at any time.</span></span> <span data-ttu-id="6b1c6-120">AzureRM コマンドの別名の詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-120">To learn about the AzureRM command aliases, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
> <span data-ttu-id="6b1c6-121">アンインストールの手順については、「[AzureRM モジュールをアンインストールする](uninstall-az-ps.md#uninstall-the-azurerm-module)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-121">For uninstall instructions, see [Uninstall the AzureRM module](uninstall-az-ps.md#uninstall-the-azurerm-module).</span></span> 

<span data-ttu-id="6b1c6-122">グローバル スコープでモジュールをインストールするには、PowerShell ギャラリーからモジュールをインストールするための、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-122">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="6b1c6-123">Azure PowerShell をインストールするには、管理者特権セッション (Windows の場合は [管理者として実行]、macOS または Linux の場合はスーパーユーザー権限) で、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-123">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="6b1c6-124">管理者特権へのアクセス許可がない場合は、`-Scope` 引数を追加することで、現在のユーザーに対してインストールできます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-124">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="6b1c6-125">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-125">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="6b1c6-126">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-126">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="6b1c6-127">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-127">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="6b1c6-128">Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-128">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="6b1c6-129">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-129">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="6b1c6-130">サインイン</span><span class="sxs-lookup"><span data-stu-id="6b1c6-130">Sign in</span></span>

<span data-ttu-id="6b1c6-131">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-131">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="6b1c6-132">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-132">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="6b1c6-133">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-133">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="6b1c6-134">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-134">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="6b1c6-135">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-135">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="6b1c6-136">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="6b1c6-136">Update the Azure PowerShell module</span></span>

<span data-ttu-id="6b1c6-137">Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-137">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="6b1c6-138">このコマンドでは、以前のバージョンはアンインストール__されません__。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-138">This command does __not__ uninstall older versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="6b1c6-139">以前のバージョンの Azure PowerShell をシステムから削除する方法については、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-az-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-139">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="6b1c6-140">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="6b1c6-140">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="6b1c6-141">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-141">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="6b1c6-142">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-142">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="6b1c6-143">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-143">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="6b1c6-144">特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` 引数を使用できます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-144">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="6b1c6-145">複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-145">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="6b1c6-146">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="6b1c6-146">Provide feedback</span></span>

<span data-ttu-id="6b1c6-147">Azure Powershell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-147">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="6b1c6-148">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-148">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="6b1c6-149">次の手順</span><span class="sxs-lookup"><span data-stu-id="6b1c6-149">Next Steps</span></span>

<span data-ttu-id="6b1c6-150">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-150">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="6b1c6-151">Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b1c6-151">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
