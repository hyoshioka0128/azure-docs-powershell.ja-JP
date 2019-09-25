---
title: Az 2.0.0 の移行ガイド
description: この移行ガイドには、Az バージョン 2.0 リリースの Azure PowerShell で行われた重大な変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/24/2019
ms.openlocfilehash: 5f15d1a4f1e8416d7214aceb78494867fe4aad52
ms.sourcegitcommit: 92722d603b60dc769660e7517da60110133d9959
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2019
ms.locfileid: "71226220"
---
# <a name="migration-guide-for-az-200"></a><span data-ttu-id="31e64-103">Az 2.0.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="31e64-103">Migration Guide for Az 2.0.0</span></span>

<span data-ttu-id="31e64-104">このドキュメントでは、Az のバージョン 1.0.0 と 2.0.0 の間での変更点について説明します</span><span class="sxs-lookup"><span data-stu-id="31e64-104">This document describes the changes between the 1.0.0 and 2.0.0 versions of Az</span></span> 

## <a name="table-of-contents"></a><span data-ttu-id="31e64-105">目次</span><span class="sxs-lookup"><span data-stu-id="31e64-105">Table of Contents</span></span>
- [<span data-ttu-id="31e64-106">モジュールの破壊的変更</span><span class="sxs-lookup"><span data-stu-id="31e64-106">Module breaking changes</span></span>](#module-breaking-changes)
  - [<span data-ttu-id="31e64-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="31e64-107">Az.Compute</span></span>](#azcompute)
  - [<span data-ttu-id="31e64-108">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="31e64-108">Az.HDInsight</span></span>](#azhdinsight)
  - [<span data-ttu-id="31e64-109">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="31e64-109">Az.Storage</span></span>](#azstorage)

## <a name="module-breaking-changes"></a><span data-ttu-id="31e64-110">モジュールの破壊的変更</span><span class="sxs-lookup"><span data-stu-id="31e64-110">Module breaking changes</span></span>

### <a name="azcompute"></a><span data-ttu-id="31e64-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="31e64-111">Az.Compute</span></span>

- <span data-ttu-id="31e64-112">```Sku = Aligned``` の使用を優先して、`New-AzAvailabilitySet` および `Update-AzAvailabilitySet` コマンドレットから `Managed` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-112">Removed `Managed` Parameter from `New-AzAvailabilitySet` and `Update-AzAvailabilitySet` cmdlets in favor of using ```Sku = Aligned```</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-113">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-113">Before</span></span>

  ```powershell
  Update-AzAvailabilitySet -Managed
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-114">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-114">After</span></span>

  ```powershell
  Update-AzAvailabilitySet -Sku Aligned
  ```
- <span data-ttu-id="31e64-115">一貫性を保つのために、`Update-AzImage`の 'ByName' および 'ByResourceId' パラメーター セットから `Image` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-115">For consistency, removed `Image` parameter from 'ByName' and 'ByResourceId' parameter sets in `Update-AzImage`</span></span> 
  
  #### <a name="before"></a><span data-ttu-id="31e64-116">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-116">Before</span></span>

  <span data-ttu-id="31e64-117">以下のコードは機能しますが、渡された ImageName は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-117">Note that the below code is functional, but the passed-in ImageName is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Image $Image -Tag $tags

  Update-AzImage -ResourceId $Id -Image $Image -Tag $tags
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-118">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-118">After</span></span>

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Tag $tags

  Update-AzImage -ResourceId $Id -Tag $tags
  ```

- <span data-ttu-id="31e64-119">一貫性を保つのために、`Restart-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-119">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Restart-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="31e64-120">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-120">Before</span></span>

  <span data-ttu-id="31e64-121">以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-121">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>
  ```powershell
  Restart-AzVM -InputObject $VM -Name $Name 

  Restart-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-122">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-122">After</span></span>

  ```powershell
  Restart-AzVM -InputObject $VM

  Restart-AzVM -ResourceId $Id
  ```

- <span data-ttu-id="31e64-123">一貫性を保つのために、`Start-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-123">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Start-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="31e64-124">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-124">Before</span></span>

  <span data-ttu-id="31e64-125">以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-125">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Start-AzVM -InputObject $VM -Name $Name 

  Start-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-126">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-126">After</span></span>

  ```powershell
  Start-AzVM -InputObject $VM

  Start-AzVM -ResourceId $Id
  ```

- <span data-ttu-id="31e64-127">一貫性を保つのために、`Stop-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-127">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Stop-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="31e64-128">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-128">Before</span></span>

  <span data-ttu-id="31e64-129">以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-129">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Stop-AzVM -InputObject $VM -Name $Name 

  Stop-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-130">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-130">After</span></span>

  ```powershell
  Stop-AzVM -InputObject $VM

  Stop-AzVM -ResourceId $Id
  ```

- <span data-ttu-id="31e64-131">一貫性を保つのために、`Remove-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-131">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Remove-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="31e64-132">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-132">Before</span></span>

  <span data-ttu-id="31e64-133">以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-133">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Remove-AzVM -InputObject $VM -Name $Name

  Remove-AzVM -ResourceId $Id -Name $Name 
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-134">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-134">After</span></span>

  ```powershell
  Remove-AzVM -InputObject $VM 

  Remove-AzVM -ResourceId $Id 
  ```

- <span data-ttu-id="31e64-135">一貫性を保つのために、`Set-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-135">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Set-AzVM`</span></span>
  
  #### <a name="before"></a><span data-ttu-id="31e64-136">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-136">Before</span></span>

  <span data-ttu-id="31e64-137">以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-137">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>

  ```powershell
  Set-AzVM -InputObject $VM -Name $Name ...

  Set-AzVM -ResourceId $Id -Name $Name ...
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-138">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-138">After</span></span>

  ```powershell
  Set-AzVM -InputObject $VM ...

  Set-AzVM -ResourceId $Id ...
  ```

- <span data-ttu-id="31e64-139">一貫性を保つのために、`Save-AzVMImage`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-139">For consistency, removed `Name` parameter from 'ByObject' and 'ByResourceId' parameter sets in `Save-AzVMImage`</span></span> 
  
  #### <a name="before"></a><span data-ttu-id="31e64-140">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-140">Before</span></span>
  <span data-ttu-id="31e64-141">以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="31e64-141">Note that the below code is functional, but the passed-in Name is not used, so removing this parameter has no functional impact.</span></span>
  ```powershell
  Save-AzVMImage -InputObject $VM -Name $Name ...

  Save-AzVMImage -ResourceId $Id -Name $Name ...
  ```
  #### <a name="after"></a><span data-ttu-id="31e64-142">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-142">After</span></span>
  ```powershell
  Save-AzVMImage -InputObject $VM ...

  Save-AzVMImage -ResourceId $Id ...
  ```

- <span data-ttu-id="31e64-143">`PSVirtualMachineScaleSetVM` で `ProtectFromScaleIn` プロパティをカプセル化するために ProtectionPolicy プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="31e64-143">Added ProtectionPolicy property to encapsulate `ProtectFromScaleIn` property in `PSVirtualMachineScaleSetVM`</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-144">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-144">Before</span></span>

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectFromScaleIn = $true
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-145">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-145">After</span></span>

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  ```

- <span data-ttu-id="31e64-146">`PSDisk` で `EncryptionSettings` プロパティを囲むために ```EncryptionSettingsCollection``` プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="31e64-146">Added ```EncryptionSettingsCollection``` Property to enclose `EncryptionSettings` property in `PSDisk`</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-147">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-147">Before</span></span>

  ```powershell
  $disk = New-AzDisk ... | Set-AzDiskDiskEncrytionKey ...
  $disk.EncryptionSettings

  $disk = New-AzDisk ... | Set-AzDiskKeyEncrytionKey ...
  $disk.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateDiskEncryptionKey ...
  $update.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateKeyEncryptionKey ...
  $update.EncryptionSettings
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-148">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-148">After</span></span>

  ```powershell
  $disk = New-AzDisk ... | Set-AzDiskDiskEncrytionKey ...
  $disk.EncryptionSettingsCollection.EncryptionSettings

  $disk = New-AzDisk ... | Set-AzDiskKeyEncrytionKey ...
  $disk.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateDiskEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzDiskUpdateConfig | Set-AzDiskUpdateKeyEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings
  ```

- <span data-ttu-id="31e64-149">`PSSnapshot` で `EncryptionSettings` プロパティを囲むために ```EncryptionSettingsCollection``` プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="31e64-149">Added ```EncryptionSettingsCollection``` Property to enclose `EncryptionSettings` property in `PSSnapshot`</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-150">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-150">Before</span></span>

  ```powershell
  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotDiskEncryptionKey ...
  $snap.EncryptionSettings

  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotKeyEncryptionKey ...
  $snap.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateDiskEncryptionKey ...
  $update.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateKeyEncryptionKey ...
  $update.EncryptionSettings
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-151">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-151">After</span></span>

  ```powershell
  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotDiskEncryptionKey ...
  $snap.EncryptionSettingsCollection.EncryptionSettings

  $snap = New-AzSnapshotConfig ... | Set-AzSnapshotKeyEncryptionKey ...
  $snap.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateDiskEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings

  $update = New-AzSnapshotUpdateConfig ... | Set-AzSnapshotUpdateKeyEncryptionKey ...
  $update.EncryptionSettingsCollection.EncryptionSettings
  ```

- <span data-ttu-id="31e64-152">`PSVirtualMachineScaleSet` から `VirtualMachineProfile` プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-152">Removed `VirtualMachineProfile` property from `PSVirtualMachineScaleSet`</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-153">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-153">Before</span></span>

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.VirtualMachineProfile.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-154">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-154">After</span></span>

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

- <span data-ttu-id="31e64-155">コマンドレット `Set-AzVMBootDiagnostic` のエイリアス `Set-AzVMBootDiagnostics` を削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-155">Cmdlet `Set-AzVMBootDiagnostic` removed alias to `Set-AzVMBootDiagnostics`</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-156">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-156">Before</span></span>

  <span data-ttu-id="31e64-157">非推奨のエイリアスを使用</span><span class="sxs-lookup"><span data-stu-id="31e64-157">Using deprecated alias</span></span>

  ```powershell
  Set-AzVMBootDiagnostics
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-158">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-158">After</span></span>

  ```powershell
  Set-AzVMBootDIagnostic
  ```

- <span data-ttu-id="31e64-159">コマンドレット `Export-AzLogAnalyticThrottledRequest` のエイリアス `Export-AzLogAnalyticThrottledRequests` を削除しました</span><span class="sxs-lookup"><span data-stu-id="31e64-159">Cmdlet `Export-AzLogAnalyticThrottledRequest` removed alias to `Export-AzLogAnalyticThrottledRequests`</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-160">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-160">Before</span></span>

  <span data-ttu-id="31e64-161">非推奨のエイリアスを使用</span><span class="sxs-lookup"><span data-stu-id="31e64-161">Using deprectaed alias</span></span>

  ```powershell
  Export-AzLogAnalyticThrottledRequests
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-162">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-162">After</span></span>

  ```powershell
  Export-AzLogAnalyticThrottledRequest
  ```

### <a name="azhdinsight"></a><span data-ttu-id="31e64-163">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="31e64-163">Az.HDInsight</span></span>

- <span data-ttu-id="31e64-164">`Grant-AzHDInsightHttpServicesAccess` および `Revoke-AzHDInsightHttpServicesAccess` コマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="31e64-164">Removed the `Grant-AzHDInsightHttpServicesAccess` and `Revoke-AzHDInsightHttpServicesAccess` cmdlets.</span></span> <span data-ttu-id="31e64-165">HTTP アクセスは常にすべての HDInsight クラスターで有効になっているため、これらは不要になりました。</span><span class="sxs-lookup"><span data-stu-id="31e64-165">These are no longer necessary because HTTP access is always enabled on all HDInsight clusters.</span></span>
- <span data-ttu-id="31e64-166">新しい `Set-AzHDInsightGatewayCredential` コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="31e64-166">Added a new `Set-AzHDInsightGatewayCredential`  cmdlet.</span></span> <span data-ttu-id="31e64-167">このコマンドレットを使用して、ゲートウェイの HTTP ユーザー名とパスワードを変更します (`Grant-AzHDInsightHttpServicesAccess` に代わるもの)。</span><span class="sxs-lookup"><span data-stu-id="31e64-167">Use this cmdlet to change the gateway HTTP username and password (replaces `Grant-AzHDInsightHttpServicesAccess`).</span></span>
- <span data-ttu-id="31e64-168">ストレージ キーに対するきめ細かいロールベースのアクセスをサポートするため、`Get-AzHDInsightJobOutput` コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="31e64-168">Updated the `Get-AzHDInsightJobOutput` cmdlet to support granular role-based access to the storage key.</span></span>
    - <span data-ttu-id="31e64-169">HDInsight クラスターのオペレーター、共同作成者、または所有者のロールを持つユーザーには影響を及ぼしません。</span><span class="sxs-lookup"><span data-stu-id="31e64-169">Users with HDInsight Cluster Operator, Contributor, or Owner roles will not be affected.</span></span>
    - <span data-ttu-id="31e64-170">閲覧者のロールのみを持つユーザーは、`DefaultStorageAccountKey` パラメーターを明示的に指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="31e64-170">Users with only the Reader role will need to specify `DefaultStorageAccountKey` parameter explicitly.</span></span>

<span data-ttu-id="31e64-171">これらのロールベースのアクセスの変更の詳細については、[aka.ms/hdi-config-update](http://aka.ms/hdi-config-update) を参照してください</span><span class="sxs-lookup"><span data-stu-id="31e64-171">For more information about these role-based access changes, see [aka.ms/hdi-config-update](http://aka.ms/hdi-config-update)</span></span>

  #### <a name="before"></a><span data-ttu-id="31e64-172">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-172">Before</span></span>

  ```powershell
  Grant-AzHDInsightHttpServicesAccess -ClusterName $cluster -HttpCredential $credential
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-173">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-173">After</span></span>

  ```powershell
  Set-AzHDInsightGatewayCredential -ClusterName $cluster -HttpCredential $credential
  ```

###  <a name="users-with-only-reader-role-for-cmdlet-get-azhdinsightjoboutput"></a><span data-ttu-id="31e64-174">コマンドレット Get AzHDInsightJobOutput の閲覧者のロールのみを持つユーザー</span><span class="sxs-lookup"><span data-stu-id="31e64-174">Users with only Reader role for cmdlet Get-AzHDInsightJobOutput</span></span>

  ####  <a name="before"></a><span data-ttu-id="31e64-175">実装する前</span><span class="sxs-lookup"><span data-stu-id="31e64-175">Before</span></span>

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId
  ```

  #### <a name="after"></a><span data-ttu-id="31e64-176">実装した後</span><span class="sxs-lookup"><span data-stu-id="31e64-176">After</span></span>

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId -DefaultStorageAccountKey $storageAccountKey
  ```

### <a name="azstorage"></a><span data-ttu-id="31e64-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="31e64-177">Az.Storage</span></span>

- <span data-ttu-id="31e64-178">Blob、キュー、およびファイルのコマンドレットから返される型の名前空間は、名前空間を `Microsoft.WindowsAzure.Storage` から `Microsoft.Azure.Storage` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="31e64-178">Namespaces for types returned from Blob, Queue, and File cmdlets have changed their namespace from `Microsoft.WindowsAzure.Storage` to `Microsoft.Azure.Storage`.</span></span>  <span data-ttu-id="31e64-179">これは厳密に言えば重大な変更ポリシーに従った重大な変更ではありませんが、これらのコマンドレットから返されたオブジェクトを操作するために Storage .Net SDK からのメソッドを使用するコードに、何らかの変更が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="31e64-179">While this is not technically a breaking change according to the breaking change policy, it may require some changes in code that uses the methods from the Storage .Net SDK to interact with the objects returned from these cmdlets.</span></span>

  #### <a name="example-1--add-a-message-to-a-queue-change-cloudqueuemessage-object-namespace"></a><span data-ttu-id="31e64-180">例 1:メッセージをキューに追加します (CloudQueueMessage オブジェクトの名前空間を変更)</span><span class="sxs-lookup"><span data-stu-id="31e64-180">Example 1:  Add a message to a Queue (change CloudQueueMessage object namespace)</span></span>

  <span data-ttu-id="31e64-181">変更前:</span><span class="sxs-lookup"><span data-stu-id="31e64-181">Before:</span></span> 

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.WindowsAzure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)" -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  <span data-ttu-id="31e64-182">変更後:</span><span class="sxs-lookup"><span data-stu-id="31e64-182">After:</span></span>

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.Azure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)"  -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  #### <a name="example-2--fetch-blobfile-attributes-with-accesscondition-change-accesscondition-object-namespace"></a><span data-ttu-id="31e64-183">例 2:AccessCondition を使用して BLOB/ファイル属性を取得します (AccessCondition オブジェクトの名前空間を変更)</span><span class="sxs-lookup"><span data-stu-id="31e64-183">Example 2:  Fetch Blob/File Attributes with AccessCondition (change AccessCondition object namespace)</span></span>

  <span data-ttu-id="31e64-184">変更前:</span><span class="sxs-lookup"><span data-stu-id="31e64-184">Before:</span></span> 

  ```powershell
  $accessCondition= New-Object Microsoft.WindowsAzure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

  <span data-ttu-id="31e64-185">変更後:</span><span class="sxs-lookup"><span data-stu-id="31e64-185">After:</span></span>

  ```powershell
  $accessCondition= New-Object Microsoft.Azure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

- <span data-ttu-id="31e64-186">厳密に言えば重大な変更ではありませんが、`New/Get/Set-AzStorageAccount` の変更から返されるストレージ アカウントの Sku.Name プロパティの出力の違いが次のようになることがわかります。</span><span class="sxs-lookup"><span data-stu-id="31e64-186">While not technically a breaking change, you will notice output differences in the Sku.Name property of Storage Accounts returned from  `New/Get/Set-AzStorageAccount` changes are as follows.</span></span> <span data-ttu-id="31e64-187">(この変更の後、出力と入力の SkuName が調整されます。)</span><span class="sxs-lookup"><span data-stu-id="31e64-187">(After the change, output and input SkuName are aligned.)</span></span>
  - <span data-ttu-id="31e64-188">"StandardLRS" -> "Standard_LRS";</span><span class="sxs-lookup"><span data-stu-id="31e64-188">"StandardLRS" -> "Standard_LRS";</span></span>
  - <span data-ttu-id="31e64-189">"StandardGRS" -> "Standard_GRS";</span><span class="sxs-lookup"><span data-stu-id="31e64-189">"StandardGRS" -> "Standard_GRS";</span></span>
  - <span data-ttu-id="31e64-190">"StandardRAGRS" -> "Standard_RAGRS";</span><span class="sxs-lookup"><span data-stu-id="31e64-190">"StandardRAGRS" -> "Standard_RAGRS";</span></span>
  - <span data-ttu-id="31e64-191">"StandardZRS" -> "Standard_ZRS";</span><span class="sxs-lookup"><span data-stu-id="31e64-191">"StandardZRS" -> "Standard_ZRS";</span></span>
  - <span data-ttu-id="31e64-192">"PremiumLRS" -> "Premium_LRS";</span><span class="sxs-lookup"><span data-stu-id="31e64-192">"PremiumLRS" -> "Premium_LRS";</span></span>

- <span data-ttu-id="31e64-193">種類を指定せずにストレージ アカウントを作成するときの既定のサービスの動作が変更されました。</span><span class="sxs-lookup"><span data-stu-id="31e64-193">The default service behavior when creating a storage account withous specifying a Kind has changed.</span></span>  <span data-ttu-id="31e64-194">以前のバージョンでは、`Kind` を指定せずにストレージ アカウントを作成すると、種類が `Storage` のストレージ アカウントが使用されました。新しいバージョンでは、`StorageV2` が既定の `Kind` の値です。</span><span class="sxs-lookup"><span data-stu-id="31e64-194">In previous versions, when a storage account was created with no `Kind` specified, the Storage account Kind of `Storage` was used, in the new version `StorageV2` is the default `Kind` value.</span></span> <span data-ttu-id="31e64-195">種類が 'Storage' の V1 ストレージ アカウントを作成する必要がある場合は、パラメーター '-Kind Storage' を追加します</span><span class="sxs-lookup"><span data-stu-id="31e64-195">If you need to create a V1 Storage account with Kind 'Storage', add parameter '-Kind Storage'</span></span>

  #### <a name="example--create-a-storage-account-default-kind-change"></a><span data-ttu-id="31e64-196">例:ストレージ アカウントを作成する (既定の種類の変更)</span><span class="sxs-lookup"><span data-stu-id="31e64-196">Example : Create a storage Account (Default Kind change)</span></span>  

  <span data-ttu-id="31e64-197">変更前:</span><span class="sxs-lookup"><span data-stu-id="31e64-197">Before:</span></span>

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName     Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------     ----      ---------- ------------          ----------------- ----------------------
  accountname        groupname         westus   StandardLRS Storage   Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```

  <span data-ttu-id="31e64-198">変更後:</span><span class="sxs-lookup"><span data-stu-id="31e64-198">After:</span></span>

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName      Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------      ----      ----------  ------------          ----------------- ----------------------
  accountname        groupname         westus   Standard_LRS StorageV2 Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```
