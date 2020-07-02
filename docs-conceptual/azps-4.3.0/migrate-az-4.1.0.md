---
title: Az 4.1.0 の移行ガイド
description: この移行ガイドには、Az バージョン 4.1.0 リリースの Azure PowerShell で行われた破壊的変更が記載されています。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/23/2020
ms.openlocfilehash: e3a4563acf4b0820b61a2ac5da244b26490c8174
ms.sourcegitcommit: 747769a143ddebff39e78c2cc62a182401adddb9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2020
ms.locfileid: "85268085"
---
# <a name="migration-guide-for-az-410"></a><span data-ttu-id="af34c-103">Az 4.1.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="af34c-103">Migration Guide for Az 4.1.0</span></span>

<span data-ttu-id="af34c-104">このドキュメントでは、Az のバージョン 3.0.0 と 4.1.0 の間での変更点について説明します。</span><span class="sxs-lookup"><span data-stu-id="af34c-104">This document describes the changes between the 3.0.0 and 4.1.0 versions of Az.</span></span>

- [<span data-ttu-id="af34c-105">Az 4.1.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="af34c-105">Migration Guide for Az 4.1.0</span></span>](#migration-guide-for-az-410)
  - [<span data-ttu-id="af34c-106">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af34c-106">Az.ApiManagement</span></span>](#azapimanagement)
    - [`Add-AzApiManagementRegion`](#add-azapimanagementregion)
    - [`New-AzApiManagement`](#new-azapimanagement)
    - [`Set-AzApiManagement`](#set-azapimanagement)
    - [`Get-AzApiManagementProperty`](#get-azapimanagementproperty)
    - [`New-AzApiManagementProperty`](#new-azapimanagementproperty)
    - [`Remove-AzApiManagementProperty`](#remove-azapimanagementproperty)
    - [`Set-AzApiManagementProperty`](#set-azapimanagementproperty)
  - [<span data-ttu-id="af34c-107">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="af34c-107">Az.Batch</span></span>](#azbatch)
    - [<span data-ttu-id="af34c-108">`Get-AzBatchApplication`、`New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="af34c-108">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>](#get-azbatchapplication-new-azbatchapplication)
    - [<span data-ttu-id="af34c-109">`Get-AzBatchComputeNode`、`New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="af34c-109">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>](#get-azbatchcomputenode-new-azbatchpool)
    - [<span data-ttu-id="af34c-110">`Get-AzBatchApplicationPackage`、`New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="af34c-110">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>](#get-azbatchapplicationpackage-new-azbatchapplicationpackage)
  - [<span data-ttu-id="af34c-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af34c-111">Az.Compute</span></span>](#azcompute)
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
  - [<span data-ttu-id="af34c-112">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af34c-112">Az.KeyVault</span></span>](#azkeyvault)
    - [`New-AzKeyVaultCertificateOrganizationDetail`](#new-azkeyvaultcertificateorganizationdetail)
    - [`New-AzKeyVaultCertificateAdministratorDetail`](#new-azkeyvaultcertificateadministratordetail)
    - [`New-AzKeyVault`](#new-azkeyvault)
  - [<span data-ttu-id="af34c-113">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af34c-113">Az.Monitor</span></span>](#azmonitor)
    - [`Add-AzLogProfile`](#add-azlogprofile)
    - [`Get-AzLogProfile`](#get-azlogprofile)
    - [`New-AzMetricAlertRuleV2Criteria`](#new-azmetricalertrulev2criteria)
  - [<span data-ttu-id="af34c-114">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af34c-114">Az.Network</span></span>](#aznetwork)
    - [`Get-AzNetworkWatcherConnectionMonitor`](#get-aznetworkwatcherconnectionmonitor)
    - [`New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`](#new-aznetworkwatcherconnectionmonitortestconfigurationobject)
  - [<span data-ttu-id="af34c-115">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af34c-115">Az.OperationalInsights</span></span>](#azoperationalinsights)
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
  - [<span data-ttu-id="af34c-116">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af34c-116">Az.Resources</span></span>](#azresources)
    - [`Get-AzDeploymentScript`](#get-azdeploymentscript)
    - [`Get-AzDeploymentScriptLog`](#get-azdeploymentscriptlog)
    - [`Save-AzDeploymentScriptLog`](#save-azdeploymentscriptlog)
    - [`Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`](#get-azresourcelock-new-azresourcelock-remove-azresourcelock-set-azresourcelock)
    - [`Get-AzPolicyAlias`](#get-azpolicyalias)
    - [`New-AzPolicyAssignment`](#new-azpolicyassignment)
    - [`Remove-AzDeploymentScript`](#remove-azdeploymentscript)
  - [<span data-ttu-id="af34c-117">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af34c-117">Az.Storage</span></span>](#azstorage)
    - [<span data-ttu-id="af34c-118">`Update-AzStorageAccountNetworkRuleSet`、`Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="af34c-118">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>](#update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset)
    - [<span data-ttu-id="af34c-119">`New-AzStorageTable`、`Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="af34c-119">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>](#new-azstoragetable-get-azstoragetable)
    - [<span data-ttu-id="af34c-120">`Get-AzStorageFile`、`Remove-AzStorageFile`、`Get-AzStorageFileContent`、`Set-AzStorageFileContent`、`Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="af34c-120">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>](#get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy)
    - [<span data-ttu-id="af34c-121">`Get-AzStorageFile`、`New-AzStorageDirectory`、`Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="af34c-121">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>](#get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory)
    - [<span data-ttu-id="af34c-122">`Get-AzStorageShare`、`New-AzStorageShare`、`Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="af34c-122">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>](#get-azstorageshare-new-azstorageshare-remove-azstorageshare)
    - [`Set-AzStorageShareQuota`](#set-azstoragesharequota)
    - [`Remove-AzStorageDirectory`](#remove-azstoragedirectory)

## <a name="azapimanagement"></a><span data-ttu-id="af34c-123">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af34c-123">Az.ApiManagement</span></span>

### `Add-AzApiManagementRegion`

<span data-ttu-id="af34c-124">`Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` 型のプロパティ `Type` の型が、`Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` から `System.String` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-124">The type of property `Type` of type `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` has changed from `Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` to `System.String`.</span></span>

### `New-AzApiManagement`

- <span data-ttu-id="af34c-125">コマンドレット `New-AzApiManagement` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-125">The cmdlet `New-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-126">コマンドレット `New-AzApiManagement` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-126">The parameter set `__AllParameterSets` for cmdlet `New-AzApiManagement` has been removed.</span></span>

### `Set-AzApiManagement`

- <span data-ttu-id="af34c-127">コマンドレット `Set-AzApiManagement` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-127">The cmdlet `Set-AzApiManagement` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-128">コマンドレット `Set-AzApiManagement` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-128">The parameter set `__AllParameterSets` for cmdlet `Set-AzApiManagement` has been removed.</span></span>

### `Get-AzApiManagementProperty`

<span data-ttu-id="af34c-129">コマンドレット `Get-AzApiManagementProperty` が `Get-AzureApiManagementNamedValue` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af34c-129">The cmdlet `Get-AzApiManagementProperty` has been replaced by `Get-AzureApiManagementNamedValue`.</span></span>

### `New-AzApiManagementProperty`

<span data-ttu-id="af34c-130">コマンドレット `New-AzApiManagementProperty` が `New-AzureApiManagementNamedValue` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af34c-130">The cmdlet `New-AzApiManagementProperty` has been replaced by `New-AzureApiManagementNamedValue`.</span></span>

### `Remove-AzApiManagementProperty`

<span data-ttu-id="af34c-131">コマンドレット `Remove-AzApiManagementProperty` が `Remove-AzureApiManagementNamedValue` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af34c-131">The cmdlet `Remove-AzApiManagementProperty` has been replaced by `Remove-AzureApiManagementNamedValue`.</span></span>

### `Set-AzApiManagementProperty`

<span data-ttu-id="af34c-132">コマンドレット `Set-AzApiManagementProperty` が `Set-AzureApiManagementNamedValue` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="af34c-132">The cmdlet `Set-AzApiManagementProperty` has been replaced by `Set-AzureApiManagementNamedValue`.</span></span>

## <a name="azbatch"></a><span data-ttu-id="af34c-133">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="af34c-133">Az.Batch</span></span>

### <a name="get-azbatchapplication-new-azbatchapplication"></a><span data-ttu-id="af34c-134">`Get-AzBatchApplication`, `New-AzBatchApplication`</span><span class="sxs-lookup"><span data-stu-id="af34c-134">`Get-AzBatchApplication`, `New-AzBatchApplication`</span></span>

<span data-ttu-id="af34c-135">`Microsoft.Azure.Commands.Batch.Models.PSApplication` 型の `ApplicationPackages` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-135">The property `ApplicationPackages` of type `Microsoft.Azure.Commands.Batch.Models.PSApplication` has been removed.</span></span>

### <a name="get-azbatchcomputenode-new-azbatchpool"></a><span data-ttu-id="af34c-136">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span><span class="sxs-lookup"><span data-stu-id="af34c-136">`Get-AzBatchComputeNode`, `New-AzBatchPool`</span></span>

<span data-ttu-id="af34c-137">`Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` 型の `PublicIPs` プロパティが削除されました</span><span class="sxs-lookup"><span data-stu-id="af34c-137">The property `PublicIPs` of type `Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` has been removed</span></span>

### <a name="get-azbatchapplicationpackage-new-azbatchapplicationpackage"></a><span data-ttu-id="af34c-138">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span><span class="sxs-lookup"><span data-stu-id="af34c-138">`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`</span></span>

<span data-ttu-id="af34c-139">`Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` 型のプロパティ `StorageUrlExpiry` の型が、`System.DateTime` から `System.DateTime?` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-139">The type of property `StorageUrlExpiry` of type `Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` has changed from `System.DateTime` to `System.DateTime?`.</span></span>

## <a name="azcompute"></a><span data-ttu-id="af34c-140">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af34c-140">Az.Compute</span></span>

### `Remove-AzVmssDiagnosticsExtension`

<span data-ttu-id="af34c-141">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-141">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVMImage`

- <span data-ttu-id="af34c-142">コマンドレット `Get-AzVMImage` でパラメーター `FilterExpression` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-142">The cmdlet `Get-AzVMImage` no longer supports the parameter `FilterExpression` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-143">コマンドレット `Get-AzVMImage` のパラメーター セット `ListVMImage` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-143">The parameter set `ListVMImage` for cmdlet `Get-AzVMImage` has been removed.</span></span>

### `New-AzVMConfig`

- <span data-ttu-id="af34c-144">コマンドレット `New-AzVMConfig` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-144">The cmdlet `New-AzVMConfig` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-145">コマンドレット `New-AzVMConfig` のパラメーター セット `AssignIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-145">The parameter set `AssignIdentityParameterSet` for cmdlet `New-AzVMConfig` has been removed.</span></span>

### `Update-AzVM`

- <span data-ttu-id="af34c-146">コマンドレット `Update-AzVM` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-146">The cmdlet `Update-AzVM` no longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-147">コマンドレット `Update-AzVM` のパラメーター セット `AssignIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-147">The parameter set `AssignIdentityParameterSet` for cmdlet `Update-AzVM` has been removed.</span></span>

### `New-AzProximityPlacementGroup`

- <span data-ttu-id="af34c-148">プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-148">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="af34c-149">`Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-149">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-150">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-150">Before</span></span>

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

#### <a name="after"></a><span data-ttu-id="af34c-151">After</span><span class="sxs-lookup"><span data-stu-id="af34c-151">After</span></span>

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

- <span data-ttu-id="af34c-152">プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-152">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="af34c-153">`Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-153">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-154">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-154">Before</span></span>

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

#### <a name="after"></a><span data-ttu-id="af34c-155">After</span><span class="sxs-lookup"><span data-stu-id="af34c-155">After</span></span>

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

- <span data-ttu-id="af34c-156">プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-156">The generic type for property `VirtualMachines`, `VirtualMachineScaleSets`, and `AvailabilitySets` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]`.</span></span>
- <span data-ttu-id="af34c-157">`Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-157">The property `VirtualMachinesColocationStatus`, `VirtualMachineScaleSetsColocationStatus`, and `AvailabilitySetsColocationStatus` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` has been removed.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-158">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-158">Before</span></span>

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

#### <a name="after"></a><span data-ttu-id="af34c-159">After</span><span class="sxs-lookup"><span data-stu-id="af34c-159">After</span></span>

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

<span data-ttu-id="af34c-160">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-160">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssDataDisk`

<span data-ttu-id="af34c-161">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-161">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssExtension`

<span data-ttu-id="af34c-162">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-162">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="af34c-163">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-163">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSecret`

<span data-ttu-id="af34c-164">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-164">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssSshPublicKey`

<span data-ttu-id="af34c-165">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-165">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Add-AzVmssWinRMListener`

<span data-ttu-id="af34c-166">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-166">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmssConfig`

- <span data-ttu-id="af34c-167">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-167">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="af34c-168">パラメーター `AutomaticRepairMaxInstanceRepairsPercent` はサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-168">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-169">パラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-169">No longer supports the parameter `AssignIdentity` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-170">パラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-170">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="af34c-171">パラメーター セット `ExplicitIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-171">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>
- <span data-ttu-id="af34c-172">パラメーター セット `AssignIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-172">The parameter set `AssignIdentityParameterSet` has been removed.</span></span>

### `Remove-AzVmssDataDisk`

<span data-ttu-id="af34c-173">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-173">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssExtension`

<span data-ttu-id="af34c-174">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-174">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Remove-AzVmssNetworkInterfaceConfiguration`

<span data-ttu-id="af34c-175">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-175">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssBootDiagnostic`

<span data-ttu-id="af34c-176">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-176">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOsProfile`

<span data-ttu-id="af34c-177">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-177">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssRollingUpgradePolicy`

<span data-ttu-id="af34c-178">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-178">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssStorageProfile`

<span data-ttu-id="af34c-179">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-179">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `New-AzVmss`

<span data-ttu-id="af34c-180">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-180">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Repair-AzVmssServiceFabricUpdateDomain`

<span data-ttu-id="af34c-181">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-181">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Get-AzVmss`

<span data-ttu-id="af34c-182">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-182">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Set-AzVmssOrchestrationServiceState`

<span data-ttu-id="af34c-183">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-183">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Update-AzVmss`

- <span data-ttu-id="af34c-184">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-184">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>
- <span data-ttu-id="af34c-185">パラメーター `AutomaticRepairMaxInstanceRepairsPercent` はサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-185">No longer supports the parameter `AutomaticRepairMaxInstanceRepairsPercent` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-186">パラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-186">The parameter set `__AllParameterSets` has been removed.</span></span>
- <span data-ttu-id="af34c-187">パラメーター セット `ExplicitIdentityParameterSet` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-187">The parameter set `ExplicitIdentityParameterSet` has been removed.</span></span>

### `Add-AzVmssDiagnosticsExtension`

<span data-ttu-id="af34c-188">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-188">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

### `Disable-AzVmssDiskEncryption`

<span data-ttu-id="af34c-189">`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-189">The type of property `AutomaticRepairsPolicy` of type `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` has changed from `Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` to `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy`.</span></span>

## <a name="azkeyvault"></a><span data-ttu-id="af34c-190">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af34c-190">Az.KeyVault</span></span>

### `New-AzKeyVaultCertificateOrganizationDetail`

<span data-ttu-id="af34c-191">別名 `New-AzKeyVaultCertificateOrganizationDetails` は削除されています。</span><span class="sxs-lookup"><span data-stu-id="af34c-191">The alias `New-AzKeyVaultCertificateOrganizationDetails` is removed.</span></span> <span data-ttu-id="af34c-192">`New-AzKeyVaultCertificateOrganizationDetail` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="af34c-192">Please use `New-AzKeyVaultCertificateOrganizationDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-193">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-193">Before</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetails -AdministratorDetails $AdminDetails
```

#### <a name="after"></a><span data-ttu-id="af34c-194">After</span><span class="sxs-lookup"><span data-stu-id="af34c-194">After</span></span>

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetail -AdministratorDetails $AdminDetails
```

### `New-AzKeyVaultCertificateAdministratorDetail`

<span data-ttu-id="af34c-195">別名 `New-AzKeyVaultCertificateAdministratorDetails` は削除されています。</span><span class="sxs-lookup"><span data-stu-id="af34c-195">The alias `New-AzKeyVaultCertificateAdministratorDetails` is removed.</span></span> <span data-ttu-id="af34c-196">`New-AzKeyVaultCertificateAdministratorDetail` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="af34c-196">Please use `New-AzKeyVaultCertificateAdministratorDetail`.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-197">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-197">Before</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetails -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

#### <a name="after"></a><span data-ttu-id="af34c-198">After</span><span class="sxs-lookup"><span data-stu-id="af34c-198">After</span></span>

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetail -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

### `New-AzKeyVault`

<span data-ttu-id="af34c-199">論理的な削除が既定で有効になっているため、`-EnableSoftDelete` は削除されています。</span><span class="sxs-lookup"><span data-stu-id="af34c-199">`-EnableSoftDelete` is removed, as soft delete is enabled by default.</span></span> <span data-ttu-id="af34c-200">この動作を希望しない場合は、`-DisableSoftDelete` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="af34c-200">Please use `-DisableSoftDelete` if you do not want this behavior.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-201">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-201">Before</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US' -EnableSoftDelete
```

#### <a name="after"></a><span data-ttu-id="af34c-202">After</span><span class="sxs-lookup"><span data-stu-id="af34c-202">After</span></span>

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US'
```

## <a name="azmonitor"></a><span data-ttu-id="af34c-203">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af34c-203">Az.Monitor</span></span>

### `Add-AzLogProfile`

<span data-ttu-id="af34c-204">`Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` 型のプロパティ `RetentionPolicy` の型が、`Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` から `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-204">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `Get-AzLogProfile`

<span data-ttu-id="af34c-205">`Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` 型のプロパティ `RetentionPolicy` の型が、`Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` から `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-205">The type of property `RetentionPolicy` of type `Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` has changed from `Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` to `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy`.</span></span>

### `New-AzMetricAlertRuleV2Criteria`

<span data-ttu-id="af34c-206">コマンドレット `New-AzMetricAlertRuleV2Criteria` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-206">The parameter set `__AllParameterSets` for cmdlet `New-AzMetricAlertRuleV2Criteria` has been removed.</span></span>

## <a name="aznetwork"></a><span data-ttu-id="af34c-207">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af34c-207">Az.Network</span></span>

### `Get-AzNetworkWatcherConnectionMonitor`

<span data-ttu-id="af34c-208">プロパティ `RoundTripTimeMs` のジェネリック型が `System.Nullable1[System.Int32]` から `System.Nullable1[System.Double]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-208">The generic type for property `RoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

### `New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`

<span data-ttu-id="af34c-209">パラメーター `SuccessThresholdRoundTripTimeMs` のジェネリック型が `System.Nullable1[System.Int32]` から `System.Nullable1[System.Double]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-209">The generic type for parameter `SuccessThresholdRoundTripTimeMs` has been changed from `System.Nullable1[System.Int32]` to `System.Nullable1[System.Double]`.</span></span>

## <a name="azoperationalinsights"></a><span data-ttu-id="af34c-210">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af34c-210">Az.OperationalInsights</span></span>

### `Get-AzOperationalInsightsDataSource`

<span data-ttu-id="af34c-211">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-211">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsApplicationInsightsDataSource`

<span data-ttu-id="af34c-212">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-212">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsAzureActivityLogDataSource`

<span data-ttu-id="af34c-213">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-213">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsCustomLogDataSource`

<span data-ttu-id="af34c-214">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-214">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxPerformanceObjectDataSource`

<span data-ttu-id="af34c-215">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-215">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsLinuxSyslogDataSource`

<span data-ttu-id="af34c-216">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-216">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsEventDataSource`

<span data-ttu-id="af34c-217">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-217">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWindowsPerformanceCounterDataSource`

<span data-ttu-id="af34c-218">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-218">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsDataSource`

<span data-ttu-id="af34c-219">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-219">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="af34c-220">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-220">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="af34c-221">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-221">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="af34c-222">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-222">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Disable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="af34c-223">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-223">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsIISLogCollection`

<span data-ttu-id="af34c-224">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-224">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxCustomLogCollection`

<span data-ttu-id="af34c-225">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-225">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxPerformanceCollection`

<span data-ttu-id="af34c-226">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-226">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Enable-AzOperationalInsightsLinuxSyslogCollection`

<span data-ttu-id="af34c-227">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-227">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearch`

<span data-ttu-id="af34c-228">`Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` 型の `Metadata` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-228">The property `Metadata` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` has been removed.</span></span>

### `Get-AzOperationalInsightsSavedSearchResult`

<span data-ttu-id="af34c-229">コマンドレット `Get-AzOperationalInsightsSavedSearchResult` は SDK でサポートされなくなったため、削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-229">The cmdlet `Get-AzOperationalInsightsSavedSearchResult` was not supported by SDK anymore and has been removed.</span></span>

### `Get-AzOperationalInsightsSearchResult`

<span data-ttu-id="af34c-230">コマンドレット `Get-AzOperationalInsightsSearchResult` は SDK でサポートされなくなったため、削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-230">The cmdlet `Get-AzOperationalInsightsSearchResult` was not supported by SDK anymore and has been removed.</span></span>

### `Get-AzOperationalInsightsStorageInsight`

<span data-ttu-id="af34c-231">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-231">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsStorageInsight`

<span data-ttu-id="af34c-232">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-232">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Remove-AzOperationalInsightsStorageInsight`

<span data-ttu-id="af34c-233">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-233">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsStorageInsight`

<span data-ttu-id="af34c-234">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-234">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Get-AzOperationalInsightsLinkTarget`

<span data-ttu-id="af34c-235">コマンドレット `Get-AzOperationalInsightsLinkTarget` は SDK でサポートされなくなったため、削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-235">The cmdlet `Get-AzOperationalInsightsLinkTarget` was not supported by SDK anymore and has been removed.</span></span>

### `Get-AzOperationalInsightsWorkspace`

<span data-ttu-id="af34c-236">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-236">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `New-AzOperationalInsightsWorkspace`

- <span data-ttu-id="af34c-237">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-237">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>
- <span data-ttu-id="af34c-238">コマンドレット `New-AzOperationalInsightsWorkspace` でパラメーター `CustomerId` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="af34c-238">The cmdlet `New-AzOperationalInsightsWorkspace` no longer supports the parameter `CustomerId` and no alias was found for the original parameter name.</span></span>
- <span data-ttu-id="af34c-239">コマンドレット `New-AzOperationalInsightsWorkspace` のパラメーター セット `__AllParameterSets` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-239">The parameter set `__AllParameterSets` for cmdlet `New-AzOperationalInsightsWorkspace` has been removed.</span></span>

### `Set-AzOperationalInsightsWorkspace`

<span data-ttu-id="af34c-240">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-240">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

### `Invoke-AzOperationalInsightsQuery`

<span data-ttu-id="af34c-241">`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-241">The property `PortalUrl` of type `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` has been removed.</span></span>

## <a name="azresources"></a><span data-ttu-id="af34c-242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af34c-242">Az.Resources</span></span>

### `Get-AzDeploymentScript`

<span data-ttu-id="af34c-243">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-243">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzDeploymentScriptLog`

<span data-ttu-id="af34c-244">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-244">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Save-AzDeploymentScriptLog`

<span data-ttu-id="af34c-245">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-245">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

### `Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`

<span data-ttu-id="af34c-246">パラメーター `TenantLevel` は削除されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-246">Parameter `TenantLevel` has been removed.</span></span>

### `Get-AzPolicyAlias`

<span data-ttu-id="af34c-247">プロパティ `Aliases` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-247">The generic type for property `Aliases` has been changed from `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` to `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]`.</span></span>

### `New-AzPolicyAssignment`

- <span data-ttu-id="af34c-248">コマンドレット `New-AzPolicyAssignment` では、パラメーター `PolicyDefinition` の `System.Management.Automation.PSObject` 型はサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="af34c-248">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicyDefinition`.</span></span>
- <span data-ttu-id="af34c-249">コマンドレット `New-AzPolicyAssignment` では、パラメーター `PolicySetDefinition` の `System.Management.Automation.PSObject` 型はサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="af34c-249">The cmdlet `New-AzPolicyAssignment` no longer supports the type `System.Management.Automation.PSObject` for parameter `PolicySetDefinition`.</span></span>

### `Remove-AzDeploymentScript`

<span data-ttu-id="af34c-250">`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="af34c-250">The type of property `Status` of type `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` has changed from `Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` to `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus`.</span></span>

## <a name="azstorage"></a><span data-ttu-id="af34c-251">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af34c-251">Az.Storage</span></span>

### <a name="update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset"></a><span data-ttu-id="af34c-252">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span><span class="sxs-lookup"><span data-stu-id="af34c-252">`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`</span></span>

<span data-ttu-id="af34c-253">NetWorkRule DefaultAction の値が以下のように変更されました。Allow = 1、Deny = 0 が以下になります。Allow = 0、Deny = 1。</span><span class="sxs-lookup"><span data-stu-id="af34c-253">Changed NetWorkRule DefaultAction value from: Allow = 1, Deny = 0, to: Allow = 0, Deny = 1.</span></span>

### <a name="new-azstoragetable-get-azstoragetable"></a><span data-ttu-id="af34c-254">`New-AzStorageTable`, `Get-AzStorageTable`</span><span class="sxs-lookup"><span data-stu-id="af34c-254">`New-AzStorageTable`, `Get-AzStorageTable`</span></span>

<span data-ttu-id="af34c-255">出力オブジェクト AzureStorageTable.CloudTable.ServiceClient で 2 つのプロパティが削除されました。ConnectionPolicy、ConsistencyLevel。</span><span class="sxs-lookup"><span data-stu-id="af34c-255">Output object AzureStorageTable.CloudTable.ServiceClient have 2 properties removed: ConnectionPolicy, ConsistencyLevel.</span></span>

### <a name="get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy"></a><span data-ttu-id="af34c-256">`Get-AzStorageFile`、`Remove-AzStorageFile`、`Get-AzStorageFileContent`、`Set-AzStorageFileContent`、`Start-AzStorageFileCopy`</span><span class="sxs-lookup"><span data-stu-id="af34c-256">`Get-AzStorageFile`, `Remove-AzStorageFile`, `Get-AzStorageFileContent`, `Set-AzStorageFileContent`, `Start-AzStorageFileCopy`</span></span>

<span data-ttu-id="af34c-257">出力の種類が CloudFile から AzureStorageFile に変更されています。元の出力は新しい出力の子プロパティ "CloudFile" になります</span><span class="sxs-lookup"><span data-stu-id="af34c-257">Change output type from CloudFile to AzureStorageFile, the original output will become child property "CloudFile" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-258">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-258">Before</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file
```

#### <a name="after"></a><span data-ttu-id="af34c-259">After</span><span class="sxs-lookup"><span data-stu-id="af34c-259">After</span></span>

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file.CloudFile
```

### <a name="get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory"></a><span data-ttu-id="af34c-260">`Get-AzStorageFile`、`New-AzStorageDirectory`、`Remove-AzStorageDirectory`</span><span class="sxs-lookup"><span data-stu-id="af34c-260">`Get-AzStorageFile`, `New-AzStorageDirectory`, `Remove-AzStorageDirectory`</span></span>

<span data-ttu-id="af34c-261">出力の種類が CloudFileDirectory から AzureStorageFileDirectory に変更されています。元の出力は新しい出力の子プロパティ "CloudFileDirectory" になります</span><span class="sxs-lookup"><span data-stu-id="af34c-261">Change output type from CloudFileDirectory to AzureStorageFileDirectory, the original output will become child property "CloudFileDirectory" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-262">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-262">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="af34c-263">After</span><span class="sxs-lookup"><span data-stu-id="af34c-263">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```

### <a name="get-azstorageshare-new-azstorageshare-remove-azstorageshare"></a><span data-ttu-id="af34c-264">`Get-AzStorageShare`、`New-AzStorageShare`、`Remove-AzStorageShare`</span><span class="sxs-lookup"><span data-stu-id="af34c-264">`Get-AzStorageShare`, `New-AzStorageShare`, `Remove-AzStorageShare`</span></span>

<span data-ttu-id="af34c-265">出力の種類が FileShareProperties から AzureStorageFileShare に変更されています。元の出力は新しい出力の子プロパティ "CloudFileShare" になります</span><span class="sxs-lookup"><span data-stu-id="af34c-265">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become child property "CloudFileShare" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-266">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-266">Before</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share
```

#### <a name="after"></a><span data-ttu-id="af34c-267">After</span><span class="sxs-lookup"><span data-stu-id="af34c-267">After</span></span>

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share.CloudFileShare
```

### `Set-AzStorageShareQuota`

<span data-ttu-id="af34c-268">出力の種類が FileShareProperties から AzureStorageFileShare に変更されています。元の出力は新しい出力のサブの子プロパティ ""CloudFileShare.Properties"" になります</span><span class="sxs-lookup"><span data-stu-id="af34c-268">Change output type from FileShareProperties to AzureStorageFileShare, the original output will become sub child property ""CloudFileShare.Properties"" of the new output</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-269">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-269">Before</span></span>

```powershell
PS C:\> $shareProperties = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $shareProperties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

#### <a name="after"></a><span data-ttu-id="af34c-270">After</span><span class="sxs-lookup"><span data-stu-id="af34c-270">After</span></span>

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

<span data-ttu-id="af34c-271">親ディレクトリ オブジェクトと -Path を指定してサブ ファイル ディレクトリを削除すると、型 (文字列) の一致を使用してパイプラインから -Path を入力できなくなります。</span><span class="sxs-lookup"><span data-stu-id="af34c-271">When removing sub File Directories with parent Directory object and -Path, Can't input -Path from pipeline with type (string) match anymore.</span></span>

#### <a name="before"></a><span data-ttu-id="af34c-272">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="af34c-272">Before</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> @('dir1', 'dir2') | Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a><span data-ttu-id="af34c-273">After</span><span class="sxs-lookup"><span data-stu-id="af34c-273">After</span></span>

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> $paths = @(
    [PSCustomObject]@{  Path = 'dir1 }
    [PSCustomObject]@{ Path = 'dir2' }
)

PS C:\> $paths | Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```
