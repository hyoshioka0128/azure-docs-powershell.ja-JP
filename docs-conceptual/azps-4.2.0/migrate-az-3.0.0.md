---
title: Az 3.0.0 の移行ガイド
description: この移行ガイドには、Az バージョン 3.0 リリースの Azure PowerShell で行われた破壊的変更が記載されています。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/04/2019
ms.openlocfilehash: 06be35bc3573d00d90a8cf2d822ac051ab72f6bb
ms.sourcegitcommit: cef87acc9f2a0d296bef74f526afd2e067e8146b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "84299087"
---
# <a name="migration-guide-for-az-300"></a><span data-ttu-id="40284-103">Az 3.0.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="40284-103">Migration Guide for Az 3.0.0</span></span>

<span data-ttu-id="40284-104">このドキュメントでは、Az のバージョン 2.0.0 と 3.0.0 の間での変更点について説明します</span><span class="sxs-lookup"><span data-stu-id="40284-104">This document describes the changes between the 2.0.0 and 3.0.0 versions of Az</span></span>

<!-- TOC -->

- [<span data-ttu-id="40284-105">Az 3.0.0 の移行ガイド</span><span class="sxs-lookup"><span data-stu-id="40284-105">Migration Guide for Az 3.0.0</span></span>](#migration-guide-for-az-300)
  - [<span data-ttu-id="40284-106">Batch</span><span class="sxs-lookup"><span data-stu-id="40284-106">Batch</span></span>](#batch)
    - [`Get-AzBatchNodeAgentSku`](#get-azbatchnodeagentsku)
    - [<span data-ttu-id="40284-107">以前のバージョンの `Az.Resources` との非互換性</span><span class="sxs-lookup"><span data-stu-id="40284-107">Incompatibility with previous versions of `Az.Resources`</span></span>](#previous-version-incompatibility-with-azresources-module)
  - [<span data-ttu-id="40284-108">Compute</span><span class="sxs-lookup"><span data-stu-id="40284-108">Compute</span></span>](#compute)
    - [`New-AzDiskConfig`](#new-azdiskconfig)
  - [<span data-ttu-id="40284-109">HDInsight</span><span class="sxs-lookup"><span data-stu-id="40284-109">HDInsight</span></span>](#hdinsight)
    - [`Get-AzHDInsightJobOutput`](#get-azhdinsightjoboutput)
    - [`Add-AzHDInsightConfigValues`](#add-azhdinsightconfigvalues)
    - [`Disable-AzHDInsightMonitoring`](#disable-azhdinsightmonitoring)
    - [`Enable-AzHDInsightMonitoring`](#enable-azhdinsightmonitoring)
    - [`Get-AzHDInsightMonitoring`](#get-azhdinsightmonitoring)
    - [`Get-AzHDInsightProperty`](#get-azhdinsightproperty)
    - [`Grant-AzHDInsightRdpServicesAccess`](#grant-azhdinsightrdpservicesaccess)
    - [`Remove-AzHDInsightCluster`](#remove-azhdinsightcluster)
    - [`Revoke-AzHDInsightRdpServicesAccess`](#revoke-azhdinsightrdpservicesaccess)
    - [`Set-AzHDInsightGatewayCredential`](#set-azhdinsightgatewaycredential)
  - [<span data-ttu-id="40284-110">IotHub</span><span class="sxs-lookup"><span data-stu-id="40284-110">IotHub</span></span>](#iothub)
    - [`New-AzIotHubImportDevices`](#new-aziothubimportdevices)
    - [`New-AzIotHubExportDevices`](#new-aziothubexportdevices)
    - [`Add-AzIotHubEventHubConsumerGroup`](#add-aziothubeventhubconsumergroup)
    - [`Get-AzIotHubEventHubConsumerGroup`](#get-aziothubeventhubconsumergroup)
    - [`Remove-AzIotHubEventHubConsumerGroup`](#remove-aziothubeventhubconsumergroup)
    - [`Set-AzIotHub`](#set-aziothub)
  - [<span data-ttu-id="40284-111">RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="40284-111">RecoveryServices</span></span>](#recoveryservices)
    - [`Edit-AzRecoveryServicesAsrRecoveryPlan`](#edit-azrecoveryservicesasrrecoveryplan)
    - [`Get-AzRecoveryServicesAsrRecoveryPlan`](#get-azrecoveryservicesasrrecoveryplan)
    - [`New-AzRecoveryServicesAsrReplicationProtectedItem`](#new-azrecoveryservicesasrreplicationprotecteditem)
  - [<span data-ttu-id="40284-112">リソース</span><span class="sxs-lookup"><span data-stu-id="40284-112">Resources</span></span>](#resources)
    - [<span data-ttu-id="40284-113">以前のバージョンの `Az.Batch` との非互換性</span><span class="sxs-lookup"><span data-stu-id="40284-113">Incompatibility with previous versions of `Az.Batch`</span></span>](#previous-version-incompatibility-with-azbatch-module)
  - [<span data-ttu-id="40284-114">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="40284-114">ServiceFabric</span></span>](#servicefabric)
    - [`Add-ServiceFabricApplicationCertificate`](#add-servicefabricapplicationcertificate)
  - [<span data-ttu-id="40284-115">Sql</span><span class="sxs-lookup"><span data-stu-id="40284-115">Sql</span></span>](#sql)
    - [`Get-AzSqlDatabaseSecureConnectionPolicy`](#get-azsqldatabasesecureconnectionpolicy)
    - [`Get-AzSqlDatabaseIndexRecommendations`](#get-azsqldatabaseindexrecommendations)
    - [`Get-AzSqlDatabaseRestorePoints`](#get-azsqldatabaserestorepoints)
    - [`Get-AzSqlDatabaseAuditing`](#get-azsqldatabaseauditing)
    - [`Set-AzSqlDatabaseAuditing`](#set-azsqldatabaseauditing)
    - [`Get-AzSqlServerAuditing`](#get-azsqlserverauditing)
    - [`Set-AzSqlServerAuditing`](#set-azsqlserverauditing)
    - [`Get-AzSqlServerAdvancedThreatProtectionSettings`](#get-azsqlserveradvancedthreatprotectionsettings)
    - [`Clear-AzSqlServerAdvancedThreatProtectionSettings`](#clear-azsqlserveradvancedthreatprotectionsettings)
    - [`Update-AzSqlServerAdvancedThreatProtectionSettings`](#update-azsqlserveradvancedthreatprotectionsettings)
    - [`Get-AzSqlDatabaseAdvancedThreatProtectionSettings`](#get-azsqldatabaseadvancedthreatprotectionsettings)
    - [`Update-AzSqlDatabaseAdvancedThreatProtectionSettings`](#update-azsqldatabaseadvancedthreatprotectionsettings)
    - [`Clear-AzSqlDatabaseAdvancedThreatProtectionSettings`](#clear-azsqldatabaseadvancedthreatprotectionsettings)
    - [`Update-AzSqlDatabaseVulnerabilityAssessmentSettings`](#update-azsqldatabasevulnerabilityassessmentsettings)
    - [`Get-AzSqlDatabaseVulnerabilityAssessmentSettings`](#get-azsqldatabasevulnerabilityassessmentsettings)
    - [`Clear-AzSqlDatabaseVulnerabilityAssessmentSettings`](#clear-azsqldatabasevulnerabilityassessmentsettings)
    - [`Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`](#update-azsqlinstancedatabasevulnerabilityassessmentsettings)
    - [`Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`](#get-azsqlinstancedatabasevulnerabilityassessmentsettings)
    - [`Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`](#clear-azsqlinstancedatabasevulnerabilityassessmentsettings)
    - [`Update-AzSqlInstanceVulnerabilityAssessmentSettings`](#update-azsqlinstancevulnerabilityassessmentsettings)
    - [`Get-AzSqlInstanceVulnerabilityAssessmentSettings`](#get-azsqlinstancevulnerabilityassessmentsettings)
    - [`Clear-AzSqlInstanceVulnerabilityAssessmentSettings`](#clear-azsqlinstancevulnerabilityassessmentsettings)
    - [`Update-AzSqlServerVulnerabilityAssessmentSettings`](#update-azsqlservervulnerabilityassessmentsettings)
    - [`Get-AzSqlServerVulnerabilityAssessmentSettings`](#get-azsqlservervulnerabilityassessmentsettings)
    - [`Clear-AzSqlServerVulnerabilityAssessmentSettings`](#clear-azsqlservervulnerabilityassessmentsettings)
    - [`Get-AzSqlServerAdvancedThreatProtectionPolicy`](#get-azsqlserveradvancedthreatprotectionpolicy)
    - [`Get-AzSqlServerThreatDetectionPolicy`](#get-azsqlserverthreatdetectionpolicy)
    - [`Remove-AzSqlServerThreatDetectionPolicy`](#remove-azsqlserverthreatdetectionpolicy)
    - [`Set-AzSqlServerThreatDetectionPolicy`](#set-azsqlserverthreatdetectionpolicy)
    - [`Get-AzSqlDatabaseThreatDetectionPolicy`](#get-azsqldatabasethreatdetectionpolicy)
    - [`Set-AzSqlDatabaseThreatDetectionPolicy`](#set-azsqldatabasethreatdetectionpolicy)
    - [`Remove-AzSqlDatabaseThreatDetectionPolicy`](#remove-azsqldatabasethreatdetectionpolicy)

<!-- /TOC -->


## <a name="batch"></a><span data-ttu-id="40284-116">Batch</span><span class="sxs-lookup"><span data-stu-id="40284-116">Batch</span></span>

### `Get-AzBatchNodeAgentSku`
- <span data-ttu-id="40284-117">`Get-AzBatchNodeAgentSku` が削除され、`Get-AzBatchSupportedImage` に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="40284-117">Removed `Get-AzBatchNodeAgentSku` and replaced it with  `Get-AzBatchSupportedImage`.</span></span>
- <span data-ttu-id="40284-118">`Get-AzBatchSupportedImage` は `Get-AzBatchNodeAgentSku` と同じデータを返しますが、よりわかりやすい形式にします。</span><span class="sxs-lookup"><span data-stu-id="40284-118">`Get-AzBatchSupportedImage` returns the same data as `Get-AzBatchNodeAgentSku` but in a more friendly format.</span></span>
- <span data-ttu-id="40284-119">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="40284-119">New non-verified images are also now returned.</span></span> <span data-ttu-id="40284-120">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="40284-120">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-121">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-121">Before</span></span>
```powershell
$Context = Get-AzBatchAccountKeys -AccountName "ContosoBatchAccount"
Get-AzBatchNodeAgentSku -BatchContext $Context
```

#### <a name="after"></a><span data-ttu-id="40284-122">After</span><span class="sxs-lookup"><span data-stu-id="40284-122">After</span></span>
```powershell
$Context = Get-AzBatchAccountKey -AccountName "ContosoBatchAccount"
Get-AzBatchSupportedImage -BatchContext $Context
```
### <a name="previous-version-incompatibility-with-azresources-module"></a><span data-ttu-id="40284-123">以前のバージョンと Az.Resources モジュールとの非互換性</span><span class="sxs-lookup"><span data-stu-id="40284-123">Previous Version Incompatibility with Az.Resources Module</span></span>
<span data-ttu-id="40284-124">'Az.Batch' モジュールのバージョン 2.0.1 は、'Az.Resources' モジュールの以前のバージョン (バージョン 1.7.0 以前) と互換性がありません。</span><span class="sxs-lookup"><span data-stu-id="40284-124">Version 2.0.1 of the ‘Az.Batch’ module is incompatible with earlier versions (version 1.7.0 or earlier) of the ‘Az.Resources’ module.</span></span>  <span data-ttu-id="40284-125">これにより、'Az.Batch' モジュールのバージョン 2.0.1 がインポートされたときに、'Az.Resources' モジュールのバージョン 1.7.0 をインポートできなくなります。</span><span class="sxs-lookup"><span data-stu-id="40284-125">This will result in being unable to import  version 1.7.0 of the ‘Az.Resources’ module when version 2.0.1 of the ‘Az.Batch’ module is imported.</span></span>  <span data-ttu-id="40284-126">この問題を解決するには、'Az.Resources' モジュールをバージョン 1.7.1 以上に更新するか、'Az' モジュールの最新バージョンをインストールします。</span><span class="sxs-lookup"><span data-stu-id="40284-126">To fix this issue, simply update the ‘Az.Resources’ module to version 1.7.1 or greater, or simply install the latest version of the ‘Az’ module.</span></span>

## <a name="compute"></a><span data-ttu-id="40284-127">Compute</span><span class="sxs-lookup"><span data-stu-id="40284-127">Compute</span></span>

### `New-AzDiskConfig`
<span data-ttu-id="40284-128">`New-AzDiskConfig`で CreateOption が Upload の場合、`DiskSizeGB` の代わりに `UploadSizeInBytes` パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="40284-128">`UploadSizeInBytes` parameter is used instead of `DiskSizeGB` for `New-AzDiskConfig` when CreateOption is Upload</span></span>

#### <a name="before"></a><span data-ttu-id="40284-129">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-129">Before</span></span>
```powershell
$diskconfig = New-AzDiskConfig -Location 'Central US' -DiskSizeGB 1023 -SkuName Standard_LRS -OsType Windows -CreateOption Upload -DiskIOPSReadWrite 500 -DiskMBpsReadWrite 8
```

#### <a name="after"></a><span data-ttu-id="40284-130">After</span><span class="sxs-lookup"><span data-stu-id="40284-130">After</span></span>
```powershell
$diskconfig = New-AzDiskConfig -Location 'Central US' -UploadSizeInBytes 1023 * 1024 * 1024 * 1024 -SkuName Standard_LRS -OsType Windows -CreateOption Upload -DiskIOPSReadWrite 500 -DiskMBpsReadWrite 8
```

## <a name="hdinsight"></a><span data-ttu-id="40284-131">HDInsight</span><span class="sxs-lookup"><span data-stu-id="40284-131">HDInsight</span></span>

### `Get-AzHDInsightJobOutput`
- <span data-ttu-id="40284-132">ストレージ キーに対するきめ細かいロールベースのアクセスをサポートするため、`Get-AzHDInsightJobOutput` コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="40284-132">Updated the `Get-AzHDInsightJobOutput` cmdlet to support granular role-based access to the storage key.</span></span>
- <span data-ttu-id="40284-133">HDInsight クラスターのオペレーター、共同作成者、または所有者のロールを持つユーザーには影響を及ぼしません。</span><span class="sxs-lookup"><span data-stu-id="40284-133">Users with HDInsight Cluster Operator, Contributor, or Owner roles will not be affected.</span></span>
- <span data-ttu-id="40284-134">閲覧者のロールのみを持つユーザーは、`DefaultStorageAccountKey` パラメーターを明示的に指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="40284-134">Users with only the Reader role will need to specify `DefaultStorageAccountKey` parameter explicitly.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-135">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-135">Before</span></span>
```powershell
Get-AzHDInsightJobOutput  -ClusterName $clusterName -JobId $jobId
```

#### <a name="after"></a><span data-ttu-id="40284-136">After</span><span class="sxs-lookup"><span data-stu-id="40284-136">After</span></span>
```powershell
Get-AzHDInsightJobOutput -ClusterName $clusterName -JobId $jobId -DefaultStorageAccountKey $storageAccountKey
```

### `Add-AzHDInsightConfigValues`
<span data-ttu-id="40284-137">コマンドレット `Add-AzHDInsightConfigValue` のエイリアス `Add-AzHDInsightConfigValues` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="40284-137">Cmdlet `Add-AzHDInsightConfigValue` removed alias to `Add-AzHDInsightConfigValues`.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-138">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-138">Before</span></span>
<span data-ttu-id="40284-139">非推奨のエイリアスを使用</span><span class="sxs-lookup"><span data-stu-id="40284-139">Using deprecated alias</span></span>
```powershell
Add-AzHDInsightConfigValues
```

#### <a name="after"></a><span data-ttu-id="40284-140">After</span><span class="sxs-lookup"><span data-stu-id="40284-140">After</span></span>
```powershell
Add-AzHDInsightConfigValue
```


### `Disable-AzHDInsightMonitoring`
<span data-ttu-id="40284-141">新しい `Disable-AzHDInsightMonitoring` コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="40284-141">Added a new `Disable-AzHDInsightMonitoring` cmdlet.</span></span> <span data-ttu-id="40284-142">このコマンドレットを使用して、HDInsight クラスターの監視を無効にします (`Disable-AzHDInsightOperationsManagementSuite` と `Disable-AzHDInsightOMS` を置き換えます)。</span><span class="sxs-lookup"><span data-stu-id="40284-142">Use this cmdlet to disable monitoring in a HDInsight cluster (replaces `Disable-AzHDInsightOperationsManagementSuite` and `Disable-AzHDInsightOMS`).</span></span>

#### <a name="before"></a><span data-ttu-id="40284-143">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-143">Before</span></span>
```powershell
Disable-AzHDInsightOMS -Name testcluster
```
```powershell
Disable-AzHDInsightOperationsManagementSuite -Name testcluster
```

#### <a name="after"></a><span data-ttu-id="40284-144">After</span><span class="sxs-lookup"><span data-stu-id="40284-144">After</span></span>
```powershell
Disable-AzHDInsightMonitoring -Name testcluster
```


### `Enable-AzHDInsightMonitoring`
<span data-ttu-id="40284-145">新しい `Enable-AzHDInsightMonitoring` コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="40284-145">Added a new `Enable-AzHDInsightMonitoring` cmdlet.</span></span> <span data-ttu-id="40284-146">このコマンドレットを使用して、HDInsight クラスターの監視を有効にします (`Enable-AzHDInsightOperationsManagementSuite` と `Enable-AzHDInsightOMS` を置き換えます)。</span><span class="sxs-lookup"><span data-stu-id="40284-146">Use this cmdlet to enable monitoring in a HDInsight cluster (replaces `Enable-AzHDInsightOperationsManagementSuite` and `Enable-AzHDInsightOMS`).</span></span>

#### <a name="before"></a><span data-ttu-id="40284-147">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-147">Before</span></span>
```powershell
Enable-AzHDInsightOMS Enable-AzHDInsightMonitoring -Name testcluster -WorkspaceId 1d364e89-bb71-4503-aa3d-a23535aea7bd -PrimaryKey <key for workspace 1d364e89-bb71-4503-aa3d-a23535aea7bd>
```
```powershell
Enable-AzHDInsightOperationsManagementSuite Enable-AzHDInsightMonitoring -Name testcluster -WorkspaceId 1d364e89-bb71-4503-aa3d-a23535aea7bd -PrimaryKey <key for workspace 1d364e89-bb71-4503-aa3d-a23535aea7bd>
```

#### <a name="after"></a><span data-ttu-id="40284-148">After</span><span class="sxs-lookup"><span data-stu-id="40284-148">After</span></span>
```powershell
Enable-AzHDInsightMonitoring Enable-AzHDInsightMonitoring -Name testcluster -WorkspaceId 1d364e89-bb71-4503-aa3d-a23535aea7bd -PrimaryKey <key for workspace 1d364e89-bb71-4503-aa3d-a23535aea7bd>
```

### `Get-AzHDInsightMonitoring`
<span data-ttu-id="40284-149">新しい `Get-AzHDInsightMonitoring` コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="40284-149">Added a new `Get-AzHDInsightMonitoring` cmdlet.</span></span> <span data-ttu-id="40284-150">このコマンドレットを使用して、Azure HDInsight クラスターでのインストールの監視状態を取得します (`Get-AzHDInsightOperationsManagementSuite` と `Get-AzHDInsightOMS` を置き換えます)。</span><span class="sxs-lookup"><span data-stu-id="40284-150">Use this cmdlet to get the status of monitoring installation in an Azure HDInsight cluster (replaces `Get-AzHDInsightOperationsManagementSuite` and `Get-AzHDInsightOMS`).</span></span>

#### <a name="before"></a><span data-ttu-id="40284-151">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-151">Before</span></span>
```powershell
Get-AzHDInsightOMS -Name testcluster
```
```powershell
Get-AzHDInsightOperationsManagementSuite -Name testcluster
```

#### <a name="after"></a><span data-ttu-id="40284-152">After</span><span class="sxs-lookup"><span data-stu-id="40284-152">After</span></span>
```powershell
Get-AzHDInsightMonitoring -Name testcluster
```

### `Get-AzHDInsightProperty`
<span data-ttu-id="40284-153">コマンドレット `Get-HDInsightProperty` のエイリアス `Get-AzHDInsightProperties` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="40284-153">Cmdlet `Get-HDInsightProperty` removed alias to `Get-AzHDInsightProperties`.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-154">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-154">Before</span></span>
<span data-ttu-id="40284-155">非推奨のエイリアスを使用</span><span class="sxs-lookup"><span data-stu-id="40284-155">Using deprecated alias</span></span>
```powershell
Get-AzHDInsightProperties -Location "East US 2"
```

#### <a name="after"></a><span data-ttu-id="40284-156">After</span><span class="sxs-lookup"><span data-stu-id="40284-156">After</span></span>
```powershell
Get-AzHDInsightProperty -Location "East US 2"
```

### `Grant-AzHDInsightRdpServicesAccess`
<span data-ttu-id="40284-157">`Grant-AzHDInsightRdpServicesAccess` および `Revoke-AzHDInsightRdpServicesAccess` コマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="40284-157">Removed the `Grant-AzHDInsightRdpServicesAccess` and `Revoke-AzHDInsightRdpServicesAccess` cmdlets.</span></span> <span data-ttu-id="40284-158">Windows OS の種類を使用するクラスターはサポートされていないため、これらは不要になりました。</span><span class="sxs-lookup"><span data-stu-id="40284-158">These are no longer necessary because clusters using Windows OS type are not supported.</span></span> <span data-ttu-id="40284-159">代わりに Linux OS の種類を使用してクラスターを作成してください。</span><span class="sxs-lookup"><span data-stu-id="40284-159">Please create a cluster using Linux OS type instead.</span></span>

### `Remove-AzHDInsightCluster`
<span data-ttu-id="40284-160">`Remove-AzHDInsightCluster` の出力型が `Microsoft.Azure.Management.HDInsight.Models.ClusterGetResponse` から `bool` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="40284-160">The output type of `Remove-AzHDInsightCluster` changed from `Microsoft.Azure.Management.HDInsight.Models.ClusterGetResponse` to `bool`.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-161">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-161">Before</span></span>
```powershell
$cluster = Remove-AzHDInsightCluster -ClusterName "your-hadoop-001"
```

#### <a name="after"></a><span data-ttu-id="40284-162">After</span><span class="sxs-lookup"><span data-stu-id="40284-162">After</span></span>
```powershell
Remove-AzHDInsightCluster -ClusterName "your-hadoop-001" -PassThru
True
```

### `Revoke-AzHDInsightRdpServicesAccess`
<span data-ttu-id="40284-163">このコマンドレットは非推奨になります。</span><span class="sxs-lookup"><span data-stu-id="40284-163">The cmdlet is deprecated.</span></span> <span data-ttu-id="40284-164">これに代わるものはありません。</span><span class="sxs-lookup"><span data-stu-id="40284-164">There is no replacement for it.</span></span>

### `Set-AzHDInsightGatewayCredential`
<span data-ttu-id="40284-165">`Set-AzHDInsightGatewayCredential` の出力型が `HttpConnectivitySettings` から `AzureHDInsightGatewaySettings` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="40284-165">The output type of `Set-AzHDInsightGatewayCredential` changed from `HttpConnectivitySettings` to `AzureHDInsightGatewaySettings`.</span></span>



## <a name="iothub"></a><span data-ttu-id="40284-166">IotHub</span><span class="sxs-lookup"><span data-stu-id="40284-166">IotHub</span></span>

### `New-AzIotHubImportDevices`
<span data-ttu-id="40284-167">このエイリアスは削除されました。代わりに `New-AzIotHubImportDevice` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="40284-167">This alias is removed, please use `New-AzIotHubImportDevice` instead.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-168">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-168">Before</span></span>
```powershell
New-AzIotHubImportDevices -ResourceGroupName "myresourcegroup" -Name "myiothub" -InputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -OutputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D"
```

#### <a name="after"></a><span data-ttu-id="40284-169">After</span><span class="sxs-lookup"><span data-stu-id="40284-169">After</span></span>
```powershell
New-AzIotHubImportDevice -ResourceGroupName "myresourcegroup" -Name "myiothub" -InputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -OutputBlobContainerUri "https://mystorageaccount.blob.core.windows.net/?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D"
```

### `New-AzIotHubExportDevices`
<span data-ttu-id="40284-170">このエイリアスは削除されました。代わりに `New-AzIotHubExportDevice` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="40284-170">This alias is removed, please use `New-AzIotHubExportDevice` instead.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-171">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-171">Before</span></span>
```powershell
New-AzIotHubExportDevices -ResourceGroupName "myresourcegroup" -Name "myiothub" -ExportBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -ExcludeKeys
```

#### <a name="after"></a><span data-ttu-id="40284-172">After</span><span class="sxs-lookup"><span data-stu-id="40284-172">After</span></span>
```powershell
New-AzIotHubExportDevice -ResourceGroupName "myresourcegroup" -Name "myiothub" -ExportBlobContainerUri "https://mystorageaccount.blob.core.windows.net/mystoragecontainer?sv=2015-04-05&ss=bfqt&sr=c&srt=sco&sp=rwdl&se=2016-10-27T04:01:48Z&st=2016-10-26T20:01:48Z&spr=https&sig=QqpIhHsIMF8hNuFO%3D" -ExcludeKeys
```

### `Add-AzIotHubEventHubConsumerGroup`
<span data-ttu-id="40284-173">IotHub には、システムおよびデバイスのメッセージを処理できる組み込みエンドポイント ("events") が 1 つしかないため、パラメーター `EventHubEndPointName` は非推奨になり、代わるものはありません。</span><span class="sxs-lookup"><span data-stu-id="40284-173">Parameter `EventHubEndPointName` is deprecated without being replaced as IotHub comes with only one built-in endpoint("events") which could handle system and device messages.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-174">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-174">Before</span></span>
```powershell
Add-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName "myconsumergroup" -EventHubEndpointName "/EventHubEndpointName"
```

#### <a name="after"></a><span data-ttu-id="40284-175">After</span><span class="sxs-lookup"><span data-stu-id="40284-175">After</span></span>
```powershell
Add-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName "myconsumergroup"
```

### `Get-AzIotHubEventHubConsumerGroup`
<span data-ttu-id="40284-176">IotHub には、システムおよびデバイスのメッセージを処理できる組み込みエンドポイント ("events") が 1 つしかないため、パラメーター `EventHubEndPointName` は非推奨になり、代わるものはありません。</span><span class="sxs-lookup"><span data-stu-id="40284-176">Parameter `EventHubEndPointName` is deprecated without being replaced as IotHub comes with only one built-in endpoint("events") which could handle system and device messages.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-177">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-177">Before</span></span>
```powershell
Get-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubEndpointName "/EventHubEndpointName"
```

#### <a name="after"></a><span data-ttu-id="40284-178">After</span><span class="sxs-lookup"><span data-stu-id="40284-178">After</span></span>
```powershell
Get-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub"
```

### `Remove-AzIotHubEventHubConsumerGroup`
<span data-ttu-id="40284-179">IotHub には、システムおよびデバイスのメッセージを処理できる組み込みエンドポイント ("events") が 1 つしかないため、パラメーター `EventHubEndPointName` は非推奨になり、代わるものはありません。</span><span class="sxs-lookup"><span data-stu-id="40284-179">Parameter `EventHubEndPointName` is deprecated without being replaced as IotHub comes with only one built-in endpoint("events") which could handle system and device messages.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-180">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-180">Before</span></span>
```powershell
Remove-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName myconsumergroup -EventHubEndpointName "/EventHubEndpointName"
```

#### <a name="after"></a><span data-ttu-id="40284-181">After</span><span class="sxs-lookup"><span data-stu-id="40284-181">After</span></span>
```powershell
Remove-AzIotHubEventHubConsumerGroup -ResourceGroupName "myresourcegroup" -Name "myiothub" -EventHubConsumerGroupName myconsumergroup
```

### `Set-AzIotHub`
<span data-ttu-id="40284-182">IotHub が組み込みのエンドポイント ("operationsMonitoringEvents") を使用しなくなったため、パラメーター `OperationsMonitoringProperties` は非推奨となり、代わるものはありません。</span><span class="sxs-lookup"><span data-stu-id="40284-182">Parameter `OperationsMonitoringProperties` is deprecated without being replaced as IotHub is no longer using built-in endpoint("operationsMonitoringEvents").</span></span>



## <a name="recoveryservices"></a><span data-ttu-id="40284-183">RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="40284-183">RecoveryServices</span></span>

### `Edit-AzRecoveryServicesAsrRecoveryPlan`
<span data-ttu-id="40284-184">出力から `ASRRecoveryPlanGroup.ReplicationProtectedItems`、`ASRRecoveryPlanGroup.StartGroupActions`、および `ASRRecoveryPlanGroup.EndGroupActions` が削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-184">`ASRRecoveryPlanGroup.ReplicationProtectedItems`, `ASRRecoveryPlanGroup.StartGroupActions` and `ASRRecoveryPlanGroup.EndGroupActions` is removed from output.</span></span>

### `Get-AzRecoveryServicesAsrRecoveryPlan`
<span data-ttu-id="40284-185">出力から `ASRRecoveryPlanGroup.ReplicationProtectedItems`、`ASRRecoveryPlanGroup.StartGroupActions`、および `ASRRecoveryPlanGroup.EndGroupActions` が削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-185">`ASRRecoveryPlanGroup.ReplicationProtectedItems`, `ASRRecoveryPlanGroup.StartGroupActions` and `ASRRecoveryPlanGroup.EndGroupActions` is removed from output.</span></span>

### `New-AzRecoveryServicesAsrReplicationProtectedItem`
<span data-ttu-id="40284-186">パラメーター IncludeDiskId は、Azure Site Recovery でマネージド ディスクへの直接書き込みをサポートするように変更されています。</span><span class="sxs-lookup"><span data-stu-id="40284-186">Parameter IncludeDiskId is changed to support directly writing to a managed disk in Azure Site Recovery.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-187">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-187">Before</span></span>
```powershell
$job = New-AzRecoveryServicesAsrReplicationProtectedItem -RecoveryAzureStorageAccountId $recoveryAzureStorageAccountId -IncludeDiskId $includeDiskId -VMwareToAzure -Account $fabric.FabricSpecificDetails.RunAsAccounts[0] -RecoveryResourceGroupId $RecoveryResourceGroupId -RecoveryAzureNetworkId $RecoveryAzureNetworkId -name $name -ProcessServer $fabric.FabricSpecificDetails.ProcessServers[0] -ProtectableItem $protectableItem -ProtectionContainerMapping $pcm -RecoveryAzureSubnetName $RecoveryAzureSubnetName -RecoveryVmName $RecoveryVmName -LogStorageAccountId $LogStorageAccountId
```

#### <a name="after"></a><span data-ttu-id="40284-188">After</span><span class="sxs-lookup"><span data-stu-id="40284-188">After</span></span>
```powershell
$disk1 = New-AzRecoveryServicesAsrInMageAzureV2DiskInput -DiskId $diskId -LogStorageAccountId $logStorageAccountId -DiskType $diskType
$disk2 = New-AzRecoveryServicesAsrInMageAzureV2DiskInput -DiskId $diskId2 -LogStorageAccountId $logStorageAccountId -DiskType $diskType2
$job = New-AzRecoveryServicesAsrReplicationProtectedItem -VMwareToAzure -Account $fabric.FabricSpecificDetails.RunAsAccounts[0] -RecoveryResourceGroupId $RecoveryResourceGroupId -RecoveryAzureNetworkId $RecoveryAzureNetworkId -name $name -ProcessServer $fabric.FabricSpecificDetails.ProcessServers[0] -ProtectableItem $protectableItem -ProtectionContainerMapping $pcm -RecoveryAzureSubnetName $RecoveryAzureSubnetName -RecoveryVmName $RecoveryVmName -LogStorageAccountId $LogStorageAccountId -InMageAzureV2DiskInput $disk1,$disk2
```

## <a name="resources"></a><span data-ttu-id="40284-189">リソース</span><span class="sxs-lookup"><span data-stu-id="40284-189">Resources</span></span>

### <a name="previous-version-incompatibility-with-azbatch-module"></a><span data-ttu-id="40284-190">以前のバージョンと Az.Batch モジュールとの非互換性</span><span class="sxs-lookup"><span data-stu-id="40284-190">Previous Version Incompatibility with Az.Batch Module</span></span>
<span data-ttu-id="40284-191">'Az.Resources' モジュールのバージョン 1.7.1 は、'Az.Batch' モジュールの以前のバージョン (バージョン 1.1.2 以前) と互換性がありません。</span><span class="sxs-lookup"><span data-stu-id="40284-191">Version 1.7.1 of the ‘Az.Resources’ module is incompatible with earlier versions (version 1.1.2 or earlier) of the ‘Az.Batch’ module.</span></span>  <span data-ttu-id="40284-192">これにより、'Az.Resources' モジュールのバージョン 1.7.1 がインポートされたときに、'Az.Batch' モジュールのバージョン 1.1.2 をインポートできなくなります。</span><span class="sxs-lookup"><span data-stu-id="40284-192">This will result in being unable to import  version 1.1.2 of the ‘Az.Batch’ module when version 1.7.1 of the ‘Az.Resources’ module is imported.</span></span>  <span data-ttu-id="40284-193">この問題を解決するには、'Az.Batch' モジュールをバージョン 2.0.1 以上に更新するか、'Az' モジュールの最新バージョンをインストールします。</span><span class="sxs-lookup"><span data-stu-id="40284-193">To fix this issue, update the ‘Az.Batch’ module to version 2.0.1 or greater, or simply install the latest version of the ‘Az’ module.</span></span>

## <a name="servicefabric"></a><span data-ttu-id="40284-194">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="40284-194">ServiceFabric</span></span>

### `Add-ServiceFabricApplicationCertificate`
<span data-ttu-id="40284-195">`Add-ServiceFabricApplicationCertificate` を削除しました。このシナリオは `Add-AzVmssSecret` によりカバーされます。</span><span class="sxs-lookup"><span data-stu-id="40284-195">Removed `Add-ServiceFabricApplicationCertificate` as this scenario is covered by `Add-AzVmssSecret`.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-196">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-196">Before</span></span>
```powershell
Add-AzServiceFabricApplicationCertificate -ResourceGroupName "Group1" -Name "Contoso01SFCluster" -SecretIdentifier "http://keyVaultName.vault.contoso.net/secrets/secretName/secretVersion"
```

#### <a name="after"></a><span data-ttu-id="40284-197">After</span><span class="sxs-lookup"><span data-stu-id="40284-197">After</span></span>
```powershell
$Vault = Get-AzKeyVault -VaultName "ContosoVault"
$CertConfig = New-AzVmssVaultCertificateConfig -CertificateUrl "http://keyVaultName.vault.contoso.net/secrets/secretName/secretVersion" -CertificateStore "Certificates"
$VMSS = New-AzVmssConfig
Add-AzVmssSecret -VirtualMachineScaleSet $VMSS -SourceVaultId $Vault.ResourceId -VaultCertificate $CertConfig
```


## <a name="sql"></a><span data-ttu-id="40284-198">Sql</span><span class="sxs-lookup"><span data-stu-id="40284-198">Sql</span></span>

### `Get-AzSqlDatabaseSecureConnectionPolicy`
<span data-ttu-id="40284-199">セキュリティで保護された接続は非推奨となるため、コマンドは削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-199">Note that secure connection is deprecated and so command is removed.</span></span> <span data-ttu-id="40284-200">接続文字列を表示するには、Azure portal の [SQL データベース] ブレードを使用してください</span><span class="sxs-lookup"><span data-stu-id="40284-200">Please use the SQL database blade in the Azure portal to view the connection strings</span></span>

### `Get-AzSqlDatabaseIndexRecommendations`
<span data-ttu-id="40284-201">`Get-AzSqlDatabaseIndexRecommendations` エイリアスが削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-201">`Get-AzSqlDatabaseIndexRecommendations` alias is removed.</span></span> <span data-ttu-id="40284-202">代わりに `Get-AzSqlDatabaseIndexRecommendation` を使用してください</span><span class="sxs-lookup"><span data-stu-id="40284-202">Use `Get-AzSqlDatabaseIndexRecommendation` instead.</span></span>

### `Get-AzSqlDatabaseRestorePoints`
<span data-ttu-id="40284-203">`Get-AzSqlDatabaseRestorePoints` エイリアスが削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-203">`Get-AzSqlDatabaseRestorePoints` alias is removed.</span></span> <span data-ttu-id="40284-204">代わりに `Get-AzSqlDatabaseRestorePoint` を使用してください</span><span class="sxs-lookup"><span data-stu-id="40284-204">Use `Get-AzSqlDatabaseRestorePoint` instead.</span></span>

### `Get-AzSqlDatabaseAuditing`
- <span data-ttu-id="40284-205">コマンドレット `Get-AzSqlDatabaseAudit` がこのコマンドレットを置き換えます。</span><span class="sxs-lookup"><span data-stu-id="40284-205">The cmdlet `Get-AzSqlDatabaseAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="40284-206">出力の型は、既存の型 'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' から新しい型 'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseAuditingSettingsModel' に変更され、プロパティ `AuditState` および `StorageAccountName` は削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-206">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseAuditingSettingsModel', removing properties `AuditState` and `StorageAccountName`.</span></span> <span data-ttu-id="40284-207">と `StorageAccountSubscriptionId`の両方で使用できます。</span><span class="sxs-lookup"><span data-stu-id="40284-207">and `StorageAccountSubscriptionId`.</span></span>  <span data-ttu-id="40284-208">スクリプトでは、新しい `StorageAccountResourceId` プロパティからストレージ アカウント情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="40284-208">Scripts can retrieve storage account information from the new `StorageAccountResourceId` property.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-209">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-209">Before</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseAuditing -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
DatabaseName                 : database01
AuditAction                  : {}
AuditActionGroup             : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP,
                                BATCH_COMPLETED_GROUP, ...}
ResourceGroupName            : resourcegroup01
ServerName                   : server01
AuditState                   : Enabled
StorageAccountName           : mystorage
StorageKeyType               : Primary
RetentionInDays              : 0
StorageAccountSubscriptionId : 7fe3301d-31d3-4668-af5e-211a890ba6e3
PredicateExpression          : statement <> 'select 1'
```

#### <a name="after"></a><span data-ttu-id="40284-210">After</span><span class="sxs-lookup"><span data-stu-id="40284-210">After</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseAudit -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01"
ServerName                          : server01
DatabaseName                        : database01
AuditAction                         : {}
ResourceGroupName                   : resourcegroup01
AuditActionGroup                    : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP,
                                       BATCH_COMPLETED_GROUP, ...}
PredicateExpression                 : statement <> 'select 1'
BlobStorageTargetState              : Enabled
StorageAccountResourceId            : /subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage
StorageKeyType                      : Primary
RetentionInDays                     : 0
EventHubTargetState                 : Enabled
EventHubName                        : eventHubName
EventHubAuthorizationRuleResourceId : EventHubAuthorizationRuleResourceId
LogAnalyticsTargetState             : Enabled
WorkspaceResourceId                 : "/subscriptions/4b9e8510-67ab-4e9a-95a9-e2f1e570ea9c/resourceGroups/insights-integration/providers/Microsoft.OperationalInsights/workspaces/viruela2"
```

### `Set-AzSqlDatabaseAuditing`
- <span data-ttu-id="40284-211">コマンドレット `Set-AzSqlDatabaseAudit` がこのコマンドレットを置き換えます。</span><span class="sxs-lookup"><span data-stu-id="40284-211">The cmdlet `Set-AzSqlDatabaseAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="40284-212">出力の型は、既存の型 'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' から新しい型 'bool' に変更されます</span><span class="sxs-lookup"><span data-stu-id="40284-212">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'bool'</span></span>

#### <a name="before"></a><span data-ttu-id="40284-213">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-213">Before</span></span>
```powershell
Set-AzSqlDatabaseAuditing -State Enabled -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -StorageAccountName "Storage22" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-214">After</span><span class="sxs-lookup"><span data-stu-id="40284-214">After</span></span>
```powershell
Set-AzSqlDatabaseAudit -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -DatabaseName "Database01" -BlobStorageTargetState Enabled -StorageAccountResourceId "/subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage"
```

### `Get-AzSqlServerAuditing`
- <span data-ttu-id="40284-215">コマンドレット `Get-AzSqlServerAudit` がこのコマンドレットを置き換えます。</span><span class="sxs-lookup"><span data-stu-id="40284-215">The cmdlet `Get-AzSqlServerAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="40284-216">出力の型は、既存の型 'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' から新しい型 'Microsoft.Azure.Commands.Sql.Auditing.Model.ServerAuditingSettingsModel' に変更されます。</span><span class="sxs-lookup"><span data-stu-id="40284-216">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'Microsoft.Azure.Commands.Sql.Auditing.Model.ServerAuditingSettingsModel'.</span></span>  <span data-ttu-id="40284-217">プロパティ `AuditState`、`StorageAccountName`、および `StorageAccountSubscriptionId` は削除されます。</span><span class="sxs-lookup"><span data-stu-id="40284-217">Properties `AuditState`, `StorageAccountName`, and `StorageAccountSubscriptionId` are removed.</span></span>  <span data-ttu-id="40284-218">`StorageAccountName` および `StorageAccountSubscriptionId` プロパティを使用するスクリプトは、新しい `StorageAccountResourceId` プロパティからこの情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="40284-218">Scripts that use `StorageAccountName` and `StorageAccountSubscriptionId` proeprties can retrieve this information from the new `StorageAccountResourceId` property.</span></span>

#### <a name="before"></a><span data-ttu-id="40284-219">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-219">Before</span></span>
```powershell
PS C:\> Get-AzSqlServerAuditing -ResourceGroupName "resourcegroup01" -ServerName "server01"
AuditActionGroup             : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP, BATCH_COMPLETED_GROUP, ...}
ResourceGroupName            : resourcegroup01
ServerName                   : server01
AuditState                   : Enabled
StorageAccountName           : mystorage
StorageKeyType               : Primary
RetentionInDays              : 0
StorageAccountSubscriptionId : 7fe3301d-31d3-4668-af5e-211a890ba6e3
PredicateExpression          : statement <> 'select 1'
```

#### <a name="after"></a><span data-ttu-id="40284-220">After</span><span class="sxs-lookup"><span data-stu-id="40284-220">After</span></span>
```powershell
PS C:\> Get-AzSqlServerAudit -ResourceGroupName "resourcegroup01" -ServerName "server01"
ServerName                          : server01
ResourceGroupName                   : resourcegroup01
AuditActionGroup                    : {SUCCESSFUL_DATABASE_AUTHENTICATION_GROUP, FAILED_DATABASE_AUTHENTICATION_GROUP, BATCH_COMPLETED_GROUP, ...}
PredicateExpression                 : statement <> 'select 1'
BlobStorageTargetState              : Enabled
StorageAccountResourceId            : /subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage
StorageKeyType                      : Primary
RetentionInDays                     : 0
EventHubTargetState                 : Enabled
EventHubName                        : eventHubName
EventHubAuthorizationRuleResourceId : EventHubAuthorizationRuleResourceId
LogAnalyticsTargetState             : Enabled
WorkspaceResourceId                 : "/subscriptions/4b9e8510-67ab-4e9a-95a9-e2f1e570ea9c/resourceGroups/insights-integration/providers/Microsoft.OperationalInsights/workspaces/viruela2"
```

### `Set-AzSqlServerAuditing`
- <span data-ttu-id="40284-221">コマンドレット `Set-AzSqlServerAudit` がこのコマンドレットを置き換えます。</span><span class="sxs-lookup"><span data-stu-id="40284-221">The cmdlet `Set-AzSqlServerAudit` is replacing this cmdlet.</span></span>
- <span data-ttu-id="40284-222">出力の型は、既存の型 'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' から新しい型 'bool' に変更されます</span><span class="sxs-lookup"><span data-stu-id="40284-222">The output type is changing from the existing type :'Microsoft.Azure.Commands.Sql.Auditing.Model.DatabaseBlobAuditingSettingsModel' to the new type :'bool'</span></span>

#### <a name="before"></a><span data-ttu-id="40284-223">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-223">Before</span></span>
```powershell
Set-AzSqlServerAuditing -State Enabled -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -StorageAccountName "Storage22"
```

#### <a name="after"></a><span data-ttu-id="40284-224">After</span><span class="sxs-lookup"><span data-stu-id="40284-224">After</span></span>
```powershell
PS C:\> Set-AzSqlServerAudit -ResourceGroupName "ResourceGroup01" -ServerName "Server01" -BlobStorageTargetState Enabled -StorageAccountResourceId "/subscriptions/7fe3301d-31d3-4668-af5e-211a890ba6e3/resourceGroups/resourcegroup01/providers/Microsoft.Storage/storageAccounts/mystorage"
```

### `Get-AzSqlServerAdvancedThreatProtectionSettings`
<span data-ttu-id="40284-225">コマンドレット `Get-AzSqlServerAdvancedThreatProtectionSettings` が `Get-AzSqlServerAdvancedThreatProtectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-225">Cmdlet `Get-AzSqlServerAdvancedThreatProtectionSettings` is replaced by `Get-AzSqlServerAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-226">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-226">Before</span></span>
```powershell
Get-AzSqlServerAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

#### <a name="after"></a><span data-ttu-id="40284-227">After</span><span class="sxs-lookup"><span data-stu-id="40284-227">After</span></span>
```powershell
Get-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

### `Clear-AzSqlServerAdvancedThreatProtectionSettings`
<span data-ttu-id="40284-228">コマンドレット `Clear-AzSqlServerAdvancedThreatProtectionSettings` が `Clear-AzSqlServerAdvancedThreatProtectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-228">Cmdlet `Clear-AzSqlServerAdvancedThreatProtectionSettings` is replaced by `Clear-AzSqlServerAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-229">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-229">Before</span></span>
```powershell
Clear-AzSqlServerAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

#### <a name="after"></a><span data-ttu-id="40284-230">After</span><span class="sxs-lookup"><span data-stu-id="40284-230">After</span></span>
```powershell
Clear-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

### `Update-AzSqlServerAdvancedThreatProtectionSettings`
<span data-ttu-id="40284-231">コマンドレット `Update-AzSqlServerAdvancedThreatProtectionSettings` が `Update-AzSqlServerAdvancedThreatProtectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-231">Cmdlet `Update-AzSqlServerAdvancedThreatProtectionSettings` is replaced by `Update-AzSqlServerAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-232">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-232">Before</span></span>
```powershell
Update-AzSqlServerAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="40284-233">After</span><span class="sxs-lookup"><span data-stu-id="40284-233">After</span></span>
```powershell
Update-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Get-AzSqlDatabaseAdvancedThreatProtectionSettings`
<span data-ttu-id="40284-234">コマンドレット `Get-AzSqlDatabaseAdvancedThreatProtectionSettings` が `Get-AzSqlDatabaseAdvancedThreatProtectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-234">Cmdlet `Get-AzSqlDatabaseAdvancedThreatProtectionSettings` is replaced by `Get-AzSqlDatabaseAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-235">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-235">Before</span></span>
```powershell
Get-AzSqlDatabaseAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-236">After</span><span class="sxs-lookup"><span data-stu-id="40284-236">After</span></span>
```powershell
Get-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

### `Update-AzSqlDatabaseAdvancedThreatProtectionSettings`
<span data-ttu-id="40284-237">コマンドレット `Update-AzSqlDatabaseAdvancedThreatProtectionSettings` が `Update-AzSqlDatabaseAdvancedThreatProtectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-237">Cmdlet `Update-AzSqlDatabaseAdvancedThreatProtectionSettings` is repleaced by `Update-AzSqlDatabaseAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-238">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-238">Before</span></span>
```powershell
Update-AzSqlDatabaseAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="40284-239">After</span><span class="sxs-lookup"><span data-stu-id="40284-239">After</span></span>
```powershell
Update-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Clear-AzSqlDatabaseAdvancedThreatProtectionSettings`
<span data-ttu-id="40284-240">コマンドレット `Clear-AzSqlDatabaseAdvancedThreatProtectionSettings` が `Clear-AzSqlDatabaseAdvancedThreatProtectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-240">Cmdlet `Clear-AzSqlDatabaseAdvancedThreatProtectionSettings` is repleaced by `Clear-AzSqlDatabaseAdvancedThreatProtectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-241">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-241">Before</span></span>
```powershell
Clear-AzSqlDatabaseAdvancedThreatProtectionSettings -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-242">After</span><span class="sxs-lookup"><span data-stu-id="40284-242">After</span></span>
```powershell
Clear-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

### `Update-AzSqlDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-243">コマンドレット `Update-AzSqlDatabaseVulnerabilityAssessmentSettings` が `Update-AzSqlDatabaseVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-243">Cmdlet `Update-AzSqlDatabaseVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-244">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-244">Before</span></span>
```powershell
Update-AzSqlDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="40284-245">After</span><span class="sxs-lookup"><span data-stu-id="40284-245">After</span></span>
```powershell
Update-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```


### `Get-AzSqlDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-246">コマンドレット `Get-AzSqlDatabaseVulnerabilityAssessmentSettings` が `Get-AzSqlDatabaseVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-246">Cmdlet `Get-AzSqlDatabaseVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-247">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-247">Before</span></span>
```powershell
Get-AzSqlDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-248">After</span><span class="sxs-lookup"><span data-stu-id="40284-248">After</span></span>
```powershell
Get-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-249">コマンドレット `Clear-AzSqlDatabaseVulnerabilityAssessmentSettings` が `Clear-AzSqlDatabaseVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-249">Cmdlet `Clear-AzSqlDatabaseVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-250">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-250">Before</span></span>
```powershell
Clear-AzSqlDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-251">After</span><span class="sxs-lookup"><span data-stu-id="40284-251">After</span></span>
```powershell
Clear-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-252">コマンドレット `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` が `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-252">Cmdlet `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-253">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-253">Before</span></span>
```powershell
Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="40284-254">After</span><span class="sxs-lookup"><span data-stu-id="40284-254">After</span></span>
```powershell
Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -DatabaseName "Database01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

### `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-255">コマンドレット `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` が `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-255">Cmdlet `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-256">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-256">Before</span></span>
```powershell
Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-257">After</span><span class="sxs-lookup"><span data-stu-id="40284-257">After</span></span>
```powershell
Get-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-258">コマンドレット `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` が `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-258">Cmdlet `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-259">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-259">Before</span></span>
```powershell
Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-260">After</span><span class="sxs-lookup"><span data-stu-id="40284-260">After</span></span>
```powershell
Clear-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Update-AzSqlInstanceVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-261">コマンドレット `Update-AzSqlInstanceVulnerabilityAssessmentSettings` が `Update-AzSqlInstanceVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-261">Cmdlet `Update-AzSqlInstanceVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlInstanceVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-262">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-262">Before</span></span>
```powershell
Update-AzSqlInstanceVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="40284-263">After</span><span class="sxs-lookup"><span data-stu-id="40284-263">After</span></span>
```powershell
Update-AzSqlInstanceVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -InstanceName "ManagedInstance01" `
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

### `Get-AzSqlInstanceVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-264">コマンドレット `Get-AzSqlInstanceVulnerabilityAssessmentSettings` が `Get-AzSqlInstanceVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-264">Cmdlet `Get-AzSqlInstanceVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlInstanceVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-265">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-265">Before</span></span>
```powershell
Get-AzSqlInstanceVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-266">After</span><span class="sxs-lookup"><span data-stu-id="40284-266">After</span></span>
```powershell
Get-AzSqlInstanceVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlInstanceVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-267">コマンドレット `Clear-AzSqlInstanceVulnerabilityAssessmentSettings` が `Clear-AzSqlInstanceVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-267">Cmdlet `Clear-AzSqlInstanceVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlInstanceVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-268">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-268">Before</span></span>
```powershell
Clear-AzSqlInstanceVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-269">After</span><span class="sxs-lookup"><span data-stu-id="40284-269">After</span></span>
```powershell
Clear-AzSqlInstanceVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Update-AzSqlServerVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-270">コマンドレット `Update-AzSqlServerVulnerabilityAssessmentSettings` が `Update-AzSqlServerVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-270">Cmdlet `Update-AzSqlServerVulnerabilityAssessmentSettings` is repleaced by `Update-AzSqlServerVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-271">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-271">Before</span></span>
```powershell
Update-AzSqlServerVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

#### <a name="after"></a><span data-ttu-id="40284-272">After</span><span class="sxs-lookup"><span data-stu-id="40284-272">After</span></span>
```powershell
Update-AzSqlServerVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01"`
    -ServerName "Server01"`
    -StorageAccountName "mystorage" `
    -ScanResultsContainerName "vulnerability-assessment" `
    -RecurringScansInterval Weekly `
    -EmailSubscriptionAdmins $true `
    -NotificationEmail @("mail1@mail.com" , "mail2@mail.com")
```

### `Get-AzSqlServerVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-273">コマンドレット `Get-AzSqlServerVulnerabilityAssessmentSettings` が `Get-AzSqlServerVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-273">Cmdlet `Get-AzSqlServerVulnerabilityAssessmentSettings` is repleaced by `Get-AzSqlServerVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-274">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-274">Before</span></span>
```powershell
Get-AzSqlServerVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-275">After</span><span class="sxs-lookup"><span data-stu-id="40284-275">After</span></span>
```powershell
Get-AzSqlServerVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Clear-AzSqlServerVulnerabilityAssessmentSettings`
<span data-ttu-id="40284-276">コマンドレット `Clear-AzSqlServerVulnerabilityAssessmentSettings` が `Clear-AzSqlServerVulnerabilityAssessmentSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-276">Cmdlet `Clear-AzSqlServerVulnerabilityAssessmentSettings` is repleaced by `Clear-AzSqlServerVulnerabilityAssessmentSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-277">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-277">Before</span></span>
```powershell
Clear-AzSqlServerVulnerabilityAssessmentSettings `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-278">After</span><span class="sxs-lookup"><span data-stu-id="40284-278">After</span></span>
```powershell
Clear-AzSqlDatabaseVulnerabilityAssessmentSetting `
    -ResourceGroupName "ResourceGroup01" `
    -ServerName "Server01" `
    -DatabaseName "Database01"
```

### `Get-AzSqlServerAdvancedThreatProtectionPolicy`
<span data-ttu-id="40284-279">コマンドレット `Get-AzSqlServerAdvancedThreatProtectionPolicy` が削除され、これに置き換わるコマンドレットはありません</span><span class="sxs-lookup"><span data-stu-id="40284-279">Cmdlet `Get-AzSqlServerAdvancedThreatProtectionPolicy` is deleted and no cmdlet is repleaced it</span></span>

### `Get-AzSqlServerThreatDetectionPolicy`
<span data-ttu-id="40284-280">コマンドレット `Get-AzSqlServerThreatDetectionPolicy` が `Get-AzSqlServerThreatDetectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-280">Cmdlet `Get-AzSqlServerThreatDetectionPolicy` is repleaced by `Get-AzSqlServerThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-281">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-281">Before</span></span>
```powershell
PS C:\> Get-AzSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

#### <a name="after"></a><span data-ttu-id="40284-282">After</span><span class="sxs-lookup"><span data-stu-id="40284-282">After</span></span>
```powershell
PS C:\> Get-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

### `Remove-AzSqlServerThreatDetectionPolicy`
<span data-ttu-id="40284-283">コマンドレット `Remove-AzSqlServerThreatDetectionPolicy` が `Clear-AzSqlServerThreatDetectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-283">Cmdlet `Remove-AzSqlServerThreatDetectionPolicy` is repleaced by `Clear-AzSqlServerThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-284">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-284">Before</span></span>
```powershell
Remove-AzSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

#### <a name="after"></a><span data-ttu-id="40284-285">After</span><span class="sxs-lookup"><span data-stu-id="40284-285">After</span></span>
```powershell
Clear-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"
```

### `Set-AzSqlServerThreatDetectionPolicy`
<span data-ttu-id="40284-286">コマンドレット `Set-AzSqlServerThreatDetectionPolicy` が `Update-AzSqlServerThreatDetectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-286">Cmdlet `Set-AzSqlServerThreatDetectionPolicy` is repleaced by `Update-AzSqlServerThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-287">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-287">Before</span></span>
```powershell
Set-AzSqlServerThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="40284-288">After</span><span class="sxs-lookup"><span data-stu-id="40284-288">After</span></span>
```powershell
Update-AzSqlServerAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability","SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Get-AzSqlDatabaseThreatDetectionPolicy`
<span data-ttu-id="40284-289">コマンドレット `Get-AzSqlDatabaseThreatDetectionPolicy` が `Get-AzSqlDatabaseThreatDetectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-289">Cmdlet `Get-AzSqlDatabaseThreatDetectionPolicy` is repleaced by `Get-AzSqlDatabaseThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-290">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-290">Before</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName   "Database01"
DatabaseName                 : Database01
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

#### <a name="after"></a><span data-ttu-id="40284-291">After</span><span class="sxs-lookup"><span data-stu-id="40284-291">After</span></span>
```powershell
PS C:\> Get-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01"   -DatabaseName "Database01"
DatabaseName                 : Database01
ResourceGroupName            : ResourceGroup11
ServerName                   : Server01
ThreatDetectionState         : Enabled
NotificationRecipientsEmails : admin@myCompany.com
StorageAccountName           : mystorage
EmailAdmins                  : True
ExcludedDetectionTypes       : {}
RetentionInDays              : 0
```

### `Set-AzSqlDatabaseThreatDetectionPolicy`
<span data-ttu-id="40284-292">コマンドレット `Set-AzSqlDatabaseThreatDetectionPolicy` が `Update-AzSqlDatabaseThreatDetectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-292">Cmdlet `Set-AzSqlDatabaseThreatDetectionPolicy` is repleaced by `Update-AzSqlDatabaseThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-293">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-293">Before</span></span>
```powershell
Set-AzSqlDatabaseThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

#### <a name="after"></a><span data-ttu-id="40284-294">After</span><span class="sxs-lookup"><span data-stu-id="40284-294">After</span></span>
```powershell
Update-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01" -NotificationRecipientsEmails "admin01@contoso.com;secadmin@contoso.com" -EmailAdmins $False -ExcludedDetectionType "Sql_Injection_Vulnerability", "SQL_Injection" -StorageAccountName "mystorageAccount"
```

### `Remove-AzSqlDatabaseThreatDetectionPolicy`
<span data-ttu-id="40284-295">コマンドレット `Remove-AzSqlDatabaseThreatDetectionPolicy` が `Clear-AzSqlDatabaseThreatDetectionSetting` に置き換えられました</span><span class="sxs-lookup"><span data-stu-id="40284-295">Cmdlet `Remove-AzSqlDatabaseThreatDetectionPolicy` is repleaced by `Clear-AzSqlDatabaseThreatDetectionSetting`</span></span>

#### <a name="before"></a><span data-ttu-id="40284-296">[指定日付より前]</span><span class="sxs-lookup"><span data-stu-id="40284-296">Before</span></span>
```powershell
Remove-AzSqlDatabaseThreatDetectionPolicy -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```

#### <a name="after"></a><span data-ttu-id="40284-297">After</span><span class="sxs-lookup"><span data-stu-id="40284-297">After</span></span>
```powershell
Clear-AzSqlDatabaseAdvancedThreatProtectionSetting -ResourceGroupName "ResourceGroup11" -ServerName "Server01" -DatabaseName "Database01"
```
