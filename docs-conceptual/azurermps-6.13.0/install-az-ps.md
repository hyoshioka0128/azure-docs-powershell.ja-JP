---
title: PowerShellGet を使用して Azure PowerShell "Az" をインストールする
description: PowerShellGet を使用して、Windows、macOS、Linux に Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: 32e96c6459c9db0c4b9eda0cc170c85ba99a22ca
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259796"
---
# <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="4307e-103">Azure PowerShell "Az" モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="4307e-103">Install the Azure PowerShell 'Az' module</span></span>

<span data-ttu-id="4307e-104">この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="4307e-104">This article tells you how to install the Azure PowerShell modules using PowerShellGet.</span></span> <span data-ttu-id="4307e-105">これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。</span><span class="sxs-lookup"><span data-stu-id="4307e-105">These instructions work on Windows, macOS, and Linux platforms.</span></span> <span data-ttu-id="4307e-106">Az のプレビュー リリースでは、他のインストール方法はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4307e-106">For the preview release of Az, no other install methods are supported.</span></span> 

## <a name="requirements"></a><span data-ttu-id="4307e-107">必要条件</span><span class="sxs-lookup"><span data-stu-id="4307e-107">Requirements</span></span>

<span data-ttu-id="4307e-108">Azure PowerShell は、Windows 上の PowerShell 5.x、または任意のプラットフォーム上の PowerShell 6.x で動作します。</span><span class="sxs-lookup"><span data-stu-id="4307e-108">Azure PowerShell works with either PowerShell 5.x on Windows, or PowerShell 6.x on any platform.</span></span> <span data-ttu-id="4307e-109">お使いのマシンで実行されている PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="4307e-109">To check the version of PowerShell running on your machine, run the following command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="4307e-110">期限切れのバージョンをお使いの場合や PowerShell をインストールする必要がある場合は、「[PowerShell のさまざまなバージョンのインストール](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4307e-110">If you have an outdated version or need to install PowerShell, see [Installing various versions of PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-powershell?view=powershell-6).</span></span> <span data-ttu-id="4307e-111">お使いのプラットフォームでのインストール情報については、そのページにリンクがあります。</span><span class="sxs-lookup"><span data-stu-id="4307e-111">Install information for your platform is linked from that page.</span></span>

## <a name="install-the-azure-powershell-module"></a><span data-ttu-id="4307e-112">Azure PowerShell モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="4307e-112">Install the Azure PowerShell module</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="4307e-113">`AzureRM` と `Az` の両方のモジュールを同じシステムに同時にインストールすることはできません。</span><span class="sxs-lookup"><span data-stu-id="4307e-113">You shouldn't have both the `AzureRM` and `Az` modules installed on a system at the same time.</span></span> <span data-ttu-id="4307e-114">`Az` モジュールをインストールするには、`AzureRM` をアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4307e-114">In order to install the `Az` module, `AzureRM` must be uninstalled.</span></span> <span data-ttu-id="4307e-115">その方法については、[Azure PowerShell モジュール (AzureRM) のアンインストール](uninstall-azurerm-ps.md)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4307e-115">For instructions on how to do that, see [Uninstall the Azure PowerShell module (AzureRM)](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="4307e-116">グローバル スコープでモジュールをインストールするには、PowerShell ギャラリーからモジュールをインストールするための、昇格された特権が必要です。</span><span class="sxs-lookup"><span data-stu-id="4307e-116">To install modules at a global scope, you need elevated privileges to install modules from the PowerShell Gallery.</span></span> <span data-ttu-id="4307e-117">Azure PowerShell をインストールするには、管理者特権セッション (Windows の場合は [管理者として実行]、macOS または Linux の場合はスーパーユーザー権限) で、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="4307e-117">To install Azure PowerShell, run the following command in an elevated session ("Run as Administrator" on Windows, or with superuser privileges on macOS or Linux):</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

<span data-ttu-id="4307e-118">管理者特権へのアクセス許可がない場合は、`-Scope` 引数を追加することで、現在のユーザーに対してインストールできます。</span><span class="sxs-lookup"><span data-stu-id="4307e-118">If you don't have access to administrator privileges, you can install for the current user by adding the `-Scope` argument.</span></span>

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

<span data-ttu-id="4307e-119">既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。</span><span class="sxs-lookup"><span data-stu-id="4307e-119">By default, the PowerShell gallery isn't configured as a trusted repository for PowerShellGet.</span></span> <span data-ttu-id="4307e-120">PSGallery の初回使用時には、次のプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4307e-120">The first time you use the PSGallery you see the following prompt:</span></span>

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

<span data-ttu-id="4307e-121">インストールを続行するには、`Yes` または `Yes to All` を選択します。</span><span class="sxs-lookup"><span data-stu-id="4307e-121">Answer `Yes` or `Yes to All` to continue with the installation.</span></span>

<span data-ttu-id="4307e-122">`Az` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="4307e-122">The `Az` module is a rollup module for the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="4307e-123">これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="4307e-123">Installing it downloads all of the available Azure Resource Manager modules, and makes their cmdlets available for use.</span></span>

## <a name="sign-in"></a><span data-ttu-id="4307e-124">[サインイン]</span><span class="sxs-lookup"><span data-stu-id="4307e-124">Sign in</span></span>

<span data-ttu-id="4307e-125">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="4307e-125">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> <span data-ttu-id="4307e-126">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4307e-126">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="4307e-127">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="4307e-127">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="4307e-128">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="4307e-128">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="4307e-129">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4307e-129">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="update-the-azure-powershell-module"></a><span data-ttu-id="4307e-130">Azure PowerShell モジュールの更新</span><span class="sxs-lookup"><span data-stu-id="4307e-130">Update the Azure PowerShell module</span></span>

<span data-ttu-id="4307e-131">Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。</span><span class="sxs-lookup"><span data-stu-id="4307e-131">You can update your Azure PowerShell installation by running [Update-Module](/powershell/module/powershellget/update-module).</span></span> <span data-ttu-id="4307e-132">このコマンドでは、以前のバージョンはアンインストール__されません__。</span><span class="sxs-lookup"><span data-stu-id="4307e-132">This command does __not__ uninstall earlier versions.</span></span>

```powershell-interactive
Update-Module -Name Az
```

<span data-ttu-id="4307e-133">古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4307e-133">If you want to remove older versions of Azure PowerShell from your system, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

## <a name="use-multiple-versions-of-azure-powershell"></a><span data-ttu-id="4307e-134">複数のバージョンの Azure PowerShell の使用</span><span class="sxs-lookup"><span data-stu-id="4307e-134">Use multiple versions of Azure PowerShell</span></span>

<span data-ttu-id="4307e-135">複数のバージョンの Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="4307e-135">It's possible to install more than one version of Azure PowerShell.</span></span> <span data-ttu-id="4307e-136">複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="4307e-136">To check if you have multiple versions of Azure PowerShell installed, use the following command:</span></span>

```powershell-interactive
Get-Module -Name Az -List | select Name,Version
```

<span data-ttu-id="4307e-137">Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4307e-137">To remove a version of Azure PowerShell, see [Uninstall the Azure PowerShell module](uninstall-azurerm-ps.md).</span></span>

<span data-ttu-id="4307e-138">特定のバージョンの `Az` モジュールを読み込むには、`Install-Module` および `Import-Module` で `-RequiredVersion` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="4307e-138">You can load a specific version of the `Az` module by using the `-RequiredVersion` argument with `Install-Module` and `Import-Module`:</span></span>

```powershell-interactive
Install-Module -Name Az -RequiredVersion 0.4.0
Import-Module -Name Az -RequiredVersion 0.4.0
```

<span data-ttu-id="4307e-139">複数のバージョンのモジュールがインストールされている場合は、既定で最新バージョンが読み込まれます。</span><span class="sxs-lookup"><span data-stu-id="4307e-139">If you have more than one version of the module installed, the latest version is loaded by default.</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="4307e-140">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="4307e-140">Provide feedback</span></span>

<span data-ttu-id="4307e-141">Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="4307e-141">If you find a bug when using Azure Powershell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span>
<span data-ttu-id="4307e-142">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.profile/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="4307e-142">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.profile/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="4307e-143">次の手順</span><span class="sxs-lookup"><span data-stu-id="4307e-143">Next Steps</span></span>

<span data-ttu-id="4307e-144">Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4307e-144">To get started using Azure PowerShell, see [Get Started with Azure PowerShell](get-started-azureps.md) to learn more about the module and its features.</span></span>
