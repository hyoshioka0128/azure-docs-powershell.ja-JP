---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: d99265c7f156622d876d700106e2b06dd729e8b8
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365742"
---
# <a name="install-the-azure-powershell-module"></a><span data-ttu-id="a9e3e-103">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="a9e3e-103">Install the Azure PowerShell module</span></span>

<span data-ttu-id="a9e3e-104">この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="a9e3e-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="a9e3e-106">Az モジュールについては、現在他のインストール方法はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-106">For the Az module, currently no other installation methods are supported.</span></span>

## <a name="requirements"></a><span data-ttu-id="a9e3e-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="a9e3e-107">Requirements</span></span>

<span data-ttu-id="a9e3e-108">Azure PowerShell は、Windows 上の PowerShell 5.1 以降、またはすべてのプラットフォーム上の PowerShell Core 6.x 以降で動作します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-108">Azure PowerShell works with PowerShell 5.1 or higher on Windows, or PowerShell Core 6.x and later on all platforms.</span></span> <span data-ttu-id="a9e3e-109">PowerShell がインストールされているかどうか、または macOS または Linux かどうか不明な場合な場合は、[最新バージョンの PowerShell Core をインストール](/powershell/scripting/install/installing-powershell#powershell-core)してください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-109">If you aren't sure if you have PowerShell, or are on macOS or Linux, [install the latest version of PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core).</span></span>

<span data-ttu-id="a9e3e-110">PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-110">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="a9e3e-111">Windows 上の PowerShell 5.1 で Azure PowerShell を実行するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-111">To run Azure PowerShell in PowerShell 5.1 on Windows:</span></span>

1. <span data-ttu-id="a9e3e-112">必要に応じて [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-112">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="a9e3e-113">Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-113">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="a9e3e-114">[.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-114">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

<span data-ttu-id="a9e3e-115">PowerShell Core を使用する場合、Azure PowerShell にその他の要件はありません。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-115">There are no additional requirements for Azure PowerShell when using PowerShell Core.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="a9e3e-116">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="a9e3e-116">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="a9e3e-117">AzureRM と Az の両方のモジュールを同時にインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-117">You can have both the AzureRM and Az modules installed at the same time.</span></span> <span data-ttu-id="a9e3e-118">両方のモジュールをインストールした場合は、__別名を有効にしない__でください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-118">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="a9e3e-119">別名を有効にすると、AzureRM コマンドレットと Az コマンドの別名との間に競合が発生して、予期しない動作が起こる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-119">Enabling aliases will cause conflicts between AzureRM cmdlets and Az command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="a9e3e-120">Az モジュールをインストールする前に、AzureRM をアンインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-120">It's recommended that before installing the Az module, you uninstall AzureRM.</span></span> <span data-ttu-id="a9e3e-121">AzureRM のアンインストールや別名の有効化はいつでもできます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-121">You can always uninstall AzureRM or enable aliases at any time.</span></span> <span data-ttu-id="a9e3e-122">AzureRM コマンドの別名の詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-122">To learn about the AzureRM command aliases, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
> <span data-ttu-id="a9e3e-123">アンインストールの手順については、「[AzureRM モジュールをアンインストールする](uninstall-az-ps.md#uninstall-the-azurerm-module)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-123">For uninstall instructions, see [Uninstall the AzureRM module](uninstall-az-ps.md#uninstall-the-azurerm-module).</span></span> 

<span data-ttu-id="a9e3e-124">グローバル スコープでモジュールをインストールするには、PowerShell ギャラリーからモジュールをインストールするための、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-124">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="a9e3e-125">Azure PowerShell をインストールするには、管理者特権セッション (Windows の場合は [管理者として実行]、macOS または Linux の場合はスーパーユーザー権限) で、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-125">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="a9e3e-126">管理者特権へのアクセス許可がない場合は、`-Scope` 引数を追加することで、現在のユーザーに対してインストールできます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-126">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="a9e3e-127">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-127">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="a9e3e-128">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-128">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="a9e3e-129">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-129">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="a9e3e-130">Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-130">The Az module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="a9e3e-131">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-131">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="a9e3e-132">サインイン</span><span class="sxs-lookup"><span data-stu-id="a9e3e-132">Sign in</span></span>

<span data-ttu-id="a9e3e-133">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-133">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="a9e3e-134">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-134">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="a9e3e-135">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-135">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="a9e3e-136">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-136">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="a9e3e-137">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-137">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="a9e3e-138">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="a9e3e-138">Update the Azure PowerShell module</span></span>

<span data-ttu-id="a9e3e-139">Az モジュールのパッケージ方法のために、[Update-Module](/powershell/module/powershellget/update-module) コマンドではインストールは適切に更新されません。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-139">Because of how the Az module is package, the [Update-Module](/powershell/module/powershellget/update-module) command won't update your installation correctly.</span></span> <span data-ttu-id="a9e3e-140">Az は技術的にはメタモジュールであり、Azure サービスを操作するためのコマンドレットを含むすべてのサブモジュールが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-140">Az is technically a meta-module, encompassing all of the submodules that contain cmdlets to interact with Azure services.</span></span> <span data-ttu-id="a9e3e-141">つまり、Azure PowerShell モジュールを更新するには、__更新__するだけではなく__再インストール__する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-141">That means that to update the Azure PowerShell module, you will need to __reinstall__, rather than just __update__.</span></span> <span data-ttu-id="a9e3e-142">これはインストールと同じ方法で行いますが、`-Force` 引数を追加する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-142">This is done in the same way as installing, but you may need to add the `-Force` argument:</span></span>

```powershell
Install-Module -Name Az -AllowClobber -Force
```

<span data-ttu-id="a9e3e-143">これによりインストールされているモジュールを上書きできますが、システム上には以前のバージョンがそのまま残っていることがあります。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-143">Although this can overwrite installed modules, you may still have older versions left on your system.</span></span>
<span data-ttu-id="a9e3e-144">以前のバージョンの Azure PowerShell をシステムから削除する方法については、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-az-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-144">To learn how to remove old versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="a9e3e-145">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="a9e3e-145">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="a9e3e-146">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-146">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="a9e3e-147">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-147">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

<span data-ttu-id="a9e3e-148">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-148">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-az-ps.md).</span></span>

<span data-ttu-id="a9e3e-149">特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` 引数を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-149">You can install or load a specific version of the `Az` module by using the `-RequiredVersion` argument:</span></span>

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

<span data-ttu-id="a9e3e-150">複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-150">If you have more than one version of the module installed, module autoload and `Import-Module` load the latest version by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="a9e3e-151">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="a9e3e-151">Provide feedback</span></span>

<span data-ttu-id="a9e3e-152">Azure Powershell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-152">If you find a bug in Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="a9e3e-153">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-153">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="a9e3e-154">次の手順</span><span class="sxs-lookup"><span data-stu-id="a9e3e-154">Next Steps</span></span>

<span data-ttu-id="a9e3e-155">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-155">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span>
<span data-ttu-id="a9e3e-156">Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a9e3e-156">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
