# <a name="breaking-changes-for-microsoft-azure-powershell-300"></a>Microsoft Azure PowerShell 3.0.0 の重大な変更

このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。  各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。  詳細なコンテキストについては、各変更に関するプル要求を参照してください。

## <a name="table-of-contents"></a>目次
1. [Data Lake Store コマンドレットの重大な変更](#breaking-changes-to-data-lake-store-cmdlets)
2. [ApiManagement コマンドレットの重大な変更](#breaking-changes-to-apimanagement-cmdlets)
3. [Network コマンドレットの重大な変更](#breaking-changes-to-network-cmdlets)

## <a name="breaking-changes-to-data-lake-store-cmdlets"></a>Data Lake Store コマンドレットの重大な変更

このリリース ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)) で影響を受けたコマンドレットは次のとおりです。

**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**
- このコマンドレットが削除され、``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)`` に置き換えられました。
- 古いコマンドレットは、アクセス制御リスト (ACL) を表す複雑なオブジェクトを返していました。 新しいコマンドレットは、選択したパスの ACL のエントリの単純なリストを返します。

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**
- このコマンドレットは、以前の ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)`` コマンドレットに代わるものです。
- この新しいコマンドレットは、選択したパスの ACL のエントリの単純なリスト (``DataLakeStoreItemAce[]`` 型) を返します。
- このコマンドレットの出力は、次のコマンドレットの ``-Acl`` パラメーターに渡すことができます。
   - ``Remove-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAclEntry``

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**、**Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**、**Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**
- これらのコマンドレットは、``-Acl`` パラメーターの ``DataLakeStoreItemAce[]`` を受け入れるようになりました。
- ``DataLakeStoreItemAce[]`` は ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)`` から返されます。

```powershell
# Old
$acl = Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $acl

# New
$aclEntries = Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $aclEntries
```

## <a name="breaking-changes-to-apimanagement-cmdlets"></a>ApiManagement コマンドレットの重大な変更

このリリース ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)) で影響を受けたコマンドレットは次のとおりです。

**New-AzureRmApiManagementVirtualNetwork**
- 仮想ネットワークを参照する際の必須パラメーターが、SubnetName と VnetId から、``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}`` 形式の SubnetResourceId に変更されました。

```powershell
# Old
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetName <String> -VnetId <Guid>

# New
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>

```

**Deprecating Cmdlet Set-AzureRmApiManagementVirtualNetworks**
- ApiManagement のデプロイに関連する仮想ネットワークの設定方法が複数あったため、このコマンドレットは使用されなくなります。

```powershell
# Old
$networksList = @()
$networksList += New-AzureRmApiManagementVirtualNetwork -Location $vnetLocation -VnetId $vnetId -SubnetName $subnetName
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $networksList

# New
$masterRegionVirtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>
Update-AzureRmApiManagementDeployment -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetwork $masterRegionVirtualNetwork
```

## <a name="breaking-changes-to-network-cmdlets"></a>Network コマンドレットの重大な変更

このリリース ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)) で影響を受けたコマンドレットは次のとおりです。

**New-AzureRmVirtualNetworkGateway**
- 変更内容の説明: 仮想ネットワーク ゲートウェイの新規作成時にアクティブ/アクティブ機能を有効にするために、``:- Bool parameter:-ActiveActive`` が削除され、``SwitchParameter:-EnableActiveActiveFeature`` が追加されました。

```powershell
# Old 
# Sample of how the cmdlet was previously called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -ActiveActive $true

# New
# Sample of how the cmdlet should now be called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -EnableActiveActiveFeature
```

Set-AzureRmVirtualNetworkGateway
- 変更内容の説明: 仮想ネットワーク ゲートウェイでアクティブ/アクティブ機能を有効または無効にするために、``:- Bool parameter:-ActiveActive`` が削除され、2 つの ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` が追加されました。

```powershell
# Old
# Sample of how the cmdlet was previously called
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -ActiveActive $true
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -ActiveActive $false  

# New
# Sample of how the cmdlet should now be called
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -EnableActiveActiveFeature
Set-AzureRmVirtualNetworkGateway -VirtualNetworkGateway $gw -DisableActiveActiveFeature
```