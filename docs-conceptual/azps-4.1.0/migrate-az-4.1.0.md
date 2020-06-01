---
ms.openlocfilehash: 636fd0432d421f74fa74f3275abbc31ec5dc0b5c
ms.sourcegitcommit: 31f4facf815c2e25dc44e2fde0e1d2bd690bfc54
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/20/2020
ms.locfileid: "83688528"
---
# <a name="migration-guide-for-az-410"></a><span data-ttu-id="55533-101">Az 4.1.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="55533-101">Migration Guide for Az 4.1.0</span></span>

<span data-ttu-id="55533-102">このドキュメントでは、Az のバージョン 3.0.0 と 4.1.0 の間での変更点について説明します。</span><span class="sxs-lookup"><span data-stu-id="55533-102">This document describes the changes between the 3.0.0 and 4.1.0 versions of Az.</span></span>

- [<span data-ttu-id="55533-103">Az 4.1.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="55533-103">Migration Guide for Az 4.1.0</span></span>](#migration-guide-for-az-410)
  - [<span data-ttu-id="55533-104">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55533-104">Az.ApiManagement</span></span>](#azapimanagement)
    - [`Add-AzApiManagementRegion`](#add-azapimanagementregion)
    - [`New-AzApiManagement`](#new-azapimanagement)
    - [`Set-AzApiManagement`](#set-azapimanagement)
    - [`Get-AzApiManagementProperty`](#get-azapimanagementproperty)
    - [`New-AzApiManagementProperty`](#new-azapimanagementproperty)
    - [`Remove-AzApiManagementProperty`](#remove-azapimanagementproperty)
    - [`Set-AzApiManagementProperty`](#set-azapimanagementproperty)
  - [<span data-ttu-id="55533-105">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="55533-105">Az.Batch</span></span>](#azbatch)
    - [<span data-ttu-id="55533-106">`Get-AzBatchApplication`、`New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="55533-106">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>](#get-azbatchapplication-new-azbatchapplication)
    - [<span data-ttu-id="55533-107">`Get-AzBatchComputeNode`、`New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="55533-107">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>](#get-azbatchcomputenode-new-azbatchpool)
    - [<span data-ttu-id="55533-108">`Get-AzBatchApplicationPackage`、`New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="55533-108">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>](#get-azbatchapplicationpackage-new-azbatchapplicationpackage)
  - [<span data-ttu-id="55533-109">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="55533-109">Az.Compute</span></span>](#azcompute)
    - [`Remove-AzVmssDiagnosticsExtension`](#remove-azvmssdiagnosticsextension)
    - [`Get-AzVMImage`](#get-azvmimage)
    - [`New-AzVMConfig`](#new-azvmconfig)
    - [`Update-AzVM`](#update-azvm)
    - [`New-AzProximityPlacementGroup`](#new-azproximityplacementgroup)
    - [`Remove-AzProximityPlacementGroup`](#remove-azproximityplacementgroup)
    - [`Get-AzProximityPlacementGroup`](#get-azproximityplacementgroup)
    - [`Add-AzVmssAdditionalUnattendContent`](#add-azvmssadditionalunattendcontent)
    - [`Add-AzVmssDataDisk`](#add-azvmssdatadisk)
    - [`Add-AzVmssExtension`](#add-azvmssextension)
    - [`Add-AzVmssNetworkInterfaceConfiguration`](#add-azvmssnetworkinterfaceconfiguration)
    - [`Add-AzVmssSecret`](#add-azvmsssecret)
    - [`Add-AzVmssSshPublicKey`](#add-azvmsssshpublickey)
    - [`Add-AzVmssWinRMListener`](#add-azvmsswinrmlistener)
    - [`New-AzVmssConfig`](#new-azvmssconfig)
    - [`Remove-AzVmssDataDisk`](#remove-azvmssdatadisk)
    - [`Remove-AzVmssExtension`](#remove-azvmssextension)
    - [`Remove-AzVmssNetworkInterfaceConfiguration`](#remove-azvmssnetworkinterfaceconfiguration)
    - [`Set-AzVmssBootDiagnostic`](#set-azvmssbootdiagnostic)
    - [`Set-AzVmssOsProfile`](#set-azvmssosprofile)
    - [`Set-AzVmssRollingUpgradePolicy`](#set-azvmssrollingupgradepolicy)
    - [`Set-AzVmssStorageProfile`](#set-azvmssstorageprofile)
    - [`New-AzVmss`](#new-azvmss)
    - [`Repair-AzVmssServiceFabricUpdateDomain`](#repair-azvmssservicefabricupdatedomain)
    - [`Get-AzVmss`](#get-azvmss)
    - [`Set-AzVmssOrchestrationServiceState`](#set-azvmssorchestrationservicestate)
    - [`Update-AzVmss`](#update-azvmss)
    - [`Add-AzVmssDiagnosticsExtension`](#add-azvmssdiagnosticsextension)
    - [`Disable-AzVmssDiskEncryption`](#disable-azvmssdiskencryption)
  - [<span data-ttu-id="55533-110">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55533-110">Az.KeyVault</span></span>](#azkeyvault)
    - [`New-AzKeyVaultCertificateOrganizationDetail`](#new-azkeyvaultcertificateorganizationdetail)
    - [`New-AzKeyVaultCertificateAdministratorDetail`](#new-azkeyvaultcertificateadministratordetail)
    - [`New-AzKeyVault`](#new-azkeyvault)
  - [<span data-ttu-id="55533-111">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="55533-111">Az.Monitor</span></span>](#azmonitor)
    - [`Add-AzLogProfile`](#add-azlogprofile)
    - [`Get-AzLogProfile`](#get-azlogprofile)
    - [`New-AzMetricAlertRuleV2Criteria`](#new-azmetricalertrulev2criteria)
  - [<span data-ttu-id="55533-112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="55533-112">Az.Network</span></span>](#aznetwork)
    - [`Get-AzNetworkWatcherConnectionMonitor`](#get-aznetworkwatcherconnectionmonitor)
    - [`New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`](#new-aznetworkwatcherconnectionmonitortestconfigurationobject)
  - [<span data-ttu-id="55533-113">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="55533-113">Az.OperationalInsights</span></span>](#azoperationalinsights)
    - [`Get-AzOperationalInsightsDataSource`](#get-azoperationalinsightsdatasource)
    - [`New-AzOperationalInsightsApplicationInsightsDataSource`](#new-azoperationalinsightsapplicationinsightsdatasource)
    - [`New-AzOperationalInsightsAzureActivityLogDataSource`](#new-azoperationalinsightsazureactivitylogdatasource)
    - [`New-AzOperationalInsightsCustomLogDataSource`](#new-azoperationalinsightscustomlogdatasource)
    - [`New-AzOperationalInsightsLinuxPerformanceObjectDataSource`](#new-azoperationalinsightslinuxperformanceobjectdatasource)
    - [`New-AzOperationalInsightsLinuxSyslogDataSource`](#new-azoperationalinsightslinuxsyslogdatasource)
    - [`New-AzOperationalInsightsWindowsEventDataSource`](#new-azoperationalinsightswindowseventdatasource)
    - [`New-AzOperationalInsightsWindowsPerformanceCounterDataSource`](#new-azoperationalinsightswindowsperformancecounterdatasource)
    - [`Remove-AzOperationalInsightsDataSource`](#remove-azoperationalinsightsdatasource)
    - [`Disable-AzOperationalInsightsIISLogCollection`](#disable-azoperationalinsightsiislogcollection)
    - [`Disable-AzOperationalInsightsLinuxCustomLogCollection`](#disable-azoperationalinsightslinuxcustomlogcollection)
    - [`Disable-AzOperationalInsightsLinuxPerformanceCollection`](#disable-azoperationalinsightslinuxperformancecollection)
    - [`Disable-AzOperationalInsightsLinuxSyslogCollection`](#disable-azoperationalinsightslinuxsyslogcollection)
    - [`Enable-AzOperationalInsightsIISLogCollection`](#enable-azoperationalinsightsiislogcollection)
    - [`Enable-AzOperationalInsightsLinuxCustomLogCollection`](#enable-azoperationalinsightslinuxcustomlogcollection)
    - [`Enable-AzOperationalInsightsLinuxPerformanceCollection`](#enable-azoperationalinsightslinuxperformancecollection)
    - [`Enable-AzOperationalInsightsLinuxSyslogCollection`](#enable-azoperationalinsightslinuxsyslogcollection)
    - [`Get-AzOperationalInsightsSavedSearch`](#get-azoperationalinsightssavedsearch)
    - [`Get-AzOperationalInsightsSavedSearchResult`](#get-azoperationalinsightssavedsearchresult)
    - [`Get-AzOperationalInsightsSearchResult`](#get-azoperationalinsightssearchresult)
    - [`Get-AzOperationalInsightsStorageInsight`](#get-azoperationalinsightsstorageinsight)
    - [`New-AzOperationalInsightsStorageInsight`](#new-azoperationalinsightsstorageinsight)
    - [`Remove-AzOperationalInsightsStorageInsight`](#remove-azoperationalinsightsstorageinsight)
    - [`Set-AzOperationalInsightsStorageInsight`](#set-azoperationalinsightsstorageinsight)
    - [`Get-AzOperationalInsightsLinkTarget`](#get-azoperationalinsightslinktarget)
    - [`Get-AzOperationalInsightsWorkspace`](#get-azoperationalinsightsworkspace)
    - [`New-AzOperationalInsightsWorkspace`](#new-azoperationalinsightsworkspace)
    - [`Set-AzOperationalInsightsWorkspace`](#set-azoperationalinsightsworkspace)
    - [`Invoke-AzOperationalInsightsQuery`](#invoke-azoperationalinsightsquery)
  - [<span data-ttu-id="55533-114">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="55533-114">Az.Resources</span></span>](#azresources)
    - [`Get-AzDeploymentScript`](#get-azdeploymentscript)
    - [`Get-AzDeploymentScriptLog`](#get-azdeploymentscriptlog)
    - [`Save-AzDeploymentScriptLog`](#save-azdeploymentscriptlog)
    - [`Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`](#get-azresourcelock-new-azresourcelock-remove-azresourcelock-set-azresourcelock)
    - [`Get-AzPolicyAlias`](#get-azpolicyalias)
    - [`New-AzPolicyAssignment`](#new-azpolicyassignment)
    - [`Remove-AzDeploymentScript`](#remove-azdeploymentscript)
  - [<span data-ttu-id="55533-115">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="55533-115">Az.Storage</span></span>](#azstorage)
    - [<span data-ttu-id="55533-116">`Update-AzStorageAccountNetworkRuleSet`、`Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="55533-116">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>](#update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset)
    - [<span data-ttu-id="55533-117">`New-AzStorageTable`、`Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="55533-117">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>](#new-azstoragetable-get-azstoragetable)
    - [<span data-ttu-id="55533-118">`Get-AzStorageFile`、`Remove-AzStorageFile`、`Get-AzStorageFileContent`、`Set-AzStorageFileContent`、`Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="55533-118">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>](#get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy)
    - [<span data-ttu-id="55533-119">`Get-AzStorageFile`、`New-AzStorageDirectory`、`Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="55533-119">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>](#get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory)
    - [<span data-ttu-id="55533-120">`Get-AzStorageShare`、`New-AzStorageShare`、`Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="55533-120">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>](#get-azstorageshare-new-azstorageshare-remove-azstorageshare)
    - [`Set-AzStorageShareQuota`](#set-azstoragesharequota)
    - [`Remove-AzStorageDirectory`](#remove-azstoragedirectory)

## <a name="azapimanagement"></a><span data-ttu-id="55533-121">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55533-121">Az.ApiManagement</span></span>

### `Add-AzApiManagementRegion`

<span data-ttu-id="55533-122">`Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` 型のプロパティ `Type` の型が、`Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` から `System.String` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-122">The type of property `Type` of type `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` has changed from `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` to `System.String`.</span></span>

### `New-AzApiManagement`

- <span data-ttu-id="55533-123">コマンドレット `New-AzApiManagement` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-123">The cmdlet `New-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-124">コマンドレット `New-AzApiManagement` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-124">The parameter set `__AllParameterSets` for cmdlet `New-AzApiManagement` has been removed.</span></span>

### `Set-AzApiManagement`

- <span data-ttu-id="55533-125">コマンドレット `Set-AzApiManagement` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-125">The cmdlet `Set-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-126">コマンドレット `Set-AzApiManagement` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-126">The parameter set `__AllParameterSets` for cmdlet `Set-AzApiManagement` has been removed.</span></span>

### `Get-AzApiManagementProperty`

<span data-ttu-id="55533-127">コマンドレット `Get-AzApiManagementProperty` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-127">The cmdlet `Get-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

### `New-AzApiManagementProperty`

<span data-ttu-id="55533-128">コマンドレット `New-AzApiManagementProperty` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-128">The cmdlet `New-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Remove-AzApiManagementProperty`

<span data-ttu-id="55533-129">コマンドレット `Remove-AzApiManagementProperty` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-129">The cmdlet `Remove-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Set-AzApiManagementProperty`

<span data-ttu-id="55533-130">コマンドレット `Set-AzApiManagementProperty` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-130">The cmdlet `Set-AzApiManagementProperty` has been removed and no alias was found for the original cmdlet name.</span></span>

## <a name="azbatch"></a><span data-ttu-id="55533-131">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="55533-131">Az.Batch</span></span>

### <a name="get-azbatchapplication-new-azbatchapplication"></a><span data-ttu-id="55533-132">`Get-AzBatchApplication`, `New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="55533-132">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>

<span data-ttu-id="55533-133">`Microsoft.Azure.Commands.Batch.Models.PSApplication` 型の `ApplicationPackages` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-133">The property `ApplicationPackages` of type `Microsoft.Azure.Commands.Batch.Models.PSApplication` has been removed.</span></span>

### <a name="get-azbatchcomputenode-new-azbatchpool"></a><span data-ttu-id="55533-134">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="55533-134">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>

<span data-ttu-id="55533-135">`Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` 型の `PublicIPs` プロパティが削除されました</span><span class="sxs-lookup"><span data-stu-id="55533-135">The property `PublicIPs` of type `Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` has been removed</span></span>

### <a name="get-azbatchapplicationpackage-new-azbatchapplicationpackage"></a><span data-ttu-id="55533-136">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="55533-136">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>

<span data-ttu-id="55533-137">`Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` 型のプロパティ `StorageUrlExpiry` の型が、`System.DateTime` から `System.DateTime?` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-137">The type of property `StorageUrlExpiry` of type `Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` has changed from `System.DateTime` to `System.DateTime?`.</span></span>

## <a name="azcompute"></a><span data-ttu-id="55533-138">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="55533-138">Az.Compute</span></span>

### `Remove-AzVmssDiagnosticsExtension`

<span data-ttu-id="55533-139">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-139">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVMImage`

- <span data-ttu-id="55533-140">コマンドレット `Get-AzVMImage` でパラメーター `FilterExpression` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-140">The cmdlet `Get-AzVMImage` no longer supports the parameter `FilterExpression` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-141">コマンドレット `Get-AzVMImage` のパラメーター セット `ListVMImage` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-141">The parameter set `ListVMImage` for cmdlet `Get-AzVMImage` has been removed.</span></span>

### `New-AzVMConfig`

- <span data-ttu-id="55533-142">コマンドレット `New-AzVMConfig` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-142">The cmdlet `New-AzVMConfig` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-143">コマンドレット `New-AzVMConfig` のパラメーター セット `AssignIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-143">The parameter set `AssignIdentityParameterSet` for cmdlet `New-AzVMConfig` has been removed.</span></span>

### `Update-AzVM`

- <span data-ttu-id="55533-144">コマンドレット `Update-AzVM` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-144">The cmdlet `Update-AzVM` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-145">コマンドレット `Update-AzVM` のパラメーター セット `AssignIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-145">The parameter set `AssignIdentityParameterSet` for cmdlet `Update-AzVM` has been removed.</span></span>

### `New-AzProximityPlacementGroup`

- <span data-ttu-id="55533-146">プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-146">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="55533-147">`Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-147">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-148">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-148">Before</span></span>

```powershell
PS C:\> New-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName -Location $location -Tag @{key1 = 'val1'} | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : Standard
VirtualMachinesColocationStatus         : {}
VirtualMachineScaleSetsColocationStatus : {}
AvailabilitySetsColocationStatus        : {}
ColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

#### <a name="after"></a><span data-ttu-id="55533-149">After</span><span class="sxs-lookup"><span data-stu-id="55533-149">After</span></span>

```powershell
PS C:\> New-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName -Location $location -Tag @{key1 = 'val1'} | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : StandardColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

### `Remove-AzProximityPlacementGroup`

- <span data-ttu-id="55533-150">プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-150">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="55533-151">`Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-151">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-152">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-152">Before</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Remove-AzProximityPlacementGroup | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : Standard
VirtualMachinesColocationStatus         : {}
VirtualMachineScaleSetsColocationStatus : {}
AvailabilitySetsColocationStatus        : {}
ColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

#### <a name="after"></a><span data-ttu-id="55533-153">After</span><span class="sxs-lookup"><span data-stu-id="55533-153">After</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Remove-AzProximityPlacementGroup | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : StandardColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

### `Get-AzProximityPlacementGroup`

- <span data-ttu-id="55533-154">プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-154">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="55533-155">`Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-155">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-156">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-156">Before</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : Standard
VirtualMachinesColocationStatus         : {}
VirtualMachineScaleSetsColocationStatus : {}
AvailabilitySetsColocationStatus        : {}
ColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

#### <a name="after"></a><span data-ttu-id="55533-157">After</span><span class="sxs-lookup"><span data-stu-id="55533-157">After</span></span>

```powershell
PS C:\> Get-AzProximityPlacementGroup -ResourceGroupName $resourceGroupName -Name $proximityPlacementGroupName | Format-List

ResourceGroupName                       : $resourceGroupName
ProximityPlacementGroupType             : StandardColocationStatus                        :
Id                                      : /subscriptions/9e223dbe-3399-4e19-88eb-0975f02ac87f/resourceGroups/$resourceGroupName/providers/Microsoft.Compute/proximityPlacementGroups/$proximityPlacementGroupName
Name                                    : $proximityPlacementGroupName
Type                                    : Microsoft.Compute/proximityPlacementGroups
Location                                : $location
Tags                                    : {[key1, val1]}
VirtualMachines                         : {}
VirtualMachineScaleSets                 : {}
AvailabilitySets                        : {}
```

### `Add-AzVmssAdditionalUnattendContent`

<span data-ttu-id="55533-158">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-158">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssDataDisk`

<span data-ttu-id="55533-159">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-159">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssExtension`

<span data-ttu-id="55533-160">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-160">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="55533-161">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-161">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSecret`

<span data-ttu-id="55533-162">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-162">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSshPublicKey`

<span data-ttu-id="55533-163">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-163">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssWinRMListener`

<span data-ttu-id="55533-164">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-164">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmssConfig`

- <span data-ttu-id="55533-165">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-165">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="55533-166">パラメーター `AutomaticRepairMaxInstanceRepairsPercent` はサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-166">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-167">パラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-167">No longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-168">パラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-168">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="55533-169">パラメーター セット `ExplicitIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-169">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>
- <span data-ttu-id="55533-170">パラメーター セット `AssignIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-170">The parameter set `AssignIdentityParameterSet` has been removed.</span></span>

### `Remove-AzVmssDataDisk`

<span data-ttu-id="55533-171">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-171">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssExtension`

<span data-ttu-id="55533-172">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-172">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="55533-173">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-173">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssBootDiagnostic`

<span data-ttu-id="55533-174">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-174">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOsProfile`

<span data-ttu-id="55533-175">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-175">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssRollingUpgradePolicy`

<span data-ttu-id="55533-176">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-176">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssStorageProfile`

<span data-ttu-id="55533-177">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-177">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmss`

<span data-ttu-id="55533-178">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-178">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Repair-AzVmssServiceFabricUpdateDomain`

<span data-ttu-id="55533-179">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-179">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVmss`

<span data-ttu-id="55533-180">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-180">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOrchestrationServiceState`

<span data-ttu-id="55533-181">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-181">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Update-AzVmss`

- <span data-ttu-id="55533-182">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-182">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="55533-183">パラメーター `AutomaticRepairMaxInstanceRepairsPercent` はサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-183">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-184">パラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-184">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="55533-185">パラメーター セット `ExplicitIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-185">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>

### `Add-AzVmssDiagnosticsExtension`

<span data-ttu-id="55533-186">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-186">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Disable-AzVmssDiskEncryption`

<span data-ttu-id="55533-187">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-187">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

## <a name="azkeyvault"></a><span data-ttu-id="55533-188">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55533-188">Az.KeyVault</span></span>

### `New-AzKeyVaultCertificateOrganizationDetail`

<span data-ttu-id="55533-189">別名 `New-AzKeyVaultCertificateOrganizationDetails` は削除されています。</span><span class="sxs-lookup"><span data-stu-id="55533-189">The alias `New-AzKeyVaultCertificateOrganizationDetails` is removed.</span></span> <span data-ttu-id="55533-190">`New-AzKeyVaultCertificateOrganizationDetail` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="55533-190">Please use `New-AzKeyVaultCertificateOrganizationDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-191">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-191">Before</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetails -AdministratorDetails $AdminDetails
```

#### <a name="after"></a><span data-ttu-id="55533-192">After</span><span class="sxs-lookup"><span data-stu-id="55533-192">After</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetail -AdministratorDetails $AdminDetails
```

### `New-AzKeyVaultCertificateAdministratorDetail`

<span data-ttu-id="55533-193">別名 `New-AzKeyVaultCertificateAdministratorDetails` は削除されています。</span><span class="sxs-lookup"><span data-stu-id="55533-193">The alias `New-AzKeyVaultCertificateAdministratorDetails` is removed.</span></span> <span data-ttu-id="55533-194">`New-AzKeyVaultCertificateAdministratorDetail` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="55533-194">Please use `New-AzKeyVaultCertificateAdministratorDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-195">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-195">Before</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetails -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

#### <a name="after"></a><span data-ttu-id="55533-196">After</span><span class="sxs-lookup"><span data-stu-id="55533-196">After</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetail -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

### `New-AzKeyVault`

<span data-ttu-id="55533-197">論理的な削除が既定で有効になっているため、`-EnableSoftDelete` は削除されています。</span><span class="sxs-lookup"><span data-stu-id="55533-197">`-EnableSoftDelete` is removed, as soft delete is enabled by default.</span></span> <span data-ttu-id="55533-198">この動作を希望しない場合は、`-DisableSoftDelete` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="55533-198">Please use `-DisableSoftDelete` if you do not want this behavior.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-199">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-199">Before</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US' -EnableSoftDelete
```

#### <a name="after"></a><span data-ttu-id="55533-200">After</span><span class="sxs-lookup"><span data-stu-id="55533-200">After</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US'
```

## <a name="azmonitor"></a><span data-ttu-id="55533-201">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="55533-201">Az.Monitor</span></span>

### `Add-AzLogProfile`

<span data-ttu-id="55533-202">`Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` 型のプロパティ `RetentionPolicy` の型が、`Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` から `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-202">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `Get-AzLogProfile`

<span data-ttu-id="55533-203">`Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` 型のプロパティ `RetentionPolicy` の型が、`Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` から `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-203">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `New-AzMetricAlertRuleV2Criteria`

<span data-ttu-id="55533-204">コマンドレット `New-AzMetricAlertRuleV2Criteria` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-204">The parameter set `__AllParameterSets` for cmdlet `New-AzMetricAlertRuleV2Criteria` has been removed.</span></span>

## <a name="aznetwork"></a><span data-ttu-id="55533-205">Az.Network</span><span class="sxs-lookup"><span data-stu-id="55533-205">Az.Network</span></span>

### `Get-AzNetworkWatcherConnectionMonitor`

<span data-ttu-id="55533-206">プロパティ `RoundTripTimeMs` のジェネリック型が `System.Nullable1[System.Int32]` から `System.Nullable1[System.Double]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-206">The generic type for property `RoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

### `New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`

<span data-ttu-id="55533-207">パラメーター `SuccessThresholdRoundTripTimeMs` のジェネリック型が `System.Nullable1[System.Int32]` から `System.Nullable1[System.Double]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-207">The generic type for parameter `SuccessThresholdRoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

## <a name="azoperationalinsights"></a><span data-ttu-id="55533-208">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="55533-208">Az.OperationalInsights</span></span>

### `Get-AzOperationalInsightsDataSource`

<span data-ttu-id="55533-209">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-209">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsApplicationInsightsDataSource`

<span data-ttu-id="55533-210">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-210">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsAzureActivityLogDataSource`

<span data-ttu-id="55533-211">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-211">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsCustomLogDataSource`

<span data-ttu-id="55533-212">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-212">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxPerformanceObjectDataSource`

<span data-ttu-id="55533-213">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-213">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxSyslogDataSource`

<span data-ttu-id="55533-214">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-214">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsEventDataSource`

<span data-ttu-id="55533-215">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-215">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsPerformanceCounterDataSource`

<span data-ttu-id="55533-216">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-216">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsDataSource`

<span data-ttu-id="55533-217">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-217">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="55533-218">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-218">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="55533-219">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-219">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="55533-220">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-220">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="55533-221">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-221">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="55533-222">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-222">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="55533-223">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-223">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="55533-224">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-224">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="55533-225">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-225">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearch`

<span data-ttu-id="55533-226">`Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` 型の `Metadata` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-226">The property `Metadata` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearchResult`

<span data-ttu-id="55533-227">コマンドレット `Get-AzOperationalInsightsSavedSearchResult` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-227">The cmdlet `Get-AzOperationalInsightsSavedSearchResult` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Get-AzOperationalInsightsSearchResult`

<span data-ttu-id="55533-228">コマンドレット `Get-AzOperationalInsightsSearchResult` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-228">The cmdlet `Get-AzOperationalInsightsSearchResult` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Get-AzOperationalInsightsStorageInsight`

<span data-ttu-id="55533-229">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-229">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsStorageInsight`

<span data-ttu-id="55533-230">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-230">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsStorageInsight`

<span data-ttu-id="55533-231">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-231">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsStorageInsight`

<span data-ttu-id="55533-232">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-232">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsLinkTarget`

<span data-ttu-id="55533-233">コマンドレット `Get-AzOperationalInsightsLinkTarget` が削除され、元のコマンドレット名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-233">The cmdlet `Get-AzOperationalInsightsLinkTarget` has been removed and no alias was found for the original cmdlet name.</span></span>

### `Get-AzOperationalInsightsWorkspace`

<span data-ttu-id="55533-234">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-234">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWorkspace`

- <span data-ttu-id="55533-235">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-235">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>
- <span data-ttu-id="55533-236">コマンドレット `New-AzOperationalInsightsWorkspace` でパラメーター `CustomerId` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="55533-236">The cmdlet `New-AzOperationalInsightsWorkspace` no longer supports the parameter `CustomerId` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="55533-237">コマンドレット `New-AzOperationalInsightsWorkspace` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-237">The parameter set `__AllParameterSets` for cmdlet `New-AzOperationalInsightsWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsWorkspace`

<span data-ttu-id="55533-238">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-238">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Invoke-AzOperationalInsightsQuery`

<span data-ttu-id="55533-239">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-239">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

## <a name="azresources"></a><span data-ttu-id="55533-240">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="55533-240">Az.Resources</span></span>

### `Get-AzDeploymentScript`

<span data-ttu-id="55533-241">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-241">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzDeploymentScriptLog`

<span data-ttu-id="55533-242">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-242">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Save-AzDeploymentScriptLog`

<span data-ttu-id="55533-243">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-243">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`

<span data-ttu-id="55533-244">パラメーター `TenantLevel` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-244">Parameter `TenantLevel` has been removed.</span></span>

### `Get-AzPolicyAlias`

<span data-ttu-id="55533-245">プロパティ `Aliases` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-245">The generic type for property `Aliases` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]`.</span></span>

### `New-AzPolicyAssignment`

- <span data-ttu-id="55533-246">コマンドレット `New-AzPolicyAssignment` では、パラメーター `PolicyDefinition` の `System.Management.Automation.PSObject` 型はサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="55533-246">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicyDefinition`.</span></span>
- <span data-ttu-id="55533-247">コマンドレット `New-AzPolicyAssignment` では、パラメーター `PolicySetDefinition` の `System.Management.Automation.PSObject` 型はサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="55533-247">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicySetDefinition`.</span></span>

### `Remove-AzDeploymentScript`

<span data-ttu-id="55533-248">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-248">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

## <a name="azstorage"></a><span data-ttu-id="55533-249">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="55533-249">Az.Storage</span></span>

### <a name="update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset"></a><span data-ttu-id="55533-250">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="55533-250">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>

<span data-ttu-id="55533-251">NetWorkRule の DefaultAction 値が、Allow = 1、Deny = 0 から Allow = 0、Deny = 1 に変更されました。</span><span class="sxs-lookup"><span data-stu-id="55533-251">Changed NetWorkRule DefaultAction value from: Allow = 1, Deny = 0, to: Allow = 0, Deny = 1.</span></span>

### <a name="new-azstoragetable-get-azstoragetable"></a><span data-ttu-id="55533-252">`New-AzStorageTable`, `Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="55533-252">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>

<span data-ttu-id="55533-253">出力オブジェクト AzureStorageTable.CloudTable.ServiceClient で 2 つのプロパティ ConnectionPolicy と ConsistencyLevel が削除されました。</span><span class="sxs-lookup"><span data-stu-id="55533-253">Output object AzureStorageTable.CloudTable.ServiceClient have 2 properties removed: ConnectionPolicy, ConsistencyLevel.</span></span>

### <a name="get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy"></a><span data-ttu-id="55533-254">`Get-AzStorageFile`、`Remove-AzStorageFile`、`Get-AzStorageFileContent`、`Set-AzStorageFileContent`、`Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="55533-254">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>

<span data-ttu-id="55533-255">出力の種類が CloudFile から AzureStorageFile に変更されています。元の出力は新しい出力の子プロパティ "CloudFile" になります</span><span class="sxs-lookup"><span data-stu-id="55533-255">Change output type from CloudFile to AzureStorageFile, the original output will become child property "CloudFile" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="55533-256">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-256">Before</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file
```

#### <a name="after"></a><span data-ttu-id="55533-257">After</span><span class="sxs-lookup"><span data-stu-id="55533-257">After</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file.CloudFile
```

### <a name="get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory"></a><span data-ttu-id="55533-258">`Get-AzStorageFile`、`New-AzStorageDirectory`、`Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="55533-258">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>

<span data-ttu-id="55533-259">出力の種類が CloudFileDirectory から AzureStorageFileDirectory に変更されています。元の出力は新しい出力の子プロパティ "CloudFileDirectory" になります</span><span class="sxs-lookup"><span data-stu-id="55533-259">Change output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become child property "CloudFileDirectory" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="55533-260">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-260">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="55533-261">After</span><span class="sxs-lookup"><span data-stu-id="55533-261">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```

### <a name="get-azstorageshare-new-azstorageshare-remove-azstorageshare"></a><span data-ttu-id="55533-262">`Get-AzStorageShare`、`New-AzStorageShare`、`Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="55533-262">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>

<span data-ttu-id="55533-263">出力の種類が FileShareProperties から AzureStorageFileShare に変更されています。元の出力は新しい出力の子プロパティ "CloudFileShare" になります</span><span class="sxs-lookup"><span data-stu-id="55533-263">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become child property "CloudFileShare" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="55533-264">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-264">Before</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share
```

#### <a name="after"></a><span data-ttu-id="55533-265">After</span><span class="sxs-lookup"><span data-stu-id="55533-265">After</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share.CloudFileShare
```

### `Set-AzStorageShareQuota`

<span data-ttu-id="55533-266">出力の種類が FileShareProperties から AzureStorageFileShare に変更されています。元の出力は新しい出力のサブの子プロパティ ""CloudFileShare.Properties"" になります</span><span class="sxs-lookup"><span data-stu-id="55533-266">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become sub child property ""CloudFileShare.Properties"" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="55533-267">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-267">Before</span></span>

```powershell
PS C:\> $shareProperties = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $shareProperties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

#### <a name="after"></a><span data-ttu-id="55533-268">After</span><span class="sxs-lookup"><span data-stu-id="55533-268">After</span></span>

```powershell
PS C:\> $share = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $share

   File End Point: https://weiors1.file.core.windows.net/

Name     QuotaGiB LastModified                IsSnapshot SnapshotTime
----     -------- ------------                ---------- ------------
weitest1 100      5/11/2020 3:03:30 PM +00:00 False

PS C:\> $share.CloudFileShare.Properties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

### `Remove-AzStorageDirectory`

<span data-ttu-id="55533-269">親ディレクトリ オブジェクトと -Path を指定してサブ ファイル ディレクトリを削除すると、型 (文字列) の一致を使用してパイプラインから -Path を入力できなくなります。</span><span class="sxs-lookup"><span data-stu-id="55533-269">When removing sub File Directories with parent Directory object and -Path, Can't input -Path from pipeline with type (string) match anymore.</span></span>

#### <a name="before"></a><span data-ttu-id="55533-270">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="55533-270">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> @('dir1', 'dir2') | Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="55533-271">After</span><span class="sxs-lookup"><span data-stu-id="55533-271">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> $paths = @(
    [PSCustomObject]@{  Path = 'dir1 }
    [PSCustomObject]@{ Path = 'dir2' }
)

PS C:\> $paths | Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```
