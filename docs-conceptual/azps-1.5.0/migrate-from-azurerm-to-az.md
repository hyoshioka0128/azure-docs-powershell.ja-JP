---
title: AzureRM から Az への Azure PowerShell スクリプトの移行
description: AzureRM モジュールから新しい Az モジュールにスクリプトを移行するための手順とツールについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 28122ca953d62b405f19effbbc680f2dc6202cca
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882570"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a><span data-ttu-id="18811-103">AzureRM から Azure PowerShell Az への移行</span><span class="sxs-lookup"><span data-stu-id="18811-103">Migrate from AzureRM to Azure PowerShell Az</span></span>

<span data-ttu-id="18811-104">Az モジュールには AzureRM との機能パリティがありますが、より短く一貫性のあるコマンドレット名が使用されます。</span><span class="sxs-lookup"><span data-stu-id="18811-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="18811-105">AzureRM コマンドレット用に記述されたスクリプトは、新しいモジュールで自動的に機能するわけではありません。</span><span class="sxs-lookup"><span data-stu-id="18811-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="18811-106">移行を容易にするために、Az には AzureRM を使用する既存のスクリプトを実行できるようにするツールが用意されています。</span><span class="sxs-lookup"><span data-stu-id="18811-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="18811-107">新しいコマンド セットへの移行がないに越したことはありませんが、この記事は、新しいモジュールへの切り替えを開始する際に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="18811-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

<span data-ttu-id="18811-108">AzureRM と Az の間の破壊的変更の完全な一覧については、「[Migration guide for Az 1.0.0 (Az 1.0.0 の移行ガイド)](migrate-az-1.0.0.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="18811-108">To see the full list of breaking changes between AzureRM and Az, see the [Migration guide for Az 1.0.0](migrate-az-1.0.0.md)</span></span>

## <a name="check-for-installed-versions-of-azurerm"></a><span data-ttu-id="18811-109">インストールされている AzureRM のバージョンを確認する</span><span class="sxs-lookup"><span data-stu-id="18811-109">Check for installed versions of AzureRM</span></span>

<span data-ttu-id="18811-110">Az モジュールは AzureRM モジュールと同時にインストールできますが、これはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="18811-110">The Az module can be installed side-by-side with the AzureRM module, but this is not recommended.</span></span> <span data-ttu-id="18811-111">移行手順を実行する前に、システムにインストールされている AzureRM のバージョンを確認します。</span><span class="sxs-lookup"><span data-stu-id="18811-111">Before taking any migration steps, check which versions of AzureRM are installed on your system.</span></span> <span data-ttu-id="18811-112">これにより、スクリプトが最新のリリースで既に実行中であることを確認し、AzureRM をアンインストールせずにコマンドの別名を有効にできるかどうかを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="18811-112">Doing so allows you to make sure scripts are already running on the latest release, and let you know if you can enable command aliases without uninstalling AzureRM.</span></span>

<span data-ttu-id="18811-113">インストールされている AzureRM のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="18811-113">To check which version(s) of AzureRM you have installed, run the command:</span></span>

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="18811-114">既存スクリプトが AzureRM の最新リリースで機能することを確認する</span><span class="sxs-lookup"><span data-stu-id="18811-114">Ensure your existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="18811-115">これは最も重要な手順です。</span><span class="sxs-lookup"><span data-stu-id="18811-115">This is the most important step!</span></span> <span data-ttu-id="18811-116">既存のスクリプトを実行し、AzureRM の "_最新_" リリース (__6.13.1__) で機能することを確認します。</span><span class="sxs-lookup"><span data-stu-id="18811-116">Run your existing scripts, and make sure that they work with the _latest_ release of AzureRM (__6.13.1__).</span></span> <span data-ttu-id="18811-117">スクリプトが機能しない場合は、必ず [AzureRM 移行ガイド](/powershell/azure/azurerm/migration-guide.6.0.0)をお読みください。</span><span class="sxs-lookup"><span data-stu-id="18811-117">If your scripts don't work, make sure to read the [AzureRM migration guide](/powershell/azure/azurerm/migration-guide.6.0.0).</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="18811-118">Azure PowerShell Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="18811-118">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="18811-119">最初の手順では、お使いのプラットフォームに Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="18811-119">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="18811-120">Az をインストールするときは、AzureRM をアンインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="18811-120">When you install Az, it's recommended that you uninstall AzureRM.</span></span> <span data-ttu-id="18811-121">次の手順では、既存のスクリプトを引き続き実行できるようにする方法と、古いコマンドレット名の互換性を有効にする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="18811-121">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="18811-122">Azure PowerShell Az モジュールをインストールするには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="18811-122">To install the Azure PowerShell Az module, follow these steps:</span></span>

* <span data-ttu-id="18811-123">__推奨__:[AzureRM モジュールをアンインストールする](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)。</span><span class="sxs-lookup"><span data-stu-id="18811-123">__RECOMMENDED__: [Uninstall the AzureRM module](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).</span></span>
  <span data-ttu-id="18811-124">最新のバージョンだけでなく、インストールした "_すべて_" のバージョンの AzureRM を必ず削除します。</span><span class="sxs-lookup"><span data-stu-id="18811-124">Make sure that you remove _all_ installed versions of AzureRM, not just the most recent version.</span></span>
* [<span data-ttu-id="18811-125">Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="18811-125">Install the Az module</span></span>](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-compatibility-aliases"></a><span data-ttu-id="18811-126"><a name="aliases"/>AzureRM と互換性のある別名を有効にする</span><span class="sxs-lookup"><span data-stu-id="18811-126"><a name="aliases"/>Enable AzureRM compatibility aliases</span></span> 

> [!IMPORTANT]
>
> <span data-ttu-id="18811-127">AzureRM の "_すべて_" のバージョンをアンインストールした場合のみ、互換モードを有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="18811-127">Only enable compatibility mode if you've uninstalled _all_ versions of AzureRM.</span></span> <span data-ttu-id="18811-128">AzureRM コマンドレットがまだ使用できる状態で互換モードを有効にすると、予期しない動作が発生する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="18811-128">Enabling compatibility mode with AzureRM cmdlets still available may result in unpredictable behavior.</span></span> <span data-ttu-id="18811-129">AzureRM をインストールしたままにする場合はこの手順をスキップしてください。ただし、AzureRM コマンドレットは、Az コマンドレットを呼び出さずに、古いモジュールを使用することに注意してください。</span><span class="sxs-lookup"><span data-stu-id="18811-129">Skip this step if you decided to keep AzureRM installed, but be aware that any AzureRM cmdlets will use the older modules and not call any Az cmdlets.</span></span>

<span data-ttu-id="18811-130">AzureRM をアンインストールして、スクリプトが最新バージョンの AzureRM で機能するようになったら、次の手順で Az モジュールの互換モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="18811-130">With AzureRM uninstalled and your scripts working with the latest AzureRM version, the next step is to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="18811-131">次のコマンドを使用して、互換性を有効にします。</span><span class="sxs-lookup"><span data-stu-id="18811-131">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="18811-132">別名を使用することによって、Az モジュールがインストールされた状態で、古いコマンドレット名を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="18811-132">Aliases enable the ability to use old cmdlet names with the Az module installed.</span></span> <span data-ttu-id="18811-133">これらの別名は、選択したスコープのユーザー プロファイルに書き込まれます。</span><span class="sxs-lookup"><span data-stu-id="18811-133">These aliases are written to the user profile for the selected scope.</span></span> <span data-ttu-id="18811-134">ユーザー プロファイルが存在しない場合は、ユーザー プロファイルが作成されます。</span><span class="sxs-lookup"><span data-stu-id="18811-134">If no user profile exists, one is created.</span></span>

> [!WARNING]
>
> <span data-ttu-id="18811-135">このコマンドに別の `-Scope` を使用することができますが、これはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="18811-135">You can use a different `-Scope` for this command, but it's not recommended.</span></span> <span data-ttu-id="18811-136">別名は選択したスコープのユーザー プロファイルに書き込まれるので、できるだけ限られたスコープに対して有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="18811-136">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="18811-137">別名をシステム全体で有効にすると、ローカル スコープに AzureRM をインストールしている他のユーザーに問題が生じることもあります。</span><span class="sxs-lookup"><span data-stu-id="18811-137">Enabling aliases system-wide could also cause issues for other users which have AzureRM installed in their local scope.</span></span>

<span data-ttu-id="18811-138">別名モードを有効にしたら、、スクリプトを再度実行して、スクリプトが引き続き想定どおりに機能することを確認します。</span><span class="sxs-lookup"><span data-stu-id="18811-138">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span> 

## <a name="change-module-imports-and-cmdlet-names"></a><span data-ttu-id="18811-139">モジュールのインポートとコマンドレット名を変更する</span><span class="sxs-lookup"><span data-stu-id="18811-139">Change module imports and cmdlet names</span></span>

<span data-ttu-id="18811-140">一般的に、モジュール名は `AzureRM` および `Azure` が `Az` になるように変更されています。また、コマンドレットについても同様です。</span><span class="sxs-lookup"><span data-stu-id="18811-140">In general, the module names have been changed so that `AzureRM` and `Azure` become `Az`, and the same for cmdlets.</span></span>
<span data-ttu-id="18811-141">たとえば、`AzureRM.Compute` モジュールは名前が `Az.Compute` に変更されています。</span><span class="sxs-lookup"><span data-stu-id="18811-141">For example, the `AzureRM.Compute` module has been renamed to `Az.Compute`.</span></span> <span data-ttu-id="18811-142">`New-AzureRMVM` は `New-AzVM` になり、`Get-AzureStorageBlob` は `Get-AzStorageBlob` になっています。</span><span class="sxs-lookup"><span data-stu-id="18811-142">`New-AzureRMVM` has become `New-AzVM`, and `Get-AzureStorageBlob` is now `Get-AzStorageBlob`.</span></span>

<span data-ttu-id="18811-143">この名前付けの変更には例外があるため、注意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="18811-143">There are exceptions to this naming change that you should be aware of.</span></span> <span data-ttu-id="18811-144">`AzureRM` または `Azure` から `Az` への変更以外に、一部のモジュールは、コマンドレットのサフィックスに影響を与えることなく、名前が変更されたか、既存のモジュールにマージされています。</span><span class="sxs-lookup"><span data-stu-id="18811-144">Some modules were renamed or merged into existing modules without this affecting the suffix of their cmdlets, other than changing `AzureRM` or `Azure` to `Az`.</span></span> <span data-ttu-id="18811-145">それ以外の場合は、コマンドレットの完全なサフィックスは、新しいモジュール名を反映するように変更されました。</span><span class="sxs-lookup"><span data-stu-id="18811-145">Otherwise, the full cmdlet suffix was changed to reflect the new module name.</span></span>

| <span data-ttu-id="18811-146">AzureRM モジュール</span><span class="sxs-lookup"><span data-stu-id="18811-146">AzureRM module</span></span> | <span data-ttu-id="18811-147">Az モジュール</span><span class="sxs-lookup"><span data-stu-id="18811-147">Az module</span></span> | <span data-ttu-id="18811-148">コマンドレットのサフィックスの変更</span><span class="sxs-lookup"><span data-stu-id="18811-148">Cmdlet suffix changed?</span></span> |
|----------------|-----------|------------------------|
| <span data-ttu-id="18811-149">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18811-149">AzureRM.Profile</span></span> | <span data-ttu-id="18811-150">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="18811-150">Az.Accounts</span></span> | <span data-ttu-id="18811-151">はい</span><span class="sxs-lookup"><span data-stu-id="18811-151">Yes</span></span> |
| <span data-ttu-id="18811-152">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="18811-152">AzureRM.Insights</span></span> | <span data-ttu-id="18811-153">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="18811-153">Az.Monitor</span></span> | <span data-ttu-id="18811-154">はい</span><span class="sxs-lookup"><span data-stu-id="18811-154">Yes</span></span> |
| <span data-ttu-id="18811-155">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="18811-155">AzureRM.DataFactories</span></span> | <span data-ttu-id="18811-156">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="18811-156">Az.DataFactory</span></span> | <span data-ttu-id="18811-157">はい</span><span class="sxs-lookup"><span data-stu-id="18811-157">Yes</span></span> |
| <span data-ttu-id="18811-158">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="18811-158">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="18811-159">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="18811-159">Az.DataFactory</span></span> | <span data-ttu-id="18811-160">はい</span><span class="sxs-lookup"><span data-stu-id="18811-160">Yes</span></span> |
| <span data-ttu-id="18811-161">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="18811-161">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="18811-162">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="18811-162">Az.RecoveryServices</span></span> | <span data-ttu-id="18811-163">いいえ </span><span class="sxs-lookup"><span data-stu-id="18811-163">No</span></span> |
| <span data-ttu-id="18811-164">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="18811-164">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="18811-165">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="18811-165">Az.RecoveryServices</span></span> | <span data-ttu-id="18811-166">いいえ </span><span class="sxs-lookup"><span data-stu-id="18811-166">No</span></span> |
| <span data-ttu-id="18811-167">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="18811-167">AzureRM.Tags</span></span> | <span data-ttu-id="18811-168">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="18811-168">Az.Resources</span></span> | <span data-ttu-id="18811-169">いいえ </span><span class="sxs-lookup"><span data-stu-id="18811-169">No</span></span> |
| <span data-ttu-id="18811-170">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="18811-170">AzureRM.MachineLearningCompute</span></span> | <span data-ttu-id="18811-171">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="18811-171">Az.MachineLearning</span></span> | <span data-ttu-id="18811-172">いいえ </span><span class="sxs-lookup"><span data-stu-id="18811-172">No</span></span> |
| <span data-ttu-id="18811-173">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="18811-173">AzureRM.UsageAggregates</span></span> | <span data-ttu-id="18811-174">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="18811-174">Az.Billing</span></span> | <span data-ttu-id="18811-175">いいえ </span><span class="sxs-lookup"><span data-stu-id="18811-175">No</span></span> |
| <span data-ttu-id="18811-176">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="18811-176">AzureRM.Consumption</span></span> | <span data-ttu-id="18811-177">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="18811-177">Az.Billing</span></span> | <span data-ttu-id="18811-178">いいえ </span><span class="sxs-lookup"><span data-stu-id="18811-178">No</span></span> |

## <a name="summary"></a><span data-ttu-id="18811-179">まとめ</span><span class="sxs-lookup"><span data-stu-id="18811-179">Summary</span></span>

<span data-ttu-id="18811-180">これらの手順に従うと、既存のスクリプトをすべて更新して、新しいモジュールを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="18811-180">By following these steps, you can update all of your existing scripts to use the new module.</span></span> <span data-ttu-id="18811-181">これらの手順に関する質問や、移行を困難にしている問題がある場合は、手順を改善できるようにこの記事にコメントを追加してください。</span><span class="sxs-lookup"><span data-stu-id="18811-181">If you have any questions or problems with these steps that made your migration difficult, please comment on this article so that we can improve the instructions.</span></span>
