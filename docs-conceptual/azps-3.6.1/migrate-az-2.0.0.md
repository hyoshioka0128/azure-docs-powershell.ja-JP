---
title: Az 2.0.0 の移行ガイド
description: この移行ガイドには、Az バージョン 2.0 リリースの Azure PowerShell で行われた重大な変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/24/2019
ms.openlocfilehash: 133769c09f74e1d0d90eff0c6c4bdbb90d1ebe24
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2020
ms.locfileid: "79035704"
---
# <a name="migration-guide-for-az-200"></a>Az 2.0.0 の移行ガイド

このドキュメントでは、Az のバージョン 1.0.0 と 2.0.0 の間での変更点について説明します 

## <a name="table-of-contents"></a>目次
- [モジュールの破壊的変更](#module-breaking-changes)
  - [Az.Compute](#azcompute)
  - [Az.HDInsight](#azhdinsight)
  - [Az.Storage](#azstorage)

## <a name="module-breaking-changes"></a>モジュールの破壊的変更

### <a name="azcompute"></a>Az.Compute

- ```Sku = Aligned``` の使用を優先して、`New-AzAvailabilitySet` および `Update-AzAvailabilitySet` コマンドレットから `Managed` パラメーターを削除しました

  #### <a name="before"></a>[指定日付より前]

  ```powershell
  Update-AzAvailabilitySet -Managed
  ```

  #### <a name="after"></a>After

  ```powershell
  Update-AzAvailabilitySet -Sku Aligned
  ```
- 一貫性を保つのために、`Update-AzImage`の 'ByName' および 'ByResourceId' パラメーター セットから `Image` パラメーターを削除しました 
  
  #### <a name="before"></a>[指定日付より前]

  以下のコードは機能しますが、渡された ImageName は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Image $Image -Tag $tags

  Update-AzImage -ResourceId $Id -Image $Image -Tag $tags
  ```

  #### <a name="after"></a>After

  ```powershell
  Update-AzImage -ResourceGroupName $Rg -ImageName $Name -Tag $tags

  Update-AzImage -ResourceId $Id -Tag $tags
  ```

- 一貫性を保つのために、`Restart-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました
  
  #### <a name="before"></a>[指定日付より前]

  以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。
  ```powershell
  Restart-AzVM -InputObject $VM -Name $Name 

  Restart-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a>After

  ```powershell
  Restart-AzVM -InputObject $VM

  Restart-AzVM -ResourceId $Id
  ```

- 一貫性を保つのために、`Start-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました
  
  #### <a name="before"></a>[指定日付より前]

  以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。

  ```powershell
  Start-AzVM -InputObject $VM -Name $Name 

  Start-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a>After

  ```powershell
  Start-AzVM -InputObject $VM

  Start-AzVM -ResourceId $Id
  ```

- 一貫性を保つのために、`Stop-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました
  
  #### <a name="before"></a>[指定日付より前]

  以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。

  ```powershell
  Stop-AzVM -InputObject $VM -Name $Name 

  Stop-AzVM -ResourceId $Id -Name $Name
  ```

  #### <a name="after"></a>After

  ```powershell
  Stop-AzVM -InputObject $VM

  Stop-AzVM -ResourceId $Id
  ```

- 一貫性を保つのために、`Remove-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました
  
  #### <a name="before"></a>[指定日付より前]

  以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。

  ```powershell
  Remove-AzVM -InputObject $VM -Name $Name

  Remove-AzVM -ResourceId $Id -Name $Name 
  ```

  #### <a name="after"></a>After

  ```powershell
  Remove-AzVM -InputObject $VM 

  Remove-AzVM -ResourceId $Id 
  ```

- 一貫性を保つのために、`Set-AzVM`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました
  
  #### <a name="before"></a>[指定日付より前]

  以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。

  ```powershell
  Set-AzVM -InputObject $VM -Name $Name ...

  Set-AzVM -ResourceId $Id -Name $Name ...
  ```

  #### <a name="after"></a>After

  ```powershell
  Set-AzVM -InputObject $VM ...

  Set-AzVM -ResourceId $Id ...
  ```

- 一貫性を保つのために、`Save-AzVMImage`の 'ByObject' および 'ByResourceId' パラメーター セットから `Name` パラメーターを削除しました 
  
  #### <a name="before"></a>[指定日付より前]
  以下のコードは機能しますが、渡された Name は使用されないため、このパラメーターを削除しても機能への影響はないことに注意してください。
  ```powershell
  Save-AzVMImage -InputObject $VM -Name $Name ...

  Save-AzVMImage -ResourceId $Id -Name $Name ...
  ```
  #### <a name="after"></a>After
  ```powershell
  Save-AzVMImage -InputObject $VM ...

  Save-AzVMImage -ResourceId $Id ...
  ```

- `PSVirtualMachineScaleSetVM` で `ProtectFromScaleIn` プロパティをカプセル化するために ProtectionPolicy プロパティを追加しました

  #### <a name="before"></a>[指定日付より前]

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectFromScaleIn = $true
  ```

  #### <a name="after"></a>After

  ```powershell
  $vmss = Get-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Update-AzVMssVM ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  $vmss = Remove-AzVMssVMDataDisk ...
  $vmss.ProtectionPolicy.ProtectFromScaleIn = $true

  ```

- `PSDisk` で `EncryptionSettings` プロパティを囲むために ```EncryptionSettingsCollection``` プロパティを追加しました

  #### <a name="before"></a>[指定日付より前]

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

  #### <a name="after"></a>After

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

- `PSSnapshot` で `EncryptionSettings` プロパティを囲むために ```EncryptionSettingsCollection``` プロパティを追加しました

  #### <a name="before"></a>[指定日付より前]

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

  #### <a name="after"></a>After

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

- `PSVirtualMachineScaleSet` から `VirtualMachineProfile` プロパティを削除しました

  #### <a name="before"></a>[指定日付より前]

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.VirtualMachineProfile.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

  #### <a name="after"></a>After

  ```powershell
  $vmss = New-AzVMSSConfig ...
  $vmss.AdditionalCapabilities.UltraSSDEnabled = $true
  ```

- コマンドレット `Set-AzVMBootDiagnostic` のエイリアス `Set-AzVMBootDiagnostics` を削除しました

  #### <a name="before"></a>[指定日付より前]

  非推奨のエイリアスを使用

  ```powershell
  Set-AzVMBootDiagnostics
  ```

  #### <a name="after"></a>After

  ```powershell
  Set-AzVMBootDIagnostic
  ```

- コマンドレット `Export-AzLogAnalyticThrottledRequest` のエイリアス `Export-AzLogAnalyticThrottledRequests` を削除しました

  #### <a name="before"></a>[指定日付より前]

  非推奨のエイリアスを使用

  ```powershell
  Export-AzLogAnalyticThrottledRequests
  ```

  #### <a name="after"></a>After

  ```powershell
  Export-AzLogAnalyticThrottledRequest
  ```

### <a name="azhdinsight"></a>Az.HDInsight

- `Grant-AzHDInsightHttpServicesAccess` および `Revoke-AzHDInsightHttpServicesAccess` コマンドレットを削除しました。 HTTP アクセスは常にすべての HDInsight クラスターで有効になっているため、これらは不要になりました。
- 新しい `Set-AzHDInsightGatewayCredential` コマンドレットを追加しました。 このコマンドレットを使用して、ゲートウェイの HTTP ユーザー名とパスワードを変更します (`Grant-AzHDInsightHttpServicesAccess` に代わるもの)。
- ストレージ キーに対するきめ細かいロールベースのアクセスをサポートするため、`Get-AzHDInsightJobOutput` コマンドレットを更新しました。
    - HDInsight クラスターのオペレーター、共同作成者、または所有者のロールを持つユーザーには影響を及ぼしません。
    - 閲覧者のロールのみを持つユーザーは、`DefaultStorageAccountKey` パラメーターを明示的に指定する必要があります。

これらのロールベースのアクセスの変更の詳細については、[aka.ms/hdi-config-update](https://aka.ms/hdi-config-update) を参照してください

  #### <a name="before"></a>[指定日付より前]

  ```powershell
  Grant-AzHDInsightHttpServicesAccess -ClusterName $cluster -HttpCredential $credential
  ```

  #### <a name="after"></a>After

  ```powershell
  Set-AzHDInsightGatewayCredential -ClusterName $cluster -HttpCredential $credential
  ```

###  <a name="users-with-only-reader-role-for-cmdlet-get-azhdinsightjoboutput"></a>コマンドレット Get AzHDInsightJobOutput の閲覧者のロールのみを持つユーザー

  ####  <a name="before"></a>[指定日付より前]

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId
  ```

  #### <a name="after"></a>After

  ```powershell
  Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId -DefaultStorageAccountKey $storageAccountKey
  ```

### <a name="azstorage"></a>Az.Storage

- Blob、キュー、およびファイルのコマンドレットから返される型の名前空間は、名前空間を `Microsoft.WindowsAzure.Storage` から `Microsoft.Azure.Storage` に変更しました。  これは厳密に言えば重大な変更ポリシーに従った重大な変更ではありませんが、これらのコマンドレットから返されたオブジェクトを操作するために Storage .Net SDK からのメソッドを使用するコードに、何らかの変更が必要になる場合があります。

  #### <a name="example-1--add-a-message-to-a-queue-change-cloudqueuemessage-object-namespace"></a>例 1:メッセージをキューに追加します (CloudQueueMessage オブジェクトの名前空間を変更)

  次の処理の前 

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.WindowsAzure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)" -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  次の処理の後

  ```powershell
  $queue = Get-AzStorageQueue –Name $queueName –Context $ctx
  $queueMessage = New-Object -TypeName "Microsoft.Azure.Storage.Queue.CloudQueueMessage,$($queue.CloudQueue.GetType().Assembly.FullName)"  -ArgumentList "This is message 1"
  $queue.CloudQueue.AddMessageAsync($QueueMessage)
  ```

  #### <a name="example-2--fetch-blobfile-attributes-with-accesscondition-change-accesscondition-object-namespace"></a>例 2:AccessCondition を使用して BLOB/ファイル属性を取得します (AccessCondition オブジェクトの名前空間を変更)

  次の処理の前 

  ```powershell
  $accessCondition= New-Object Microsoft.WindowsAzure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

  次の処理の後

  ```powershell
  $accessCondition= New-Object Microsoft.Azure.Storage.AccessCondition

  $blob = Get-AzureStorageBlob -Container $containerName -Blob $blobName
  $blob.ICloudBlob.FetchAttributes($accessCondition)

  $file = Get-AzureStorageFile -ShareName $shareName -Path $filepath
  $file.FetchAttributes($accessCondition)
  ```

- 厳密に言えば重大な変更ではありませんが、`New/Get/Set-AzStorageAccount` の変更から返されるストレージ アカウントの Sku.Name プロパティの出力の違いが次のようになることがわかります。 (この変更の後、出力と入力の SkuName が調整されます。)
  - "StandardLRS" -> "Standard_LRS";
  - "StandardGRS" -> "Standard_GRS";
  - "StandardRAGRS" -> "Standard_RAGRS";
  - "StandardZRS" -> "Standard_ZRS";
  - "PremiumLRS" -> "Premium_LRS";

- 種類を指定せずにストレージ アカウントを作成するときの既定のサービスの動作が変更されました。  以前のバージョンでは、`Kind` を指定せずにストレージ アカウントを作成すると、種類が `Storage` のストレージ アカウントが使用されました。新しいバージョンでは、`StorageV2` が既定の `Kind` の値です。 種類が 'Storage' の V1 ストレージ アカウントを作成する必要がある場合は、パラメーター '-Kind Storage' を追加します

  #### <a name="example--create-a-storage-account-default-kind-change"></a>例:ストレージ アカウントを作成する (既定の種類の変更)  

  次の処理の前

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName     Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------     ----      ---------- ------------          ----------------- ----------------------
  accountname        groupname         westus   StandardLRS Storage   Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```

  次の処理の後

  ```powershell
  PS c:\> New-AzStorageAccount -ResourceGroupName groupname -Name accountname -SkuName Standard_LRS -Location "westus"

  StorageAccountName ResourceGroupName Location SkuName      Kind      AccessTier CreationTime          ProvisioningState EnableHttpsTrafficOnly
  ------------------ ----------------- -------- -------      ----      ----------  ------------          ----------------- ----------------------
  accountname        groupname         westus   Standard_LRS StorageV2 Hot        4/17/2018 10:34:32 AM Succeeded         False
  ```
