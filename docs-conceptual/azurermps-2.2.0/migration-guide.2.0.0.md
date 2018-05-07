# <a name="table-of-contents"></a>目次
1. [Force パラメーターの削除](#removal-of-force-parameters)
2. [Tag パラメーターの変更](#change-of-tag-parameters)
3. [Storage コマンドレットの重大な変更](#breaking-changes-to-storage-cmdlets)
4. [AD コマンドレットの重大な変更](#breaking-changes-to-ad-cmdlets)

## <a name="removal-of-force-parameters"></a>Force パラメーターの削除

このリリースでは、コマンドレットから古い `Force` パラメーターがすべて削除されました。また、将来のリリースでこのパラメーターが削除されることを示す対応する警告も削除されました。

この変更の影響を受けるコマンドレットは次のとおりです。

**ApiManagement**
- Remove-AzureRmApiManagement
- Remove-AzureRmApiManagementApi
- Remove-AzureRmApiManagementGroup
- Remove-AzureRmApiManagementLogger
- Remove-AzureRmApiManagementOpenIdConnectProvider
- Remove-AzureRmApiManagementOperation
- Remove-AzureRmApiManagementPolicy
- Remove-AzureRmApiManagementProduct
- Remove-AzureRmApiManagementProperty
- Remove-AzureRmApiManagementSubscription
- Remove-AzureRmApiManagementUser

**Automation**
- Remove-AzureRmAutomationCertificate
- Remove-AzureRmAutomationCredential
- Remove-AzureRmAutomationVariable
- Remove-AzureRmAutomationWebhook

**Batch**
- Remove-AzureBatchCertificate
- Remove-AzureBatchComputeNode
- Remove-AzureBatchComputeNodeUser

**DataFactories**
- Resume-AzureRmDataFactoryPipeline
- Set-AzureRmDataFactoryPipelineActivePeriod
- Suspend-AzureRmDataFactoryPipeline

**DataLakeStore**
- Remove-AzureRmDataLakeStoreItemAclEntry
- Set-AzureRmDataLakeStoreItemAcl
- Set-AzureRmDataLakeStoreItemAclEntry
- Set-AzureRmDataLakeStoreItemOwner

**OperationalInsights**
- Remove-AzureRmOperationalInsightsSavedSearch

**プロファイル**
- Remove-AzureRmEnvironment

**RedisCache**
- Remove-AzureRmRedisCacheDiagnostics

**リソース**
- Register-AzureRmProviderFeature
- Register-AzureRmResourceProvider
- Remove-AzureRmADServicePrincipal
- Remove-AzureRmPolicyAssignment
- Remove-AzureRmResourceGroupDeployment
- Remove-AzureRmRoleAssignment
- Stop-AzureRmResourceGroupDeployment
- Unregister-AzureRmResourceProvider

**Storage**
- Remove-AzureStorageContainerStoredAccessPolicy
- Remove-AzureStorageQueueStoredAccessPolicy
- Remove-AzureStorageShareStoredAccessPolicy
- Remove-AzureStorageTableStoredAccessPolicy

**StreamAnalytics**
- Remove-AzureRmStreamAnalyticsFunction
- Remove-AzureRmStreamAnalyticsInput
- Remove-AzureRmStreamAnalyticsJob
- Remove-AzureRmStreamAnalyticsOutput

**Tag**
- Remove-AzureRmTag

<br>

上記のコマンドレットのいずれかを使用するスクリプトがある場合は、`Force` パラメーターを削除するだけで重大な変更に対処できます。

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location -Force

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location $location
```

<br>

## <a name="change-of-tag-parameters"></a>Tag パラメーターの変更

このリリースでは、`Tags` パラメーターの名前が `Tag` に変更されました。また、型が `Hashtable[]` から `Hashtable` に変更され、キーと値のペアの形式が変更されました。

これまで、`Hashtable[]` 内の各エントリは 1 つのキーと値のペアを表していました。

```powershell
$tags = @{ Name = "test1"; Value = "testval1" }, @{ Name = "test2", Value = "testval2" }
$tags[0].Name  # Key for the first entry, "test1"
$tags[0].Value # Value for the first entry, "testval1"
$tags[1].Name  # Key for the second entry, "test2"
$tags[1].Value # Value for the second entry, "testval2"
```

現在、`Name` と `Value` が不要になり、`Hashtable` で `Key = "Value"` を割り当てることで、キーと値のペアを作成できます。

```powershell
$tag = @{ test1 = "testval1"; test2 = "testval2" }
$tag["test1"] # Gets the value associated with the key "test1"
$tag["test2"] # Gets the value associated with the key "test2"
```

この変更の影響を受けるコマンドレットは次のとおりです。

**Batch**
- Get-AzureRmBatchAccount
- New-AzureRmBatchAccount
- Set-AzureRmBatchAccount

**Compute**
- New-AzureRmVM
- Update-AzureRmVM

**DataLakeAnalytics**
- New-AzureRmDataLakeAnalyticsAccount
- Set-AzureRmDataLakeAnalyticsAccount

**DataLakeStore**
- New-AzureRmDataLakeStoreAccount
- Set-AzureRmDataLakeStoreAccount

**Dns**
- New-AzureRmDnsZone
- Set-AzureRmDnsZone

**KeyVault**
- Get-AzureRmKeyVault
- New-AzureRmKeyVault

**ネットワーク**
- New-AzureRmApplicationGateway
- New-AzureRmExpressRouteCircuit
- New-AzureRmLoadBalancer
- New-AzureRmLocalNetworkGateway
- New-AzureRmNetworkInterface
- New-AzureRmNetworkSecurityGroup
- New-AzureRmPublicIpAddress
- New-AzureRmRouteTable
- New-AzureRmVirtualNetwork
- New-AzureRmVirtualNetworkGateway
- New-AzureRmVirtualNetworkGatewayConnection
- New-AzureRmVirtualNetworkPeering

**リソース**
- Find-AzureRmResource
- Find-AzureRmResourceGroup
- New-AzureRmResource
- New-AzureRmResourceGroup
- Set-AzureRmResource
- Set-AzureRmResourceGroup

**SQL**
- New-AzureRmSqlDatabase
- New-AzureRmSqlDatabaseCopy
- New-AzureRmSqlDatabaseSecondary
- New-AzureRmSqlElasticPool
- New-AzureRmSqlServer
- Set-AzureRmSqlDatabase
- Set-AzureRmSqlElasticPool
- Set-AzureRmSqlServer

**Storage**
- New-AzureRmStorageAccount
- Set-AzureRmStorageAccount

**TrafficManager**
- New-AzureRmTrafficManagerProfile

<br>

上記のコマンドレットのいずれかを使用するスクリプトがある場合は、`Tags` パラメーターを `Tag` に変更し、`Tag` を新しい形式に変更することで、重大な変更に対処できます。

```powershell
# Old
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tags @{ Name = "testtag"; Value = "testval" }

# New
New-AzureRmResourceGroup -Name $resourceGroupName -Location -location -Tag @{ testtag = "testval" }
```

<br>

## <a name="breaking-changes-to-storage-cmdlets"></a>Storage コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。

**Get-AzureRmStorageAccountKey**
- このコマンドレットは、各キーのプロパティを含むオブジェクトではなく、キーのリストを返すようになりました。

```powershell
# Old
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Key1

# New
$key = (Get-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName)[0].Value
```

**New-AzureRmStorageAccountKey**
- このコマンドレットの出力の `StorageAccountRegenerateKeyResponse` フィールドの名前が `StorageAccountListKeysResults` に変更され、各キーのプロパティを含むオブジェクトではなく、キーのリストになりました。

```powershell
# Old
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).StorageAccountKeys.Key1

# New
$key = (New-AzureRmStorageAccountKey -ResourceGroupName $resourceGroupName -Name $accountName).Keys[0].Value
```

**New/Get/Set-AzureRmStorageAccount**
- このコマンドレットの出力の `AccountType` フィールドの名前が `Sku.Name` に変更されました。
- PrimaryEndpoints/Secondary endpoints blob/table/queue/file の出力の型が `Uri` から `String` に変更されました。

```powershell
# Old
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).AccountType

# New
$accountType = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).Sku.Name
```

```powershell
# Old 
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.AbsolutePath

# New
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob.ToString()
$blobEndpoint = (Get-AzureRmStorageAccount -ResourceGroupName $resourceGroupName -Name $accountName).PrimaryEndpoints.Blob
```

<br>

## <a name="breaking-changes-to-ad-cmdlets"></a>AD コマンドレットの重大な変更

このリリースで影響を受けたコマンドレットは次のとおりです。

**Get-AzureRMADServicePrincipal**
- このコマンドレットの出力の `ServicePrincipalName` フィールドの名前が `ServicePrincipalNames` に変更され、コレクションになりました。 identifierUri に加え、SPN の 1 つとして `ApplicationId` も表示されるようになりました。

```powershell
# Old
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalName

# New
$servicePrincipals = Get-AzureRmADServicePrincipal -SearchString $displayName
$spn = $servicePrincipals[0].ServicePrincipalNames[0]
```

**Get-AzureRmADApplication**
- `ApplicationObjectId` パラメーターの名前が `ObjectId` に変更されました。
- このコマンドレットの出力の `ApplicationObjectId` の名前が `ObjectId` に変更されました。

```powershell
# Old
$app = Get-AzureRmADApplication -ApplicationObjectId $applicationObjectId
$objectId = $app.ApplicationObjectId

# New
$app = Get-AzureRmADApplication -ObjectId $objectId
$objectId = $app.ObjectId
```

**Remove-AzureRmADApplication**
- `ApplicationObjectId` パラメーターの名前が `ObjectId` に変更されました。

```powershell
# Old
$app = Remove-AzureRmADApplication -ApplicationObjectId $applicationObjectId -Force

# New
$app = Remove-AzureRmADApplication -ObjectId $objectId -Force
```

**New-AzureRmADApplication**
- このコマンドレットの出力の `ApplicationObjectId` の名前が `ObjectId` に変更されました。
- `KeyValue`、`KeyUsage`、`KeyType` の各パラメーターが削除されました。

```powershell
# Old
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris -KeyValue $kv -KeyType $kt -KeyUsage $ku
$id = $app.ApplicationObjectId

# New
$app = New-AzureRmADApplication -DisplayName $displayName -HomePage $homePage -IdentifierUris $identifierUris
$id = $app.ObjectId
New-AzureRmADAppCredential -ObjectId $id -Password $kv
```

**Get-AzureRmADGroup**
- 出力から `Mail` フィールドが削除されました。

**Get-AzureRmADUser**
- 出力から `Mail` フィールドが削除されました。

**New-AzureRmADServicePrincipal**
- `DisableAccount` パラメーターが削除されました。

```powershell
# Old
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password -DisableAccount true

# New
$servicePrincipal = New-AzureRmADServicePrincipal -DisplayName $displayName -Password $password
Remove-AzureRmADServicePrincipal -ObjectId $servicePrincipal.ObjectId
```