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
# <a name="breaking-changes-for-microsoft-azure-powershell-400"></a><span data-ttu-id="9a0a3-103">Microsoft Azure PowerShell 4.0.0 の重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-103">Breaking changes for Microsoft Azure PowerShell 4.0.0</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="9a0a3-104">このドキュメントは、Microsoft Azure PowerShell コマンドレットのコンシューマー向けに、重大な変更を通知すると同時に、移行ガイドとしても役立ちます。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-104">This document serves as both a breaking change notification and migration guide for consumers of the Microsoft Azure PowerShell cmdlets.</span></span> <span data-ttu-id="9a0a3-105">各セクションでは、重大な変更の影響と抵抗を最小限に抑える移行パスを示しています。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-105">Each section describes both the impetus for the breaking change and the migration path of least resistance.</span></span> <span data-ttu-id="9a0a3-106">詳細なコンテキストについては、各変更に関する pull request を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-106">For in-depth context, please refer to the pull request associated with each change.</span></span>

## <a name="table-of-contents"></a><span data-ttu-id="9a0a3-107">目次</span><span class="sxs-lookup"><span data-stu-id="9a0a3-107">Table of Contents</span></span>

- [<span data-ttu-id="9a0a3-108">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-108">Breaking changes to Compute cmdlets</span></span>](#breaking-changes-to-compute-cmdlets)
- [<span data-ttu-id="9a0a3-109">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-109">Breaking changes to EventHub cmdlets</span></span>](#breaking-changes-to-eventhub-cmdlets)
- [<span data-ttu-id="9a0a3-110">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-110">Breaking changes to Insights cmdlets</span></span>](#breaking-changes-to-insights-cmdlets)
- [<span data-ttu-id="9a0a3-111">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-111">Breaking changes to Network cmdlets</span></span>](#breaking-changes-to-network-cmdlets)
- [<span data-ttu-id="9a0a3-112">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-112">Breaking changes to ServiceBus cmdlets</span></span>](#breaking-changes-to-servicebus-cmdlets)
- [<span data-ttu-id="9a0a3-113">Sql コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-113">Breaking changes to Sql cmdlets</span></span>](#breaking-changes-to-sql-cmdlets)
- [<span data-ttu-id="9a0a3-114">Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-114">Breaking changes to Storage cmdlets</span></span>](#breaking-changes-to-storage-cmdlets)
- [<span data-ttu-id="9a0a3-115">Profile コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-115">Breaking Changes to Profile Cmdlets</span></span>](#breaking-changes-to-profile-cmdlets)
  ## <a name="breaking-changes-to-compute-cmdlets"></a><span data-ttu-id="9a0a3-116">Compute コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-116">Breaking changes to Compute cmdlets</span></span>

<span data-ttu-id="9a0a3-117">このリリースで影響を受けた出力の型は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-117">The following output types were affected this release:</span></span>

### <a name="psvirtualmachine"></a><span data-ttu-id="9a0a3-118">PSVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="9a0a3-118">PSVirtualMachine</span></span>
- <span data-ttu-id="9a0a3-119">`PSVirtualMachine` オブジェクトの最上位レベルのプロパティ `DataDiskNames` と `NetworkInterfaceIDs` が出力の型から削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-119">Top level properties `DataDiskNames` and `NetworkInterfaceIDs` of nthe `PSVirtualMachine` object have been removed from the output type.</span></span> <span data-ttu-id="9a0a3-120">これらのプロパティは、`PSVirtualMachine` オブジェクトの `StorageProfile` プロパティと `NetworkProfile` プロパティで常に使用できましたが、今後はアクセスすることが必要になります。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-120">These properties have always been available in the `StorageProfile` and `NetworkProfile` properties of the `PSVirtualMachine` object and will be the way they will need to be accessed going forward.</span></span>
- <span data-ttu-id="9a0a3-121">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-121">This change affects the following cmdlets:</span></span>
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

## <a name="breaking-changes-to-eventhub-cmdlets"></a><span data-ttu-id="9a0a3-122">EventHub コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-122">Breaking changes to EventHub cmdlets</span></span>

<span data-ttu-id="9a0a3-123">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-123">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermeventhubnamespace"></a><span data-ttu-id="9a0a3-124">Get-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="9a0a3-124">Get-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="9a0a3-125">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-125">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermeventhubnamespace"></a><span data-ttu-id="9a0a3-126">New-AzureRmEventHubNamespace</span><span class="sxs-lookup"><span data-stu-id="9a0a3-126">New-AzureRmEventHubNamespace</span></span>
- <span data-ttu-id="9a0a3-127">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-127">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-insights-cmdlets"></a><span data-ttu-id="9a0a3-128">Insights コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-128">Breaking changes to Insights cmdlets</span></span>

<span data-ttu-id="9a0a3-129">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-129">The following cmdlets were affected this release:</span></span>
    
### <a name="get-azurermusage"></a><span data-ttu-id="9a0a3-130">Get-AzureRmUsage</span><span class="sxs-lookup"><span data-stu-id="9a0a3-130">Get-AzureRmUsage</span></span>
- <span data-ttu-id="9a0a3-131">このコマンドレットは非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-131">This cmdlet has been deprecated.</span></span>

### <a name="remove-azurermalertrule"></a><span data-ttu-id="9a0a3-132">Remove-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="9a0a3-132">Remove-AzureRmAlertRule</span></span>
- <span data-ttu-id="9a0a3-133">このコマンドレットの出力が、単一のオブジェクトを含むリストから単一のオブジェクトに変更されました。このオブジェクトには、requestId と状態コードが含まれます。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-133">The output of this cmdlet has changed from a list with a single object to a single object; this object includes the requestId, and status code.</span></span>
    
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
    
### <a name="add-azurermlogalertrule"></a><span data-ttu-id="9a0a3-134">Add-AzureRmLogAlertRule</span><span class="sxs-lookup"><span data-stu-id="9a0a3-134">Add-AzureRmLogAlertRule</span></span>
- <span data-ttu-id="9a0a3-135">このコマンドレットは非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-135">This cmdlet has been deprecated.</span></span>
    
### <a name="get-azurermalertrule"></a><span data-ttu-id="9a0a3-136">Get-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="9a0a3-136">Get-AzureRmAlertRule</span></span>
- <span data-ttu-id="9a0a3-137">このコマンドレットの出力 (オブジェクトのリスト) の各要素がフラット化されます。つまり、構造体 `{ Id, Location, Name, Tags, Properties }` を持つオブジェクトを返す代わりに、構造体 `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}` を持つオブジェクトを返します。この構造体は、Azure リソースのすべての属性と、最上位レベルの AlertRuleResource のすべての属性です。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-137">Each element of the output (a list of objects) of this cmdlet is flattened, i.e. instead of returning objects with the structure `{ Id, Location, Name, Tags, Properties }` it will return objects with the structure `{ Id, Location, Name, Tags, Type, Description, IsEnabled, Condition, Actions, LastUpdatedTime, ...}`, which is all of the attributes of an Azure Resource plus all of the attributes of an AlertRuleResource at the top level.</span></span>
    
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
    
### <a name="get-azurermautoscalesetting"></a><span data-ttu-id="9a0a3-138">Get-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="9a0a3-138">Get-AzureRmAutoscaleSetting</span></span>
- <span data-ttu-id="9a0a3-139">`AutoscaleSettingResourceName` フィールドには `Name` フィールドと常に同じ値が含まれるため、非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-139">The `AutoscaleSettingResourceName` field is deprecated since it always has the same value as the `Name` field.</span></span>

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
    
### <a name="remove-azurermlogprofile"></a><span data-ttu-id="9a0a3-140">Remove-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="9a0a3-140">Remove-AzureRmLogProfile</span></span>
- <span data-ttu-id="9a0a3-141">このコマンドレットの出力が、`Boolean` から、`RequestId` と `StatusCode` を含むオブジェクトに変更されます。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-141">The output of this cmdlet will change from `Boolean` to and object containing `RequestId` and `StatusCode`</span></span>

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
    
### <a name="add-azurermlogprofile"></a><span data-ttu-id="9a0a3-142">Add-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="9a0a3-142">Add-AzureRmLogProfile</span></span>
- <span data-ttu-id="9a0a3-143">このコマンドレットの出力が、requestId、状態コード、更新されたリソースまたは新しく作成されたリソースを含むオブジェクトに変更されます。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-143">The output of this cmdlet will change from an object that includes the requestId, status code, and the updated or newly created resource</span></span>
    
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
    
### <a name="set-azurermdiagnosticsettings"></a><span data-ttu-id="9a0a3-144">Set-AzureRmDiagnosticSettings</span><span class="sxs-lookup"><span data-stu-id="9a0a3-144">Set-AzureRmDiagnosticSettings</span></span>
- <span data-ttu-id="9a0a3-145">このコマンドの名前が `Update-AzureRmDiagnosticSettings` に変更されます。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-145">The command is going to be renamed to `Update-AzureRmDiagnosticSettings`</span></span>

```powershell-interactive
# Old
Set-AzureRmDiagnosticSettings

# New
Update-AzureRmDiagnosticSettings
```

## <a name="breaking-changes-to-network-cmdlets"></a><span data-ttu-id="9a0a3-146">Network コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-146">Breaking changes to Network cmdlets</span></span>

<span data-ttu-id="9a0a3-147">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-147">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermvirtualnetworkgatewayconnection"></a><span data-ttu-id="9a0a3-148">New-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="9a0a3-148">New-AzureRmVirtualNetworkGatewayConnection</span></span>
- <span data-ttu-id="9a0a3-149">`EnableBgp` パラメーターが、`string` ではなく `boolean` を受け取るように変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-149">`EnableBgp` parameter has been changed to take a `boolean` instead of a `string`</span></span>

```powershell-interactive
# Old
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp "true"

# New
New-AzureRmVirtualNetworkGatewayConnection -ResourceGroupName "RG" -name "conn1" -VirtualNetworkGateway1 $vnetGateway -LocalNetworkGateway2 $localnetGateway -ConnectionType IPsec -SharedKey "key" -EnableBgp $true
```

## <a name="breaking-changes-to-servicebus-cmdlets"></a><span data-ttu-id="9a0a3-150">ServiceBus コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-150">Breaking changes to ServiceBus cmdlets</span></span>

<span data-ttu-id="9a0a3-151">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-151">The following cmdlets were affected this release:</span></span>

### <a name="get-azurermservicebusnamespace"></a><span data-ttu-id="9a0a3-152">Get-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="9a0a3-152">Get-AzureRmServiceBusNamespace</span></span>
- <span data-ttu-id="9a0a3-153">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-153">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

### <a name="new-azurermservicebusnamespace"></a><span data-ttu-id="9a0a3-154">New-AzureRmServiceBusNamespace</span><span class="sxs-lookup"><span data-stu-id="9a0a3-154">New-AzureRmServiceBusNamespace</span></span>

- <span data-ttu-id="9a0a3-155">出力の型 `NamespaceAttributes` から `ResourceGroupName` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-155">The property `ResourceGroupName` has been removed from the output type `NamespaceAttributes`</span></span>

## <a name="breaking-changes-to-sql-cmdlets"></a><span data-ttu-id="9a0a3-156">Sql コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-156">Breaking changes to Sql cmdlets</span></span>

<span data-ttu-id="9a0a3-157">このリリースで影響を受けたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-157">The following cmdlets were affected this release:</span></span>

### <a name="new-azurermsqldatabasefailovergroup"></a><span data-ttu-id="9a0a3-158">New-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="9a0a3-158">New-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="9a0a3-159">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-159">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="9a0a3-160">`GracePeriodWithDataLossHour` パラメーターの名前が `GracePeriodWithDataLossHours` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-160">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell-interactive
# Old
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
New-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="set-azurermsqldatabasefailovergroup"></a><span data-ttu-id="9a0a3-161">Set-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="9a0a3-161">Set-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="9a0a3-162">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-162">`Tag` parameter has been removed</span></span>
- <span data-ttu-id="9a0a3-163">`GracePeriodWithDataLossHour` パラメーターの名前が `GracePeriodWithDataLossHours` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-163">`GracePeriodWithDataLossHour` parameter has been renamed to `GracePeriodWithDataLossHours`</span></span>

```powershell-interactive
# Old
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHour 1 -Tag @{ Environment="Test" }

# New
Set-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -FailoverPolicy Automatic -GracePeriodWithDataLossHours 1
```

### <a name="add-azurermsqldatabasetofailovergroup"></a><span data-ttu-id="9a0a3-164">Add-AzureRmSqlDatabaseToFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="9a0a3-164">Add-AzureRmSqlDatabaseToFailoverGroup</span></span>
- <span data-ttu-id="9a0a3-165">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-165">`Tag` parameter has been removed</span></span>

```powershell-interactive
# Old
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Add-AzureRmSqlDatabaseToFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

###  <a name="remove-azurermsqldatabasefromfailovergroup"></a><span data-ttu-id="9a0a3-166">Remove-AzureRmSqlDatabaseFromFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="9a0a3-166">Remove-AzureRmSqlDatabaseFromFailoverGroup</span></span>
- <span data-ttu-id="9a0a3-167">`Tag` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-167">`Tag` parameter has been removed</span></span>

```powershell-interactive
# Old
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1 -Tag @{ Environment="Test" }

# New
Remove-AzureRmSqlDatabaseFromFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -Database $db1
```

### <a name="remove-azurermsqldatabasefailovergroup"></a><span data-ttu-id="9a0a3-168">Remove-AzureRmSqlDatabaseFailoverGroup</span><span class="sxs-lookup"><span data-stu-id="9a0a3-168">Remove-AzureRmSqlDatabaseFailoverGroup</span></span>
- <span data-ttu-id="9a0a3-169">`PartnerResourceGroupName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-169">`PartnerResourceGroupName` parameter has been removed</span></span>
- <span data-ttu-id="9a0a3-170">`PartnerServerName` パラメーターが削除されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-170">`PartnerServerName` parameter has been removed</span></span>

```powershell-interactive
# Old
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg -PartnerServerName server2 -PartnerResourceGroupName rg

# New
Remove-AzureRmSqlDatabaseFailoverGroup -ResourceGroupName rg -ServerName server1 -FailoverGroupName fg
```

### <a name="set-azurermsqldatabasethreatdetectionpolicy"></a><span data-ttu-id="9a0a3-171">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9a0a3-171">Set-AzureRmSqlDatabaseThreatDetectionPolicy</span></span>
- <span data-ttu-id="9a0a3-172">`ExcludedDetectionType` パラメーターで値 `Usage_Anomaly` が無効になりました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-172">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

### <a name="set-azurermsqlserverthreatdetectionpolicy"></a><span data-ttu-id="9a0a3-173">Set-AzureRmSqlServerThreatDetectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9a0a3-173">Set-AzureRmSqlServerThreatDetectionPolicy</span></span>
- <span data-ttu-id="9a0a3-174">`ExcludedDetectionType` パラメーターで値 `Usage_Anomaly` が無効になりました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-174">The value `Usage_Anomaly` is no longer valid for the parameter `ExcludedDetectionType`</span></span>

## <a name="breaking-changes-to-storage-cmdlets"></a><span data-ttu-id="9a0a3-175">Storage コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-175">Breaking changes to Storage cmdlets</span></span>

<span data-ttu-id="9a0a3-176">このリリースで影響を受けた出力の型プロパティは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-176">The following output type properties were affected this release:</span></span>

### <a name="azurestorageblobicloudblobserviceclient"></a><span data-ttu-id="9a0a3-177">AzureStorageBlob.ICloudBlob.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="9a0a3-177">AzureStorageBlob.ICloudBlob.ServiceClient</span></span>
- <span data-ttu-id="9a0a3-178">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-178">The following properties were removed from this type (_note_: they can still be found in `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="9a0a3-179">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-179">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageBlob`
    - `Get-AzureStorageBlobContent`
    - `Get-AzureStorageBlobCopyState`
    - `Set-AzureStorageBlobContent`
    - `Start-AzureStorageBlobCopy`
    - `Stop-AzureStorageBlobCopy`
    
### <a name="azurestoragecontainercloudblobcontainerserviceclient"></a><span data-ttu-id="9a0a3-180">AzureStorageContainer.CloudBlobContainer.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="9a0a3-180">AzureStorageContainer.CloudBlobContainer.ServiceClient</span></span>
- <span data-ttu-id="9a0a3-181">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-181">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `ServerTimeout`
    - `ParallelOperationThreadCount`
    - `SingleBlobUploadThresholdInBytes`
- <span data-ttu-id="9a0a3-182">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-182">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageContainer`
    - `New-AzureStorageContainer`
    - `Set-AzureStorageContainerAcl`
    
### <a name="azurestoragequeuecloudqueueserviceclient"></a><span data-ttu-id="9a0a3-183">AzureStorageQueue.CloudQueue.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="9a0a3-183">AzureStorageQueue.CloudQueue.ServiceClient</span></span>
- <span data-ttu-id="9a0a3-184">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-184">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="9a0a3-185">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-185">This change affects the following cmdlets:</span></span>
    - `Get-AzureStorageQueue`
    - `New-AzureStorageQueue`
    
### <a name="azurestoragetablecloudtableserviceclient"></a><span data-ttu-id="9a0a3-186">AzureStorageTable.CloudTable.ServiceClient</span><span class="sxs-lookup"><span data-stu-id="9a0a3-186">AzureStorageTable.CloudTable.ServiceClient</span></span>
- <span data-ttu-id="9a0a3-187">次のプロパティはこの型から削除されました (_注_: `DefaultRequestOptions` プロパティには引き続き存在します)。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-187">The following properties were removed from this type (_note_: they can still be found in the `DefaultRequestOptions` property):</span></span>
    - `LocationMode`
    - `MaximumExecutionTime`
    - `PayloadFormat`
    - `RetryPolicy`
    - `ServerTimeout`
- <span data-ttu-id="9a0a3-188">この変更は次のコマンドレットに影響します。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-188">This change affects the following cmdlets:</span></span>
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

## <a name="breaking-changes-to-profile-cmdlets"></a><span data-ttu-id="9a0a3-189">Profile コマンドレットの重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-189">Breaking Changes to Profile Cmdlets</span></span>

<span data-ttu-id="9a0a3-190">次のコマンドレットとコマンドレットの出力の型が、このリリースで変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-190">The following cmdlets and cmdlet output types were changed in this release.</span></span>

### <a name="add-azurermaccount-breaking-changes"></a><span data-ttu-id="9a0a3-191">Add-AzureRmAccount の重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-191">Add-AzureRmAccount breaking changes</span></span>

- <span data-ttu-id="9a0a3-192">```EnvironmentName``` パラメーターが削除され、```Environment``` に置き換えられました。```Environment``` は、```AzureEnvironment``` オブジェクトではなく文字列を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-192">```EnvironmentName``` parameter has been removed and replaced with ```Environment```, the ```Environment``` now takes a string and not an ```AzureEnvironment``` object</span></span>

```powershell-interactive
# Old
Add-AzureRmAccount -EnvironmentName AzureChinaCloud

# New
Add-AzureRmAccount -Environment AzureChinaCloud
```

### <a name="select-azurermprofile-was-renamed-to-import-azurermcontext"></a><span data-ttu-id="9a0a3-193">Select-AzureRmProfile の名前を Import-AzureRmContext に変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-193">Select-AzureRmProfile was renamed to Import-AzureRmContext</span></span>

<span data-ttu-id="9a0a3-194">```Select-AzureRmProfile``` の名前が ```Import-AzureRmContext``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-194">```Select-AzureRmProfile``` was renamed to ```Import-AzureRmContext```</span></span>

```powershell-interactive
# Old
Select-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Import-AzureRmContext -Path c:\mydir\myprofile.json
```

### <a name="save-azurermprofile-was-renamed-to-save-azurermcontext"></a><span data-ttu-id="9a0a3-195">Save-AzureRmProfile の名前を Save-AzureRmContext に変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-195">Save-AzureRmProfile was renamed to Save-AzureRmContext</span></span>

<span data-ttu-id="9a0a3-196">```Save-AzureRmProfile``` の名前が ```Save-AzureRmContext``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-196">```Save-AzureRmProfile``` was renamed to ```Save-AzureRmContext```</span></span>

```powershell-interactive
# Old
Save-AzureRmProfile -Path c:\mydir\myprofile.json

# New
Save-AzureRmContext -Path c:\mydir\myprofile.json
```
### <a name="breaking-changes-to-output-psazurecontext-type"></a><span data-ttu-id="9a0a3-197">出力の PSAzureContext 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-197">Breaking Changes to output PSAzureContext Type</span></span>

- <span data-ttu-id="9a0a3-198">```TokenCache``` プロパティが、```byte[]``` ではなく ```IAzureTokenCache``` を実装する型に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-198">The ```TokenCache``` property changed to a type that implements ```IAzureTokenCache``` instead of a ```byte[]```</span></span>

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

### <a name="breaking-changes-to-the-output-psazureaccount-type"></a><span data-ttu-id="9a0a3-199">出力の PSAzureAccount 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-199">Breaking Changes to the output PSAzureAccount Type</span></span>

- <span data-ttu-id="9a0a3-200">```AccountType``` プロパティが ```Type``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-200">The ```AccountType``` property was changed to ```Type```</span></span>

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

### <a name="breaking-changes-to-the-output-psazuresubscription-type"></a><span data-ttu-id="9a0a3-201">出力の PSAzureSubscription 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-201">Breaking Changes to the output PSAzureSubscription Type</span></span>
- <span data-ttu-id="9a0a3-202">```SubscriptionId``` プロパティが ```Id``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-202">The ```SubscriptionId``` property was changed to ```Id```</span></span>

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

- <span data-ttu-id="9a0a3-203">```SubscriptionName``` プロパティが ```Name``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-203">The ```SubscriptionName``` property was changed to ```Name```</span></span>

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

### <a name="breaking-changes-to-the-output-psazuretenant-type"></a><span data-ttu-id="9a0a3-204">出力の PSAzureTenant 型の重大な変更</span><span class="sxs-lookup"><span data-stu-id="9a0a3-204">Breaking Changes to the output PSAzureTenant Type</span></span>

- <span data-ttu-id="9a0a3-205">```TenantId``` プロパティが ```Id``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-205">The ```TenantId``` property was changed to ```Id```</span></span>

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

- <span data-ttu-id="9a0a3-206">```Domain``` プロパティが ```Directory``` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="9a0a3-206">The ```Domain``` property was changed to ```Directory```</span></span>

```powershell-interactive
# Old
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Domain

# New
$tenantName =(Get-AzureRmTenant -TenantId xxxx-xxxx-xxxx-xxxx).Directory
```
