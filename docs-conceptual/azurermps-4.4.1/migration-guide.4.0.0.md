---
title: Microsoft Azure PowerShell 4.0.0 の重大な変更
description: この移行ガイドには、バージョン 4 リリースの Azure PowerShell で行われた重大な変更が記載されています。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/01/2018
ms.openlocfilehash: 2f61e41b701dfc263df18064f6ac2cc4c6e4021e
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "67863548"
---
# <a name="breaking-changes-for-microsoft-azure-powershell-400"></a>Microsoft Azure PowerShell 4.0.0 の重大な変更

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。 各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。 詳細なコンテキストについては、各変更に関する pull request を参照してください。

## <a name="table-of-contents"></a>目次

- [Compute コマンドレットの重大な変更](#breaking-changes-to-compute-cmdlets)
- [EventHub コマンドレットの重大な変更](#breaking-changes-to-eventhub-cmdlets)
- [Insights コマンドレットの重大な変更](#breaking-changes-to-insights-cmdlets)
- [Network コマンドレットの重大な変更](#breaking-changes-to-network-cmdlets)
- [ServiceBus コマンドレットの重大な変更](#breaking-changes-to-servicebus-cmdlets)
- [Sql コマンドレットの重大な変更](#breaking-changes-to-sql-cmdlets)
- [Storage コマンドレットの重大な変更](#breaking-changes-to-storage-cmdlets)
- [Profile コマンドレットの重大な変更](#breaking-changes-to-profile-cmdlets)
  ## <a name="breaking-changes-to-compute-cmdlets"></a>Compute コマンドレットの重大な変更

このリリースで影響を受けた出力の型は次のとおりです。

### <a name="psvirtualmachine"></a>PSVirtualMachine
- `PSVirtualMachine` オブジェクトの最上位レベルのプロパティ `DataDiskNames` と `NetworkInterfaceIDs` が出力の型から削除されました。 これらのプロパティは、`PSVirtualMachine` オブジェクトの `StorageProfile` プロパティと `NetworkProfile` プロパティで常に使用できましたが、今後はアクセスすることが必要になります。
- この変更は次のコマンドレットに影響します。
    - `Add-AzureRmVMDataDisk`
    - `Add-AzureRmVMNetworkInterface`
    - `Get-AzureRmVM`
    - `Remove-AzureRmVMDataDisk`
    - `Remove-AzureRmVMNetworkInterface`
    - `Set-AzureRmVMDataDisk`

```powershell-interactive
# Old
$vm.DataDiskNames
$vm.NetworkInterfaceIDs

# New
$vm.StorageProfile.DataDisks | Select -Property Name
$vm.NetworkProfile.NetworkInterfaces | Select -Property Id
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a>EventHub コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。

### <a name="get-azurermeventhubnamespace"></a>Get-AzureRmEventHubNamespace
- 出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。

### <a name="new-azurermeventhubnamespace"></a>New-AzureRmEventHubNamespace
- 出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。

## <a name="breaking-changes-to-insights-cmdlets"></a>Insights コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。
    
### <a name="get-azurermusage"></a>Get-AzureRmUsage
- このコマンドレットは非推奨になりました。

### <a name="remove-azurermalertrule"></a>Remove-AzureRmAlertRule
- このコマンドレットの出力が、単一のオブジェクトを含むリストから単一のオブジェクトに変更されました。このオブジェクトには、requestId と状態コードが含まれます。
    
```powershell-interactive
# Old  
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name chiricutin
if ($s1 -ne $null)
{
    $r = $s1(0).RequestId
    $s = $s1(0).StatusCode
}

# New
$s1 = Remove-AzureRmAlertRule -ResourceGroup $resourceGroup -name chiricutin
$r = $s1.RequestId
$s = $s1.StatusCode
```
    
### <a name="add-azurermlogalertrule"></a>Add-AzureRmLogAlertRule
- このコマンドレットは非推奨になりました。
    
### <a name="get-azurermalertrule"></a>Get-AzureRmAlertRule
- このコマンドレットの出力 (オブジェクトのリスト) の各要素がフラット化されます。つまり、構造体 `{ Id, Location, Name, Tags, Properties }` を持つオブジェクトを返す代わりに、構造体 `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}` を持つオブジェクトを返します。この構造体は、Azure リソースのすべての属性と、最上位レベルの AlertRuleResource のすべての属性です。
    
```powershell-interactive
# Old
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -fore red "Error updating alert rule"
      
    Write-Host $rules(0).Id
    Write-Host $rules(0).Properties.IsEnabled
    Write-Host $rules(0).Properties.Condition
}

# New
$rules = Get-AzureRmAlertRule -ResourceGroup $resourceGroup
if ($rules -and $rules.count -ge 1)
{
    Write-Host -fore red "Error updating alert rule"
 
    Write-Host $rules(0).Id
      
    # Properties will remain for a while
    Write-Host $rules(0).Properties.IsEnabled
      
    # But the properties will be at the top level too. Later Properties will be removed
    Write-Host $rules(0).IsEnabled
    Write-Host $rules(0).Condition
}
```
    
### <a name="get-azurermautoscalesetting"></a>Get-AzureRmAutoscaleSetting
- `AutoscaleSettingResourceName` フィールドには `Name` フィールドと常に同じ値が含まれるため、非推奨となりました。

```powershell-interactive
# Old  
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
if ($s1.AutoscaleSettingResourceName -ne $s1.Name)
{
    Write-Host "There is something wrong with the name"
}

# New
$s1 = Get-AzureRmAutoscaleSetting -ResourceGroup $resourceGroup -Name MySetting
    
# There won't be a AutoscaleSettingResourceName
Write-Host $s1.Name
```
    
### <a name="remove-azurermlogprofile"></a>Remove-AzureRmLogProfile
- このコマンドレットの出力が、`Boolean` から、`RequestId` と `StatusCode` を含むオブジェクトに変更されます。

```powershell-interactive
# Old  
$s1 = Remove-AzureRmLogProfile -Name myLogProfile
if ($s1 -eq $true)
{
    Write-Host "Removed"
}
else
{
    Write-Host "Failed"
}

# New
$s1 = Remove-AzureRmLogProfile -Name myLogProfile
$r = $s1.RequestId
$s = $s1.StatusCode
```
    
### <a name="add-azurermlogprofile"></a>Add-AzureRmLogProfile
- このコマンドレットの出力が、requestId、状態コード、更新されたリソースまたは新しく作成されたリソースを含むオブジェクトに変更されます。
    
```powershell-interactive
# Old  
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.ServiceBusRuleId

# New
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.RequestId
$s = $s1.StatusCode
$a = $s1.NewResource.ServiceBusRuleId
    
```
    
### <a name="set-azurermdiagnosticsettings"></a>Set-AzureRmDiagnosticSettings
- このコマンドの名前が `Update-AzureRmDiagnosticSettings` に変更されます。

```powershell-interactive
# Old
Set-AzureRmDiagnosticSettings

# New
Update-AzureRmDiagnosticSettings
```

## <a name="breaking-changes-to-network-cmdlets"></a>Network コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。

### <a name="new-azurermvirtualnetworkgatewayconnection"></a>New-AzureRmVirtualNetworkGatewayConnection
- `EnableBgp` パラメーターが、`string` ではなく `boolean` を受け取るように変更されました。

```powershell-interactive
# Old
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp "true"

# New
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp $true
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a>ServiceBus コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。

### <a name="get-azurermservicebusnamespace"></a>Get-AzureRmServiceBusNamespace
- 出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。

### <a name="new-azurermservicebusnamespace"></a>New-AzureRmServiceBusNamespace

- 出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。

## <a name="breaking-changes-to-sql-cmdlets"></a>Sql コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。

### <a name="new-azurermsqldatabasefailovergroup"></a>New-AzureRmSqlDatabaseFailoverGroup
- `Tag` パラメーターが削除されました。
- `GracePeriodWithDataLossHour` パラメーターの名前が `GracePeriodWithDataLossHours` に変更されました。

```powershell-interactive
# Old
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="set-azurermsqldatabasefailovergroup"></a>Set-AzureRmSqlDatabaseFailoverGroup
- `Tag` パラメーターが削除されました。
- `GracePeriodWithDataLossHour` パラメーターの名前が `GracePeriodWithDataLossHours` に変更されました。

```powershell-interactive
# Old
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="add-azurermsqldatabasetofailovergroup"></a>Add-AzureRmSqlDatabaseToFailoverGroup
- `Tag` パラメーターが削除されました。

```powershell-interactive
# Old
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

###  <a name="remove-azurermsqldatabasefromfailovergroup"></a>Remove-AzureRmSqlDatabaseFromFailoverGroup
- `Tag` パラメーターが削除されました。

```powershell-interactive
# Old
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

### <a name="remove-azurermsqldatabasefailovergroup"></a>Remove-AzureRmSqlDatabaseFailoverGroup
- `PartnerResourceGroupName` パラメーターが削除されました。
- `PartnerServerName` パラメーターが削除されました。

```powershell-interactive
# Old
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -PartnerResourceGroupName rg

# New
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg
```

### <a name="set-azurermsqldatabasethreatdetectionpolicy"></a>Set-AzureRmSqlDatabaseThreatDetectionPolicy
- `ExcludedDetectionType` パラメーターで値 `Usage_Anomaly` が無効になりました。

### <a name="set-azurermsqlserverthreatdetectionpolicy"></a>Set-AzureRmSqlServerThreatDetectionPolicy
- `ExcludedDetectionType` パラメーターで値 `Usage_Anomaly` が無効になりました。

## <a name="breaking-changes-to-storage-cmdlets"></a>Storage コマンドレットの重大な変更

このリリースで影響を受けた出力の型プロパティは次のとおりです。

### <a name="azurestorageblobicloudblobserviceclient"></a>AzureStorageBlob.ICloudBlob.ServiceClient
- 次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- この変更は次のコマンドレットに影響します。
    - `Get-AzureStorageBlob`
    - `Get-AzureStorageBlobContent`
    - `Get-AzureStorageBlobCopyState`
    - `Set-AzureStorageBlobContent`
    - `Start-AzureStorageBlobCopy`
    - `Stop-AzureStorageBlobCopy`
    
### <a name="azurestoragecontainercloudblobcontainerserviceclient"></a>AzureStorageContainer.CloudBlobContainer.ServiceClient
- 次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- この変更は次のコマンドレットに影響します。
    - `Get-AzureStorageContainer`
    - `New-AzureStorageContainer`
    - `Set-AzureStorageContainerAcl`
    
### <a name="azurestoragequeuecloudqueueserviceclient"></a>AzureStorageQueue.CloudQueue.ServiceClient
- 次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。
    - `LocationMode`
    - `MaximumExecutionTime`
    - `RetryPolicy`
    - `ServerTimeout`
- この変更は次のコマンドレットに影響します。
    - `Get-AzureStorageQueue`
    - `New-AzureStorageQueue`
    
### <a name="azurestoragetablecloudtableserviceclient"></a>AzureStorageTable.CloudTable.ServiceClient
- 次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。
    - `LocationMode`
    - `MaximumExecutionTime`
    - `PayloadFormat`
    - `RetryPolicy`
    - `ServerTimeout`
- この変更は次のコマンドレットに影響します。
    - `Get-AzureStorageTable`
    - `New-AzureStorageTable`
    
```powershell-interactive
# Old
$LocationMode = (Get-AzureStorageBlob -Container $containername)[0].ICloudBlob.ServiceClient.LocationMode       
$ParallelOperationThreadCount = (Get-AzureStorageContainer -Container $containername).CloudBlobContainer.ServiceClient.ParallelOperationThreadCount
$PayloadFormat = (Get-AzureStorageTable -Name $tablename).CloudTable.ServiceClient.PayloadFormat
$RetryPolicy = (Get-AzureStorageQueue -Name $queuename).CloudQueue.ServiceClient.RetryPolicy

# New
$LocationMode = (Get-AzureStorageBlob -Container $containername)[0].ICloudBlob.ServiceClient.DefaultRequestOptions.LocationMode     
$ParallelOperationThreadCount = (Get-AzureStorageContainer -Container $containername).CloudBlobContainer.ServiceClient.DefaultRequestOptions.ParallelOperationThreadCount
$PayloadFormat = (Get-AzureStorageTable -Name $tablename).CloudTable.ServiceClient.DefaultRequestOptions.PayloadFormat
$RetryPolicy = (Get-AzureStorageQueue -Name $queuename).CloudQueue.ServiceClient.DefaultRequestOptions.RetryPolicy
```

## <a name="breaking-changes-to-profile-cmdlets"></a>Profile コマンドレットの重大な変更

次のコマンドレットとコマンドレットの出力の型が、このリリースで変更されました。

### <a name="add-azurermaccount-breaking-changes"></a>Add-AzureRmAccount の重大な変更

- ```EnvironmentName``` パラメーターが削除され、```Environment``` に置き換えられました。```Environment``` は、```AzureEnvironment``` オブジェクトではなく文字列を受け取ります。

```powershell-interactive
# Old
Add-AzureRmAccount -EnvironmentName AzureChinaCloud

# New
Add-AzureRmAccount -Environment AzureChinaCloud
```

### <a name="select-azurermprofile-was-renamed-to-import-azurermcontext"></a>Select-AzureRmProfile の名前を Import-AzureRmContext に変更

```Select-AzureRmProfile``` の名前が ```Import-AzureRmContext``` に変更されました。

```powershell-interactive
# Old
Select-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Import-AzureRmContext -Path c:\mydir\myprofile.json
```

### <a name="save-azurermprofile-was-renamed-to-save-azurermcontext"></a>Save-AzureRmProfile の名前を Save-AzureRmContext に変更

```Save-AzureRmProfile``` の名前が ```Save-AzureRmContext``` に変更されました。

```powershell-interactive
# Old
Save-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Save-AzureRmContext -Path c:\mydir\myprofile.json
```
### <a name="breaking-changes-to-output-psazurecontext-type"></a>出力の PSAzureContext 型の重大な変更

- ```TokenCache``` プロパティが、```byte[]``` ではなく ```IAzureTokenCache``` を実装する型に変更されました。

```powershell-interactive
# Old
$bytes = (Get-AzureRmContext).TokenCache
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache
$bytes = (Add-AzureRmAccount).Context.TokenCache

# New
$bytes = (Get-AzureRmContext).TokenCache.CacheData
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache.CacheData
$bytes = (Add-AzureRmAccount).Context.TokenCache.CacheData
```

### <a name="breaking-changes-to-the-output-psazureaccount-type"></a>出力の PSAzureAccount 型の重大な変更

- ```AccountType``` プロパティが ```Type``` に変更されました。

```powershell-interactive
# Old
$type = (Get-AzureRmContext).Account.AccountType
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.AccountType
$type = (Add-AzureRmAccount).Context.Account.AccountType

# New 
$type = (Get-AzureRmContext).Account.Type
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.Type
$type = (Add-AzureRmAccount).Context.Account.Type
```

### <a name="breaking-changes-to-the-output-psazuresubscription-type"></a>出力の PSAzureSubscription 型の重大な変更
- ```SubscriptionId``` プロパティが ```Id``` に変更されました。

```powershell-interactive
# Old
$id =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).SubscriptionId
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.SubscriptionId
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionId
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionId

# New
$id =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).Id
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.Id
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Id
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Id
```

- ```SubscriptionName``` プロパティが ```Name``` に変更されました。

```powershell-interactive
# Old
$name =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).SubscriptionName
$name =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.SubscriptionName
$name =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionName
$name =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.SubscriptionName

# New
$name =(Get-AzureRmSubscription -SubscriptionId xxxx-xxxx-xxxx-xxxx).Name
$name =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Subscription.Name
$name =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Name
$name =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Subscription.Name
```

### <a name="breaking-changes-to-the-output-psazuretenant-type"></a>出力の PSAzureTenant 型の重大な変更

- ```TenantId``` プロパティが ```Id``` に変更されました。

```powershell-interactive
# Old
$id =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).TenantId
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Tenant.TenantId
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.TenantId
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.TenantId

# New
$id =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Id
$id =(Add-AzureRmAccount -SubscriptionId xxxx-xxxx-xxxx-xxxx).Context.Tenant.Id
$id =(Get-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.Id
$id =(Set-AzureRmContext -SubscriptionId xxxx-xxxx-xxxx-xxxx).Tenant.Id
```

- ```Domain``` プロパティが ```Directory``` に変更されました。

```powershell-interactive
# Old
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Domain

# New
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Directory
```
