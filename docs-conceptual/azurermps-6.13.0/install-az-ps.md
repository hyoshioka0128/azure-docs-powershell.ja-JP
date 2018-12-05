---
title: PowerShellGet を使用して Azure PowerShell "Az" をインストールする
description: PowerShellGet を使用して、Windows、macOS、Linux に Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/26/2018
ms.openlocfilehash: 3d52b18750341f220dc8e10d6bf89796457c5a10
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "52588181"
---
# <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="c118e-103">Azure PowerShell "Az" モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="c118e-103">Install the Azure PowerShell 'Az' module</span></span>

<span data-ttu-id="c118e-104">この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="c118e-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="c118e-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="c118e-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="c118e-106">Az のプレビュー リリースでは、他のインストール方法はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c118e-106">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="c118e-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="c118e-107">Requirements</span></span>

<span data-ttu-id="c118e-108">Azure PowerShell は、Windows 上の PowerShell 5.x、または任意のプラットフォーム上の PowerShell 6.x で動作します。</span><span class="sxs-lookup"><span data-stu-id="c118e-108">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="c118e-109">お使いのマシンで実行されている PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="c118e-109">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="c118e-110">期限切れのバージョンをお使いの場合や PowerShell をインストールする必要がある場合は、「[PowerShell のさまざまなバージョンのインストール](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c118e-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="c118e-111">お使いのプラットフォームでのインストール情報については、そのページにリンクがあります。</span><span class="sxs-lookup"><span data-stu-id="c118e-111">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="c118e-112">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="c118e-112">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="c118e-113">`AzureRM` と `Az` の両方のモジュールを同時にインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="c118e-113">You can have both the `AzureRM` and `Az` modules installed at the same time.</span></span> <span data-ttu-id="c118e-114">両方のモジュールをインストールした場合は、__別名を有効にしない__でください。</span><span class="sxs-lookup"><span data-stu-id="c118e-114">If you have both modules installed, __don't enable aliases__.</span></span>
> <span data-ttu-id="c118e-115">別名を有効にすると、`AzureRM` コマンドレットと `Az` コマンドの別名との間に競合が発生して、予期しない動作が起こる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="c118e-115">Enabling aliases will cause conflicts between `AzureRM` cmdlets and `Az` command aliases, and could cause unexpected behavior.</span></span>
> <span data-ttu-id="c118e-116">`Az` モジュールをインストールする前に、`AzureRM` をアンインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="c118e-116">It's recommended that before installing the `Az` module, you uninstall `AzureRM`.</span></span> <span data-ttu-id="c118e-117">`AzureRM` のインストールや別名の有効化はいつでもできます。</span><span class="sxs-lookup"><span data-stu-id="c118e-117">You can always uninstall `AzureRM` or enable aliases at any time.</span></span> <span data-ttu-id="c118e-118">アンインストールの手順については、[Azure PowerShell モジュール (AzureRM) のアンインストール](uninstall-azurerm-ps.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c118e-118">For uninstall instructions, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span> 

<span data-ttu-id="c118e-119">グローバル スコープでモジュールをインストールするには、PowerShell ギャラリーからモジュールをインストールするための、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="c118e-119">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="c118e-120">Azure PowerShell をインストールするには、管理者特権セッション (Windows の場合は [管理者として実行]、macOS または Linux の場合はスーパーユーザー権限) で、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="c118e-120">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="c118e-121">管理者特権へのアクセス許可がない場合は、`-Scope` 引数を追加することで、現在のユーザーに対してインストールできます。</span><span class="sxs-lookup"><span data-stu-id="c118e-121">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="c118e-122">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="c118e-122">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="c118e-123">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="c118e-123">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="c118e-124">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="c118e-124">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="c118e-125">`Az` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="c118e-125">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="c118e-126">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="c118e-126">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="c118e-127">[サインイン]</span><span class="sxs-lookup"><span data-stu-id="c118e-127">Sign in</span></span>

<span data-ttu-id="c118e-128">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="c118e-128">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="c118e-129">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c118e-129">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="c118e-130">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="c118e-130">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="c118e-131">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="c118e-131">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="c118e-132">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c118e-132">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="c118e-133">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="c118e-133">Update the Azure PowerShell module</span></span>

<span data-ttu-id="c118e-134">Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。</span><span class="sxs-lookup"><span data-stu-id="c118e-134">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="c118e-135">このコマンドでは、以前のバージョンはアンインストール__されません__。</span><span class="sxs-lookup"><span data-stu-id="c118e-135">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="c118e-136">古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c118e-136">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="c118e-137">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="c118e-137">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="c118e-138">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="c118e-138">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="c118e-139">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="c118e-139">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="c118e-140">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c118e-140">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="c118e-141">特定のバージョンの `Az` モジュールを読み込むには、`Install-Module` および `Import-Module` で `-RequiredVersion` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="c118e-141">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` and `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="c118e-142">複数のバージョンのモジュールがインストールされている場合は、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="c118e-142">If you have more than one version of the module installed, the latest version is loaded by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="c118e-143">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="c118e-143">Provide feedback</span></span>

<span data-ttu-id="c118e-144">Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="c118e-144">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="c118e-145">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.profile/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="c118e-145">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="c118e-146">次の手順</span><span class="sxs-lookup"><span data-stu-id="c118e-146">Next Steps</span></span>

<span data-ttu-id="c118e-147">Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c118e-147">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
