# <a name="breaking-changes-for-microsoft-azure-powershell-300"></a><span data-ttu-id="f0254-101">Microsoft Azure PowerShell 3.0.0 の重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-101">Breaking changes for Microsoft Azure PowerShell 3.0.0.</span></span>

<span data-ttu-id="f0254-102">このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。</span><span class="sxs-lookup"><span data-stu-id="f0254-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span>  <span data-ttu-id="f0254-103">各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。</span><span class="sxs-lookup"><span data-stu-id="f0254-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span>  <span data-ttu-id="f0254-104">詳細なコンテキストについては、各変更に関するプル要求を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f0254-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="f0254-105">目次</span><span class="sxs-lookup"><span data-stu-id="f0254-105">Table of Contents</span></span>
1. [<span data-ttu-id="f0254-106">Data Lake Store コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-106">Breaking changes to Data Lake Store cmdlets</span></span>](#breaking-changes-to-data-lake-store-cmdlets)
2. [<span data-ttu-id="f0254-107">ApiManagement コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-107">Breaking changes to ApiManagement cmdlets</span></span>](#breaking-changes-to-apimanagement-cmdlets)
3. [<span data-ttu-id="f0254-108">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-108">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)

## <a name="breaking-changes-to-data-lake-store-cmdlets"></a><span data-ttu-id="f0254-109">Data Lake Store コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-109">Breaking changes to Data Lake Store cmdlets</span></span>

<span data-ttu-id="f0254-110">このリリース ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)) で影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f0254-110">The following cmdlets were affected this release ([PR 2965](https://github.com/Azure/azure-powershell/pull/2965)):</span></span>

<span data-ttu-id="f0254-111">**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**</span><span class="sxs-lookup"><span data-stu-id="f0254-111">**Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)**</span></span>
- <span data-ttu-id="f0254-112">このコマンドレットが削除され、``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)`` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="f0254-112">This cmdlet was removed and replaced with ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span></span>
- <span data-ttu-id="f0254-113">古いコマンドレットは、アクセス制御リスト (ACL) を表す複雑なオブジェクトを返していました。</span><span class="sxs-lookup"><span data-stu-id="f0254-113">The old cmdlet returned a complex object representing the access control list (ACL).</span></span> <span data-ttu-id="f0254-114">新しいコマンドレットは、選択したパスの ACL のエントリの単純なリストを返します。</span><span class="sxs-lookup"><span data-stu-id="f0254-114">The new cmdlet returns a simple list of entries in the chosen path's ACL.</span></span>

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

<span data-ttu-id="f0254-115">**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**</span><span class="sxs-lookup"><span data-stu-id="f0254-115">**Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)**</span></span>
- <span data-ttu-id="f0254-116">このコマンドレットは、以前の ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)`` コマンドレットに代わるものです。</span><span class="sxs-lookup"><span data-stu-id="f0254-116">This cmdlet replaces the old cmdlet ``Get-AzureRmDataLakeStoreItemAcl (Get-AdlStoreItemAcl)``.</span></span>
- <span data-ttu-id="f0254-117">この新しいコマンドレットは、選択したパスの ACL のエントリの単純なリスト (``DataLakeStoreItemAce[]`` 型) を返します。</span><span class="sxs-lookup"><span data-stu-id="f0254-117">This new cmdlet returns a simple list of entries in the chosen path's ACL, with type ``DataLakeStoreItemAce[]``.</span></span>
- <span data-ttu-id="f0254-118">このコマンドレットの出力は、次のコマンドレットの ``-Acl`` パラメーターに渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="f0254-118">The output of this cmdlet can be passed in to the ``-Acl`` parameter of the following cmdlets:</span></span>
   - ``Remove-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAcl``
   - ``Set-AzureRmDataLakeStoreItemAclEntry``

```powershell
# Old
Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo

# New
Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
```

<span data-ttu-id="f0254-119">**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**、**Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**、**Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**</span><span class="sxs-lookup"><span data-stu-id="f0254-119">**Remove-AzureRmDataLakeStoreItemAcl (Remove-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAcl (Set-AdlStoreItemAcl)**, **Set-AzureRmDataLakeStoreItemAclEntry (Set-AdlStoreItemAclEntry)**</span></span>
- <span data-ttu-id="f0254-120">これらのコマンドレットは、``-Acl`` パラメーターの ``DataLakeStoreItemAce[]`` を受け入れるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f0254-120">These cmdlets now accept ``DataLakeStoreItemAce[]`` for the ``-Acl`` parameter.</span></span>
- <span data-ttu-id="f0254-121">``DataLakeStoreItemAce[]`` は ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)`` から返されます。</span><span class="sxs-lookup"><span data-stu-id="f0254-121">``DataLakeStoreItemAce[]`` is returned by ``Get-AzureRmDataLakeStoreItemAclEntry (Get-AdlStoreItemAclEntry)``.</span></span>

```powershell
# Old
$acl = Get-AdlStoreItemAcl -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $acl

# New
$aclEntries = Get-AdlStoreItemAclEntry -Account myadlsaccount -Path /foo
Set-AdlStoreItemAcl -Account myadlsaccount -Path /foo -Acl $aclEntries
```

## <a name="breaking-changes-to-apimanagement-cmdlets"></a><span data-ttu-id="f0254-122">ApiManagement コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-122">Breaking changes to ApiManagement cmdlets</span></span>

<span data-ttu-id="f0254-123">このリリース ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)) で影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f0254-123">The following cmdlets were affected this release ([PR 2971](https://github.com/Azure/azure-powershell/pull/2971)):</span></span>

<span data-ttu-id="f0254-124">**New-AzureRmApiManagementVirtualNetwork**</span><span class="sxs-lookup"><span data-stu-id="f0254-124">**New-AzureRmApiManagementVirtualNetwork**</span></span>
- <span data-ttu-id="f0254-125">仮想ネットワークを参照する際の必須パラメーターが、SubnetName と VnetId から、``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}`` 形式の SubnetResourceId に変更されました。</span><span class="sxs-lookup"><span data-stu-id="f0254-125">The required parameters to reference a virtual network changed from requiring SubnetName and VnetId to SubnetResourceId in format ``/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.ClassicNetwork/virtualNetworks/{virtualNetworkName}/subnets/{subnetName}``</span></span>

```powershell
# Old
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetName <String> -VnetId <Guid>

# New
$virtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>

```

<span data-ttu-id="f0254-126">**Deprecating Cmdlet Set-AzureRmApiManagementVirtualNetworks**</span><span class="sxs-lookup"><span data-stu-id="f0254-126">**Deprecating Cmdlet Set-AzureRmApiManagementVirtualNetworks**</span></span>
- <span data-ttu-id="f0254-127">ApiManagement のデプロイに関連する仮想ネットワークの設定方法が複数あったため、このコマンドレットは使用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="f0254-127">The Cmdlet is getting deprecated as there was more than one way to Set Virtual Network associated to ApiManagement deployment.</span></span>

```powershell
# Old
$networksList = @()
$networksList += New-AzureRmApiManagementVirtualNetwork -Location $vnetLocation -VnetId $vnetId -SubnetName $subnetName
Set-AzureRmApiManagementVirtualNetworks -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetworks $networksList

# New
$masterRegionVirtualNetwork = New-AzureRmApiManagementVirtualNetwork -Location <String> -SubnetResourceId <String>
Update-AzureRmApiManagementDeployment -ResourceGroupName "ContosoGroup" -Name "ContosoApi" -VirtualNetwork $masterRegionVirtualNetwork
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="f0254-128">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="f0254-128">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="f0254-129">このリリース ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)) で影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f0254-129">The following cmdlets were affected this release ([PR 2982](https://github.com/Azure/azure-powershell/pull/2982)):</span></span>

<span data-ttu-id="f0254-130">**New-AzureRmVirtualNetworkGateway**</span><span class="sxs-lookup"><span data-stu-id="f0254-130">**New-AzureRmVirtualNetworkGateway**</span></span>
- <span data-ttu-id="f0254-131">変更内容の説明: 仮想ネットワーク ゲートウェイの新規作成時にアクティブ/アクティブ機能を有効にするために、``:- Bool parameter:-ActiveActive`` が削除され、``SwitchParameter:-EnableActiveActiveFeature`` が追加されました。</span><span class="sxs-lookup"><span data-stu-id="f0254-131">Description of what has changed ``:- Bool parameter:-ActiveActive`` is removed and ``SwitchParameter:-EnableActiveActiveFeature`` is added for enabling Active-Active feature on newly creating virtual network gateway.</span></span>

```powershell
# Old 
# Sample of how the cmdlet was previously called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -ActiveActive $true

# New
# Sample of how the cmdlet should now be called
New-AzureRmVirtualNetworkGateway -ResourceGroupName $rgname -name $rname -Location $location -IpConfigurations $vnetIpConfig1,$vnetIpConfig2 -GatewayType Vpn -VpnType RouteBased -EnableBgp $false -GatewaySku HighPerformance -EnableActiveActiveFeature
```

<span data-ttu-id="f0254-132">Set-AzureRmVirtualNetworkGateway</span><span class="sxs-lookup"><span data-stu-id="f0254-132">Set-AzureRmVirtualNetworkGateway</span></span>
- <span data-ttu-id="f0254-133">変更内容の説明: 仮想ネットワーク ゲートウェイでアクティブ/アクティブ機能を有効または無効にするために、``:- Bool parameter:-ActiveActive`` が削除され、2 つの ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` が追加されました。</span><span class="sxs-lookup"><span data-stu-id="f0254-133">Description of what has changed ``:- Bool parameter:-ActiveActive`` is removed and 2 ``SwitchParameters:-EnableActiveActiveFeature`` / ``DisableActiveActiveFeature`` are added for enabling and disabling Active-Active feature on virtual network gateway.</span></span>

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