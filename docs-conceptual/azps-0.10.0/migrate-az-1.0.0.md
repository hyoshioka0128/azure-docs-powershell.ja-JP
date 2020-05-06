---
title: AzureRM から Azure PowerShell Az 1.0.0 へのすべての変更
description: この移行ガイドには、Az バージョン 1 リリースの Azure PowerShell で行われた破壊的変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2019
ms.openlocfilehash: e5121d61b0f5f68ff3e1f33d774e3533adfeb64f
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "81445545"
---
# <a name="breaking-changes-for-az-100"></a><span data-ttu-id="1ae13-103">Az 1.0.0 の破壊的変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-103">Breaking changes for Az 1.0.0</span></span>

<span data-ttu-id="1ae13-104">このドキュメントでは、AzureRM 6.x と新しい Az モジュール、バージョン 1.x 以降の間の変更について詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-104">This document provides detailed information on the changes between AzureRM 6.x and the new Az module, version 1.x and later.</span></span> <span data-ttu-id="1ae13-105">目次は、スクリプトに影響する可能性のあるモジュール固有の変更など、完全な移行パスのすべての段階で役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-105">The table of contents will help guide you through a full migration path, including module-specific changes that may affect your scripts.</span></span>

<span data-ttu-id="1ae13-106">AzureRM から Az への移行の開始に関する一般的なアドバイスについては、[AzureRM から Az への移行の開始](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-106">For general advice on getting started with a migration from AzureRM to Az, see [Start migration from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1ae13-107">Az 1.0.0 と Az 2.0.0 の間にも重大な変更がありました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-107">There have been breaking changes between Az 1.0.0 and Az 2.0.0 as well.</span></span> <span data-ttu-id="1ae13-108">このガイドに従って AzureRM から Az に更新した後、追加の変更を加える必要がある場合は、[Az 2.0.0 の重大な変更](migrate-az-2.0.0.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-108">After following this guide for updating from AzureRM to Az, see the [Az 2.0.0 breaking changes](migrate-az-2.0.0.md) to find out if you need to make additional changes.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="1ae13-109">目次</span><span class="sxs-lookup"><span data-stu-id="1ae13-109">Table of Contents</span></span>

- [<span data-ttu-id="1ae13-110">重大な変更 - 全般</span><span class="sxs-lookup"><span data-stu-id="1ae13-110">General breaking changes</span></span>](#general-breaking-changes)
  - [<span data-ttu-id="1ae13-111">コマンドレットの名詞プレフィックスの変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-111">Cmdlet noun prefix changes</span></span>](#cmdlet-noun-prefix-changes)
  - [<span data-ttu-id="1ae13-112">モジュール名の変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-112">Module name changes</span></span>](#module-name-changes)
  - [<span data-ttu-id="1ae13-113">削除されたモジュール</span><span class="sxs-lookup"><span data-stu-id="1ae13-113">Removed modules</span></span>](#removed-modules)
  - [<span data-ttu-id="1ae13-114">Windows PowerShell 5.1 と .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="1ae13-114">Windows PowerShell 5.1 and .NET 4.7.2</span></span>](#windows-powershell-51-and-net-472)
  - [<span data-ttu-id="1ae13-115">PSCredential を使用したユーザー ログインの一時的な削除</span><span class="sxs-lookup"><span data-stu-id="1ae13-115">Temporary removal of user login using PSCredential</span></span>](#temporary-removal-of-user-login-using-pscredential)
  - [<span data-ttu-id="1ae13-116">Web ブラウザー プロンプトの代わりにデバイス コード ログインを既定で使用</span><span class="sxs-lookup"><span data-stu-id="1ae13-116">Default device code login instead of web browser prompt</span></span>](#default-device-code-login-instead-of-web-browser-prompt)
- [<span data-ttu-id="1ae13-117">モジュールの破壊的変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-117">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="1ae13-118">Az.ApiManagement (以前の AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="1ae13-118">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>](#azapimanagement-previously-azurermapimanagement)
  - [<span data-ttu-id="1ae13-119">Az.Billing (以前の AzureRM.Billing、AzureRM.Consumption、および AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="1ae13-119">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>](#azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates)
  - [<span data-ttu-id="1ae13-120">Az.CognitiveServices (以前の AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="1ae13-120">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>](#azcognitiveservices-previously-azurermcognitiveservices)
  - [<span data-ttu-id="1ae13-121">Az.Compute (以前の AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="1ae13-121">Az.Compute (previously AzureRM.Compute)</span></span>](#azcompute-previously-azurermcompute)
  - [<span data-ttu-id="1ae13-122">Az.DataFactory (以前の AzureRM.DataFactories および AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="1ae13-122">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>](#azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2)
  - [<span data-ttu-id="1ae13-123">Az.DataLakeAnalytics (以前の AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="1ae13-123">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>](#azdatalakeanalytics-previously-azurermdatalakeanalytics)
  - [<span data-ttu-id="1ae13-124">Az.DataLakeStore (以前の AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="1ae13-124">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>](#azdatalakestore-previously-azurermdatalakestore)
  - [<span data-ttu-id="1ae13-125">Az.KeyVault (以前の AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="1ae13-125">Az.KeyVault (previously AzureRM.KeyVault)</span></span>](#azkeyvault-previously-azurermkeyvault)
  - [<span data-ttu-id="1ae13-126">Az.Media (以前の AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="1ae13-126">Az.Media (previously AzureRM.Media)</span></span>](#azmedia-previously-azurermmedia)
  - [<span data-ttu-id="1ae13-127">Az.Monitor (以前の AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="1ae13-127">Az.Monitor (previously AzureRM.Insights)</span></span>](#azmonitor-previously-azurerminsights)
  - [<span data-ttu-id="1ae13-128">Az.Network (以前の AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="1ae13-128">Az.Network (previously AzureRM.Network)</span></span>](#aznetwork-previously-azurermnetwork)
  - [<span data-ttu-id="1ae13-129">Az.OperationalInsights (以前の AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="1ae13-129">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>](#azoperationalinsights-previously-azurermoperationalinsights)
  - [<span data-ttu-id="1ae13-130">Az.RecoveryServices (以前の AzureRM.RecoveryServices、AzureRM.RecoveryServices.Backup、および AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="1ae13-130">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>](#azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery)
  - [<span data-ttu-id="1ae13-131">Az.Resources (以前の AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="1ae13-131">Az.Resources (previously AzureRM.Resources)</span></span>](#azresources-previously-azurermresources)
  - [<span data-ttu-id="1ae13-132">Az.ServiceFabric (以前の AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="1ae13-132">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>](#azservicefabric-previously-azurermservicefabric)
  - [<span data-ttu-id="1ae13-133">Az.Sql (以前の AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="1ae13-133">Az.Sql (previously AzureRM.Sql)</span></span>](#azsql-previously-azurermsql)
  - [<span data-ttu-id="1ae13-134">Az.Storage (以前の Azure.Storage and AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="1ae13-134">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>](#azstorage-previously-azurestorage-and-azurermstorage)
  - [<span data-ttu-id="1ae13-135">Az.Websites (以前の AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="1ae13-135">Az.Websites (previously AzureRM.Websites)</span></span>](#azwebsites-previously-azurermwebsites)

## <a name="general-breaking-changes"></a><span data-ttu-id="1ae13-136">重大な変更 - 全般</span><span class="sxs-lookup"><span data-stu-id="1ae13-136">General breaking changes</span></span>

<span data-ttu-id="1ae13-137">このセクションでは、Az モジュールの再設計の一部である、一般的な重大な変更について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-137">This section details the general breaking changes that are part of the redesign of the Az module.</span></span>

### <a name="cmdlet-noun-prefix-changes"></a><span data-ttu-id="1ae13-138">コマンドレットの名詞プレフィックスの変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-138">Cmdlet Noun Prefix Changes</span></span>

<span data-ttu-id="1ae13-139">AzureRM モジュールでは、コマンドレットの名詞プレフィックスとして `AzureRM` または `Azure` が使用されていました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-139">In the AzureRM module, cmdlets used either `AzureRM` or `Azure` as a noun prefix.</span></span>  <span data-ttu-id="1ae13-140">Az ではコマンドレット名が簡略化され、正規化されています。そのため、すべてのコマンドレットでコマンドレット名詞プレフィックスとして "Az" が使用されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-140">Az simplifies and normalizes cmdlet names, so that all cmdlets use 'Az' as their cmdlet noun prefix.</span></span> <span data-ttu-id="1ae13-141">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-141">For example:</span></span>

```azurepowershell-interactive
Get-AzureRMVM
Get-AzureKeyVaultSecret
```

<span data-ttu-id="1ae13-142">次のように変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-142">Has changed to:</span></span>

```azurepowershell-interactive
Get-AzVM
Get-AzKeyVaultSecret
```

<span data-ttu-id="1ae13-143">これらの新しいコマンドレット名に簡単に移行できるように、Az では [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) と [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias) の 2 つの新しいコマンドレットが導入されています。</span><span class="sxs-lookup"><span data-stu-id="1ae13-143">To make the transition to these new cmdlet names simpler, Az introduces two new cmdlets, [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) and [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias).</span></span>  <span data-ttu-id="1ae13-144">`Enable-AzureRmAlias` では、新しい Az コマンドレット名に対応する、AzureRM の古いコマンドレット名のエイリアスが作成されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-144">`Enable-AzureRmAlias` creates aliases for the older cmdlet names in AzureRM that map to the newer Az cmdlet names.</span></span> <span data-ttu-id="1ae13-145">`-Scope` で `Enable-AzureRmAlias` 引数を使用すると、エイリアスを有効にする場所を選択することができます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-145">Using the `-Scope` argument with `Enable-AzureRmAlias` allows you to choose where aliases are enabled.</span></span>

<span data-ttu-id="1ae13-146">たとえば、AzureRM の次のスクリプトがあるとします。</span><span class="sxs-lookup"><span data-stu-id="1ae13-146">For example, the following script in AzureRM:</span></span>

```azurepowershell-interactive
#Requires -Modules AzureRM.Storage
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="1ae13-147">`Enable-AzureRmAlias` を使用すると、最小限の変更で実行できます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-147">Can be run with minimal changes using `Enable-AzureRmAlias`:</span></span>

```azurepowershell-interactive
#Requires -Modules Az.Storage
Enable-AzureRmAlias -Scope Process
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="1ae13-148">`Enable-AzureRmAlias -Scope CurrentUser` を実行すると、現在のユーザーが開くすべての PowerShell セッションでエイリアスが有効になるため、このコマンドレットの実行後は、次のようなスクリプトを変更する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="1ae13-148">Running `Enable-AzureRmAlias -Scope CurrentUser` will enable the aliases for all PowerShell sessions you open, so that after executing this cmdlet, a script like this would not need to be changed at all:</span></span>

```azurepowershell-interactive
Get-AzureRmStorageAccount | Get-AzureStorageContainer | Get-AzureStorageBlob
```

<span data-ttu-id="1ae13-149">エイリアス コマンドレットの使用方法の詳細については、[Enable-AzureRmAlias リファレンス](/powershell/module/az.accounts/enable-azurermalias)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-149">For complete details on the usage of the alias cmdlets, see the [Enable-AzureRmAlias reference](/powershell/module/az.accounts/enable-azurermalias).</span></span>

<span data-ttu-id="1ae13-150">エイリアスを無効にする準備ができたら、`Disable-AzureRmAlias` により作成されたエイリアスが削除されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-150">When you're ready to disable aliases, `Disable-AzureRmAlias` removes the created aliases.</span></span> <span data-ttu-id="1ae13-151">詳細については、[Disable-AzureRmAlias リファレンス](/powershell/module/az.accounts/disable-azurermalias)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-151">For complete details, see the [Disable-AzureRmAlias reference](/powershell/module/az.accounts/disable-azurermalias).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1ae13-152">エイリアスを無効にする場合は、必ず、エイリアスが有効になっている_すべて_のスコープに対して無効にしてください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-152">When disabling aliases, make sure that they are disabled for _all_ scopes which had aliases enabled.</span></span>

### <a name="module-name-changes"></a><span data-ttu-id="1ae13-153">モジュール名の変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-153">Module Name Changes</span></span>

<span data-ttu-id="1ae13-154">次のモジュールを除き、モジュール名が `AzureRM.*` から `Az.*` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-154">The module names have changed from `AzureRM.*` to `Az.*`, except for the following modules:</span></span>

| <span data-ttu-id="1ae13-155">AzureRM モジュール</span><span class="sxs-lookup"><span data-stu-id="1ae13-155">AzureRM module</span></span> | <span data-ttu-id="1ae13-156">Az モジュール</span><span class="sxs-lookup"><span data-stu-id="1ae13-156">Az module</span></span> |
|----------------|-----------|
| <span data-ttu-id="1ae13-157">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1ae13-157">Azure.Storage</span></span> | <span data-ttu-id="1ae13-158">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1ae13-158">Az.Storage</span></span> |
| <span data-ttu-id="1ae13-159">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1ae13-159">Azure.AnalysisServices</span></span> | <span data-ttu-id="1ae13-160">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1ae13-160">Az.AnalysisServices</span></span> |
| <span data-ttu-id="1ae13-161">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="1ae13-161">AzureRM.Profile</span></span> | <span data-ttu-id="1ae13-162">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1ae13-162">Az.Accounts</span></span> |
| <span data-ttu-id="1ae13-163">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="1ae13-163">AzureRM.Insights</span></span> | <span data-ttu-id="1ae13-164">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1ae13-164">Az.Monitor</span></span> |
| <span data-ttu-id="1ae13-165">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="1ae13-165">AzureRM.DataFactories</span></span> | <span data-ttu-id="1ae13-166">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1ae13-166">Az.DataFactory</span></span> |
| <span data-ttu-id="1ae13-167">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1ae13-167">AzureRM.DataFactoryV2</span></span> | <span data-ttu-id="1ae13-168">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1ae13-168">Az.DataFactory</span></span> |
| <span data-ttu-id="1ae13-169">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1ae13-169">AzureRM.RecoveryServices.Backup</span></span> | <span data-ttu-id="1ae13-170">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1ae13-170">Az.RecoveryServices</span></span> |
| <span data-ttu-id="1ae13-171">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1ae13-171">AzureRM.RecoveryServices.SiteRecovery</span></span> | <span data-ttu-id="1ae13-172">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1ae13-172">Az.RecoveryServices</span></span> |
| <span data-ttu-id="1ae13-173">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="1ae13-173">AzureRM.Tags</span></span> | <span data-ttu-id="1ae13-174">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1ae13-174">Az.Resources</span></span> |
| <span data-ttu-id="1ae13-175">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="1ae13-175">AzureRM.MachineLearningCompute</span></span> | <span data-ttu-id="1ae13-176">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1ae13-176">Az.MachineLearning</span></span> |
| <span data-ttu-id="1ae13-177">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="1ae13-177">AzureRM.UsageAggregates</span></span> | <span data-ttu-id="1ae13-178">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="1ae13-178">Az.Billing</span></span> |
| <span data-ttu-id="1ae13-179">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="1ae13-179">AzureRM.Consumption</span></span> | <span data-ttu-id="1ae13-180">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="1ae13-180">Az.Billing</span></span> |

<span data-ttu-id="1ae13-181">モジュール名が変更されたので、`#Requires` または `Import-Module` を使用して特定のモジュールを読み込むスクリプトは、新しいモジュールを代わりに使用するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-181">The changes in module names mean that any script that uses `#Requires` or `Import-Module` to load specific modules will need to be changed to use the new module instead.</span></span> <span data-ttu-id="1ae13-182">コマンドレットのサフィックスが変更されていないモジュールの場合、これは、モジュール名が変更されていても操作スペースを示すサフィックスは_変更されていない_ことを意味します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-182">For modules where the cmdlet suffix has not changed, this means that although the module name has changed, the suffix indicating the operation space has _not_.</span></span>

#### <a name="migrating-requires-and-import-module-statements"></a><span data-ttu-id="1ae13-183">#Requires ステートメントと Import-Module ステートメントの移行</span><span class="sxs-lookup"><span data-stu-id="1ae13-183">Migrating #Requires and Import-Module Statements</span></span>

<span data-ttu-id="1ae13-184">`#Requires` または `Import-Module` を使用して AzureRM モジュールへの依存関係を宣言しているスクリプトは、新しいモジュール名を使用するように更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-184">Scripts that use `#Requires` or `Import-Module` to declare a dependency on AzureRM modules must be updated to use the new module names.</span></span> <span data-ttu-id="1ae13-185">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-185">For example:</span></span>

```azurepowershell-interactive
#Requires -Module AzureRM.Compute
```

<span data-ttu-id="1ae13-186">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-186">Should be changed to:</span></span>

```azurepowershell-interactive
#Requires -Module Az.Compute
```

<span data-ttu-id="1ae13-187">`Import-Module` の場合:</span><span class="sxs-lookup"><span data-stu-id="1ae13-187">For `Import-Module`:</span></span>

```azurepowershell-interactive
Import-Module -Name AzureRM.Compute
```

<span data-ttu-id="1ae13-188">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-188">Should be changed to:</span></span>

```azurepowershell-interactive
Import-Module -Name Az.Compute
```

### <a name="migrating-fully-qualified-cmdlet-invocations"></a><span data-ttu-id="1ae13-189">完全修飾コマンドレットの呼び出しの移行</span><span class="sxs-lookup"><span data-stu-id="1ae13-189">Migrating Fully-Qualified Cmdlet Invocations</span></span>

<span data-ttu-id="1ae13-190">次のように、モジュール修飾コマンドレットの呼び出しを使用するスクリプトは、</span><span class="sxs-lookup"><span data-stu-id="1ae13-190">Scripts that use module-qualified cmdlet invocations, such as:</span></span>

```azurepowershell-interactive
AzureRM.Compute\Get-AzureRmVM
```

<span data-ttu-id="1ae13-191">新しいモジュール名とコマンドレット名を使用するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-191">Must be changed to use the new module and cmdlet names:</span></span>

```azurepowershell-interactive
Az.Compute\Get-AzVM
```

### <a name="migrating-module-manifest-dependencies"></a><span data-ttu-id="1ae13-192">モジュール マニフェスト依存関係の移行</span><span class="sxs-lookup"><span data-stu-id="1ae13-192">Migrating module manifest dependencies</span></span>

<span data-ttu-id="1ae13-193">モジュール マニフェスト (.psd1) ファイルを使用して AzureRM モジュールへの依存関係を表すモジュールは、`RequiredModules` セクションのモジュール名を更新する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-193">Modules that express dependencies on AzureRM modules through a module manifest (.psd1) file will need to updated the module names in their `RequiredModules` section:</span></span>

```powershell
RequiredModules = @(@{ModuleName="AzureRM.Profile"; ModuleVersion="5.8.2"})
```

<span data-ttu-id="1ae13-194">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-194">Must be changed to:</span></span>

```powershell
RequiredModules = @(@{ModuleName="Az.Profile"; ModuleVersion="1.0.0"})
```

### <a name="removed-modules"></a><span data-ttu-id="1ae13-195">削除されたモジュール</span><span class="sxs-lookup"><span data-stu-id="1ae13-195">Removed modules</span></span>

<span data-ttu-id="1ae13-196">次のモジュールが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-196">The following modules have been removed:</span></span>

- `AzureRM.Backup`
- `AzureRM.Compute.ManagedService`
- `AzureRM.Scheduler`

<span data-ttu-id="1ae13-197">これらのサービス用のツールは積極的にサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-197">The tools for these services are no longer actively supported.</span></span>  <span data-ttu-id="1ae13-198">都合がつき次第、代替サービスに移行することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="1ae13-198">Customers are encouraged to move to alternative services as soon as it is convenient.</span></span>

### <a name="windows-powershell-51-and-net-472"></a><span data-ttu-id="1ae13-199">Windows PowerShell 5.1 と .NET 4.7.2</span><span class="sxs-lookup"><span data-stu-id="1ae13-199">Windows PowerShell 5.1 and .NET 4.7.2</span></span>

<span data-ttu-id="1ae13-200">Windows 用の PowerShell 5.1 で Az を使用するには、.NET Framework 4.7.2 をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-200">Using Az with PowerShell 5.1 for Windows requires the installation of .NET Framework 4.7.2.</span></span> <span data-ttu-id="1ae13-201">PowerShell Core 6.x 以降を使用する場合、.NET Fremework は不要です。</span><span class="sxs-lookup"><span data-stu-id="1ae13-201">Using PowerShell Core 6.x or later does not require .NET Framework.</span></span>

### <a name="temporary-removal-of-user-login-using-pscredential"></a><span data-ttu-id="1ae13-202">PSCredential を使用したユーザー ログインの一時的な削除</span><span class="sxs-lookup"><span data-stu-id="1ae13-202">Temporary removal of User login using PSCredential</span></span>

<span data-ttu-id="1ae13-203">.NET Standard の認証フローの変更により、PSCredential を使用したユーザー ログインが一時的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-203">Due to changes in the authentication flow for .NET Standard, we are temporarily removing user login via PSCredential.</span></span> <span data-ttu-id="1ae13-204">この機能は、Windows 用の PowerShell 5.1 の 2019/1/15 リリースで再導入されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-204">This capability will be re-introduced in the 1/15/2019 release for PowerShell 5.1 for Windows.</span></span> <span data-ttu-id="1ae13-205">詳細については、[こちらの GitHub の問題](https://github.com/Azure/azure-powershell/issues/7430)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-205">This is discussed in detail in [this GitHub issue.](https://github.com/Azure/azure-powershell/issues/7430)</span></span>

### <a name="default-device-code-login-instead-of-web-browser-prompt"></a><span data-ttu-id="1ae13-206">Web ブラウザー プロンプトの代わりにデバイス コード ログインを既定で使用</span><span class="sxs-lookup"><span data-stu-id="1ae13-206">Default device code login instead of web browser prompt</span></span>

<span data-ttu-id="1ae13-207">.NET Standard の認証フローの変更により、対話型ログイン時の既定のログイン フローとしてデバイス ログインが使用されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-207">Due to changes in the authentication flow for .NET Standard, we are using device login as the default login flow during interactive login.</span></span> <span data-ttu-id="1ae13-208">Web ブラウザー ベースのログインは、Windows 用の PowerShell 5.1 の 2019/1/15 リリースで既定のログインとして再導入されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-208">Web browser based login will be re-introduced for PowerShell 5.1 for Windows as the default in the 1/15/2019 release.</span></span> <span data-ttu-id="1ae13-209">その時点で、ユーザーは Switch パラメーターを使用してデバイス ログインを選択できるようになります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-209">At that time, users will be able to choose device login using a Switch parameter.</span></span>

## <a name="module-breaking-changes"></a><span data-ttu-id="1ae13-210">モジュールの破壊的変更</span><span class="sxs-lookup"><span data-stu-id="1ae13-210">Module breaking changes</span></span>

<span data-ttu-id="1ae13-211">このセクションでは、個々のモジュールとコマンドレットの特定の重大な変更について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-211">This section details specific breaking changes for individual modules and cmdlets.</span></span>

### <a name="azapimanagement-previously-azurermapimanagement"></a><span data-ttu-id="1ae13-212">Az.ApiManagement (以前の AzureRM.ApiManagement)</span><span class="sxs-lookup"><span data-stu-id="1ae13-212">Az.ApiManagement (previously AzureRM.ApiManagement)</span></span>

- <span data-ttu-id="1ae13-213">次のコマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-213">Removed the following cmdlets:</span></span>
  - <span data-ttu-id="1ae13-214">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="1ae13-214">New-AzureRmApiManagementHostnameConfiguration</span></span>
  - <span data-ttu-id="1ae13-215">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="1ae13-215">Set-AzureRmApiManagementHostnames</span></span>
  - <span data-ttu-id="1ae13-216">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="1ae13-216">Update-AzureRmApiManagementDeployment</span></span>
  - <span data-ttu-id="1ae13-217">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="1ae13-217">Import-AzureRmApiManagementHostnameCertificate</span></span>
  - <span data-ttu-id="1ae13-218">代わりに、**Set-AzApiManagement** コマンドレットを使用してこれらのプロパティを設定します</span><span class="sxs-lookup"><span data-stu-id="1ae13-218">Use **Set-AzApiManagement** cmdlet to set these properties instead</span></span>
- <span data-ttu-id="1ae13-219">次のプロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-219">Removed the following properties:</span></span>
  - <span data-ttu-id="1ae13-220">`PortalHostnameConfiguration` から、`ProxyHostnameConfiguration` 型の `ManagementHostnameConfiguration`、`ScmHostnameConfiguration`、`PsApiManagementHostnameConfiguration`、`PsApiManagementContext` の各プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-220">Removed property `PortalHostnameConfiguration`, `ProxyHostnameConfiguration`, `ManagementHostnameConfiguration` and `ScmHostnameConfiguration` of type `PsApiManagementHostnameConfiguration` from `PsApiManagementContext`.</span></span> <span data-ttu-id="1ae13-221">代わりに、`PortalCustomHostnameConfiguration` 型の `ProxyCustomHostnameConfiguration`、`ManagementCustomHostnameConfiguration`、`ScmCustomHostnameConfiguration`、`PsApiManagementCustomHostNameConfiguration` を使用します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-221">Instead use `PortalCustomHostnameConfiguration`, `ProxyCustomHostnameConfiguration`, `ManagementCustomHostnameConfiguration` and `ScmCustomHostnameConfiguration` of type `PsApiManagementCustomHostNameConfiguration`.</span></span>
  - <span data-ttu-id="1ae13-222">PsApiManagementContext から `StaticIPs` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-222">Removed property `StaticIPs` from PsApiManagementContext.</span></span> <span data-ttu-id="1ae13-223">このプロパティは、`PublicIPAddresses` と `PrivateIPAddresses` に分割されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-223">The property has been split into `PublicIPAddresses` and `PrivateIPAddresses`.</span></span>
  - <span data-ttu-id="1ae13-224">New-AzureApiManagementVirtualNetwork コマンドレットから、必須の `Location` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-224">Removed required property `Location` from New-AzureApiManagementVirtualNetwork cmdlet.</span></span>

### <a name="azbilling-previously-azurermbilling-azurermconsumption-and-azurermusageaggregates"></a><span data-ttu-id="1ae13-225">Az.Billing (以前の AzureRM.Billing、AzureRM.Consumption、および AzureRM.UsageAggregates)</span><span class="sxs-lookup"><span data-stu-id="1ae13-225">Az.Billing (previously AzureRM.Billing, AzureRM.Consumption, and AzureRM.UsageAggregates)</span></span>

- <span data-ttu-id="1ae13-226">`InvoiceName` コマンドレットから、`Get-AzConsumptionUsageDetail` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-226">The `InvoiceName` parameter was removed from the `Get-AzConsumptionUsageDetail` cmdlet.</span></span>  <span data-ttu-id="1ae13-227">スクリプトでは、請求書に他の ID パラメーターを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-227">Scripts will need to use other identity parameters for the invoice.</span></span>

### <a name="azcognitiveservices-previously-azurermcognitiveservices"></a><span data-ttu-id="1ae13-228">Az.CognitiveServices (以前の AzureRM.CognitiveServices)</span><span class="sxs-lookup"><span data-stu-id="1ae13-228">Az.CognitiveServices (previously AzureRM.CognitiveServices)</span></span>

- <span data-ttu-id="1ae13-229">`GetSkusWithAccountParamSetName` コマンドレットから、`Get-AzCognitiveServicesAccountSkus` パラメーター セットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-229">Removed `GetSkusWithAccountParamSetName` parameter set from `Get-AzCognitiveServicesAccountSkus` cmdlet.</span></span>  <span data-ttu-id="1ae13-230">ResourceGroupName とアカウント名を使用するのではなく、アカウントの種類と場所で SKU を取得する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-230">You must get Skus by Account Type and Location, instead of using ResourceGroupName and Account Name.</span></span>

### <a name="azcompute-previously-azurermcompute"></a><span data-ttu-id="1ae13-231">Az.Compute (以前の AzureRM.Compute)</span><span class="sxs-lookup"><span data-stu-id="1ae13-231">Az.Compute (previously AzureRM.Compute)</span></span>

- <span data-ttu-id="1ae13-232">`IdentityIds` および `Identity` オブジェクトの `PSVirtualMachine` プロパティから `PSVirtualMachineScaleSet` が削除されました。スクリプトでは、このフィールドの値を使用して処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-232">`IdentityIds` are removed from `Identity` property in `PSVirtualMachine` and `PSVirtualMachineScaleSet` objects Scripts should no longer use the value of this field to make processing decisions.</span></span>
- <span data-ttu-id="1ae13-233">`InstanceView` オブジェクトの `PSVirtualMachineScaleSetVM` プロパティの型が、`VirtualMachineInstanceView` から `VirtualMachineScaleSetVMInstanceView` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-233">The type of `InstanceView` property of `PSVirtualMachineScaleSetVM` object is changed from `VirtualMachineInstanceView` to `VirtualMachineScaleSetVMInstanceView`</span></span>
- <span data-ttu-id="1ae13-234">`AutoOSUpgradePolicy` プロパティから、`AutomaticOSUpgrade` および `UpgradePolicy` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-234">`AutoOSUpgradePolicy` and `AutomaticOSUpgrade` properties are removed from `UpgradePolicy` property</span></span>
- <span data-ttu-id="1ae13-235">`Sku` オブジェクトの `PSSnapshotUpdate` プロパティの型が、`DiskSku` から `SnapshotSku` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-235">The type of `Sku` property in `PSSnapshotUpdate` object is changed from `DiskSku` to `SnapshotSku`</span></span>
- <span data-ttu-id="1ae13-236">`VmScaleSetVMParameterSet` コマンドレットから、`Add-AzVMDataDisk` が削除されました。スケールセット VM にデータ ディスクを個別に追加することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-236">`VmScaleSetVMParameterSet` is removed from `Add-AzVMDataDisk` cmdlet, you can no longer add a data disk individually to a ScaleSet VM.</span></span>

### <a name="azdatafactory-previously-azurermdatafactories-and-azurermdatafactoryv2"></a><span data-ttu-id="1ae13-237">Az.DataFactory (以前の AzureRM.DataFactories および AzureRM.DataFactoryV2)</span><span class="sxs-lookup"><span data-stu-id="1ae13-237">Az.DataFactory (previously AzureRM.DataFactories and AzureRM.DataFactoryV2)</span></span>

- <span data-ttu-id="1ae13-238">`GatewayName` コマンドレットで `New-AzDataFactoryEncryptValue` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-238">The `GatewayName` parameter has become mandatory in the `New-AzDataFactoryEncryptValue` cmdlet</span></span>
- <span data-ttu-id="1ae13-239">`New-AzDataFactoryGatewayKey` コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-239">Removed `New-AzDataFactoryGatewayKey` cmdlet</span></span>
- <span data-ttu-id="1ae13-240">`LinkedServiceName` コマンドレットから、`Get-AzDataFactoryV2ActivityRun` パラメーターが削除されました。スクリプトでは、このフィールドの値を使用して処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-240">Removed `LinkedServiceName` parameter from `Get-AzDataFactoryV2ActivityRun` cmdlet Scripts should no longer use the value of this field to make processing decisions.</span></span>

### <a name="azdatalakeanalytics-previously-azurermdatalakeanalytics"></a><span data-ttu-id="1ae13-241">Az.DataLakeAnalytics (以前の AzureRM.DataLakeAnalytics)</span><span class="sxs-lookup"><span data-stu-id="1ae13-241">Az.DataLakeAnalytics (previously AzureRM.DataLakeAnalytics)</span></span>

- <span data-ttu-id="1ae13-242">非推奨の `New-AzDataLakeAnalyticsCatalogSecret`、`Remove-AzDataLakeAnalyticsCatalogSecret`、`Set-AzDataLakeAnalyticsCatalogSecret` の各コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-242">Removed deprecated cmdlets: `New-AzDataLakeAnalyticsCatalogSecret`, `Remove-AzDataLakeAnalyticsCatalogSecret`, and `Set-AzDataLakeAnalyticsCatalogSecret`</span></span>

### <a name="azdatalakestore-previously-azurermdatalakestore"></a><span data-ttu-id="1ae13-243">Az.DataLakeStore (以前の AzureRM.DataLakeStore)</span><span class="sxs-lookup"><span data-stu-id="1ae13-243">Az.DataLakeStore (previously AzureRM.DataLakeStore)</span></span>

- <span data-ttu-id="1ae13-244">次のコマンドレットの `Encoding` パラメーターの型が、`FileSystemCmdletProviderEncoding` から `System.Text.Encoding` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-244">The following cmdlets have had the `Encoding` parameter changed from the type `FileSystemCmdletProviderEncoding` to `System.Text.Encoding`.</span></span> <span data-ttu-id="1ae13-245">この変更により、エンコード値 `String` と `Oem` が削除されます。</span><span class="sxs-lookup"><span data-stu-id="1ae13-245">This change removes the encoding values `String` and `Oem`.</span></span> <span data-ttu-id="1ae13-246">以前からの他のエンコード値はすべて残ります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-246">All the other prior encoding values remain.</span></span>
  - <span data-ttu-id="1ae13-247">New-AzureRmDataLakeStoreItem</span><span class="sxs-lookup"><span data-stu-id="1ae13-247">New-AzureRmDataLakeStoreItem</span></span>
  - <span data-ttu-id="1ae13-248">Add-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="1ae13-248">Add-AzureRmDataLakeStoreItemContent</span></span>
  - <span data-ttu-id="1ae13-249">Get-AzureRmDataLakeStoreItemContent</span><span class="sxs-lookup"><span data-stu-id="1ae13-249">Get-AzureRmDataLakeStoreItemContent</span></span>
- <span data-ttu-id="1ae13-250">`Tags` および `New-AzDataLakeStoreAccount` コマンドレットから、非推奨の `Set-AzDataLakeStoreAccount` プロパティのエイリアスが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-250">Removed deprecated `Tags` property alias from `New-AzDataLakeStoreAccount` and `Set-AzDataLakeStoreAccount` cmdlets</span></span>

  <span data-ttu-id="1ae13-251">次のコマンドレットを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="1ae13-251">Scripts using</span></span>
  ```azurepowershell-interactive
  New-AzureRMDataLakeStoreAccount -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="1ae13-252">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-252">Should be changed to</span></span>
  ```azurepowershell-interactive
  New-AzDataLakeStoreAccount -Tag @{TagName="TagValue"}
  ```

- <span data-ttu-id="1ae13-253">`Identity` オブジェクトから、非推奨の `EncryptionState`、`EncryptionProvisioningState`、`EncryptionConfig`、`FirewallState`、`FirewallRules`、`VirtualNetworkRules`、`TrustedIdProviderState`、`TrustedIdProviders`、`DefaultGroup`、`NewTier`、`CurrentTier`、`FirewallAllowAzureIps`、`PSDataLakeStoreAccountBasic` の各プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-253">Removed deprecated properties `Identity`, `EncryptionState`, `EncryptionProvisioningState`, `EncryptionConfig`, `FirewallState`, `FirewallRules`, `VirtualNetworkRules`, `TrustedIdProviderState`, `TrustedIdProviders`, `DefaultGroup`, `NewTier`, `CurrentTier`, `FirewallAllowAzureIps` from `PSDataLakeStoreAccountBasic` object.</span></span>  <span data-ttu-id="1ae13-254">`PSDatalakeStoreAccount` から返された `Get-AzDataLakeStoreAccount` を使用するスクリプトでは、これらのプロパティを参照しないでください。</span><span class="sxs-lookup"><span data-stu-id="1ae13-254">Any script that uses the `PSDatalakeStoreAccount` returned from `Get-AzDataLakeStoreAccount` should not reference these properties.</span></span>

### <a name="azkeyvault-previously-azurermkeyvault"></a><span data-ttu-id="1ae13-255">Az.KeyVault (以前の AzureRM.KeyVault)</span><span class="sxs-lookup"><span data-stu-id="1ae13-255">Az.KeyVault (previously AzureRM.KeyVault)</span></span>

- <span data-ttu-id="1ae13-256">`PurgeDisabled`、`PSKeyVaultKeyAttributes`、`PSKeyVaultKeyIdentityItem` の各オブジェクトから、`PSKeyVaultSecretAttributes` プロパティが削除されました。スクリプトでは、```PurgeDisabled``` プロパティを参照して処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-256">The `PurgeDisabled` property was removed from the `PSKeyVaultKeyAttributes`, `PSKeyVaultKeyIdentityItem`, and `PSKeyVaultSecretAttributes` objects Scripts should no longer reference the ```PurgeDisabled``` property to make processing decisions.</span></span>

### <a name="azmedia-previously-azurermmedia"></a><span data-ttu-id="1ae13-257">Az.Media (以前の AzureRM.Media)</span><span class="sxs-lookup"><span data-stu-id="1ae13-257">Az.Media (previously AzureRM.Media)</span></span>

- <span data-ttu-id="1ae13-258">`Tags` コマンドレットから、非推奨の `New-AzMediaService` プロパティのエイリアスが削除されました。次のコマンドレットを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="1ae13-258">Remove deprecated `Tags` property alias from `New-AzMediaService` cmdlet Scripts using</span></span>
  ```azurepowershell-interactive
  New-AzureRMMediaService -Tags @{TagName="TagValue"}
  ```

  <span data-ttu-id="1ae13-259">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-259">Should be changed to</span></span>
  ```azurepowershell-interactive
  New-AzMediaService -Tag @{TagName="TagValue"}
  ```

### <a name="azmonitor-previously-azurerminsights"></a><span data-ttu-id="1ae13-260">Az.Monitor (以前の AzureRM.Insights)</span><span class="sxs-lookup"><span data-stu-id="1ae13-260">Az.Monitor (previously AzureRM.Insights)</span></span>

- <span data-ttu-id="1ae13-261">単数形のパラメーター名を優先して、`Categories` コマンドレットから複数形のパラメーター名 `Timegrains` と `Set-AzDiagnosticSetting` が削除されました。次のコマンドレットを使用するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="1ae13-261">Removed plural names `Categories` and `Timegrains` parameter in favor of singular parameter names from `Set-AzDiagnosticSetting` cmdlet Scripts using</span></span>
  ```azurepowershell-interactive
  Set-AzureRmDiagnosticSetting -Timegrains PT1M -Categories Category1, Category2
  ```

  <span data-ttu-id="1ae13-262">次のように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-262">Should be changed to</span></span>
  ```azurepowershell-interactive
  Set-AzDiagnosticSetting -Timegrain PT1M -Category Category1, Category2
  ```

### <a name="aznetwork-previously-azurermnetwork"></a><span data-ttu-id="1ae13-263">Az.Network (以前の AzureRM.Network)</span><span class="sxs-lookup"><span data-stu-id="1ae13-263">Az.Network (previously AzureRM.Network)</span></span>

- <span data-ttu-id="1ae13-264">`ResourceId` コマンドレットから、非推奨の `Get-AzServiceEndpointPolicyDefinition` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-264">Removed deprecated `ResourceId` parameter from `Get-AzServiceEndpointPolicyDefinition` cmdlet</span></span>
- <span data-ttu-id="1ae13-265">`EnableVmProtection` オブジェクトから、非推奨の `PSVirtualNetwork` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-265">Removed deprecated `EnableVmProtection` property from `PSVirtualNetwork` object</span></span>
- <span data-ttu-id="1ae13-266">非推奨の `Set-AzVirtualNetworkGatewayVpnClientConfig` コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-266">Removed deprecated `Set-AzVirtualNetworkGatewayVpnClientConfig` cmdlet</span></span>

<span data-ttu-id="1ae13-267">スクリプトでは、これらのフィールドの値に基づいて処理を決定することはできなくなりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-267">Scripts should no longer make processing decisions based on the values fo these fields.</span></span>

### <a name="azoperationalinsights-previously-azurermoperationalinsights"></a><span data-ttu-id="1ae13-268">Az.OperationalInsights (以前の AzureRM.OperationalInsights)</span><span class="sxs-lookup"><span data-stu-id="1ae13-268">Az.OperationalInsights (previously AzureRM.OperationalInsights)</span></span>

- <span data-ttu-id="1ae13-269">`Get-AzOperationalInsightsDataSource` の既定のパラメーター セットが削除され、`ByWorkspaceNameByKind` が既定のパラメーター セットになりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-269">Default parameter set for `Get-AzOperationalInsightsDataSource` is removed, and `ByWorkspaceNameByKind` has become the default parameter set</span></span>

  <span data-ttu-id="1ae13-270">次のコマンドレットを使用してデータ ソースのリストを表示するスクリプトは</span><span class="sxs-lookup"><span data-stu-id="1ae13-270">Scripts that listed data sources using</span></span>
  ```azurepowershell-interactive
  Get-AzureRmOperationalInsightsDataSource
  ```

  <span data-ttu-id="1ae13-271">種類 (Kind) を指定するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-271">Should be changed to specify a Kind</span></span>
  ```azurepowershell-interactive
  Get-AzOperationalInsightsDataSource -Kind AzureActivityLog
  ```

### <a name="azrecoveryservices-previously-azurermrecoveryservices-azurermrecoveryservicesbackup-and-azurermrecoveryservicessiterecovery"></a><span data-ttu-id="1ae13-272">Az.RecoveryServices (以前の AzureRM.RecoveryServices、AzureRM.RecoveryServices.Backup、および AzureRM.RecoveryServices.SiteRecovery)</span><span class="sxs-lookup"><span data-stu-id="1ae13-272">Az.RecoveryServices (previously AzureRM.RecoveryServices, AzureRM.RecoveryServices.Backup, and AzureRM.RecoveryServices.SiteRecovery)</span></span>

- <span data-ttu-id="1ae13-273">`Encryption` コマンドレットから、`New/Set-AzRecoveryServicesAsrPolicy` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-273">Removed `Encryption` parameter from `New/Set-AzRecoveryServicesAsrPolicy` cmdlet</span></span>
- <span data-ttu-id="1ae13-274">`TargetStorageAccountName` コマンドレットでのマネージド ディスクの復元に `Restore-AzRecoveryServicesBackupItem` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-274">`TargetStorageAccountName` parameter is now mandatory for managed disk restores in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="1ae13-275">`StorageAccountName` コマンドレットの `StorageAccountResourceGroupName` および `Restore-AzRecoveryServicesBackupItem` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-275">Removed `StorageAccountName` and `StorageAccountResourceGroupName` parameters in `Restore-AzRecoveryServicesBackupItem` cmdlet</span></span>
- <span data-ttu-id="1ae13-276">`Name` コマンドレットの `Get-AzRecoveryServicesBackupContainer` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-276">Removed `Name`parameter in `Get-AzRecoveryServicesBackupContainer` cmdlet</span></span>

### <a name="azresources-previously-azurermresources"></a><span data-ttu-id="1ae13-277">Az.Resources (以前の AzureRM.Resources)</span><span class="sxs-lookup"><span data-stu-id="1ae13-277">Az.Resources (previously AzureRM.Resources)</span></span>

- <span data-ttu-id="1ae13-278">`Sku` コマンドレットから、`New/Set-AzPolicyAssignment` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-278">Removed `Sku` parameter from `New/Set-AzPolicyAssignment` cmdlet</span></span>
- <span data-ttu-id="1ae13-279">`Password` および `New-AzADServicePrincipal` コマンドレットから、`New-AzADSpCredential` パラメーターが削除されました。パスワードは自動的に生成されます。次のようにパスワードを指定しているスクリプトは</span><span class="sxs-lookup"><span data-stu-id="1ae13-279">Removed `Password` parameter from `New-AzADServicePrincipal` and `New-AzADSpCredential` cmdlet Passwords are automatically generated, scripts that provided the password:</span></span>

  ```azurepowershell-interactive
  New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476 -Password $secPassword
  ```

  <span data-ttu-id="1ae13-280">出力からパスワードを取得するように変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1ae13-280">Should be changed to retrieve the password from the output:</span></span>

  ```azurepowershell-interactive
  $credential = New-AzAdSpCredential -ObjectId 1f99cf81-0146-4f4e-beae-2007d0668476
  $secPassword = $credential.Secret
  ```

### <a name="azservicefabric-previously-azurermservicefabric"></a><span data-ttu-id="1ae13-281">Az.ServiceFabric (以前の AzureRM.ServiceFabric)</span><span class="sxs-lookup"><span data-stu-id="1ae13-281">Az.ServiceFabric (previously AzureRM.ServiceFabric)</span></span>

- <span data-ttu-id="1ae13-282">コマンドレットの次の戻り値の型が変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-282">The following cmdlet return types have been changed:</span></span>
  - <span data-ttu-id="1ae13-283">`ServiceTypeHealthPolicies` 型の `ApplicationHealthPolicy` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-283">The property `ServiceTypeHealthPolicies` of type `ApplicationHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="1ae13-284">`ApplicationHealthPolicies` 型の `ClusterUpgradeDeltaHealthPolicy` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-284">The property `ApplicationHealthPolicies` of type `ClusterUpgradeDeltaHealthPolicy` has been removed.</span></span>
  - <span data-ttu-id="1ae13-285">`OverrideUserUpgradePolicy` 型の `ClusterUpgradePolicy` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-285">The property `OverrideUserUpgradePolicy` of type `ClusterUpgradePolicy` has been removed.</span></span>
  - <span data-ttu-id="1ae13-286">これらの変更は、次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="1ae13-286">These changes affect the following cmdlets:</span></span>
    - <span data-ttu-id="1ae13-287">Add-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="1ae13-287">Add-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="1ae13-288">Add-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="1ae13-288">Add-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="1ae13-289">Add-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="1ae13-289">Add-AzServiceFabricNode</span></span>
    - <span data-ttu-id="1ae13-290">Add-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="1ae13-290">Add-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="1ae13-291">Get-AzServiceFabricCluster</span><span class="sxs-lookup"><span data-stu-id="1ae13-291">Get-AzServiceFabricCluster</span></span>
    - <span data-ttu-id="1ae13-292">Remove-AzServiceFabricClientCertificate</span><span class="sxs-lookup"><span data-stu-id="1ae13-292">Remove-AzServiceFabricClientCertificate</span></span>
    - <span data-ttu-id="1ae13-293">Remove-AzServiceFabricClusterCertificate</span><span class="sxs-lookup"><span data-stu-id="1ae13-293">Remove-AzServiceFabricClusterCertificate</span></span>
    - <span data-ttu-id="1ae13-294">Remove-AzServiceFabricNode</span><span class="sxs-lookup"><span data-stu-id="1ae13-294">Remove-AzServiceFabricNode</span></span>
    - <span data-ttu-id="1ae13-295">Remove-AzServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="1ae13-295">Remove-AzServiceFabricNodeType</span></span>
    - <span data-ttu-id="1ae13-296">Remove-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="1ae13-296">Remove-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="1ae13-297">Set-AzServiceFabricSetting</span><span class="sxs-lookup"><span data-stu-id="1ae13-297">Set-AzServiceFabricSetting</span></span>
    - <span data-ttu-id="1ae13-298">Set-AzServiceFabricUpgradeType</span><span class="sxs-lookup"><span data-stu-id="1ae13-298">Set-AzServiceFabricUpgradeType</span></span>
    - <span data-ttu-id="1ae13-299">Update-AzServiceFabricDurability</span><span class="sxs-lookup"><span data-stu-id="1ae13-299">Update-AzServiceFabricDurability</span></span>
    - <span data-ttu-id="1ae13-300">Update-AzServiceFabricReliability</span><span class="sxs-lookup"><span data-stu-id="1ae13-300">Update-AzServiceFabricReliability</span></span>

### <a name="azsql-previously-azurermsql"></a><span data-ttu-id="1ae13-301">Az.Sql (以前の AzureRM.Sql)</span><span class="sxs-lookup"><span data-stu-id="1ae13-301">Az.Sql (previously AzureRM.Sql)</span></span>

- <span data-ttu-id="1ae13-302">`State` コマンドレットから、`ResourceId` および `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-302">Removed `State` and `ResourceId` parameters from `Set-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="1ae13-303">非推奨の `Get/Set-AzSqlServerBackupLongTermRetentionVault`、`Get/Start/Stop-AzSqlServerUpgrade`、`Get/Set-AzSqlDatabaseAuditingPolicy`、`Get/Set-AzSqlServerAuditingPolicy`、`Remove-AzSqlDatabaseAuditing`、`Remove-AzSqlServerAuditing` の各コマンドレットが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-303">Removed deprecated cmdlets: `Get/Set-AzSqlServerBackupLongTermRetentionVault`, `Get/Start/Stop-AzSqlServerUpgrade`, `Get/Set-AzSqlDatabaseAuditingPolicy`, `Get/Set-AzSqlServerAuditingPolicy`, `Remove-AzSqlDatabaseAuditing`, `Remove-AzSqlServerAuditing`</span></span>
- <span data-ttu-id="1ae13-304">`Current` コマンドレットから、非推奨の `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-304">Removed deprecated parameter `Current` from `Get-AzSqlDatabaseBackupLongTermRetentionPolicy` cmdlet</span></span>
- <span data-ttu-id="1ae13-305">`DatabaseName` コマンドレットから、非推奨の `Get-AzSqlServerServiceObjective` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-305">Removed deprecated parameter `DatabaseName` from `Get-AzSqlServerServiceObjective` cmdlet</span></span>
- <span data-ttu-id="1ae13-306">`PrivilegedLogin` コマンドレットから、非推奨の `Set-AzSqlDatabaseDataMaskingPolicy` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-306">Removed deprecated parameter `PrivilegedLogin` from `Set-AzSqlDatabaseDataMaskingPolicy` cmdlet</span></span>

### <a name="azstorage-previously-azurestorage-and-azurermstorage"></a><span data-ttu-id="1ae13-307">Az.Storage (以前の Azure.Storage and AzureRM.Storage)</span><span class="sxs-lookup"><span data-stu-id="1ae13-307">Az.Storage (previously Azure.Storage and AzureRM.Storage)</span></span>

- <span data-ttu-id="1ae13-308">ストレージ アカウント名のみを使用した Oauth ストレージ コンテキストの作成をサポートするために、既定のパラメーター セットが `OAuthParameterSet` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-308">To support creating an Oauth storage context with only the storage account name, the default parameter set has been changed to `OAuthParameterSet`</span></span>
  - <span data-ttu-id="1ae13-309">例: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span><span class="sxs-lookup"><span data-stu-id="1ae13-309">Example: `$ctx = New-AzureStorageContext -StorageAccountName $accountName`</span></span>
- <span data-ttu-id="1ae13-310">`Location` コマンドレットで `Get-AzStorageUsage` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-310">The `Location` parameter has become mandatory in the `Get-AzStorageUsage` cmdlet</span></span>
- <span data-ttu-id="1ae13-311">Storage API のメソッドで、同期 API 呼び出しの代わりに、タスク ベースの非同期パターン (TAP) が使用されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-311">The Storage API methods now use the Task-based Asynchronous Pattern (TAP), instead of synchronous API calls.</span></span> <span data-ttu-id="1ae13-312">次の例は、新しい非同期コマンドを示しています。</span><span class="sxs-lookup"><span data-stu-id="1ae13-312">The following examples demonstrate the new asynchronous commands:</span></span>

#### <a name="blob-snapshot"></a><span data-ttu-id="1ae13-313">BLOB スナップショット</span><span class="sxs-lookup"><span data-stu-id="1ae13-313">Blob Snapshot</span></span>

<span data-ttu-id="1ae13-314">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="1ae13-314">AzureRM:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$b.ICloudBlob.Snapshot()
```

<span data-ttu-id="1ae13-315">Az:</span><span class="sxs-lookup"><span data-stu-id="1ae13-315">Az:</span></span>

```azurepowershell-interactive
$b = Get-AzStorageBlob -Container $containerName -Blob $blobName -Context $ctx
$task = $b.ICloudBlob.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="share-snapshot"></a><span data-ttu-id="1ae13-316">スナップショットの共有</span><span class="sxs-lookup"><span data-stu-id="1ae13-316">Share Snapshot</span></span>

<span data-ttu-id="1ae13-317">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="1ae13-317">AzureRM:</span></span>

```azurepowershell-interactive
$Share = Get-AzureStorageShare -Name $containerName -Context $ctx
$snapshot = $Share.Snapshot()
```

<span data-ttu-id="1ae13-318">Az:</span><span class="sxs-lookup"><span data-stu-id="1ae13-318">Az:</span></span>

```azurepowershell-interactive
$Share = Get-AzStorageShare -Name $containerName -Context $ctx
$task = $Share.SnapshotAsync()
$task.Wait()
$snapshot = $task.Result
```

#### <a name="undelete-soft-deleted-blob"></a><span data-ttu-id="1ae13-319">論理的に削除された BLOB の削除の取り消し</span><span class="sxs-lookup"><span data-stu-id="1ae13-319">Undelete soft-deleted blob</span></span>

<span data-ttu-id="1ae13-320">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="1ae13-320">AzureRM:</span></span>

```azurepowershell-interactive
$b = Get-AzureStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$b.ICloudBlob.Undelete()
```

<span data-ttu-id="1ae13-321">Az:</span><span class="sxs-lookup"><span data-stu-id="1ae13-321">Az:</span></span>

```azurepowershell-interactive
$b = Get-AzStorageBlob -Container $containerName -Blob $blobName -IncludeDeleted -Context $ctx
$task = $b.ICloudBlob.UndeleteAsync()
$task.Wait()
```

#### <a name="set-blob-tier"></a><span data-ttu-id="1ae13-322">BLOB 層の設定</span><span class="sxs-lookup"><span data-stu-id="1ae13-322">Set Blob Tier</span></span>

<span data-ttu-id="1ae13-323">AzureRM:</span><span class="sxs-lookup"><span data-stu-id="1ae13-323">AzureRM:</span></span>

```azurepowershell-interactive
$blockBlob = Get-AzureStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$blockBlob.ICloudBlob.SetStandardBlobTier("hot")

$pageBlob = Get-AzureStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$pageBlob.ICloudBlob.SetPremiumBlobTier("P4")
```

<span data-ttu-id="1ae13-324">Az:</span><span class="sxs-lookup"><span data-stu-id="1ae13-324">Az:</span></span>

```azurepowershell-interactive
$blockBlob = Get-AzStorageBlob -Container $containerName -Blob $blockBlobName -Context $ctx
$task = $blockBlob.ICloudBlob.SetStandardBlobTierAsync("hot")
$task.Wait()

$pageBlob = Get-AzStorageBlob -Container $containerName -Blob $pageBlobName -Context $ctx
$task = $pageBlob.ICloudBlob.SetPremiumBlobTierAsync("P4")
$task.Wait()
```

### <a name="azwebsites-previously-azurermwebsites"></a><span data-ttu-id="1ae13-325">Az.Websites (以前の AzureRM.Websites)</span><span class="sxs-lookup"><span data-stu-id="1ae13-325">Az.Websites (previously AzureRM.Websites)</span></span>

- <span data-ttu-id="1ae13-326">`PSAppServicePlan`、`PSCertificate`、`PSCloningInfo`、`PSSite` の各オブジェクトから非推奨のプロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="1ae13-326">Removed deprecated properties from the `PSAppServicePlan`, `PSCertificate`, `PSCloningInfo`, and `PSSite` objects</span></span>
