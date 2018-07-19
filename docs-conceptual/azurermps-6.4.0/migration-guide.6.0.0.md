---
title: Microsoft Azure PowerShell 6.0.0 の重大な変更
description: この移行ガイドには、バージョン 6 リリースの Azure PowerShell で行われた重大な変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 5/1/2018
ms.openlocfilehash: 4f9c99152fd6ddc23aec005c8e8957e545e65246
ms.sourcegitcommit: 990f82648b0aa2e970f96c02466a7134077c8c56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/11/2018
ms.locfileid: "38100207"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-600"></a>Microsoft Azure PowerShell 6.0.0 の重大な変更

このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。 各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。 詳細なコンテキストについては、各変更に関するプル要求を参照してください。

## <a name="table-of-contents"></a>目次

- [重大な変更 - 全般](#general-breaking-changes)
    - [5.0 に引き上げられた PowerShell の必要最小バージョン](#minimum-powershell-version-required-bumped-to-50)
    - [既定で有効になっているコンテキスト自動保存](#context-autosaved-enabled-by-default)
    - [Tags エイリアスの削除](#removal-of-tags-alias)
- [AzureRM.Compute コマンドレットの重大な変更](#breaking-changes-to-azurermcompute-cmdlets)
- [AzureRM.DataLakeStore コマンドレットの重大な変更](#breaking-changes-to-azurermdatalakestore-cmdlets)
- [AzureRM.Dns コマンドレットの重大な変更](#breaking-changes-to-azurermdns-cmdlets)
- [AzureRM.Insights コマンドレットの重大な変更](#breaking-changes-to-azurerminsights-cmdlets)
- [AzureRM.KeyVault コマンドレットの重大な変更](#breaking-changes-to-azurermkeyvault-cmdlets)
- [AzureRM.Network コマンドレットの重大な変更](#breaking-changes-to-azurermnetwork-cmdlets)
- [AzureRM.RedisCache コマンドレットの重大な変更](#breaking-changes-to-azurermrediscache-cmdlets)
- [AzureRM.Resources コマンドレットの重大な変更](#breaking-changes-to-azurermresources-cmdlets)
- [AzureRM.Storage コマンドレットの重大な変更](#breaking-changes-to-azurermstorage-cmdlets)
- [削除されたモジュール](#removed-modules)
    - [`AzureRM.ServerManagement`](#azurermservermanagement)
    - [`AzureRM.SiteRecovery`](#azurermsiterecovery)

## <a name="general-breaking-changes"></a>重大な変更 - 全般

### <a name="minimum-powershell-version-required-bumped-to-50"></a>5.0 に引き上げられた PowerShell の必要最小バージョン

以前は、Azure PowerShell でコマンドレットを実行するには、PowerShell のバージョン 3.0 "_以上_" が必要でした。 今後、この要件は PowerShell のバージョン 5.0 に引き上げられます。 PowerShell 5.0 へのアップグレードについては、[こちらの表](https://docs.microsoft.com/en-us/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)をご覧ください。

### <a name="context-autosave-enabled-by-default"></a>既定で有効になっているコンテキスト自動保存

コンテキスト自動保存は、新しい PowerShell セッションと別の PowerShell セッション間で使用できる Azure サインイン情報のストレージです。 コンテキスト自動保存の詳細については、[こちらのドキュメント](https://docs.microsoft.com/en-us/powershell/azure/context-persistence)をご覧ください。

以前は、既定でコンテキスト自動保存は無効になっていました。つまり、`Enable-AzureRmContextAutosave` コマンドレットを実行してコンテキストの永続化を有効にするまで、ユーザーの Azure 認証情報はセッション間で保存されませんでした。 今後は、コンテキスト自動保存が既定で有効になります。つまり、"_コンテキスト自動保存設定を保存していない_" ユーザーも、次回サインインしたときにコンテキストが保存されています。 ユーザーは `Disable-AzureRmContextAutosave` コマンドレットを使用して、この機能を無効にすることができます。

_注_: これまでコンテキスト自動保存を無効にしていたユーザーまたは有効にしていたユーザーと既存のコンテキストはこの変更の影響を受けません。

### <a name="removal-of-tags-alias"></a>Tags エイリアスの削除

多数のコマンドレットで、`Tag` パラメーターの `Tags` エイリアスが削除されました。 この影響を受けるモジュール (および対応するコマンドレット) は次のとおりです。

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

## <a name="breaking-changes-to-azurermcompute-cmdlets"></a>AzureRM.Compute コマンドレットの重大な変更

**その他**
- `PSDisk` 型と `PSSnapshot` 型に入れ子になった SKU 名プロパティが、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

```powershell
$disk = Get-AzureRmDisk -ResourceGroupName "MyResourceGroup" -DiskName "MyDiskName"
$disk.Sku.Name       # This will now return Standard_LRS or Premium_LRS

$snapshot = Get-AzureRmSnapshot -ResourceGroupName "MyResourceGroup" -SnapshotName "MySnapshotName"
$snapshot.Sku.Name   # This will now return Standard_LRS or Premium_LRS
```

- `PSVirtualMachine`、`PSVirtualMachineScaleSet`、`PSImage` の各型に入れ子になったストレージ アカウントの種類プロパティが、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

```powershell
$vm = Get-AzureRmVM -ResourceGroupName "MyResourceGroup" -Name "MyVM"
$vm.StorageProfile.DataDisks[0].ManagedDisk.StorageAccountType   # This will now return Standard_LRS or Premium_LRS
```

**Add-AzureRmImageDataDisk**
- `StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Add-AzureRmVMDataDisk**
- `StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Add-AzureRmVmssDataDisk**
- `StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**New-AzureRmAvailabilitySet**
- `Sku` を優先して、`Managed` パラメーターが削除されました。

```powershell
# Old
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Managed

# New
New-AzureRmAvailabilitySet -ResourceGroupName "MyRG" -Name "MyAvailabilitySet" -Location "West US" -Sku "Aligned"
```

**New-AzureRmDiskConfig**
- `SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**New-AzureRmDiskUpdateConfig**
- `SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**New-AzureRmSnapshotConfig**
- `SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**New-AzureRmSnapshotUpdateConfig**
- `SkuName` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Set-AzureRmImageOsDisk**
- `StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Set-AzureRmVMAEMExtension**
- `DisableWAD` パラメーターが削除されました。
    -  Windows Azure 診断が既定で無効になっています。

**Set-AzureRmVMDataDisk**
- `StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Set-AzureRmVMOSDisk**
- `StorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Set-AzureRmVmssStorageProfile**
- `ManagedDisk` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

**Update-AzureRmVmss**
- `ManagedDiskStorageAccountType` パラメーターに指定できる値が、`StandardLRS`、`PremiumLRS` から `Standard_LRS`、`Premium_LRS` にそれぞれ変更されました。

## <a name="breaking-changes-to-azurermdatalakestore-cmdlets"></a>AzureRM.DataLakeStore コマンドレットの重大な変更

**Export-AzureRmDataLakeStoreItem**
- `PerFileThreadCount` パラメーターと `ConcurrentFileCount` パラメーターが削除されました。 今後は `Concurrency` パラメーターを使用してください。

```powershell
# Old
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Export-AzureRmDataLakeStoreItem -Account contoso -Path /test -Destination C:\test -Recurse -Resume -Concurrency 160
```

**Import-AzureRmDataLakeStoreItem**
- `PerFileThreadCount` パラメーターと `ConcurrentFileCount` パラメーターが削除されました。 今後は `Concurrency` パラメーターを使用してください。

```powershell
# Old
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -PerFileThreadCount 2 -ConcurrentFileCount 80

# New
Import-AzureRmDataLakeStoreItem -Account contoso -Path C:\test -Destination /test -Recurse -Resume -ForceBinary -Concurrency 160
```

**Remove-AzureRmDataLakeStoreItem**
- `Clean` パラメーターが削除されました。

```powershell
# Old
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse -Clean

# New
Remove-AzureRmDataLakeStoreItem -Account "ContosoADL" -path /myFolder -Recurse
```

## <a name="breaking-changes-to-azurermdns-cmdlets"></a>AzureRM.Dns コマンドレットの重大な変更

**New-AzureRmDnsRecordSet**
- `Force` パラメーターが削除されました。

**Remove-AzureRmDnsRecordSet**
- `Force` パラメーターが削除されました。

**Remove-AzureRmDnsZone**
- `Force` パラメーターが削除されました。

## <a name="breaking-changes-to-azurerminsights-cmdlets"></a>AzureRM.Insights コマンドレットの重大な変更

**Add-AzureRmAutoscaleSetting**
- パラメーター エイリアス `AutoscaleProfiles` と `Notifications` が削除されました。

**Add-AzureRmLogProfile**
- パラメーター エイリアス `Categories` と `Locations` が削除されました。

**Add-AzureRmMetricAlertRule**
- パラメーター エイリアス `Actions` が削除されました。

**Add-AzureRmWebtestAlertRule**
- パラメーター エイリアス `Actions` が削除されました。

**Get-AzureRmLog**
- パラメーター エイリアス `MaxRecords` と `MaxEvents` が削除されました。

**Get-AzureRmMetricDefinition**
- パラメーター エイリアス `MetricNames` が削除されました。

**New-AzureRmAlertRuleEmail**
- パラメーター エイリアス `CustomEmails` と `SendToServiceOwners` が削除されました。

**New-AzureRmAlertRuleWebhook**
- パラメーター エイリアス `Properties` が削除されました。

**New-AzureRmAutoscaleNotification**
- パラメーター エイリアス `CustomEmails`、`SendEmailToSubscriptionCoAdministrators`、`Webhooks` が削除されました。

**New-AzureRmAutoscaleProfile**
- パラメーター エイリアス `Rules`、`ScheduleDays`、`ScheduleHours`、`ScheduleMinutes` が削除されました。

**New-AzureRmAutoscaleWebhook**
- パラメーター エイリアス `Properties` が削除されました。

## <a name="breaking-changes-to-azurermkeyvault-cmdlets"></a>AzureRM.KeyVault コマンドレットの重大な変更

**Add-AzureKeyVaultCertificate**
- `CertificatePolicy` パラメーターが必須になりました。

**Set-AzureKeyVaultManagedStorageSasDefinition**
- このコマンドレットは、アクセス トークンを構成する個々のパラメーターを受け入れなくなりました。代わりに、`Service` や `Permissions` などの明示的なトークン パラメーターが、他の場所で定義されたサンプル アクセス トークン (Storage PowerShell コマンドレットを使用するか、Storage ドキュメントに従って手動で構成) に対応する汎用の `TemplateUri` パラメーターに置き換えられます。`ValidityPeriod` パラメーターは保持されます。

Azure Storage の共有アクセス トークンの構成の詳細については、それぞれのドキュメント ページをご覧ください。
- [サービス SAS の作成] (https://docs.microsoft.com/en-us/rest/api/storageservices/Constructing-a-Service-SAS)
- [アカウント SAS の作成] (https://docs.microsoft.com/en-us/rest/api/storageservices/constructing-an-account-sas)

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

**Set-AzureKeyVaultCertificateIssuer**
- `IssuerProvider` パラメーターが必須になりました。

**Undo-AzureKeyVaultCertificateRemoval**
- このコマンドレットの出力が、`CertificateBundle` から `PSKeyVaultCertificate` に変更されました。

**Undo-AzureRmKeyVaultRemoval**
- `ResourceGroupName` が `InputObject` パラメーター セットから削除されました。代わりに、`InputObject` パラメーターの `ResourceId` プロパティから取得されます。

**Set-AzureRmKeyVaultAccessPolicy**
- `PermissionsToKeys`、`PermissionsToSecrets`、`PermissionsToCertificates` から、`all` アクセス許可が削除されました。

**全般**
- `InputObject` によるパイプ処理が有効になっているすべてのコマンドレットから、`ValueFromPipelineByPropertyName` プロパティが削除されました。  影響を受けるコマンドレットは次のとおりです。
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

- すべてのコマンドレットから `ConfirmImpact` レベルが削除されました。  影響を受けるコマンドレットは次のとおりです。
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

- `IKeyVaultDataServiceClient` が更新されました。これにより、すべての証明書操作で、SDK の種類ではなく PSTypes が返されます。 次のトピックがあります。
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

## <a name="breaking-changes-to-azurermnetwork-cmdlets"></a>AzureRM.Network コマンドレットの重大な変更


**Add-AzureRmApplicationGatewayBackendHttpSettings**
- `ProbeEnabled` パラメーターが削除されました。

**Add-AzureRmVirtualNetworkPeering**
- パラメーター エイリアス `AlloowGatewayTransit` が削除されました。

**New-AzureRmApplicationGatewayBackendHttpSettings**
- `ProbeEnabled` パラメーターが削除されました。

**Set-AzureRmApplicationGatewayBackendHttpSettings**
- `ProbeEnabled` パラメーターが削除されました。

## <a name="breaking-changes-to-azurermrediscache-cmdlets"></a>AzureRM.RedisCache コマンドレットの重大な変更

**New-AzureRmRedisCache**
- `SubnetId` を優先して、`Subnet` パラメーターと `VirtualNetwork` パラメーターが削除されました。
- `RedisVersion` パラメーターが削除されました。
- `RedisConfiguration` を優先して、`MaxMemoryPolicy` パラメーターが削除されました。

```powershell
# Old
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -MaxMemoryPolicy "allkeys-lru"

# New
New-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -Location "North Central US" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

**Set-AzureRmRedisCache**
- `RedisConfiguration` を優先して、`MaxMemoryPolicy` パラメーターが削除されました。

```powershell
# Old
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -MaxMemoryPolicy "allkeys-lru"

# New
Set-AzureRmRedisCache -ResourceGroupName "MyRG" -Name "MyRedisCache" -RedisConfiguration @{"maxmemory-policy" = "allkeys-lru"}
```

## <a name="breaking-changes-to-azurermresources-cmdlets"></a>AzureRM.Resources コマンドレットの重大な変更

**Find-AzureRmResource**
- このコマンドレットは削除され、機能が `Get-AzureRmResource` に移動されました。

```powershell
# Old
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupNameContains "ResourceGroup"
Find-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceNameContains "test"

# New
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -ResourceGroupName "*ResourceGroup*"
Get-AzureRmResource -ResourceType "Microsoft.Web/sites" -Name "*test*"
```

**Find-AzureRmResourceGroup**
- このコマンドレットは削除され、機能が `Get-AzureRmResourceGroup` に移動されました。

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

**Get-AzureRmRoleDefinition**
- `AtScopeAndBelow` パラメーターが削除されました。

```powershell

# Old
Get-AzureRmRoleDefinition [other required parameters] -AtScopeAndBelow

# New
Get-AzureRmRoleDefinition [other required parameters]
```

## <a name="breaking-changes-to-azurermstorage-cmdlets"></a>AzureRM.Storage コマンドレットの重大な変更

**New-AzureRmStorageAccount**
- `EnableEncryptionService` パラメーターが削除されました。

**Set-AzureRmStorageAccount**
- `EnableEncryptionService` パラメーターと `DisableEncryptionService` パラメーターが削除されました。

## <a name="removed-modules"></a>削除されたモジュール

### `AzureRM.ServerManagement`

Server Management Tools サービスが[昨年廃止](https://blogs.technet.microsoft.com/servermanagement/2017/05/17/smt-preview-service-is-being-retired-on-june-30-2017/)されました。これにより、SMT の対応するモジュール `AzureRM.ServerManagement` が `AzureRM` から削除され、今後は出荷されなくなります。

### `AzureRM.SiteRecovery`

`AzureRM.SiteRecovery` モジュールは `AzureRM.RecoveryServices.SiteRecovery` に置き換えられます。これは、`AzureRM.SiteRecovery` モジュールの機能的なスーパーセットであり、一連の新しい同等のコマンドレットが含まれます。 古いコマンドレットから新しいコマンドレットへのマッピングの一覧を次に示します。

| 非推奨のコマンドレット                                        | 同等のコマンドレット                                                | エイリアス                                  |
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
