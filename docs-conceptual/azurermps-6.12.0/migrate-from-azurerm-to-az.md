---
title: AzureRM から Az への Azure PowerShell スクリプトの移行
description: AzureRM モジュールから新しい Az モジュールにスクリプトを移行するための手順とツールについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 0c73e7ac1d47a2a97b6136fa481d0adce8de33db
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274900"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="83888-103">AzureRM から Azure PowerShell Az への移行</span><span class="sxs-lookup"><span data-stu-id="83888-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="83888-104">Az モジュールには AzureRM との機能パリティがありますが、より短く一貫性のあるコマンドレット名が使用されます。</span><span class="sxs-lookup"><span data-stu-id="83888-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="83888-105">AzureRM コマンドレット用に記述されたスクリプトは、新しいモジュールで自動的に機能するわけではありません。</span><span class="sxs-lookup"><span data-stu-id="83888-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="83888-106">移行を容易にするために、Az には AzureRM を使用する既存のスクリプトを実行できるようにするツールが用意されています。</span><span class="sxs-lookup"><span data-stu-id="83888-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="83888-107">新しいコマンド セットへの移行がないに越したことはありませんが、この記事は、新しいモジュールへの切り替えを開始する際に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="83888-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="83888-108">既存スクリプトが AzureRM の最新リリースで機能することを確認する</span><span class="sxs-lookup"><span data-stu-id="83888-108">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="83888-109">これは最も重要な手順です。</span><span class="sxs-lookup"><span data-stu-id="83888-109">This is the most important step!</span></span> <span data-ttu-id="83888-110">既存のスクリプトを実行し、AzureRM の "_最新_" リリース (__6.12.0__) で機能することを確認します。</span><span class="sxs-lookup"><span data-stu-id="83888-110">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.12.0__).</span></span> <span data-ttu-id="83888-111">スクリプトが機能しない場合は、必ず [AzureRM 移行ガイド](migration-guide.6.0.0.md)をお読みください。</span><span class="sxs-lookup"><span data-stu-id="83888-111">If your scripts don't work, make sure to read the [AzureRM migration guide](migration-guide.6.0.0.md).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="83888-112">Azure PowerShell Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="83888-112">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="83888-113">最初の手順では、お使いのプラットフォームに Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="83888-113">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="83888-114">Az をインストールするには、AzureRM をアンインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="83888-114">To install Az, you need to uninstall AzureRM.</span></span>
<span data-ttu-id="83888-115">次の手順では、既存のスクリプトを引き続き実行できるようにする方法と、古いコマンドレット名の互換性を有効にする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="83888-115">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="83888-116">Azure PowerShell Az モジュールをインストールするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="83888-116">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="83888-117">[AzureRM モジュールをアンインストールする](uninstall-azurerm-ps.md)。</span><span class="sxs-lookup"><span data-stu-id="83888-117">[Uninstall the AzureRM module](uninstall-azurerm-ps.md).</span></span> <span data-ttu-id="83888-118">最新のバージョンだけでなく、インストールした "_すべて_" のバージョンの AzureRM を必ず削除します。</span><span class="sxs-lookup"><span data-stu-id="83888-118">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="83888-119">Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="83888-119">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><span data-ttu-id="83888-120"><a name="aliases"/>AzureRM 別名モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="83888-120"><a name="aliases"/>Enable AzureRM alias mode</span></span>

<span data-ttu-id="83888-121">スクリプトが最新バージョンの AzureRM で機能し、AzureRM をアンインストールしたら、次は Az モジュールの互換モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="83888-121">With AzureRM uninstalled and your scripts working with the latest AzureRM version, now is the time to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="83888-122">次のコマンドを使用して、互換性を有効にします。</span><span class="sxs-lookup"><span data-stu-id="83888-122">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="83888-123">別名を使用することによって、`Az` モジュールがインストールされた状態で、古いコマンドレット名を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="83888-123">Aliases enable the ability to use old cmdlet names with the `Az` module installed.</span></span> <span data-ttu-id="83888-124">これらの別名は、選択したスコープのユーザー プロファイルに書き込まれます。</span><span class="sxs-lookup"><span data-stu-id="83888-124">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="83888-125">ユーザー プロファイルが存在しない場合は、ユーザー プロファイルが作成されます。</span><span class="sxs-lookup"><span data-stu-id="83888-125">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="83888-126">このコマンドに別の `-Scope` を使用することができますが、これはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="83888-126">You can use a different `-Scope` for this command, but it's not recommended!</span></span> <span data-ttu-id="83888-127">別名は選択したスコープのユーザー プロファイルに書き込まれるので、できるだけ限られたスコープに対して有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="83888-127">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="83888-128">別名をシステム全体で有効にすると、ローカル スコープに `AzureRM` をインストールしている他のユーザーに問題が生じることもあります。</span><span class="sxs-lookup"><span data-stu-id="83888-128">Enabling aliases system-wide could also cause issues for other users which have `AzureRM` installed in their local scope.</span></span>

<span data-ttu-id="83888-129">別名モードを有効にしたら、、スクリプトを再度実行して、スクリプトが引き続き想定どおりに機能することを確認します。</span><span class="sxs-lookup"><span data-stu-id="83888-129">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="83888-130">モジュールのインポートとコマンドレット名を変更する</span><span class="sxs-lookup"><span data-stu-id="83888-130">Change module imports and cmdlet names</span></span>

<span data-ttu-id="83888-131">一般的に、モジュール名は `AzureRM` および `Azure` が `Az` になるように変更されています。また、コマンドレットについても同様です。</span><span class="sxs-lookup"><span data-stu-id="83888-131">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="83888-132">たとえば、`AzureRM.Compute` モジュールは名前が `Az.Compute` に変更されています。</span><span class="sxs-lookup"><span data-stu-id="83888-132">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="83888-133">`New-AzureRmVM` は `New-AzVM` になり、`Get-AzureStorageBlob` は `Get-AzStorageBlob` になっています。</span><span class="sxs-lookup"><span data-stu-id="83888-133">`New-AzureRmVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="83888-134">この名前付けの変更には例外があるため、名前を変更する前に注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="83888-134">There are exceptions to this naming change that you should be aware of before doing any renaming:</span></span>

| <span data-ttu-id="83888-135">AzureRM モジュール</span><span class="sxs-lookup"><span data-stu-id="83888-135">AzureRM module</span></span> | <span data-ttu-id="83888-136">Az モジュール</span><span class="sxs-lookup"><span data-stu-id="83888-136">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="83888-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="83888-137">AzureRM.DataFactories</span></span> | <span data-ttu-id="83888-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83888-138">Az.DataFactory</span></span> |
| <span data-ttu-id="83888-139">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="83888-139">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="83888-140">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="83888-140">Az.DataFactory</span></span> |
| <span data-ttu-id="83888-141">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="83888-141">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="83888-142">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83888-142">Az.RecoveryServices</span></span> |
| <span data-ttu-id="83888-143">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="83888-143">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="83888-144">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="83888-144">Az.RecoveryServices</span></span> |

## <a name="summary"></a><span data-ttu-id="83888-145">まとめ</span><span class="sxs-lookup"><span data-stu-id="83888-145">Summary</span></span>

<span data-ttu-id="83888-146">これらの手順に従うと、既存のスクリプトをすべて更新して、新しいモジュールを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="83888-146">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="83888-147">これらの手順に関する質問や、移行を困難にしている問題がある場合は、手順を改善できるようにこの記事にコメントを追加してください。</span><span class="sxs-lookup"><span data-stu-id="83888-147">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>