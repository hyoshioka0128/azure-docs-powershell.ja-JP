# <a name="breaking-changes-for-microsoft-azure-powershell-400"></a><span data-ttu-id="e09e4-101">Microsoft Azure PowerShell 4.0.0 の重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-101">Breaking changes for Microsoft Azure PowerShell 4.0.0</span></span>

<span data-ttu-id="e09e4-102">このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。</span><span class="sxs-lookup"><span data-stu-id="e09e4-102">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="e09e4-103">各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。</span><span class="sxs-lookup"><span data-stu-id="e09e4-103">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="e09e4-104">詳細なコンテキストについては、各変更に関するプル要求を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e09e4-104">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="e09e4-105">目次</span><span class="sxs-lookup"><span data-stu-id="e09e4-105">Table of Contents</span></span>

- [<span data-ttu-id="e09e4-106">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-106">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="e09e4-107">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-107">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="e09e4-108">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-108">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="e09e4-109">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-109">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="e09e4-110">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-110">Breaking changes to ServiceBus cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)
- [<span data-ttu-id="e09e4-111">Sql コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-111">Breaking changes to Sql cmdlets</span></span>](#breaking-changes-to-sql-cmdlets)
- [<span data-ttu-id="e09e4-112">Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-112">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
- [<span data-ttu-id="e09e4-113">Profile コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-113">Breaking Changes to Profile Cmdlets</span></span>](#breaking-changes-to-profile-cmdlets)
## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="e09e4-114">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-114">Breaking changes to Compute cmdlets</span></span>

<span data-ttu-id="e09e4-115">このリリースで影響を受けた出力の型は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-115">The following output types were affected this release:</span></span>

### <a name="psvirtualmachine"></a><span data-ttu-id="e09e4-116">PSVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="e09e4-116">PSVirtualMachine</span></span>
- <span data-ttu-id="e09e4-117">`PSVirtualMachine` オブジェクトの最上位レベルのプロパティ `DataDiskNames` と `NetworkInterfaceIDs` が出力の型から削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-117">Top level properties `DataDiskNames` and `NetworkInterfaceIDs` of nthe `PSVirtualMachine` object have been removed from the output type.</span></span> <span data-ttu-id="e09e4-118">これらのプロパティは、`PSVirtualMachine` オブジェクトの `StorageProfile` プロパティと `NetworkProfile` プロパティで常に使用できましたが、今後はアクセスすることが必要になります。</span><span class="sxs-lookup"><span data-stu-id="e09e4-118">These properties have always been available in the `StorageProfile` and `NetworkProfile` properties of the `PSVirtualMachine` object and will be the way they will need to be accessed going forward.</span></span>
- <span data-ttu-id="e09e4-119">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="e09e4-119">This change affects the following cmdlets:</span></span>
    - `Add-AzureRmVMDataDisk`
    - `Add-AzureRmVMNetworkInterface`
    - `Get-AzureRmVM`
    - `Remove-AzureRmVMDataDisk`
    - `Remove-AzureRmVMNetworkInterface`
    - `Set-AzureRmVMDataDisk`

```powershell
# Old
$vm.DataDiskNames
$vm.NetworkInterfaceIDs

# New
$vm.StorageProfile.DataDisks | Select -Property Name
$vm.NetworkProfile.NetworkInterfaces | Select -Property Id
```

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="e09e4-120">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-120">Breaking changes to EventHub cmdlets</span></span>

<span data-ttu-id="e09e4-121">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-121">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="e09e4-122">Get-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="e09e4-122">Get-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="e09e4-123">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-123">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="e09e4-124">New-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="e09e4-124">New-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="e09e4-125">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-125">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="e09e4-126">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-126">Breaking changes to Insights cmdlets</span></span>

<span data-ttu-id="e09e4-127">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-127">The following cmdlets were affected this release:</span></span>
    
### <a name="get-azurermusage"></a><span data-ttu-id="e09e4-128">Get-AzureRmUsage</span><span class="sxs-lookup"><span data-stu-id="e09e4-128">Get-AzureRmUsage</span></span>
- <span data-ttu-id="e09e4-129">このコマンドレットは非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-129">This cmdlet has been deprecated.</span></span>

### <a name="remove-azurermalertrule"></a><span data-ttu-id="e09e4-130">Remove-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="e09e4-130">Remove-AzureRmAlertRule</span></span>
- <span data-ttu-id="e09e4-131">このコマンドレットの出力が、単一のオブジェクトを含むリストから単一のオブジェクトに変更されました。このオブジェクトには、requestId と状態コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e09e4-131">The output of this cmdlet has changed from a list with a single object to a single object; this object includes the requestId, and status code.</span></span>
    
```powershell
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
    
### <a name="add-azurermlogalertrule"></a><span data-ttu-id="e09e4-132">Add-AzureRmLogAlertRule</span><span class="sxs-lookup"><span data-stu-id="e09e4-132">Add-AzureRmLogAlertRule</span></span>
- <span data-ttu-id="e09e4-133">このコマンドレットは非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-133">This cmdlet has been deprecated.</span></span>
    
### <a name="get-azurermalertrule"></a><span data-ttu-id="e09e4-134">Get-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="e09e4-134">Get-AzureRmAlertRule</span></span>
- <span data-ttu-id="e09e4-135">このコマンドレットの出力 (オブジェクトのリスト) の各要素がフラット化されます。つまり、構造体 `{ Id, Location, Name, Tags, Properties }` を持つオブジェクトを返す代わりに、構造体 `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}` を持つオブジェクトを返します。この構造体は、Azure リソースのすべての属性と、最上位レベルの AlertRuleResource のすべての属性です。</span><span class="sxs-lookup"><span data-stu-id="e09e4-135">Each element of the the output (a list of objects) of this cmdlet is flattened, i.e. instead of returning objects with the structure `{ Id, Location, Name, Tags, Properties }` it will return objects with the structure `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, which is all of the attributes of an Azure Resource plus all of the attributes of an AlertRuleResource at the top level.</span></span>
    
```powershell
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
    
### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="e09e4-136">Get-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="e09e4-136">Get-AzureRmAutoscaleSetting</span></span>
- <span data-ttu-id="e09e4-137">`AutoscaleSettingResourceName`&gt; フィールドには `Name` フィールドと常に同じ値が含まれるため、非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-137">The `AutoscaleSettingResourceName` field is deprecated since it always has the same value as the `Name` field.</span></span>

```powershell
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
    
### <a name="remove-azurermlogprofile"></a><span data-ttu-id="e09e4-138">Remove-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="e09e4-138">Remove-AzureRmLogProfile</span></span>
- <span data-ttu-id="e09e4-139">このコマンドレットの出力が、`Boolean` から、`RequestId` と `StatusCode` を含むオブジェクトに変更されます。</span><span class="sxs-lookup"><span data-stu-id="e09e4-139">The output of this cmdlet will change from `Boolean` to and object containing `RequestId` and `StatusCode`</span></span>

```powershell
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
    
### <a name="add-azurermlogprofile"></a><span data-ttu-id="e09e4-140">Add-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="e09e4-140">Add-AzureRmLogProfile</span></span>
- <span data-ttu-id="e09e4-141">このコマンドレットの出力が、requestId、状態コード、更新されたリソースまたは新しく作成されたリソースを含むオブジェクトに変更されます。</span><span class="sxs-lookup"><span data-stu-id="e09e4-141">The output of this cmdlet will change from an object that includes the requestId, status code, and the updated or newly created resource</span></span>
    
```powershell
# Old  
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.ServiceBusRuleId

# New
$s1 = Add-AzureRmLogProfile -Name default -StorageAccountId /subscriptions/df602c9c-7aa0-407d-a6fb-eb20c8bd1192/resourceGroups/JohnKemTest/providers/Microsoft.Storage/storageAccounts/johnkemtest8162 -Locations Global -categ Delete, Write, Action -retention 3
$r = $s1.RequestId
$s = $s1.StatusCode
$a = $s1.NewResource.ServiceBusRuleId
    
```
    
### <a name="set-azurermdiagnosticsettings"></a><span data-ttu-id="e09e4-142">Set-AzureRmDiagnosticSettings</span><span class="sxs-lookup"><span data-stu-id="e09e4-142">Set-AzureRmDiagnosticSettings</span></span>
- <span data-ttu-id="e09e4-143">このコマンドの名前が `Update-AzureRmDiagnsoticSettings` に変更されます。</span><span class="sxs-lookup"><span data-stu-id="e09e4-143">The command is going to be renamed to `Update-AzureRmDiagnsoticSettings`</span></span>

```powershell
# Old
Set-AzureRmDiagnosticSettings

# New
Update-AzureRmDiagnosticSettings
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="e09e4-144">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-144">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="e09e4-145">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-145">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermvirtualnetworkgatewayconnection"></a><span data-ttu-id="e09e4-146">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="e09e4-146">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="e09e4-147">`EnableBgp` パラメーターが、`string` ではなく `boolean` を受け取るように変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-147">`EnableBgp` parameter has been changed to take a `boolean` instead of a `string`</span></span>

```powershell
# Old
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp "true"

# New
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp $true
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="e09e4-148">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-148">Breaking changes to ServiceBus cmdlets</span></span>

<span data-ttu-id="e09e4-149">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-149">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermservicebusnamespace"></a><span data-ttu-id="e09e4-150">Get-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="e09e4-150">Get-AzureRmServiceBusNamespace</span></span>
- <span data-ttu-id="e09e4-151">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-151">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermservicebusnamespace"></a><span data-ttu-id="e09e4-152">New-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="e09e4-152">New-AzureRmServiceBusNamespace</span></span>

- <span data-ttu-id="e09e4-153">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-153">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-sql-cmdlets"></a><span data-ttu-id="e09e4-154">Sql コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-154">Breaking changes to Sql cmdlets</span></span>

<span data-ttu-id="e09e4-155">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-155">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermsqldatabasefailovergroup"></a><span data-ttu-id="e09e4-156">New-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="e09e4-156">New-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="e09e4-157">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-157">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="e09e4-158">`GracePeriodWithDataLossHour` パラメーターの名前が `GracePeriodWithDataLossHours` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-158">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell
# Old
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="set-azurermsqldatabasefailovergroup"></a><span data-ttu-id="e09e4-159">Set-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="e09e4-159">Set-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="e09e4-160">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-160">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="e09e4-161">`GracePeriodWithDataLossHour` パラメーターの名前が `GracePeriodWithDataLossHours` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-161">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell
# Old
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="add-azurermsqldatabasetofailovergroup"></a><span data-ttu-id="e09e4-162">Add-AzureRmSqlDatabaseToFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="e09e4-162">Add-AzureRmSqlDatabaseToFailoverGroup</span></span>
- <span data-ttu-id="e09e4-163">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-163">`Tag` parameter has been removed</span></span>

```powershell
# Old
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

###  <a name="remove-azurermsqldatabasefromfailovergroup"></a><span data-ttu-id="e09e4-164">Remove-AzureRmSqlDatabaseFromFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="e09e4-164">Remove-AzureRmSqlDatabaseFromFailoverGroup</span></span>
- <span data-ttu-id="e09e4-165">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-165">`Tag` parameter has been removed</span></span>

```powershell
# Old
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

### <a name="remove-azurermsqldatabasefailovergroup"></a><span data-ttu-id="e09e4-166">Remove-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="e09e4-166">Remove-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="e09e4-167">`PartnerResourceGroupName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-167">`PartnerResourceGroupName` parameter has been removed</span></span>
- <span data-ttu-id="e09e4-168">`PartnerServerName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-168">`PartnerServerName` parameter has been removed</span></span>

```powershell
# Old
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -PartnerResourceGroupName rg

# New
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg
```

### <a name="set-azurermsqldatabasethreatdetectionpolicy"></a><span data-ttu-id="e09e4-169">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e09e4-169">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span></span>
- <span data-ttu-id="e09e4-170">`ExcludedDetectionType` パラメーターで値 `Usage_Anomaly` が無効になりました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-170">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

### <a name="set-azurermsqlserverthreatdetectionpolicy"></a><span data-ttu-id="e09e4-171">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="e09e4-171">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
- <span data-ttu-id="e09e4-172">`ExcludedDetectionType` パラメーターで値 `Usage_Anomaly` が無効になりました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-172">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="e09e4-173">Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-173">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="e09e4-174">このリリースで影響を受けた出力の型プロパティは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="e09e4-174">The following output type properties were affected this release:</span></span>

### <a name="azurestorageblobicloudblobserviceclient"></a><span data-ttu-id="e09e4-175">AzureStorageBlob.ICloudBlob.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="e09e4-175">AzureStorageBlob.ICloudBlob.ServiceClient</span></span>
- <span data-ttu-id="e09e4-176">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="e09e4-176">The following properties were removed from this type (_note_: they can still be found in `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="e09e4-177">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="e09e4-177">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageBlob`
    - `Get-AzureStorageBlobContent`
    - `Get-AzureStorageBlobCopyState`
    - `Set-AzureStorageBlobContent`
    - `Start-AzureStorageBlobCopy`
    - `Stop-AzureStorageBlobCopy`
    
### <a name="azurestoragecontainercloudblobcontainerserviceclient"></a><span data-ttu-id="e09e4-178">AzureStorageContainer.CloudBlobContainer.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="e09e4-178">AzureStorageContainer.CloudBlobContainer.ServiceClient</span></span>
- <span data-ttu-id="e09e4-179">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="e09e4-179">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="e09e4-180">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="e09e4-180">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageContainer`
    - `New-AzureStorageContainer`
    - `Set-AzureStorageContainerAcl`
    
### <a name="azurestoragequeuecloudqueueserviceclient"></a><span data-ttu-id="e09e4-181">AzureStorageQueue.CloudQueue.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="e09e4-181">AzureStorageQueue.CloudQueue.ServiceClient</span></span>
- <span data-ttu-id="e09e4-182">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="e09e4-182">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="e09e4-183">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="e09e4-183">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageQueue`
    - `New-AzureStorageQueue`
    
### <a name="azurestoragetablecloudtableserviceclient"></a><span data-ttu-id="e09e4-184">AzureStorageTable.CloudTable.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="e09e4-184">AzureStorageTable.CloudTable.ServiceClient</span></span>
- <span data-ttu-id="e09e4-185">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="e09e4-185">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `PayloadFormat`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="e09e4-186">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="e09e4-186">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageTable`
    - `New-AzureStorageTable`
    
```powershell
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

## <a name="breaking-changes-to-profile-cmdlets"></a><span data-ttu-id="e09e4-187">Profile コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-187">Breaking Changes to Profile Cmdlets</span></span>

<span data-ttu-id="e09e4-188">次のコマンドレットとコマンドレットの出力の型が、このリリースで変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-188">The following cmdlets and cmdlet output types were changed in this release.</span></span>

### <a name="add-azurermaccount-breaking-changes"></a><span data-ttu-id="e09e4-189">Add-AzureRmAccount の重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-189">Add-AzureRmAccount breaking changes</span></span>

- <span data-ttu-id="e09e4-190">```EnvironmentName``` パラメーターが削除され、```Environment``` に置き換えられました。```Environment``` は、```AzureEnvironment``` オブジェクトではなく文字列を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="e09e4-190">```EnvironmentName``` parameter has been removed and replaced with ```Environment```, the ```Environment``` now takes a string and not an ```AzureEnvironment``` object</span></span>

```powershell
# Old
Add-AzureRmAccount -EnvironmentName AzureChinaCloud

# New
Add-AzureRmAccount -Environment AzureChinaCloud
```

### <a name="select-azurermprofile-was-renamed-to-import-azurermcontext"></a><span data-ttu-id="e09e4-191">Select-AzureRmProfile の名前を Import-AzureRmContext に変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-191">Select-AzureRmProfile was renamed to Import-AzureRmContext</span></span>

<span data-ttu-id="e09e4-192">```Select-AzureRmProfile``` の名前が ```Import-AzureRmContext``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-192">```Select-AzureRmProfile``` was renamed to ```Import-AzureRmContext```</span></span>

```powershell
# Old
Select-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Import-AzureRmContext -Path c:\mydir\myprofile.json
```

### <a name="save-azurermprofile-was-renamed-to-save-azurermcontext"></a><span data-ttu-id="e09e4-193">Save-AzureRmProfile の名前を Save-AzureRmContext に変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-193">Save-AzureRmProfile was renamed to Save-AzureRmContext</span></span>

<span data-ttu-id="e09e4-194">```Save-AzureRmProfile``` の名前が ```Save-AzureRmContext``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-194">```Save-AzureRmProfile``` was renamed to ```Save-AzureRmContext```</span></span>

```powershell
# Old
Save-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Save-AzureRmContext -Path c:\mydir\myprofile.json
```
### <a name="breaking-changes-to-output-psazurecontext-type"></a><span data-ttu-id="e09e4-195">出力の PSAzureContext 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-195">Breaking Changes to output PSAzureContext Type</span></span>

- <span data-ttu-id="e09e4-196">```TokenCache``` プロパティが、```byte[]``` ではなく ```IAzureTokenCache``` を実装する型に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-196">The ```TokenCache``` property changed to a type that implements ```IAzureTokenCache``` instead of a ```byte[]```</span></span>

```powershell
# Old
$bytes = (Get-AzureRmContext).TokenCache
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache
$bytes = (Add-AzureRmAccount).Context.TokenCache

# New
$bytes = (Get-AzureRmContext).TokenCache.CacheData
$bytes = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).TokenCache.CacheData
$bytes = (Add-AzureRmAccount).Context.TokenCache.CacheData
```

### <a name="breaking-changes-to-the-output-psazureaccount-type"></a><span data-ttu-id="e09e4-197">出力の PSAzureAccount 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-197">Breaking Changes to the output PSAzureAccount Type</span></span>

- <span data-ttu-id="e09e4-198">```AccountType``` プロパティが ```Type``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-198">The ```AccountType``` property was changed to ```Type```</span></span>

```powershell
# Old
$type = (Get-AzureRmContext).Account.AccountType
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.AccountType
$type = (Add-AzureRmAccount).Context.Account.AccountType

# New 
$type = (Get-AzureRmContext).Account.Type
$type = (Set-AzureRmContext -SubscriptionId xxx-xxx-xxx-xxx).Account.Type
$type = (Add-AzureRmAccount).Context.Account.Type
```

### <a name="breaking-changes-to-the-output-psazuresubscription-type"></a><span data-ttu-id="e09e4-199">出力の PSAzureSubscription 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-199">Breaking Changes to the output PSAzureSubscription Type</span></span>
- <span data-ttu-id="e09e4-200">```SubscriptionId``` プロパティが ```Id``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-200">The ```SubscriptionId``` property was changed to ```Id```</span></span>

```powershell
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

- <span data-ttu-id="e09e4-201">```SubscriptionName``` プロパティが ```Name``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-201">The ```SubscriptionName``` property was changed to ```Name```</span></span>

```powershell
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

### <a name="breaking-changes-to-the-output-psazuretenant-type"></a><span data-ttu-id="e09e4-202">出力の PSAzureTenant 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="e09e4-202">Breaking Changes to the output PSAzureTenant Type</span></span>

- <span data-ttu-id="e09e4-203">```TenantId``` プロパティが ```Id``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-203">The ```TenantId``` property was changed to ```Id```</span></span>

```powershell
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

- <span data-ttu-id="e09e4-204">```Domain``` プロパティが ```Directory``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="e09e4-204">The ```Domain``` property was changed to ```Directory```</span></span>

```powershell
# Old
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Domain

# New
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Directory
```
