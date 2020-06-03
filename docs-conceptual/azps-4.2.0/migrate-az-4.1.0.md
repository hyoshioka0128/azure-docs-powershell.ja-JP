---
title: Az 4.1.0 の移行ガイド
description: この移行ガイドには、Az バージョン 4.1.0 リリースの Azure PowerShell で行われた破壊的変更が記載されています。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/23/2020
ms.openlocfilehash: e3a4563acf4b0820b61a2ac5da244b26490c8174
ms.sourcegitcommit: cef87acc9f2a0d296bef74f526afd2e067e8146b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "84299045"
---
# <a name="migration-guide-for-az-410"></a>Az 4.1.0 の移行ガイド

このドキュメントでは、Az のバージョン 3.0.0 と 4.1.0 の間での変更点について説明します。

- [Az 4.1.0 の移行ガイド](#migration-guide-for-az-410)
  - [Az.ApiManagement](#azapimanagement)
    - [`Add-AzApiManagementRegion`](#add-azapimanagementregion)
    - [`New-AzApiManagement`](#new-azapimanagement)
    - [`Set-AzApiManagement`](#set-azapimanagement)
    - [`Get-AzApiManagementProperty`](#get-azapimanagementproperty)
    - [`New-AzApiManagementProperty`](#new-azapimanagementproperty)
    - [`Remove-AzApiManagementProperty`](#remove-azapimanagementproperty)
    - [`Set-AzApiManagementProperty`](#set-azapimanagementproperty)
  - [Az.Batch](#azbatch)
    - [`Get-AzBatchApplication`、`New-AzBatchApplication`](#get-azbatchapplication-new-azbatchapplication)
    - [`Get-AzBatchComputeNode`、`New-AzBatchPool`](#get-azbatchcomputenode-new-azbatchpool)
    - [`Get-AzBatchApplicationPackage`、`New-AzBatchApplicationPackage`](#get-azbatchapplicationpackage-new-azbatchapplicationpackage)
  - [Az.Compute](#azcompute)
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
  - [Az.KeyVault](#azkeyvault)
    - [`New-AzKeyVaultCertificateOrganizationDetail`](#new-azkeyvaultcertificateorganizationdetail)
    - [`New-AzKeyVaultCertificateAdministratorDetail`](#new-azkeyvaultcertificateadministratordetail)
    - [`New-AzKeyVault`](#new-azkeyvault)
  - [Az.Monitor](#azmonitor)
    - [`Add-AzLogProfile`](#add-azlogprofile)
    - [`Get-AzLogProfile`](#get-azlogprofile)
    - [`New-AzMetricAlertRuleV2Criteria`](#new-azmetricalertrulev2criteria)
  - [Az.Network](#aznetwork)
    - [`Get-AzNetworkWatcherConnectionMonitor`](#get-aznetworkwatcherconnectionmonitor)
    - [`New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`](#new-aznetworkwatcherconnectionmonitortestconfigurationobject)
  - [Az.OperationalInsights](#azoperationalinsights)
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
  - [Az.Resources](#azresources)
    - [`Get-AzDeploymentScript`](#get-azdeploymentscript)
    - [`Get-AzDeploymentScriptLog`](#get-azdeploymentscriptlog)
    - [`Save-AzDeploymentScriptLog`](#save-azdeploymentscriptlog)
    - [`Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`](#get-azresourcelock-new-azresourcelock-remove-azresourcelock-set-azresourcelock)
    - [`Get-AzPolicyAlias`](#get-azpolicyalias)
    - [`New-AzPolicyAssignment`](#new-azpolicyassignment)
    - [`Remove-AzDeploymentScript`](#remove-azdeploymentscript)
  - [Az.Storage](#azstorage)
    - [`Update-AzStorageAccountNetworkRuleSet`、`Get-AzStorageAccountNetworkRuleSet`](#update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset)
    - [`New-AzStorageTable`、`Get-AzStorageTable`](#new-azstoragetable-get-azstoragetable)
    - [`Get-AzStorageFile`、`Remove-AzStorageFile`、`Get-AzStorageFileContent`、`Set-AzStorageFileContent`、`Start-AzStorageFileCopy`](#get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy)
    - [`Get-AzStorageFile`、`New-AzStorageDirectory`、`Remove-AzStorageDirectory`](#get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory)
    - [`Get-AzStorageShare`、`New-AzStorageShare`、`Remove-AzStorageShare`](#get-azstorageshare-new-azstorageshare-remove-azstorageshare)
    - [`Set-AzStorageShareQuota`](#set-azstoragesharequota)
    - [`Remove-AzStorageDirectory`](#remove-azstoragedirectory)

## <a name="azapimanagement"></a>Az.ApiManagement

### `Add-AzApiManagementRegion`

`Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentity` 型のプロパティ `Type` の型が、`Microsoft.Azure.Commands.ApiManagement.Models.PsApiManagementServiceIdentityType` から `System.String` に変更されました。

### `New-AzApiManagement`

- コマンドレット `New-AzApiManagement` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- コマンドレット `New-AzApiManagement` のパラメーター セット `__AllParameterSets` は削除されました。

### `Set-AzApiManagement`

- コマンドレット `Set-AzApiManagement` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- コマンドレット `Set-AzApiManagement` のパラメーター セット `__AllParameterSets` は削除されました。

### `Get-AzApiManagementProperty`

コマンドレット `Get-AzApiManagementProperty` が `Get-AzureApiManagementNamedValue` に置き換えられました。

### `New-AzApiManagementProperty`

コマンドレット `New-AzApiManagementProperty` が `New-AzureApiManagementNamedValue` に置き換えられました。

### `Remove-AzApiManagementProperty`

コマンドレット `Remove-AzApiManagementProperty` が `Remove-AzureApiManagementNamedValue` に置き換えられました。

### `Set-AzApiManagementProperty`

コマンドレット `Set-AzApiManagementProperty` が `Set-AzureApiManagementNamedValue` に置き換えられました。

## <a name="azbatch"></a>Az.Batch

### <a name="get-azbatchapplication-new-azbatchapplication"></a>`Get-AzBatchApplication`, `New-AzBatchApplication`

`Microsoft.Azure.Commands.Batch.Models.PSApplication` 型の `ApplicationPackages` プロパティが削除されました。

### <a name="get-azbatchcomputenode-new-azbatchpool"></a>`Get-AzBatchComputeNode`, `New-AzBatchPool`

`Microsoft.Azure.Commands.Batch.Models.PSNetworkConfiguration` 型の `PublicIPs` プロパティが削除されました

### <a name="get-azbatchapplicationpackage-new-azbatchapplicationpackage"></a>`Get-AzBatchApplicationPackage`, `New-AzBatchApplicationPackage`

`Microsoft.Azure.Commands.Batch.Models.PSApplicationPackage` 型のプロパティ `StorageUrlExpiry` の型が、`System.DateTime` から `System.DateTime?` に変更されました。

## <a name="azcompute"></a>Az.Compute

### `Remove-AzVmssDiagnosticsExtension`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Get-AzVMImage`

- コマンドレット `Get-AzVMImage` でパラメーター `FilterExpression` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- コマンドレット `Get-AzVMImage` のパラメーター セット `ListVMImage` は削除されました。

### `New-AzVMConfig`

- コマンドレット `New-AzVMConfig` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- コマンドレット `New-AzVMConfig` のパラメーター セット `AssignIdentityParameterSet` は削除されました。

### `Update-AzVM`

- コマンドレット `Update-AzVM` でパラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- コマンドレット `Update-AzVM` のパラメーター セット `AssignIdentityParameterSet` は削除されました。

### `New-AzProximityPlacementGroup`

- プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。
- `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。

#### <a name="before"></a>[指定日付より前]

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

#### <a name="after"></a>After

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

- プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。
- `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。

#### <a name="before"></a>[指定日付より前]

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

#### <a name="after"></a>After

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

- プロパティ `VirtualMachines`、`VirtualMachineScaleSets`、`AvailabilitySets` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResource]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.Compute.Models.SubResourceWithColocationStatus]` に変更されました。
- `Microsoft.Azure.Commands.Compute.Automation.Models.PSProximityPlacementGroup` 型のプロパティ `VirtualMachinesColocationStatus`、`VirtualMachineScaleSetsColocationStatus`、`AvailabilitySetsColocationStatus` が削除されました。

#### <a name="before"></a>[指定日付より前]

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

#### <a name="after"></a>After

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

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Add-AzVmssDataDisk`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Add-AzVmssExtension`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Add-AzVmssNetworkInterfaceConfiguration`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Add-AzVmssSecret`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Add-AzVmssSshPublicKey`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Add-AzVmssWinRMListener`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `New-AzVmssConfig`

- `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。
- パラメーター `AutomaticRepairMaxInstanceRepairsPercent` はサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- パラメーター `AssignIdentity` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- パラメーター セット `__AllParameterSets` は削除されました。
- パラメーター セット `ExplicitIdentityParameterSet` は削除されました。
- パラメーター セット `AssignIdentityParameterSet` は削除されました。

### `Remove-AzVmssDataDisk`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Remove-AzVmssExtension`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Remove-AzVmssNetworkInterfaceConfiguration`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Set-AzVmssBootDiagnostic`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Set-AzVmssOsProfile`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Set-AzVmssRollingUpgradePolicy`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Set-AzVmssStorageProfile`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `New-AzVmss`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Repair-AzVmssServiceFabricUpdateDomain`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Get-AzVmss`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Set-AzVmssOrchestrationServiceState`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Update-AzVmss`

- `Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。
- パラメーター `AutomaticRepairMaxInstanceRepairsPercent` はサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- パラメーター セット `__AllParameterSets` は削除されました。
- パラメーター セット `ExplicitIdentityParameterSet` は削除されました。

### `Add-AzVmssDiagnosticsExtension`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

### `Disable-AzVmssDiskEncryption`

`Microsoft.Azure.Commands.Compute.Automation.Models.PSVirtualMachineScaleSet` 型のプロパティ `AutomaticRepairsPolicy` の型が、`Microsoft.Azure.Commands.Compute.Automation.Models.PSAutomaticRepairsPolicy` から `Microsoft.Azure.Management.Compute.Models.AutomaticRepairsPolicy` に変更されました。

## <a name="azkeyvault"></a>Az.KeyVault

### `New-AzKeyVaultCertificateOrganizationDetail`

別名 `New-AzKeyVaultCertificateOrganizationDetails` は削除されています。 `New-AzKeyVaultCertificateOrganizationDetail` を使用してください。

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetails -AdministratorDetails $AdminDetails
```

#### <a name="after"></a>After

```powershell
PS C:\> New-AzKeyVaultCertificateOrganizationDetail -AdministratorDetails $AdminDetails
```

### `New-AzKeyVaultCertificateAdministratorDetail`

別名 `New-AzKeyVaultCertificateAdministratorDetails` は削除されています。 `New-AzKeyVaultCertificateAdministratorDetail` を使用してください。

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetails -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

#### <a name="after"></a>After

```powershell
PS C:\> $AdminDetails = New-AzKeyVaultCertificateAdministratorDetail -FirstName 'Patti' -LastName 'Fuller' -EmailAddress 'patti.fuller@contoso.com' -PhoneNumber '5553334444'
```

### `New-AzKeyVault`

論理的な削除が既定で有効になっているため、`-EnableSoftDelete` は削除されています。 この動作を希望しない場合は、`-DisableSoftDelete` を使用してください。

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US' -EnableSoftDelete
```

#### <a name="after"></a>After

```powershell
PS C:\> New-AzKeyVault -VaultName 'Contoso03Vault' -ResourceGroupName 'Group14' -Location 'East US'
```

## <a name="azmonitor"></a>Az.Monitor

### `Add-AzLogProfile`

`Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` 型のプロパティ `RetentionPolicy` の型が、`Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` から `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy` に変更されました。

### `Get-AzLogProfile`

`Microsoft.Azure.Commands.Insights.OutputClasses.PSLogProfile` 型のプロパティ `RetentionPolicy` の型が、`Microsoft.Azure.Management.Monitor.Management.Models.RetentionPolicy` から `Microsoft.Azure.Management.Monitor.Models.RetentionPolicy` に変更されました。

### `New-AzMetricAlertRuleV2Criteria`

コマンドレット `New-AzMetricAlertRuleV2Criteria` のパラメーター セット `__AllParameterSets` は削除されました。

## <a name="aznetwork"></a>Az.Network

### `Get-AzNetworkWatcherConnectionMonitor`

プロパティ `RoundTripTimeMs` のジェネリック型が `System.Nullable1[System.Int32]` から `System.Nullable1[System.Double]` に変更されました。

### `New-AzNetworkWatcherConnectionMonitorTestConfigurationObject`

パラメーター `SuccessThresholdRoundTripTimeMs` のジェネリック型が `System.Nullable1[System.Int32]` から `System.Nullable1[System.Double]` に変更されました。

## <a name="azoperationalinsights"></a>Az.OperationalInsights

### `Get-AzOperationalInsightsDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsApplicationInsightsDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsAzureActivityLogDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsCustomLogDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsLinuxPerformanceObjectDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsLinuxSyslogDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsWindowsEventDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsWindowsPerformanceCounterDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Remove-AzOperationalInsightsDataSource`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Disable-AzOperationalInsightsIISLogCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Disable-AzOperationalInsightsLinuxCustomLogCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Disable-AzOperationalInsightsLinuxPerformanceCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Disable-AzOperationalInsightsLinuxSyslogCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Enable-AzOperationalInsightsIISLogCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Enable-AzOperationalInsightsLinuxCustomLogCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Enable-AzOperationalInsightsLinuxPerformanceCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Enable-AzOperationalInsightsLinuxSyslogCollection`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Get-AzOperationalInsightsSavedSearch`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSSearchListSavedSearchResponse` 型の `Metadata` プロパティが削除されました。

### `Get-AzOperationalInsightsSavedSearchResult`

コマンドレット `Get-AzOperationalInsightsSavedSearchResult` は SDK でサポートされなくなったため、削除されました。

### `Get-AzOperationalInsightsSearchResult`

コマンドレット `Get-AzOperationalInsightsSearchResult` は SDK でサポートされなくなったため、削除されました。

### `Get-AzOperationalInsightsStorageInsight`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsStorageInsight`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Remove-AzOperationalInsightsStorageInsight`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Set-AzOperationalInsightsStorageInsight`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Get-AzOperationalInsightsLinkTarget`

コマンドレット `Get-AzOperationalInsightsLinkTarget` は SDK でサポートされなくなったため、削除されました。

### `Get-AzOperationalInsightsWorkspace`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `New-AzOperationalInsightsWorkspace`

- `Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。
- コマンドレット `New-AzOperationalInsightsWorkspace` でパラメーター `CustomerId` がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
- コマンドレット `New-AzOperationalInsightsWorkspace` のパラメーター セット `__AllParameterSets` は削除されました。

### `Set-AzOperationalInsightsWorkspace`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

### `Invoke-AzOperationalInsightsQuery`

`Microsoft.Azure.Commands.OperationalInsights.Models.PSWorkspace` 型の `PortalUrl` プロパティが削除されました。

## <a name="azresources"></a>Az.Resources

### `Get-AzDeploymentScript`

`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。

### `Get-AzDeploymentScriptLog`

`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。

### `Save-AzDeploymentScriptLog`

`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。

### `Get-AzResourceLock, New-AzResourceLock, Remove-AzResourceLock, Set-AzResourceLock`

パラメーター `TenantLevel` は削除されました。

### `Get-AzPolicyAlias`

プロパティ `Aliases` のジェネリック型が `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.AliasType]` から `System.Collections.Generic.IList1[Microsoft.Azure.Management.ResourceManager.Models.Alias]` に変更されました。

### `New-AzPolicyAssignment`

- コマンドレット `New-AzPolicyAssignment` では、パラメーター `PolicyDefinition` の `System.Management.Automation.PSObject` 型はサポートされなくなりました。
- コマンドレット `New-AzPolicyAssignment` では、パラメーター `PolicySetDefinition` の `System.Management.Automation.PSObject` 型はサポートされなくなりました。

### `Remove-AzDeploymentScript`

`Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsDeploymentScript` 型のプロパティ `Status` の型が、`Microsoft.Azure.Management.ResourceManager.Models.ScriptStatus` から `Microsoft.Azure.Commands.ResourceManager.Cmdlets.SdkModels.PsScriptStatus` に変更されました。

## <a name="azstorage"></a>Az.Storage

### <a name="update-azstorageaccountnetworkruleset-get-azstorageaccountnetworkruleset"></a>`Update-AzStorageAccountNetworkRuleSet`, `Get-AzStorageAccountNetworkRuleSet`

NetWorkRule DefaultAction の値が以下のように変更されました。Allow = 1、Deny = 0 が以下になります。Allow = 0、Deny = 1。

### <a name="new-azstoragetable-get-azstoragetable"></a>`New-AzStorageTable`, `Get-AzStorageTable`

出力オブジェクト AzureStorageTable.CloudTable.ServiceClient で 2 つのプロパティが削除されました。ConnectionPolicy、ConsistencyLevel。

### <a name="get-azstoragefile-remove-azstoragefile-get-azstoragefilecontent-set-azstoragefilecontent-start-azstoragefilecopy"></a>`Get-AzStorageFile`、`Remove-AzStorageFile`、`Get-AzStorageFileContent`、`Set-AzStorageFileContent`、`Start-AzStorageFileCopy`

出力の種類が CloudFile から AzureStorageFile に変更されています。元の出力は新しい出力の子プロパティ "CloudFile" になります

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file
```

#### <a name="after"></a>After

```powershell
PS C:\> $file = Get-AzStorageFile -ShareName $shareName -Path testfile -Context $ctx

PS C:\> Remove-AzStorageFile -File $file.CloudFile
```

### <a name="get-azstoragefile-new-azstoragedirectory-remove-azstoragedirectory"></a>`Get-AzStorageFile`、`New-AzStorageDirectory`、`Remove-AzStorageDirectory`

出力の種類が CloudFileDirectory から AzureStorageFileDirectory に変更されています。元の出力は新しい出力の子プロパティ "CloudFileDirectory" になります

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a>After

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```

### <a name="get-azstorageshare-new-azstorageshare-remove-azstorageshare"></a>`Get-AzStorageShare`、`New-AzStorageShare`、`Remove-AzStorageShare`

出力の種類が FileShareProperties から AzureStorageFileShare に変更されています。元の出力は新しい出力の子プロパティ "CloudFileShare" になります

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share
```

#### <a name="after"></a>After

```powershell
PS C:\> $share = Get-AzStorageShare -Name $shareName -Context $ctx

PS C:\> Remove-AzStorageShare -Share $share.CloudFileShare
```

### `Set-AzStorageShareQuota`

出力の種類が FileShareProperties から AzureStorageFileShare に変更されています。元の出力は新しい出力のサブの子プロパティ ""CloudFileShare.Properties"" になります

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> $shareProperties = Set-AzStorageShareQuota -Name $shareName -Quota 100 -Context $ctx

PS C:\> $shareProperties

ETag                LastModified                Quota
----                ------------                -----
"0x8D7F5BC7789FC63" 5/11/2020 3:03:30 PM +00:00   100
```

#### <a name="after"></a>After

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

親ディレクトリ オブジェクトと -Path を指定してサブ ファイル ディレクトリを削除すると、型 (文字列) の一致を使用してパイプラインから -Path を入力できなくなります。

#### <a name="before"></a>[指定日付より前]

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> @('dir1', 'dir2') | Remove-AzStorageDirectory -Directory $dir
```

#### <a name="after"></a>After

```powershell
PS C:\> $dir = Get-AzStorageFile -ShareName $shareName -Path testdir -Context $ctx

PS C:\> $paths = @(
    [PSCustomObject]@{  Path = 'dir1 }
    [PSCustomObject]@{ Path = 'dir2' }
)

PS C:\> $paths | Remove-AzStorageDirectory -Directory $dir.CloudFileDirectory
```
