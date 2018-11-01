---
title: Microsoft Azure PowerShell 6.0.0 の重大な変更
description: この移行ガイドには、バージョン 6 リリースの Azure PowerShell で行われた重大な変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: 8b7b1422ba2881ca172e65dba61d4c4808cca7de
ms.sourcegitcommit: ff44dec6418a449757bded3c6ebe0a7d4c05ee6e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/01/2018
ms.locfileid: "50737834"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-600"></a><span data-ttu-id="904af-103">Microsoft Azure PowerShell 6.0.0 の重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-103">Breaking changes for Microsoft Azure PowerShell 6.0.0</span></span>

<span data-ttu-id="904af-104">このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。</span><span class="sxs-lookup"><span data-stu-id="904af-104">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="904af-105">各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。</span><span class="sxs-lookup"><span data-stu-id="904af-105">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="904af-106">詳細なコンテキストについては、各変更に関するプル要求を参照してください。</span><span class="sxs-lookup"><span data-stu-id="904af-106">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="904af-107">目次</span><span class="sxs-lookup"><span data-stu-id="904af-107">Table of Contents</span></span>

- [<span data-ttu-id="904af-108">重大な変更 - 全般</span><span class="sxs-lookup"><span data-stu-id="904af-108">General breaking changes</span></span>](#general-breaking-changes)
    - [<span data-ttu-id="904af-109">5.0 に引き上げられた PowerShell の必要最小バージョン</span><span class="sxs-lookup"><span data-stu-id="904af-109">Minimum PowerShell version required bumped to 5.0</span></span>](#minimum-powershell-version-required-bumped-to-50)
    - [<span data-ttu-id="904af-110">既定で有効になっているコンテキスト自動保存</span><span class="sxs-lookup"><span data-stu-id="904af-110">Context autosaved enabled by default</span></span>](#context-autosave-enabled-by-default)
    - [<span data-ttu-id="904af-111">Tags エイリアスの削除</span><span class="sxs-lookup"><span data-stu-id="904af-111">Removal of Tags alias</span></span>](#removal-of-tags-alias)
- [<span data-ttu-id="904af-112">AzureRM.Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-112">Breaking changes to AzureRM.Compute cmdlets</span></span>](#breaking-changes-to-azurermcompute-cmdlets)
- [<span data-ttu-id="904af-113">AzureRM.DataLakeStore コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-113">Breaking changes to AzureRM.DataLakeStore cmdlets</span></span>](#breaking-changes-to-azurermdatalakestore-cmdlets)
- [<span data-ttu-id="904af-114">AzureRM.Dns コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-114">Breaking changes to AzureRM.Dns cmdlets</span></span>](#breaking-changes-to-azurermdns-cmdlets)
- [<span data-ttu-id="904af-115">AzureRM.Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-115">Breaking changes to AzureRM.Insights cmdlets</span></span>](#breaking-changes-to-azurerminsights-cmdlets)
- [<span data-ttu-id="904af-116">AzureRM.KeyVault コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-116">Breaking changes to AzureRM.KeyVault cmdlets</span></span>](#breaking-changes-to-azurermkeyvault-cmdlets)
- [<span data-ttu-id="904af-117">AzureRM.Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-117">Breaking changes to AzureRM.Network cmdlets</span></span>](#breaking-changes-to-azurermnetwork-cmdlets)
- [<span data-ttu-id="904af-118">AzureRM.RedisCache コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-118">Breaking changes to AzureRM.RedisCache cmdlets</span></span>](#breaking-changes-to-azurermrediscache-cmdlets)
- [<span data-ttu-id="904af-119">AzureRM.Resources コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-119">Breaking changes to AzureRM.Resources cmdlets</span></span>](#breaking-changes-to-azurermresources-cmdlets)
- [<span data-ttu-id="904af-120">AzureRM.Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-120">Breaking changes to AzureRM.Storage cmdlets</span></span>](#breaking-changes-to-azurermstorage-cmdlets)
- [<span data-ttu-id="904af-121">削除されたモジュール</span><span class="sxs-lookup"><span data-stu-id="904af-121">Removed modules</span></span>](#removed-modules)
    - [`AzureRM.ServerManagement`](#azurermservermanagement)
    - [`AzureRM.SiteRecovery`](#azurermsiterecovery)

## <a name="general-breaking-changes"></a><span data-ttu-id="904af-122">重大な変更 - 全般</span><span class="sxs-lookup"><span data-stu-id="904af-122">General breaking changes</span></span>

### <a name="minimum-powershell-version-required-bumped-to-50"></a><span data-ttu-id="904af-123">5.0 に引き上げられた PowerShell の必要最小バージョン</span><span class="sxs-lookup"><span data-stu-id="904af-123">Minimum PowerShell version required bumped to 5.0</span></span>

<span data-ttu-id="904af-124">以前は、Azure PowerShell でコマンドレットを実行するには、PowerShell のバージョン 3.0 "_以上_" が必要でした。</span><span class="sxs-lookup"><span data-stu-id="904af-124">Previously, Azure PowerShell required _at least_ version 3.0 of PowerShell to run any cmdlet.</span></span> <span data-ttu-id="904af-125">今後、この要件は PowerShell のバージョン 5.0 に引き上げられます。</span><span class="sxs-lookup"><span data-stu-id="904af-125">Moving forward, this requirement will be raised to version 5.0 of PowerShell.</span></span> <span data-ttu-id="904af-126">PowerShell 5.0 へのアップグレードについては、[こちらの表](https://docs.microsoft.com/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="904af-126">For information on upgrading to PowerShell 5.0, please see [this table](https://docs.microsoft.com/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell).</span></span>

### <a name="context-autosave-enabled-by-default"></a><span data-ttu-id="904af-127">既定で有効になっているコンテキスト自動保存</span><span class="sxs-lookup"><span data-stu-id="904af-127">Context autosave enabled by default</span></span>

<span data-ttu-id="904af-128">コンテキスト自動保存は、新しい PowerShell セッションと別の PowerShell セッション間で使用できる Azure サインイン情報のストレージです。</span><span class="sxs-lookup"><span data-stu-id="904af-128">Context autosave is the storage of Azure sign in information that can be used between new and different PowerShell sessions.</span></span> <span data-ttu-id="904af-129">コンテキスト自動保存の詳細については、[こちらのドキュメント](https://docs.microsoft.com/powershell/azure/context-persistence)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="904af-129">For more information on context autosave, please see [this document](https://docs.microsoft.com/powershell/azure/context-persistence).</span></span>

<span data-ttu-id="904af-130">以前は、既定でコンテキスト自動保存は無効になっていました。つまり、`Enable-AzureRmContextAutosave` コマンドレットを実行してコンテキストの永続化を有効にするまで、ユーザーの Azure 認証情報はセッション間で保存されませんでした。</span><span class="sxs-lookup"><span data-stu-id="904af-130">Previously by default, context autosave was disabled, which meant the user's Azure authentication information was not stored between sessions until they ran the `Enable-AzureRmContextAutosave` cmdlet to turn on context persistence.</span></span> <span data-ttu-id="904af-131">今後は、コンテキスト自動保存が既定で有効になります。つまり、"_コンテキスト自動保存設定を保存していない_" ユーザーも、次回サインインしたときにコンテキストが保存されています。</span><span class="sxs-lookup"><span data-stu-id="904af-131">Moving forward, context autosave will be enabled by default, which means that users _with no saved context autosave settings_ will have their context stored the next time they sign in.</span></span> <span data-ttu-id="904af-132">ユーザーは `Disable-AzureRmContextAutosave` コマンドレットを使用して、この機能を無効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="904af-132">Users can opt out of this functionality by using the `Disable-AzureRmContextAutosave` cmdlet.</span></span>

<span data-ttu-id="904af-133">_注_: これまでコンテキスト自動保存を無効にしていたユーザーまたは有効にしていたユーザーと既存のコンテキストはこの変更の影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="904af-133">_Note_: users that previously disabled context autosave or users with context autosave enabled and existing contexts will not be affected by this change</span></span>

### <a name="removal-of-tags-alias"></a><span data-ttu-id="904af-134">Tags エイリアスの削除</span><span class="sxs-lookup"><span data-stu-id="904af-134">Removal of Tags alias</span></span>

<span data-ttu-id="904af-135">多数のコマンドレットで、`Tag` パラメーターの `Tags` エイリアスが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-135">The alias `Tags` for the `Tag` parameter has been removed across numerous cmdlets.</span></span> <span data-ttu-id="904af-136">この影響を受けるモジュール (および対応するコマンドレット) は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="904af-136">Below is a list of modules (and the corresponding cmdlets) affected by this:</span></span>

#### `AzureRM.ApiManagement`

- `New-AzureRmApiManagement`
- `New-AzureRmApiManagementProperty`
- `Set-AzureRmApiManagementProperty`

#### `AzureRM.Automation`
- `Set-AzureRmAutomationRunbook`

#### `AzureRM.Cdn`
- `New-AzureRmCdnEndpoint`
- `New-AzureRmCdnProfile`

#### `AzureRM.Compute`
- `New-AzureRmVM`
- `Update-AzureRmVM`

#### `AzureRM.DataFactories`
- `New-AzureRmDataFactories`

#### `AzureRM.DataLakeAnalytics`
- `New-AzureRmDataLakeAnalyticsAccount`

#### `AzureRM.DataLakeStore`
- `New-AzureRmDataLakeStoreAccount`
- `Set-AzureRmDataLakeStoreAccount`

#### `AzureRM.MachineLearning`
- `Update-AzureRmMlCommitmentPlan`

#### `AzureRM.Media`
- `Set-AzureRmMediaService`

#### `AzureRM.OperationalInsights`
- `New-AzureRmOperationalInsightsSavedSearch`
- `New-AzureRmOperationalInsightsWorkspace`
- `Set-AzureRmOperationalInsightsSavedSearch`
- `Set-AzureRmOperationalInsightsWorkspace`

## <a name="breaking-changes-to-azurermcompute-cmdlets"></a><span data-ttu-id="904af-137">AzureRM.Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-137">Breaking changes to AzureRM.Compute cmdlets</span></span>

<span data-ttu-id="904af-138">**その他**</span><span class="sxs-lookup"><span data-stu-id="904af-138">**Miscellaneous**</span></span>
- <span data-ttu-id="904af-139">`PSDisk` 型と `PSSnapshot` 型に入れ子になった SKU 名プロパティが、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-139">The sku name property nested in types `PSDisk` and `PSSnapshot` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

```powershell
$disk = Get-AzureRmDisk -ResourceGroupName "MyResourceGroup" -DiskName "MyDiskName"
$disk.Sku.Name       # This will now return Standard_LRS or Premium_LRS

$snapshot = Get-AzureRmSnapshot -ResourceGroupName "MyResourceGroup" -SnapshotName "MySnapshotName"
$snapshot.Sku.Name   # This will now return Standard_LRS or Premium_LRS
```

- <span data-ttu-id="904af-140">`PSVirtualMachine`、`PSVirtualMachineScaleSet`、`PSImage` の各型に入れ子になったストレージ アカウントの種類プロパティが、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-140">The storage account type property nested in types `PSVirtualMachine`, `PSVirtualMachineScaleSet` and `PSImage` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

```powershell
$vm = Get-AzureRmVM -ResourceGroupName "MyResourceGroup" -Name "MyVM"
$vm.StorageProfile.DataDisks[0].ManagedDisk.StorageAccountType   # This will now return Standard_LRS or Premium_LRS
```

<span data-ttu-id="904af-141">**Add-AzureRmImageDataDisk**</span><span class="sxs-lookup"><span data-stu-id="904af-141">**Add-AzureRmImageDataDisk**</span></span>
- <span data-ttu-id="904af-142">`StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-142">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-143">**Add-AzureRmVMDataDisk**</span><span class="sxs-lookup"><span data-stu-id="904af-143">**Add-AzureRmVMDataDisk**</span></span>
- <span data-ttu-id="904af-144">`StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-144">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-145">**Add-AzureRmVmssDataDisk**</span><span class="sxs-lookup"><span data-stu-id="904af-145">**Add-AzureRmVmssDataDisk**</span></span>
- <span data-ttu-id="904af-146">`StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-146">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-147">**New-AzureRmAvailabilitySet**</span><span class="sxs-lookup"><span data-stu-id="904af-147">**New-AzureRmAvailabilitySet**</span></span>
- <span data-ttu-id="904af-148">`Sku` を優先して、`Managed` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-148">The parameter `Managed` was removed in favor of `Sku`</span></span>

```powershell
# Old
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Managed

# New
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Sku "Aligned"
```

<span data-ttu-id="904af-149">**New-AzureRmDiskConfig**</span><span class="sxs-lookup"><span data-stu-id="904af-149">**New-AzureRmDiskConfig**</span></span>
- <span data-ttu-id="904af-150">`SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-150">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-151">**New-AzureRmDiskUpdateConfig**</span><span class="sxs-lookup"><span data-stu-id="904af-151">**New-AzureRmDiskUpdateConfig**</span></span>
- <span data-ttu-id="904af-152">`SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-152">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-153">**New-AzureRmSnapshotConfig**</span><span class="sxs-lookup"><span data-stu-id="904af-153">**New-AzureRmSnapshotConfig**</span></span>
- <span data-ttu-id="904af-154">`SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-154">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-155">**New-AzureRmSnapshotUpdateConfig**</span><span class="sxs-lookup"><span data-stu-id="904af-155">**New-AzureRmSnapshotUpdateConfig**</span></span>
- <span data-ttu-id="904af-156">`SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-156">The accepted values for parameter `SkuName` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-157">**Set-AzureRmImageOsDisk**</span><span class="sxs-lookup"><span data-stu-id="904af-157">**Set-AzureRmImageOsDisk**</span></span>
- <span data-ttu-id="904af-158">`StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-158">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-159">**Set-AzureRmVMAEMExtension**</span><span class="sxs-lookup"><span data-stu-id="904af-159">**Set-AzureRmVMAEMExtension**</span></span>
- <span data-ttu-id="904af-160">`DisableWAD` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-160">The parameter `DisableWAD` was removed</span></span>
    -  <span data-ttu-id="904af-161">Windows Azure 診断が既定で無効になっています。</span><span class="sxs-lookup"><span data-stu-id="904af-161">Windows Azure Diagnostics is disabled by default</span></span>

<span data-ttu-id="904af-162">**Set-AzureRmVMDataDisk**</span><span class="sxs-lookup"><span data-stu-id="904af-162">**Set-AzureRmVMDataDisk**</span></span>
- <span data-ttu-id="904af-163">`StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-163">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-164">**Set-AzureRmVMOSDisk**</span><span class="sxs-lookup"><span data-stu-id="904af-164">**Set-AzureRmVMOSDisk**</span></span>
- <span data-ttu-id="904af-165">`StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-165">The accepted values for parameter `StorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-166">**Set-AzureRmVmssStorageProfile**</span><span class="sxs-lookup"><span data-stu-id="904af-166">**Set-AzureRmVmssStorageProfile**</span></span>
- <span data-ttu-id="904af-167">`ManagedDisk` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-167">The accepted values for parameter `ManagedDisk` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

<span data-ttu-id="904af-168">**Update-AzureRmVmss**</span><span class="sxs-lookup"><span data-stu-id="904af-168">**Update-AzureRmVmss**</span></span>
- <span data-ttu-id="904af-169">`ManagedDiskStorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-169">The accepted values for parameter `ManagedDiskStorageAccountType` changed from `StandardLRS` and `PremiumLRS` to `Standard_LRS` and `Premium_LRS`, respectively</span></span>

## <a name="breaking-changes-to-azurermdatalakestore-cmdlets"></a><span data-ttu-id="904af-170">AzureRM.DataLakeStore コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-170">Breaking changes to AzureRM.DataLakeStore cmdlets</span></span>

<span data-ttu-id="904af-171">**Export-AzureRmDataLakeStoreItem**</span><span class="sxs-lookup"><span data-stu-id="904af-171">**Export-AzureRmDataLakeStoreItem**</span></span>
- <span data-ttu-id="904af-172">`PerFileThreadCount` パラメーターと `ConcurrentFileCount` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-172">Parameters `PerFileThreadCount` and `ConcurrentFileCount` were removed.</span></span> <span data-ttu-id="904af-173">今後は `Concurrency` パラメーターを使用してください。</span><span class="sxs-lookup"><span data-stu-id="904af-173">Please use the `Concurrency` parameter moving forward</span></span>

```powershell
# Old
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -Concurrency 160
```

<span data-ttu-id="904af-174">**Import-AzureRmDataLakeStoreItem**</span><span class="sxs-lookup"><span data-stu-id="904af-174">**Import-AzureRmDataLakeStoreItem**</span></span>
- <span data-ttu-id="904af-175">`PerFileThreadCount` パラメーターと `ConcurrentFileCount` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-175">Parameters `PerFileThreadCount` and `ConcurrentFileCount` were removed.</span></span> <span data-ttu-id="904af-176">今後は `Concurrency` パラメーターを使用してください。</span><span class="sxs-lookup"><span data-stu-id="904af-176">Please use the `Concurrency` parameter moving forward</span></span>

```powershell
# Old
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -Concurrency 160
```

<span data-ttu-id="904af-177">**Remove-AzureRmDataLakeStoreItem**</span><span class="sxs-lookup"><span data-stu-id="904af-177">**Remove-AzureRmDataLakeStoreItem**</span></span>
- <span data-ttu-id="904af-178">`Clean` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-178">Parameter `Clean` was removed</span></span>

```powershell
# Old
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse -Clean

# New
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse
```

## <a name="breaking-changes-to-azurermdns-cmdlets"></a><span data-ttu-id="904af-179">AzureRM.Dns コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-179">Breaking changes to AzureRM.Dns cmdlets</span></span>

<span data-ttu-id="904af-180">**New-AzureRmDnsRecordSet**</span><span class="sxs-lookup"><span data-stu-id="904af-180">**New-AzureRmDnsRecordSet**</span></span>
- <span data-ttu-id="904af-181">`Force` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-181">The parameter `Force` was removed</span></span>

<span data-ttu-id="904af-182">**Remove-AzureRmDnsRecordSet**</span><span class="sxs-lookup"><span data-stu-id="904af-182">**Remove-AzureRmDnsRecordSet**</span></span>
- <span data-ttu-id="904af-183">`Force` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-183">The parameter `Force` was removed</span></span>

<span data-ttu-id="904af-184">**Remove-AzureRmDnsZone**</span><span class="sxs-lookup"><span data-stu-id="904af-184">**Remove-AzureRmDnsZone**</span></span>
- <span data-ttu-id="904af-185">`Force` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-185">The parameter `Force` was removed</span></span>

## <a name="breaking-changes-to-azurerminsights-cmdlets"></a><span data-ttu-id="904af-186">AzureRM.Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-186">Breaking changes to AzureRM.Insights cmdlets</span></span>

<span data-ttu-id="904af-187">**Add-AzureRmAutoscaleSetting**</span><span class="sxs-lookup"><span data-stu-id="904af-187">**Add-AzureRmAutoscaleSetting**</span></span>
- <span data-ttu-id="904af-188">パラメーター エイリアス `AutoscaleProfiles` と `Notifications` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-188">The parameter aliases `AutoscaleProfiles` and `Notifications` were removed</span></span>

<span data-ttu-id="904af-189">**Add-AzureRmLogProfile**</span><span class="sxs-lookup"><span data-stu-id="904af-189">**Add-AzureRmLogProfile**</span></span>
- <span data-ttu-id="904af-190">パラメーター エイリアス `Categories` と `Locations` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-190">The parameter aliases `Categories` and `Locations` were removed</span></span>

<span data-ttu-id="904af-191">**Add-AzureRmMetricAlertRule**</span><span class="sxs-lookup"><span data-stu-id="904af-191">**Add-AzureRmMetricAlertRule**</span></span>
- <span data-ttu-id="904af-192">パラメーター エイリアス `Actions` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-192">The parameter alias `Actions` was removed</span></span>

<span data-ttu-id="904af-193">**Add-AzureRmWebtestAlertRule**</span><span class="sxs-lookup"><span data-stu-id="904af-193">**Add-AzureRmWebtestAlertRule**</span></span>
- <span data-ttu-id="904af-194">パラメーター エイリアス `Actions` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-194">The parameter alias `Actions` was removed</span></span>

<span data-ttu-id="904af-195">**Get-AzureRmLog**</span><span class="sxs-lookup"><span data-stu-id="904af-195">**Get-AzureRmLog**</span></span>
- <span data-ttu-id="904af-196">パラメーター エイリアス `MaxRecords` と `MaxEvents` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-196">The parameter aliases `MaxRecords` and `MaxEvents` were removed</span></span>

<span data-ttu-id="904af-197">**Get-AzureRmMetricDefinition**</span><span class="sxs-lookup"><span data-stu-id="904af-197">**Get-AzureRmMetricDefinition**</span></span>
- <span data-ttu-id="904af-198">パラメーター エイリアス `MetricNames` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-198">The parameter alias `MetricNames` was removed</span></span>

<span data-ttu-id="904af-199">**New-AzureRmAlertRuleEmail**</span><span class="sxs-lookup"><span data-stu-id="904af-199">**New-AzureRmAlertRuleEmail**</span></span>
- <span data-ttu-id="904af-200">パラメーター エイリアス `CustomEmails` と `SendToServiceOwners` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-200">The parameter aliases `CustomEmails` and `SendToServiceOwners` were removed</span></span>

<span data-ttu-id="904af-201">**New-AzureRmAlertRuleWebhook**</span><span class="sxs-lookup"><span data-stu-id="904af-201">**New-AzureRmAlertRuleWebhook**</span></span>
- <span data-ttu-id="904af-202">パラメーター エイリアス `Properties` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-202">The parameter alias `Properties` was removed</span></span>

<span data-ttu-id="904af-203">**New-AzureRmAutoscaleNotification**</span><span class="sxs-lookup"><span data-stu-id="904af-203">**New-AzureRmAutoscaleNotification**</span></span>
- <span data-ttu-id="904af-204">パラメーター エイリアス `CustomEmails`、`SendEmailToSubscriptionCoAdministrators`、`Webhooks` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-204">The parameter aliases `CustomEmails`, `SendEmailToSubscriptionCoAdministrators` and `Webhooks` were removed</span></span>

<span data-ttu-id="904af-205">**New-AzureRmAutoscaleProfile**</span><span class="sxs-lookup"><span data-stu-id="904af-205">**New-AzureRmAutoscaleProfile**</span></span>
- <span data-ttu-id="904af-206">パラメーター エイリアス `Rules`、`ScheduleDays`、`ScheduleHours`、`ScheduleMinutes` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-206">The parameter aliases `Rules`, `ScheduleDays`, `ScheduleHours` and `ScheduleMinutes` were removed</span></span>

<span data-ttu-id="904af-207">**New-AzureRmAutoscaleWebhook**</span><span class="sxs-lookup"><span data-stu-id="904af-207">**New-AzureRmAutoscaleWebhook**</span></span>
- <span data-ttu-id="904af-208">パラメーター エイリアス `Properties` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-208">The parameter alias `Properties` was removed</span></span>

## <a name="breaking-changes-to-azurermkeyvault-cmdlets"></a><span data-ttu-id="904af-209">AzureRM.KeyVault コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-209">Breaking changes to AzureRM.KeyVault cmdlets</span></span>

<span data-ttu-id="904af-210">**Add-AzureKeyVaultCertificate**</span><span class="sxs-lookup"><span data-stu-id="904af-210">**Add-AzureKeyVaultCertificate**</span></span>
- <span data-ttu-id="904af-211">`CertificatePolicy` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="904af-211">The `CertificatePolicy` parameter has become mandatory.</span></span>

<span data-ttu-id="904af-212">**Set-AzureKeyVaultManagedStorageSasDefinition**</span><span class="sxs-lookup"><span data-stu-id="904af-212">**Set-AzureKeyVaultManagedStorageSasDefinition**</span></span>
- <span data-ttu-id="904af-213">このコマンドレットは、アクセス トークンを構成する個々のパラメーターを受け入れなくなりました。代わりに、`Service` や `Permissions` などの明示的なトークン パラメーターが、他の場所で定義されたサンプル アクセス トークン (Storage PowerShell コマンドレットを使用するか、Storage ドキュメントに従って手動で構成) に対応する汎用の `TemplateUri` パラメーターに置き換えられます。`ValidityPeriod` パラメーターは保持されます。</span><span class="sxs-lookup"><span data-stu-id="904af-213">The cmdlet no longer accepts individual parameters that compose the access token; instead, the cmdlet replaces explicit token parameters, such as `Service` or `Permissions`, with a generic `TemplateUri` parameter, corresponding to a sample access token defined elsewhere (presumably using Storage PowerShell cmdlets, or composed manually according to the Storage documentation.) The cmdlet retains the `ValidityPeriod` parameter.</span></span>

<span data-ttu-id="904af-214">Azure Storage の共有アクセス トークンの構成の詳細については、それぞれのドキュメント ページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="904af-214">For more information on composing shared access tokens for Azure Storage, please refer to the documentation pages, respectively:</span></span>
- <span data-ttu-id="904af-215">[サービス SAS の作成] (https://docs.microsoft.com/rest/api/storageservices/Constructing-a-Service-SAS)</span><span class="sxs-lookup"><span data-stu-id="904af-215">[Constructing a Service SAS] (https://docs.microsoft.com/rest/api/storageservices/Constructing-a-Service-SAS)</span></span>
- <span data-ttu-id="904af-216">[アカウント SAS の作成] (https://docs.microsoft.com/rest/api/storageservices/constructing-an-account-sas)</span><span class="sxs-lookup"><span data-stu-id="904af-216">[Constructing an Account SAS] (https://docs.microsoft.com/rest/api/storageservices/constructing-an-account-sas)</span></span>

```powershell
# Old
$sas = Set-AzureKeyVaultManagedStorageSasDefinition -VaultName myVault -Name myKey -Service Blob -Permissions 'rcw' -ValidityPeriod 180d

# New
$sctx=New-AzureStorageContext -StorageAccountName $sa.StorageAccountName -Protocol Https -StorageAccountKey Key1
$start=[System.DateTime]::Now.AddDays(-1)
$end=[System.DateTime]::Now.AddMonths(1)
$at=New-AzureStorageAccountSasToken -Service blob -ResourceType Service,Container,Object -Permission "racwdlup" -Protocol HttpsOnly -StartTime $start -ExpiryTime $end -Context $sctx
$sas=Set-AzureKeyVaultManagedStorageSasDefinition -AccountName $sa.StorageAccountName -VaultName $kv.VaultName -Name accountsas -TemplateUri $at -SasType 'account' -ValidityPeriod ([System.Timespan]::FromDays(30))
```

<span data-ttu-id="904af-217">**Set-AzureKeyVaultCertificateIssuer**</span><span class="sxs-lookup"><span data-stu-id="904af-217">**Set-AzureKeyVaultCertificateIssuer**</span></span>
- <span data-ttu-id="904af-218">`IssuerProvider` パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="904af-218">The `IssuerProvider` parameter has become mandatory.</span></span>

<span data-ttu-id="904af-219">**Undo-AzureKeyVaultCertificateRemoval**</span><span class="sxs-lookup"><span data-stu-id="904af-219">**Undo-AzureKeyVaultCertificateRemoval**</span></span>
- <span data-ttu-id="904af-220">このコマンドレットの出力が、`CertificateBundle` から `PSKeyVaultCertificate` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="904af-220">The output of this cmdlet has changed from `CertificateBundle` to `PSKeyVaultCertificate`.</span></span>

<span data-ttu-id="904af-221">**Undo-AzureRmKeyVaultRemoval**</span><span class="sxs-lookup"><span data-stu-id="904af-221">**Undo-AzureRmKeyVaultRemoval**</span></span>
- <span data-ttu-id="904af-222">`ResourceGroupName` が `InputObject` パラメーター セットから削除されました。代わりに、`InputObject` パラメーターの `ResourceId` プロパティから取得されます。</span><span class="sxs-lookup"><span data-stu-id="904af-222">`ResourceGroupName` has been removed from the `InputObject` parameter set, and is instead obtained from the `InputObject` parameter's `ResourceId` property.</span></span>

<span data-ttu-id="904af-223">**Set-AzureRmKeyVaultAccessPolicy**</span><span class="sxs-lookup"><span data-stu-id="904af-223">**Set-AzureRmKeyVaultAccessPolicy**</span></span>
- <span data-ttu-id="904af-224">`PermissionsToKeys`、`PermissionsToSecrets`、`PermissionsToCertificates` から、`all` アクセス許可が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-224">The `all` permission was removed from `PermissionsToKeys`, `PermissionsToSecrets`, and `PermissionsToCertificates`.</span></span>

<span data-ttu-id="904af-225">**全般**</span><span class="sxs-lookup"><span data-stu-id="904af-225">**General**</span></span>
- <span data-ttu-id="904af-226">`InputObject` によるパイプ処理が有効になっているすべてのコマンドレットから、`ValueFromPipelineByPropertyName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-226">The `ValueFromPipelineByPropertyName` property was removed from all cmdlets where piping by `InputObject` was enabled.</span></span>  <span data-ttu-id="904af-227">影響を受けるコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="904af-227">The cmdlets affected are:</span></span>
    - `Add-AzureKeyVaultCertificate`
    - `Add-AzureKeyVaultCertificateContact`
    - `Add-AzureKeyVaultKey`
    - `Backup-AzureKeyVaultKey`
    - `Backup-AzureKeyVaultSecret`
    - `Get-AzureKeyVaultCertficate`
    - `Get-AzureKeyVaultCertificateContact`
    - `Get-AzureKeyVaultCertificateIssuer`
    - `Get-AzureKeyVaultCertificateOperation`
    - `Get-AzureKeyVaultCertificatePolicy`
    - `Get-AzureKeyVaultKey`
    - `Get-AzureKeyVaultManagedStorageAccount`
    - `Get-AzureKeyVaultManagedStorageSasDefinition`
    - `Get-AzureKeyVaultSecret`
    - `Remove-AzureRmKeyVault`
    - `Remove-AzureRmKeyVaultAccessPolicy`
    - `Remove-AzureKeyVaultCertificate`
    - `Remove-AzureKeyVaultCertificateContact`
    - `Remove-AzureKeyVaultCertificateIssuer`
    - `Remove-AzureKeyVaultCertificateOperation`
    - `Remove-AzureKeyVaultKey`
    - `Remove-AzureKeyVaultManagedStorageAccount`
    - `Remove-AzureKeyVaultManagedStorageSasDefinition`
    - `Remove-AzureKeyVaultSecret`
    - `Restore-AzureKeyVaultKey`
    - `Restore-AzureKeyVaultSecret`
    - `Set-AzureRmKeyVaultAccessPolicy`
    - `Set-AzureKeyVaultCertificateAttribute`
    - `Set-AzureKeyVaultCertificateIssuer`
    - `Set-AzureKeyVaultCertificatePolicy`
    - `Set-AzureKeyVaultKeyAttribute`
    - `Set-AzureKeyVaultManagedStorageSasDefinition`
    - `Set-AzureKeyVaultSecret`
    - `Set-AzureKeyVaultSecretAttribute`
    - `Stop-AzureKeyVaultCertificateOperation`
    - `Undo-AzureKeyVaultCertificateRemoval`
    - `Undo-AzureKeyVaultKeyRemoval`
    - `Undo-AzureRmKeyVaultRemoval`
    - `Undo-AzureKeyVaultSecretRemoval`
    - `Update-AzureKeyVaultManagedStorageAccount`
    - `Update-AzureKeyVaultManagedStorageAccountKey`

- <span data-ttu-id="904af-228">すべてのコマンドレットから `ConfirmImpact` レベルが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-228">`ConfirmImpact` levels were removed from all cmdlets.</span></span>  <span data-ttu-id="904af-229">影響を受けるコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="904af-229">The cmdlets affected are:</span></span>
    - `Remove-AzureRmKeyVault`
    - `Remove-AzureKeyVaultCertificate`
    - `Remove-AzureKeyVaultCertificateIssuer`
    - `Remove-AzureKeyVaultCertificateOperation`
    - `Remove-AzureKeyVaultKey`
    - `Remove-AzureKeyVaultManagedStorageAccount`
    - `Remove-AzureKeyVaultManagedStorageSasDefinition`
    - `Remove-AzureKeyVaultSecret`
    - `Stop-AzureKeyVaultCertificateOperation`
    - `Update-AzureKeyVaultManagedStorageAccountKey`

- <span data-ttu-id="904af-230">`IKeyVaultDataServiceClient` が更新されました。これにより、すべての証明書操作で、SDK の種類ではなく PSTypes が返されます。</span><span class="sxs-lookup"><span data-stu-id="904af-230">The `IKeyVaultDataServiceClient` was updated so all Certificate operations return PSTypes instead of SDK types.</span></span> <span data-ttu-id="904af-231">次のトピックがあります。</span><span class="sxs-lookup"><span data-stu-id="904af-231">This includes:</span></span>
    - `SetCertificateContacts`
    - `GetCertificateContacts`
    - `GetCertificate`
    - `GetDeletedCertificate`
    - `MergeCertificate`
    - `ImportCertificate`
    - `DeleteCertificate`
    - `RecoverCertificate`
    - `EnrollCertificate`
    - `UpdateCertificate`
    - `GetCertificateOperation`
    - `DeleteCertificateOperation`
    - `CancelCertificateOperation`
    - `GetCertificatePolicy`
    - `UpdateCertificatePolicy`
    - `GetCertificateIssuer`
    - `SetCertificateIssuer`
    - `DeleteCertificateIssuer`

## <a name="breaking-changes-to-azurermnetwork-cmdlets"></a><span data-ttu-id="904af-232">AzureRM.Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-232">Breaking changes to AzureRM.Network cmdlets</span></span>


<span data-ttu-id="904af-233">**Add-AzureRmApplicationGatewayBackendHttpSettings**</span><span class="sxs-lookup"><span data-stu-id="904af-233">**Add-AzureRmApplicationGatewayBackendHttpSettings**</span></span>
- <span data-ttu-id="904af-234">`ProbeEnabled` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-234">The parameter `ProbeEnabled` was removed</span></span>

<span data-ttu-id="904af-235">**Add-AzureRmVirtualNetworkPeering**</span><span class="sxs-lookup"><span data-stu-id="904af-235">**Add-AzureRmVirtualNetworkPeering**</span></span>
- <span data-ttu-id="904af-236">パラメーター エイリアス `AlloowGatewayTransit` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-236">The parameter alias `AlloowGatewayTransit` was removed</span></span>

<span data-ttu-id="904af-237">**New-AzureRmApplicationGatewayBackendHttpSettings**</span><span class="sxs-lookup"><span data-stu-id="904af-237">**New-AzureRmApplicationGatewayBackendHttpSettings**</span></span>
- <span data-ttu-id="904af-238">`ProbeEnabled` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-238">The parameter `ProbeEnabled` was removed</span></span>

<span data-ttu-id="904af-239">**Set-AzureRmApplicationGatewayBackendHttpSettings**</span><span class="sxs-lookup"><span data-stu-id="904af-239">**Set-AzureRmApplicationGatewayBackendHttpSettings**</span></span>
- <span data-ttu-id="904af-240">`ProbeEnabled` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-240">The parameter `ProbeEnabled` was removed</span></span>

## <a name="breaking-changes-to-azurermrediscache-cmdlets"></a><span data-ttu-id="904af-241">AzureRM.RedisCache コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-241">Breaking changes to AzureRM.RedisCache cmdlets</span></span>

<span data-ttu-id="904af-242">**New-AzureRmRedisCache**</span><span class="sxs-lookup"><span data-stu-id="904af-242">**New-AzureRmRedisCache**</span></span>
- <span data-ttu-id="904af-243">`SubnetId` を優先して、`Subnet` パラメーターと `VirtualNetwork` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-243">The parameters `Subnet` and `VirtualNetwork` were removed in favor of `SubnetId`</span></span>
- <span data-ttu-id="904af-244">`RedisVersion` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-244">The parameter `RedisVersion` was removed</span></span>
- <span data-ttu-id="904af-245">`RedisConfiguration` を優先して、`MaxMemoryPolicy` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-245">The parameter `MaxMemoryPolicy` was removed in favor of `RedisConfiguration`</span></span>

```powershell
# Old
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -MaxMemoryPolicy "allkeys-lru"

# New
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

<span data-ttu-id="904af-246">**Set-AzureRmRedisCache**</span><span class="sxs-lookup"><span data-stu-id="904af-246">**Set-AzureRmRedisCache**</span></span>
- <span data-ttu-id="904af-247">`RedisConfiguration` を優先して、`MaxMemoryPolicy` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-247">The parameter `MaxMemoryPolicy` was removed in favor of `RedisConfiguration`</span></span>

```powershell
# Old
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -MaxMemoryPolicy "allkeys-lru"

# New
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

## <a name="breaking-changes-to-azurermresources-cmdlets"></a><span data-ttu-id="904af-248">AzureRM.Resources コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-248">Breaking changes to AzureRM.Resources cmdlets</span></span>

<span data-ttu-id="904af-249">**Find-AzureRmResource**</span><span class="sxs-lookup"><span data-stu-id="904af-249">**Find-AzureRmResource**</span></span>
- <span data-ttu-id="904af-250">このコマンドレットは削除され、機能が `Get-AzureRmResource` に移動されました。</span><span class="sxs-lookup"><span data-stu-id="904af-250">This cmdlet was removed and the functionality was moved into `Get-AzureRmResource`</span></span>

```powershell
# Old
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupNameContains "ResourceGroup"
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceNameContains "test"

# New
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupName "*ResourceGroup*"
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -Name "*test*"
```

<span data-ttu-id="904af-251">**Find-AzureRmResourceGroup**</span><span class="sxs-lookup"><span data-stu-id="904af-251">**Find-AzureRmResourceGroup**</span></span>
- <span data-ttu-id="904af-252">このコマンドレットは削除され、機能が `Get-AzureRmResourceGroup` に移動されました。</span><span class="sxs-lookup"><span data-stu-id="904af-252">This cmdlet was removed and the functionality was moved into `Get-AzureRmResourceGroup`</span></span>

```powershell
# Old
Find-AzureRmResourceGroup
Find-AzureRmResourceGroup -Tag @{ "testtag" = $null }
Find-AzureRmResourceGroup -Tag @{ "testtag" = "testval" }

# New
Get-AzureRmResourceGroup
Get-AzureRmResourceGroup -Tag @{ "testtag" = $null }
Get-AzureRmResourceGroup -Tag @{ "testtag" = "testval" }
```

<span data-ttu-id="904af-253">**Get-AzureRmRoleDefinition**</span><span class="sxs-lookup"><span data-stu-id="904af-253">**Get-AzureRmRoleDefinition**</span></span>
- <span data-ttu-id="904af-254">`AtScopeAndBelow` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-254">Parameter `AtScopeAndBelow` was removed.</span></span>

```powershell

# Old
Get-AzureRmRoleDefinition [other required parameters] -AtScopeAndBelow

# New
Get-AzureRmRoleDefinition [other required parameters]
```

## <a name="breaking-changes-to-azurermstorage-cmdlets"></a><span data-ttu-id="904af-255">AzureRM.Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="904af-255">Breaking changes to AzureRM.Storage cmdlets</span></span>

<span data-ttu-id="904af-256">**New-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="904af-256">**New-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="904af-257">`EnableEncryptionService` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-257">The parameter `EnableEncryptionService` was removed</span></span>

<span data-ttu-id="904af-258">**Set-AzureRmStorageAccount**</span><span class="sxs-lookup"><span data-stu-id="904af-258">**Set-AzureRmStorageAccount**</span></span>
- <span data-ttu-id="904af-259">`EnableEncryptionService` パラメーターと `DisableEncryptionService` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="904af-259">The parameters `EnableEncryptionService` and `DisableEncryptionService` were removed</span></span>

## <a name="removed-modules"></a><span data-ttu-id="904af-260">削除されたモジュール</span><span class="sxs-lookup"><span data-stu-id="904af-260">Removed modules</span></span>

### `AzureRM.ServerManagement`

<span data-ttu-id="904af-261">Server Management Tools サービスが[昨年廃止](https://blogs.technet.microsoft.com/servermanagement/2017/05/17/smt-preview-service-is-being-retired-on-june-30-2017/)されました。これにより、SMT の対応するモジュール `AzureRM.ServerManagement` が `AzureRM` から削除され、今後は出荷されなくなります。</span><span class="sxs-lookup"><span data-stu-id="904af-261">The Server Management Tools service was [retired last year](https://blogs.technet.microsoft.com/servermanagement/2017/05/17/smt-preview-service-is-being-retired-on-june-30-2017/), and as a result, the corresponding module for SMT, `AzureRM.ServerManagement`, was removed from `AzureRM` and will stop shipping moving forward.</span></span>

### `AzureRM.SiteRecovery`

<span data-ttu-id="904af-262">`AzureRM.SiteRecovery` モジュールは `AzureRM.RecoveryServices.SiteRecovery` に置き換えられます。これは、`AzureRM.SiteRecovery` モジュールの機能的なスーパーセットであり、一連の新しい同等のコマンドレットが含まれます。</span><span class="sxs-lookup"><span data-stu-id="904af-262">The `AzureRM.SiteRecovery` module is being superseded by `AzureRM.RecoveryServices.SiteRecovery`, which is a functional superset of the `AzureRM.SiteRecovery` module and includes a new set of equivalent cmdlets.</span></span> <span data-ttu-id="904af-263">古いコマンドレットから新しいコマンドレットへのマッピングの一覧を次に示します。</span><span class="sxs-lookup"><span data-stu-id="904af-263">The full list of mappings from old to new cmdlets can be found below:</span></span>

| <span data-ttu-id="904af-264">非推奨のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="904af-264">Deprecated cmdlet</span></span>                                        | <span data-ttu-id="904af-265">同等のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="904af-265">Equivalent cmdlet</span></span>                                                | <span data-ttu-id="904af-266">エイリアス</span><span class="sxs-lookup"><span data-stu-id="904af-266">Aliases</span></span>                                  |
|----------------------------------------------------------|------------------------------------------------------------------|------------------------------------------|
| `Edit-AzureRmSiteRecoveryRecoveryPlan`                   | `Edit-AzureRmRecoveryServicesAsrRecoveryPlan`                    | `Edit-ASRRecoveryPlan`                   |
| `Get-AzureRmSiteRecoveryFabric`                          | `Get-AzureRmRecoveryServicesAsrFabric`                           | `Get-ASRFabric`                          |
| `Get-AzureRmSiteRecoveryJob`                             | `Get-AzureRmRecoveryServicesAsrJob`                              | `Get-ASRJob`                             |
| `Get-AzureRmSiteRecoveryNetwork`                         | `Get-AzureRmRecoveryServicesAsrNetwork`                          | `Get-ASRNetwork`                         |
| `Get-AzureRmSiteRecoveryNetworkMapping`                  | `Get-AzureRmRecoveryServicesAsrNetworkMapping`                   | `Get-ASRNetworkMapping`                  |
| `Get-AzureRmSiteRecoveryPolicy`                          | `Get-AzureRmRecoveryServicesAsrPolicy`                           | `Get-ASRPolicy`                          |
| `Get-AzureRmSiteRecoveryProtectableItem`                 | `Get-AzureRmRecoveryServicesAsrProtectableItem`                  | `Get-ASRProtectableItem`                 |
| `Get-AzureRmSiteRecoveryProtectionContainer`             | `Get-AzureRmRecoveryServicesAsrProtectionContainer`              | `Get-ASRProtectionContainer`             |
| `Get-AzureRmSiteRecoveryProtectionContainerMapping`      | `Get-AzureRmRecoveryServicesAsrProtectionContainerMapping`       | `Get-ASRProtectionContainerMapping`      |
| `Get-AzureRmSiteRecoveryProtectionEntity`                | `Get-AzureRmRecoveryServicesAsrProtectableItem`                  | `Get-ASRProtectableItem`                 |
| `Get-AzureRmSiteRecoveryRecoveryPlan`                    | `Get-AzureRmRecoveryServicesAsrRecoveryPlan`                     | `Get-ASRRecoveryPlan`                    |
| `Get-AzureRmSiteRecoveryRecoveryPoint`                   | `Get-AzureRmRecoveryServicesAsrRecoveryPoint`                    | `Get-ASRRecoveryPoint`                   |
| `Get-AzureRmSiteRecoveryReplicationProtectedItem`        | `Get-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Get-ASRReplicationProtectedItem`        |
| `Get-AzureRmSiteRecoveryServer`                          | `Get-AzureRmRecoveryServicesAsrServicesProvider`                 | `Get-ASRServicesProvider`                |
| `Get-AzureRmSiteRecoveryServicesProvider`                | `Get-AzureRmRecoveryServicesAsrServicesProvider`                 | `Get-ASRServicesProvider`                |
| `Get-AzureRmSiteRecoverySite`                            | `Get-AzureRmRecoveryServicesAsrFabric`                           | `Get-ASRFabric`                          |
| `Get-AzureRmSiteRecoveryStorageClassification`           | `Get-AzureRmRecoveryServicesAsrStorageClassification`            | `Get-ASRStorageClassification`           |
| `Get-AzureRmSiteRecoveryStorageClassificationMapping`    | `Get-AzureRmRecoveryServicesAsrStorageClassificationMapping`     | `Get-ASRStorageClassificationMapping`    |
| `Get-AzureRmSiteRecoveryVault`                           | `Get-AzureRmRecoveryServicesVault`                               |                                          |
| `Get-AzureRmSiteRecoveryVaultSettings`                   | `Get-AzureRmRecoveryServicesAsrVaultContext`                     |                                          |
| `Get-AzureRmSiteRecoveryVaultSettingsFile`               | `Get-AzureRmRecoveryServicesVaultSettingsFile`                   |                                          |
| `Get-AzureRmSiteRecoveryVM`                              | `Get-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Get-ASRReplicationProtectedItem`        |
| `Import-AzureRmSiteRecoveryVaultSettingsFile`            | `Import-AzureRmRecoveryServicesAsrVaultSettingsFile`             |                                          |
| `New-AzureRmSiteRecoveryFabric`                          | `New-AzureRmRecoveryServicesAsrFabric`                           | `New-ASRFabric`                          |
| `New-AzureRmSiteRecoveryNetworkMapping`                  | `New-AzureRmRecoveryServicesAsrNetworkMapping`                   | `New-ASRNetworkMapping`                  |
| `New-AzureRmSiteRecoveryPolicy`                          | `New-AzureRmRecoveryServicesAsrPolicy`                           | `New-ASRPolicy`                          |
| `New-AzureRmSiteRecoveryProtectionContainerMapping`      | `New-AzureRmRecoveryServicesAsrProtectionContainerMapping`       | `New-ASRProtectionContainerMapping`      |
| `New-AzureRmSiteRecoveryRecoveryPlan`                    | `New-AzureRmRecoveryServicesAsrRecoveryPlan`                     | `New-ASRRecoveryPlan`                    |
| `New-AzureRmSiteRecoveryReplicationProtectedItem`        | `New-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `New-ASRReplicationProtectedItem`        |
| `New-AzureRmSiteRecoverySite`                            | `New-AzureRmRecoveryServicesAsrFabric`                           | `New-ASRFabric`                          |
| `New-AzureRmSiteRecoveryStorageClassificationMapping`    | `New-AzureRmRecoveryServicesAsrStorageClassificationMapping`     | `New-ASRStorageClassificationMapping`    |
| `New-AzureRmSiteRecoveryVault`                           | `New-AzureRmRecoveryServicesVault`                               |                                          |
| `Remove-AzureRmSiteRecoveryFabric`                       | `Remove-AzureRmRecoveryServicesAsrFabric`                        | `Remove-ASRFabric`                       |
| `Remove-AzureRmSiteRecoveryNetworkMapping`               | `Remove-AzureRmRecoveryServicesAsrNetworkMapping`                | `Remove-ASRNetworkMapping`               |
| `Remove-AzureRmSiteRecoveryPolicy`                       | `Remove-AzureRmRecoveryServicesAsrPolicy`                        | `Remove-ASRPolicy`                       |
| `Remove-AzureRmSiteRecoveryProtectionContainerMapping`   | `Remove-AzureRmRecoveryServicesAsrProtectionContainerMapping`    | `Remove-ASRProtectionContainerMapping`   |
| `Remove-AzureRmSiteRecoveryRecoveryPlan`                 | `Remove-AzureRmRecoveryServicesAsrRecoveryPlan`                  | `Remove-ASRRecoveryPlan`                 |
| `Remove-AzureRmSiteRecoveryReplicationProtectedItem`     | `Remove-AzureRmRecoveryServicesAsrReplicationProtectedItem`      | `Remove-ASRReplicationProtectedItem`     |
| `Remove-AzureRmSiteRecoveryServer`                       | `Remove-AzureRmRecoveryServicesAsrServicesProvider`              |                                          |
| `Remove-AzureRmSiteRecoveryServicesProvider`             | `Remove-AzureRmRecoveryServicesAsrServicesProvider`              | `Remove-ASRServicesProvider`             |
| `Remove-AzureRmSiteRecoverySite`                         | `Remove-AzureRmRecoveryServicesAsrFabric`                        | `Remove-ASRFabric`                       |
| `Remove-AzureRmSiteRecoveryStorageClassificationMapping` | `Remove-AzureRmRecoveryServicesAsrStorageClassificationMapping`  | `Remove-ASRStorageClassificationMapping` |
| `Remove-AzureRmSiteRecoveryVault`                        | `Remove-AzureRmRecoveryServicesVault`                            |                                          |
| `Restart-AzureRmSiteRecoveryJob`                         | `Restart-AzureRmRecoveryServicesAsrJob`                          | `Restart-ASRJob`                         |
| `Resume-AzureRmSiteRecoveryJob`                          | `Resume-AzureRmRecoveryServicesAsrJob`                           | `Resume-ASRJob`                          |
| `Set-AzureRmSiteRecoveryProtectionEntity`                | `New-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `New-ASRReplicationProtectedItem`        |
| `Set-AzureRmSiteRecoveryReplicationProtectedItem`        | `Set-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Set-ASRReplicationProtectedItem`        |
| `Set-AzureRmSiteRecoveryVaultSettings`                   | `Set-AzureRmRecoveryServicesAsrVaultContext`                     | `Set-ASRVaultContext`                    |
| `Set-AzureRmSiteRecoveryVM`                              | `Set-AzureRmRecoveryServicesAsrReplicationProtectedItem`         | `Set-ASRReplicationProtectedItem`        |
| `Start-AzureRmSiteRecoveryApplyRecoveryPoint`            | `Start-AzureRmRecoveryServicesAsrApplyRecoveryPoint`             | `Start-ASRApplyRecoveryPoint`            |
| `Start-AzureRmSiteRecoveryCommitFailoverJob`             | `Start-AzureRmRecoveryServicesAsrCommitFailoverJob`              | `Start-ASRCommitFailoverJob`             |
| `Start-AzureRmSiteRecoveryPlannedFailoverJob`            | `Start-AzureRmRecoveryServicesAsrPlannedFailoverJob`             | `Start-ASRPlannedFailoverJob`            |
| `Start-AzureRmSiteRecoveryPolicyAssociationJob`          | `New-AzureRmRecoveryServicesAsrProtectionContainerMapping`       | `New-ASRProtectionContainerMapping`      |
| `Start-AzureRmSiteRecoveryPolicyDissociationJob`         | `Remove-AzureRmRecoveryServicesAsrProtectionContainerMapping`    | `Remove-ASRProtectionContainerMapping`   |
| `Start-AzureRmSiteRecoveryTestFailoverJob`               | `Start-AzureRmRecoveryServicesAsrTestFailoverJob`                | `Start-ASRTestFailoverJob`               |
| `Start-AzureRmSiteRecoveryUnplannedFailoverJob`          | `Start-AzureRmRecoveryServicesAsrUnplannedFailoverJob`           | `Start-ASRUnplannedFailoverJob`          |
| `Stop-AzureRmSiteRecoveryJob`                            | `Stop-AzureRmRecoveryServicesAsrJob`                             | `Stop-ASRJob`                            |
| `Update-AzureRmSiteRecoveryPolicy`                       | `Update-AzureRmRecoveryServicesAsrPolicy`                        | `Update-ASRPolicy`                       |
| `Update-AzureRmSiteRecoveryProtectionDirection`          | `Update-AzureRmRecoveryServicesAsrProtectionDirection`           | `Update-ASRProtectionDirection`          |
| `Update-AzureRmSiteRecoveryRecoveryPlan`                 | `Update-AzureRmRecoveryServicesAsrRecoveryPlan`                  | `Update-ASRRecoveryPlan`                 |
| `Update-AzureRmSiteRecoveryServer`                       | `Update-AzureRmRecoveryServicesAsrServicesProvider`              | `Update-ASRServicesProvider`             |
| `Update-AzureRmSiteRecoveryServicesProvider`             | `Update-AzureRmRecoveryServicesAsrvCenter`                       | `Update-ASRvCenter`                      |
