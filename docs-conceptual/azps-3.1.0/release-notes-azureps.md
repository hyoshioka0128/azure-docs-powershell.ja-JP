---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: 2280b594ee9f525b2fa3175c917f6365cea354ba
ms.sourcegitcommit: 45e1823aa1a792840aa4829831b5f67a9d5d24a0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/26/2019
ms.locfileid: "74537125"
---
## <a name="310---november-2019"></a><span data-ttu-id="59cdc-103">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-103">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="59cdc-104">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="59cdc-104">Highlights since the last major release</span></span>
* <span data-ttu-id="59cdc-105">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-105">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="59cdc-106">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-106">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-107">Az.Compute</span></span>
* <span data-ttu-id="59cdc-108">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="59cdc-108">VM Reapply feature</span></span>
    - <span data-ttu-id="59cdc-109">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-109">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="59cdc-110">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="59cdc-110">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="59cdc-111">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="59cdc-111">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="59cdc-112">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-112">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="59cdc-113">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-113">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="59cdc-114">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-114">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="59cdc-115">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="59cdc-115">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="59cdc-116">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-116">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="59cdc-117">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-117">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="59cdc-118">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-118">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="59cdc-119">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="59cdc-119">Az.DataBoxEdge</span></span>
* <span data-ttu-id="59cdc-120">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-120">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="59cdc-121">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="59cdc-121">Get the Order</span></span>
* <span data-ttu-id="59cdc-122">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-122">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="59cdc-123">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-123">Create new Order</span></span>
* <span data-ttu-id="59cdc-124">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-124">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="59cdc-125">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-125">Remove the Order</span></span>
* <span data-ttu-id="59cdc-126">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="59cdc-126">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="59cdc-127">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="59cdc-127">Now creates Local Share</span></span>
* <span data-ttu-id="59cdc-128">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-128">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="59cdc-129">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-129">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="59cdc-130">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-130">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="59cdc-131">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="59cdc-131">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="59cdc-132">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-132">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="59cdc-133">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="59cdc-133">Gets the information about Triggers</span></span>
* <span data-ttu-id="59cdc-134">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-134">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="59cdc-135">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-135">Create new Triggers</span></span>
* <span data-ttu-id="59cdc-136">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-136">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="59cdc-137">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-137">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-138">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-138">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-139">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-139">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="59cdc-140">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-140">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-141">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-141">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-142">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-142">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="59cdc-143">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-143">Az.EventHub</span></span>
* <span data-ttu-id="59cdc-144">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-144">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="59cdc-145">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="59cdc-145">Az.FrontDoor</span></span>
* <span data-ttu-id="59cdc-146">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-146">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="59cdc-147">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-147">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="59cdc-148">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-148">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="59cdc-149">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="59cdc-149">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-150">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-150">Az.Network</span></span>
* <span data-ttu-id="59cdc-151">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-151">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="59cdc-152">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="59cdc-152">Az.PrivateDns</span></span>
* <span data-ttu-id="59cdc-153">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-153">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-154">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-154">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-155">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="59cdc-155">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="59cdc-156">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="59cdc-156">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="59cdc-157">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="59cdc-157">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="59cdc-158">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="59cdc-158">Az.RedisCache</span></span>
* <span data-ttu-id="59cdc-159">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-159">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="59cdc-160">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-160">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="59cdc-161">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-161">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-162">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-162">Az.Resources</span></span>
- <span data-ttu-id="59cdc-163">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-163">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="59cdc-164">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-164">Updated create policy definition help example</span></span>
- <span data-ttu-id="59cdc-165">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-165">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="59cdc-166">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-166">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="59cdc-167">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-167">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-168">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-168">Az.Sql</span></span>
* <span data-ttu-id="59cdc-169">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-169">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="59cdc-170">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-170">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="59cdc-171">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-171">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="59cdc-172">全般</span><span class="sxs-lookup"><span data-stu-id="59cdc-172">General</span></span>
* <span data-ttu-id="59cdc-173">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-173">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="59cdc-174">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-174">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-175">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-175">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="59cdc-176">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="59cdc-176">Az.Advisor</span></span>
* <span data-ttu-id="59cdc-177">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-177">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="59cdc-178">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="59cdc-178">Az.Batch</span></span>
* <span data-ttu-id="59cdc-179">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-179">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="59cdc-180">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="59cdc-180">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="59cdc-181">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-181">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="59cdc-182">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-182">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="59cdc-183">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="59cdc-183">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="59cdc-184">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-184">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="59cdc-185">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-185">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="59cdc-186">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-186">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="59cdc-187">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-187">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="59cdc-188">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-188">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="59cdc-189">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-189">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="59cdc-190">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-190">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="59cdc-191">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-191">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="59cdc-192">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-192">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="59cdc-193">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-193">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="59cdc-194">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-194">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="59cdc-195">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-195">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="59cdc-196">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-196">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="59cdc-197">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-197">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="59cdc-198">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="59cdc-198">This operation is no longer supported.</span></span>
* <span data-ttu-id="59cdc-199">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-199">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="59cdc-200">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-200">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="59cdc-201">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-201">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="59cdc-202">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-202">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="59cdc-203">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-203">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="59cdc-204">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-204">New non-verified images are also now returned.</span></span> <span data-ttu-id="59cdc-205">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="59cdc-205">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="59cdc-206">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-206">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="59cdc-207">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-207">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="59cdc-208">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-208">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="59cdc-209">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-209">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="59cdc-210">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-210">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="59cdc-211">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-211">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="59cdc-212">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-212">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="59cdc-213">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-213">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="59cdc-214">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-214">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="59cdc-215">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cdc-215">Az.Cdn</span></span>
* <span data-ttu-id="59cdc-216">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-216">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="59cdc-217">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-217">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-218">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-218">Az.Compute</span></span>
* <span data-ttu-id="59cdc-219">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="59cdc-219">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="59cdc-220">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-220">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="59cdc-221">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="59cdc-221">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="59cdc-222">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="59cdc-222">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="59cdc-223">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-223">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="59cdc-224">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-224">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="59cdc-225">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="59cdc-225">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="59cdc-226">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-226">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="59cdc-227">重大な変更</span><span class="sxs-lookup"><span data-stu-id="59cdc-227">Breaking changes</span></span>
    - <span data-ttu-id="59cdc-228">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="59cdc-228">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="59cdc-229">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="59cdc-229">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-230">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-230">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-231">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-231">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-232">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-232">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-233">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="59cdc-233">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="59cdc-234">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-234">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="59cdc-235">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="59cdc-235">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="59cdc-236">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-236">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="59cdc-237">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-237">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="59cdc-238">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-238">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="59cdc-239">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="59cdc-239">Az.FrontDoor</span></span>
* <span data-ttu-id="59cdc-240">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-240">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="59cdc-241">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="59cdc-241">Az.HDInsight</span></span>
* <span data-ttu-id="59cdc-242">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-242">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="59cdc-243">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-243">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="59cdc-244">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-244">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="59cdc-245">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-245">Removed five cmdlets:</span></span>
    - <span data-ttu-id="59cdc-246">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="59cdc-246">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="59cdc-247">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="59cdc-247">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="59cdc-248">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="59cdc-248">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="59cdc-249">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="59cdc-249">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="59cdc-250">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="59cdc-250">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="59cdc-251">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-251">Added three cmdlets:</span></span>
    - <span data-ttu-id="59cdc-252">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-252">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="59cdc-253">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-253">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="59cdc-254">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-254">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="59cdc-255">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-255">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="59cdc-256">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-256">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="59cdc-257">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-257">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="59cdc-258">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="59cdc-258">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="59cdc-259">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-259">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="59cdc-260">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-260">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="59cdc-261">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-261">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="59cdc-262">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-262">Added some scenario test cases.</span></span>
* <span data-ttu-id="59cdc-263">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="59cdc-263">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-264">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-264">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-265">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="59cdc-265">Breaking changes:</span></span>
    - <span data-ttu-id="59cdc-266">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-266">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="59cdc-267">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-267">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="59cdc-268">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-268">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="59cdc-269">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-269">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="59cdc-270">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-270">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="59cdc-271">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-271">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="59cdc-272">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-272">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="59cdc-273">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-273">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="59cdc-274">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-274">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="59cdc-275">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-275">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="59cdc-276">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-276">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="59cdc-277">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-277">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-278">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-278">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-279">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-279">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-280">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-280">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="59cdc-281">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-281">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="59cdc-282">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-282">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-283">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-283">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-284">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-284">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-285">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-285">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-286">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-286">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-287">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-287">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-288">Az.Resources</span></span>
* <span data-ttu-id="59cdc-289">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-289">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-290">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-290">Az.Network</span></span>
* <span data-ttu-id="59cdc-291">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-291">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="59cdc-292">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-292">Updated cmdlet:</span></span>
        - <span data-ttu-id="59cdc-293">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-293">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-294">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-294">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-295">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-295">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-296">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-296">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-297">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-297">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="59cdc-298">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="59cdc-298">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="59cdc-299">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-299">New cmdlet:</span></span>
        - <span data-ttu-id="59cdc-300">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="59cdc-300">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="59cdc-301">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-301">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="59cdc-302">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-302">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="59cdc-303">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-303">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="59cdc-304">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-304">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="59cdc-305">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-305">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="59cdc-306">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-306">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="59cdc-307">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-307">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="59cdc-308">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-308">New cmdlets added:</span></span>
        - <span data-ttu-id="59cdc-309">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="59cdc-309">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="59cdc-310">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-310">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="59cdc-311">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-311">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="59cdc-312">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-312">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="59cdc-313">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-313">Set-AzVirtualHub</span></span>
* <span data-ttu-id="59cdc-314">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-314">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="59cdc-315">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="59cdc-315">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="59cdc-316">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-316">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="59cdc-317">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-317">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="59cdc-318">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-318">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="59cdc-319">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-319">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="59cdc-320">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-320">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="59cdc-321">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-321">New cmdlets added:</span></span>
        - <span data-ttu-id="59cdc-322">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-322">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="59cdc-323">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="59cdc-323">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="59cdc-324">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-324">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="59cdc-325">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-325">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="59cdc-326">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-326">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="59cdc-327">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-327">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="59cdc-328">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-328">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="59cdc-329">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-329">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="59cdc-330">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-330">New cmdlets added:</span></span>
        - <span data-ttu-id="59cdc-331">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="59cdc-331">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="59cdc-332">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="59cdc-332">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="59cdc-333">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="59cdc-333">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="59cdc-334">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="59cdc-334">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="59cdc-335">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-335">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="59cdc-336">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-336">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="59cdc-337">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="59cdc-337">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="59cdc-338">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-338">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="59cdc-339">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-339">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="59cdc-340">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-340">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="59cdc-341">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-341">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="59cdc-342">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="59cdc-342">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="59cdc-343">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-343">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="59cdc-344">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-344">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="59cdc-345">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-345">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="59cdc-346">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-346">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="59cdc-347">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-347">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="59cdc-348">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-348">New cmdlets added:</span></span>
        - <span data-ttu-id="59cdc-349">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="59cdc-349">New-AzIpGroup</span></span>
        - <span data-ttu-id="59cdc-350">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="59cdc-350">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="59cdc-351">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="59cdc-351">Get-AzIpGroup</span></span>
        - <span data-ttu-id="59cdc-352">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="59cdc-352">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-353">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-353">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-354">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="59cdc-354">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-355">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-355">Az.Sql</span></span>
* <span data-ttu-id="59cdc-356">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-356">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="59cdc-357">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-357">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="59cdc-358">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-358">Removed deprecated aliases:</span></span>
* <span data-ttu-id="59cdc-359">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="59cdc-359">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="59cdc-360">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="59cdc-360">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="59cdc-361">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-361">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="59cdc-362">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-362">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="59cdc-363">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="59cdc-363">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="59cdc-364">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-364">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-365">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-365">Az.Storage</span></span>
* <span data-ttu-id="59cdc-366">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="59cdc-366">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="59cdc-367">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-367">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="59cdc-368">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-368">Set-AzStorageAccount</span></span>
* <span data-ttu-id="59cdc-369">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="59cdc-369">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="59cdc-370">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="59cdc-370">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="59cdc-371">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="59cdc-371">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="59cdc-372">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-372">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="59cdc-373">全般</span><span class="sxs-lookup"><span data-stu-id="59cdc-373">General</span></span>
* <span data-ttu-id="59cdc-374">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-374">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="59cdc-375">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-375">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-376">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-376">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="59cdc-377">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-377">Az.ApiManagement</span></span>
* <span data-ttu-id="59cdc-378">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-378">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="59cdc-379">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="59cdc-379">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-380">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-380">Az.Automation</span></span>
* <span data-ttu-id="59cdc-381">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-381">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="59cdc-382">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="59cdc-382">Az.Batch</span></span>
* <span data-ttu-id="59cdc-383">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-383">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-384">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-384">Az.Compute</span></span>
* <span data-ttu-id="59cdc-385">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-385">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="59cdc-386">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-386">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="59cdc-387">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-387">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="59cdc-388">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-388">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-389">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-389">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-390">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="59cdc-390">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="59cdc-391">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="59cdc-391">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="59cdc-392">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-392">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-393">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-393">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-394">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-394">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="59cdc-395">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="59cdc-395">Az.HealthcareApis</span></span>
* <span data-ttu-id="59cdc-396">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-396">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="59cdc-397">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-397">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="59cdc-398">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-398">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="59cdc-399">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-399">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-400">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-400">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-401">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="59cdc-401">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="59cdc-402">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="59cdc-402">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-403">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-403">Az.Monitor</span></span>
* <span data-ttu-id="59cdc-404">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="59cdc-404">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="59cdc-405">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-405">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="59cdc-406">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="59cdc-406">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="59cdc-407">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-407">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-408">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-408">Az.Network</span></span>
* <span data-ttu-id="59cdc-409">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-409">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="59cdc-410">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-410">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="59cdc-411">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-411">New cmdlets added:</span></span>
        - <span data-ttu-id="59cdc-412">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-412">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="59cdc-413">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-413">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="59cdc-414">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-414">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="59cdc-415">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-415">Updated cmdlets:</span></span>
        - <span data-ttu-id="59cdc-416">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-416">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="59cdc-417">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-417">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="59cdc-418">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-418">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="59cdc-419">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="59cdc-419">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="59cdc-420">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="59cdc-420">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="59cdc-421">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-421">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="59cdc-422">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-422">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="59cdc-423">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="59cdc-423">Az.RedisCache</span></span>
* <span data-ttu-id="59cdc-424">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-424">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-425">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-425">Az.Sql</span></span>
* <span data-ttu-id="59cdc-426">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-426">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-427">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-427">Az.Storage</span></span>
* <span data-ttu-id="59cdc-428">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="59cdc-428">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="59cdc-429">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="59cdc-429">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="59cdc-430">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="59cdc-430">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="59cdc-431">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="59cdc-431">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="59cdc-432">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-432">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="59cdc-433">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="59cdc-433">Az.StorageSync</span></span>
* <span data-ttu-id="59cdc-434">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-434">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-435">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-435">Az.Websites</span></span>
* <span data-ttu-id="59cdc-436">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="59cdc-436">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="59cdc-437">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-437">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="59cdc-438">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-438">Az.ApiManagement</span></span>
* <span data-ttu-id="59cdc-439">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-439">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="59cdc-440">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-440">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="59cdc-441">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="59cdc-441">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-442">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-442">Az.Automation</span></span>
* <span data-ttu-id="59cdc-443">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-443">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="59cdc-444">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-444">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="59cdc-445">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-445">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-446">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-446">Az.Compute</span></span>
* <span data-ttu-id="59cdc-447">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-447">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="59cdc-448">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-448">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="59cdc-449">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-449">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="59cdc-450">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-450">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="59cdc-451">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-451">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="59cdc-452">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-452">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="59cdc-453">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-453">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="59cdc-454">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-454">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="59cdc-455">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-455">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-456">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-456">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-457">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-457">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="59cdc-458">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-458">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="59cdc-459">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="59cdc-459">Az.HDInsight</span></span>
* <span data-ttu-id="59cdc-460">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="59cdc-460">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-461">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-461">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-462">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-462">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="59cdc-463">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-463">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="59cdc-464">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="59cdc-464">New cmdlets are:</span></span>
    - <span data-ttu-id="59cdc-465">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="59cdc-465">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="59cdc-466">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="59cdc-466">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="59cdc-467">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="59cdc-467">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="59cdc-468">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="59cdc-468">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-469">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-469">Az.Monitor</span></span>
* <span data-ttu-id="59cdc-470">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="59cdc-470">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="59cdc-471">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-471">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="59cdc-472">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="59cdc-472">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="59cdc-473">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-473">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="59cdc-474">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-474">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="59cdc-475">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-475">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="59cdc-476">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="59cdc-476">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="59cdc-477">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="59cdc-477">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="59cdc-478">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-478">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="59cdc-479">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-479">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="59cdc-480">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-480">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="59cdc-481">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="59cdc-481">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="59cdc-482">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-482">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="59cdc-483">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-483">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="59cdc-484">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-484">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="59cdc-485">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="59cdc-485">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="59cdc-486">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-486">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="59cdc-487">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-487">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="59cdc-488">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-488">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="59cdc-489">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-489">Overall improved help files</span></span>
* <span data-ttu-id="59cdc-490">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-490">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-491">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-491">Az.Network</span></span>
* <span data-ttu-id="59cdc-492">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-492">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="59cdc-493">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-493">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="59cdc-494">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-494">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="59cdc-495">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-495">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="59cdc-496">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-496">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="59cdc-497">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-497">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="59cdc-498">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-498">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="59cdc-499">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-499">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="59cdc-500">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-500">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="59cdc-501">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-501">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="59cdc-502">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-502">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="59cdc-503">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-503">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="59cdc-504">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-504">New cmdlets</span></span>
        - <span data-ttu-id="59cdc-505">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="59cdc-505">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="59cdc-506">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-506">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="59cdc-507">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-507">Updated cmdlet:</span></span>
        - <span data-ttu-id="59cdc-508">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="59cdc-508">New-VpnSite</span></span>
        - <span data-ttu-id="59cdc-509">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="59cdc-509">Update-VpnSite</span></span>
        - <span data-ttu-id="59cdc-510">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-510">New-VpnConnection</span></span>
        - <span data-ttu-id="59cdc-511">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-511">Update-VpnConnection</span></span>
* <span data-ttu-id="59cdc-512">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-512">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-513">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-513">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-514">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-514">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="59cdc-515">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-515">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-516">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-516">Az.Resources</span></span>
* <span data-ttu-id="59cdc-517">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-517">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-518">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-518">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-519">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-519">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="59cdc-520">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-520">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="59cdc-521">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="59cdc-521">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="59cdc-522">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="59cdc-522">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="59cdc-523">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="59cdc-523">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="59cdc-524">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="59cdc-524">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="59cdc-525">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="59cdc-525">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="59cdc-526">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="59cdc-526">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="59cdc-527">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="59cdc-527">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="59cdc-528">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="59cdc-528">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="59cdc-529">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="59cdc-529">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="59cdc-530">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="59cdc-530">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="59cdc-531">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="59cdc-531">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="59cdc-532">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="59cdc-532">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="59cdc-533">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="59cdc-533">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="59cdc-534">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-534">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="59cdc-535">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="59cdc-535">Az.SignalR</span></span>
* <span data-ttu-id="59cdc-536">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="59cdc-536">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-537">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-537">Az.Sql</span></span>
* <span data-ttu-id="59cdc-538">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-538">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="59cdc-539">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-539">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="59cdc-540">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-540">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="59cdc-541">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-541">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="59cdc-542">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-542">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-543">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-543">Az.Storage</span></span>
* <span data-ttu-id="59cdc-544">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-544">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="59cdc-545">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="59cdc-545">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="59cdc-546">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-546">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="59cdc-547">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-547">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="59cdc-548">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-548">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="59cdc-549">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-549">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="59cdc-550">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="59cdc-550">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="59cdc-551">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="59cdc-551">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="59cdc-552">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="59cdc-552">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="59cdc-553">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="59cdc-553">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="59cdc-554">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="59cdc-554">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-555">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-555">Az.Websites</span></span>
* <span data-ttu-id="59cdc-556">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-556">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="59cdc-557">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="59cdc-557">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="59cdc-558">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-558">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="59cdc-559">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-559">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="59cdc-560">全般</span><span class="sxs-lookup"><span data-stu-id="59cdc-560">General</span></span>
* <span data-ttu-id="59cdc-561">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-561">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="59cdc-562">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-562">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-563">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="59cdc-563">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="59cdc-564">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="59cdc-564">Az.Aks</span></span>
* <span data-ttu-id="59cdc-565">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-565">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="59cdc-566">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="59cdc-566">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="59cdc-567">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-567">Az.ApiManagement</span></span>
* <span data-ttu-id="59cdc-568">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="59cdc-568">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="59cdc-569">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="59cdc-569">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="59cdc-570">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-570">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="59cdc-571">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="59cdc-571">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="59cdc-572">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-572">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="59cdc-573">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="59cdc-573">Az.Batch</span></span>
* <span data-ttu-id="59cdc-574">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-574">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="59cdc-575">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cdc-575">Az.Cdn</span></span>
* <span data-ttu-id="59cdc-576">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-576">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-577">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-577">Az.Compute</span></span>
* <span data-ttu-id="59cdc-578">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-578">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="59cdc-579">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-579">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="59cdc-580">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-580">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="59cdc-581">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-581">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="59cdc-582">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="59cdc-582">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="59cdc-583">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="59cdc-583">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="59cdc-584">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-584">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="59cdc-585">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-585">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-586">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-586">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-587">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-587">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="59cdc-588">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-588">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="59cdc-589">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-589">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="59cdc-590">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-590">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-591">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-591">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-592">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-592">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="59cdc-593">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-593">Az.EventHub</span></span>
* <span data-ttu-id="59cdc-594">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="59cdc-594">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="59cdc-595">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="59cdc-595">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="59cdc-596">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-596">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="59cdc-597">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="59cdc-597">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="59cdc-598">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="59cdc-598">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="59cdc-599">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-599">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-600">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-600">Az.Monitor</span></span>
* <span data-ttu-id="59cdc-601">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-601">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-602">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-602">Az.Network</span></span>
* <span data-ttu-id="59cdc-603">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-603">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="59cdc-604">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-604">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="59cdc-605">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-605">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="59cdc-606">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-606">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="59cdc-607">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-607">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="59cdc-608">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-608">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="59cdc-609">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-609">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-610">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-610">Az.OperationalInsights</span></span>
* <span data-ttu-id="59cdc-611">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-611">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="59cdc-612">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-612">Added example</span></span>
    - <span data-ttu-id="59cdc-613">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-613">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="59cdc-614">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-614">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="59cdc-615">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-615">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-616">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-616">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-617">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-617">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-618">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-618">Az.Resources</span></span>
* <span data-ttu-id="59cdc-619">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-619">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="59cdc-620">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-620">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="59cdc-621">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="59cdc-621">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="59cdc-622">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-622">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="59cdc-623">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cdc-623">Az.ServiceBus</span></span>
* <span data-ttu-id="59cdc-624">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="59cdc-624">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="59cdc-625">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="59cdc-625">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="59cdc-626">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-626">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-627">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-627">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-628">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-628">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="59cdc-629">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="59cdc-629">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="59cdc-630">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="59cdc-630">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="59cdc-631">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-631">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="59cdc-632">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="59cdc-632">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="59cdc-633">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-633">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-634">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-634">Az.Sql</span></span>
* <span data-ttu-id="59cdc-635">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-635">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-636">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-636">Az.Storage</span></span>
* <span data-ttu-id="59cdc-637">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-637">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="59cdc-638">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="59cdc-638">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="59cdc-639">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-639">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="59cdc-640">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="59cdc-640">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="59cdc-641">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="59cdc-641">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="59cdc-642">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="59cdc-642">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-643">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-643">Az.Websites</span></span>
* <span data-ttu-id="59cdc-644">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-644">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="59cdc-645">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-645">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-646">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-646">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-647">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-647">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="59cdc-648">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-648">Az.ApplicationInsights</span></span>
* <span data-ttu-id="59cdc-649">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-649">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="59cdc-650">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-650">Az.Automation</span></span>
* <span data-ttu-id="59cdc-651">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-651">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="59cdc-652">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-652">Az.CognitiveServices</span></span>
* <span data-ttu-id="59cdc-653">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-653">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-654">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-654">Az.Compute</span></span>
* <span data-ttu-id="59cdc-655">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-655">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="59cdc-656">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="59cdc-656">Az.ContainerRegistry</span></span>
* <span data-ttu-id="59cdc-657">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-657">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="59cdc-658">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="59cdc-658">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-659">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-659">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-660">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-660">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="59cdc-661">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-661">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="59cdc-662">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-662">Az.EventHub</span></span>
* <span data-ttu-id="59cdc-663">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="59cdc-663">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="59cdc-664">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-664">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="59cdc-665">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cdc-665">Az.KeyVault</span></span>
* <span data-ttu-id="59cdc-666">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-666">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="59cdc-667">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="59cdc-667">Az.LogicApp</span></span>
* <span data-ttu-id="59cdc-668">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-668">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="59cdc-669">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-669">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="59cdc-670">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-670">Az.ManagedServices</span></span>
* <span data-ttu-id="59cdc-671">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-671">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-672">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-672">Az.Network</span></span>
* <span data-ttu-id="59cdc-673">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-673">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="59cdc-674">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-674">New cmdlets</span></span>
        - <span data-ttu-id="59cdc-675">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="59cdc-675">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="59cdc-676">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="59cdc-676">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="59cdc-677">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-677">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-678">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-678">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-679">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-679">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-680">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-680">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="59cdc-681">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="59cdc-681">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="59cdc-682">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="59cdc-682">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="59cdc-683">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="59cdc-683">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="59cdc-684">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-684">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="59cdc-685">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-685">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="59cdc-686">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-686">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="59cdc-687">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="59cdc-687">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="59cdc-688">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-688">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="59cdc-689">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-689">Updated cmdlets</span></span>
        - <span data-ttu-id="59cdc-690">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-690">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="59cdc-691">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-691">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="59cdc-692">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-692">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="59cdc-693">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-693">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="59cdc-694">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-694">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="59cdc-695">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-695">Updated cmdlet:</span></span>
        - <span data-ttu-id="59cdc-696">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-696">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="59cdc-697">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-697">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="59cdc-698">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-698">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="59cdc-699">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-699">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="59cdc-700">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-700">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="59cdc-701">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-701">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-702">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-702">Az.OperationalInsights</span></span>
* <span data-ttu-id="59cdc-703">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-703">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="59cdc-704">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-704">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-705">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-705">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-706">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-706">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="59cdc-707">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-707">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="59cdc-708">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-708">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="59cdc-709">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-709">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="59cdc-710">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-710">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="59cdc-711">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-711">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="59cdc-712">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-712">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="59cdc-713">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-713">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="59cdc-714">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-714">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="59cdc-715">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-715">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-716">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-716">Az.Resources</span></span>
- <span data-ttu-id="59cdc-717">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-717">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="59cdc-718">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-718">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="59cdc-719">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cdc-719">Az.ServiceBus</span></span>
* <span data-ttu-id="59cdc-720">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="59cdc-720">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="59cdc-721">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-721">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-722">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-722">Az.Sql</span></span>
* <span data-ttu-id="59cdc-723">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-723">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="59cdc-724">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-724">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="59cdc-725">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-725">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-726">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-726">Az.Storage</span></span>
* <span data-ttu-id="59cdc-727">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-727">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="59cdc-728">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="59cdc-728">Az.StorageSync</span></span>
* <span data-ttu-id="59cdc-729">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-729">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="59cdc-730">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-730">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-731">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-731">Az.Websites</span></span>
* <span data-ttu-id="59cdc-732">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-732">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="59cdc-733">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-733">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="59cdc-734">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-734">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="59cdc-735">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-735">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-736">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-736">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-737">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-737">Add support for profile cmdlets</span></span>
* <span data-ttu-id="59cdc-738">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-738">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="59cdc-739">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-739">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="59cdc-740">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="59cdc-740">Az.Advisor</span></span>
* <span data-ttu-id="59cdc-741">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-741">GA release of Az.Advisor</span></span>
* <span data-ttu-id="59cdc-742">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-742">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="59cdc-743">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-743">Az.ApiManagement</span></span>
* <span data-ttu-id="59cdc-744">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="59cdc-744">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="59cdc-745">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="59cdc-745">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="59cdc-746">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-746">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="59cdc-747">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-747">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="59cdc-748">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-748">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="59cdc-749">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="59cdc-749">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="59cdc-750">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-750">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-751">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-751">Az.Automation</span></span>
* <span data-ttu-id="59cdc-752">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-752">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-753">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-753">Az.Compute</span></span>
* <span data-ttu-id="59cdc-754">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-754">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-755">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-755">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-756">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-756">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="59cdc-757">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="59cdc-757">Az.EventGrid</span></span>
* <span data-ttu-id="59cdc-758">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-758">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-759">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-759">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-760">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-760">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-761">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-761">Az.Network</span></span>
* <span data-ttu-id="59cdc-762">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-762">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="59cdc-763">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-763">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="59cdc-764">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-764">Az.PolicyInsights</span></span>
* <span data-ttu-id="59cdc-765">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-765">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="59cdc-766">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="59cdc-766">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-767">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-767">Az.OperationalInsights</span></span>
* <span data-ttu-id="59cdc-768">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-768">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-769">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-769">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-770">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-770">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-771">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-771">Az.Resources</span></span>
    - <span data-ttu-id="59cdc-772">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-772">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="59cdc-773">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-773">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="59cdc-774">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-774">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="59cdc-775">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-775">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="59cdc-776">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cdc-776">Az.ServiceBus</span></span>
* <span data-ttu-id="59cdc-777">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="59cdc-777">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-778">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-778">Az.Sql</span></span>
* <span data-ttu-id="59cdc-779">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-779">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="59cdc-780">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-780">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="59cdc-781">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="59cdc-781">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="59cdc-782">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="59cdc-782">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="59cdc-783">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="59cdc-783">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="59cdc-784">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="59cdc-784">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="59cdc-785">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="59cdc-785">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="59cdc-786">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="59cdc-786">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="59cdc-787">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-787">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-788">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-788">Az.Storage</span></span>
* <span data-ttu-id="59cdc-789">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-789">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="59cdc-790">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="59cdc-790">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="59cdc-791">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-791">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="59cdc-792">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="59cdc-792">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="59cdc-793">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-793">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="59cdc-794">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-794">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="59cdc-795">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-795">Set-AzStorageAccount</span></span>
* <span data-ttu-id="59cdc-796">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-796">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="59cdc-797">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="59cdc-797">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="59cdc-798">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="59cdc-798">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="59cdc-799">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="59cdc-799">Az.StorageSync</span></span>
* <span data-ttu-id="59cdc-800">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-800">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="59cdc-801">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-801">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-802">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-802">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-803">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-803">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="59cdc-804">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="59cdc-804">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="59cdc-805">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-805">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="59cdc-806">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="59cdc-806">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="59cdc-807">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="59cdc-807">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-808">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-808">Az.Compute</span></span>
* <span data-ttu-id="59cdc-809">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-809">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="59cdc-810">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-810">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="59cdc-811">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="59cdc-811">Az.Dns</span></span>
* <span data-ttu-id="59cdc-812">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-812">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="59cdc-813">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="59cdc-813">Az.EventGrid</span></span>
* <span data-ttu-id="59cdc-814">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-814">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="59cdc-815">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-815">New cmdlets:</span></span>
    - <span data-ttu-id="59cdc-816">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="59cdc-816">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="59cdc-817">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-817">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="59cdc-818">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="59cdc-818">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="59cdc-819">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-819">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="59cdc-820">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="59cdc-820">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="59cdc-821">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-821">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="59cdc-822">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="59cdc-822">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="59cdc-823">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-823">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="59cdc-824">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="59cdc-824">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="59cdc-825">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-825">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="59cdc-826">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="59cdc-826">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="59cdc-827">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-827">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="59cdc-828">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="59cdc-828">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="59cdc-829">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-829">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="59cdc-830">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="59cdc-830">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="59cdc-831">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-831">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="59cdc-832">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-832">Updated cmdlets:</span></span>
    - <span data-ttu-id="59cdc-833">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="59cdc-833">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="59cdc-834">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-834">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="59cdc-835">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-835">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="59cdc-836">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-836">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="59cdc-837">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="59cdc-837">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="59cdc-838">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="59cdc-838">Event subscription expiration date,</span></span>
            - <span data-ttu-id="59cdc-839">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="59cdc-839">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="59cdc-840">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-840">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="59cdc-841">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="59cdc-841">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="59cdc-842">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="59cdc-842">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="59cdc-843">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-843">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="59cdc-844">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="59cdc-844">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="59cdc-845">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-845">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="59cdc-846">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-846">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="59cdc-847">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="59cdc-847">Az.FrontDoor</span></span>
* <span data-ttu-id="59cdc-848">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="59cdc-848">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="59cdc-849">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-849">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="59cdc-850">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="59cdc-850">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="59cdc-851">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-851">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-852">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-852">Az.Network</span></span>
* <span data-ttu-id="59cdc-853">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-853">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="59cdc-854">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-854">New cmdlets</span></span>
        - <span data-ttu-id="59cdc-855">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="59cdc-855">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="59cdc-856">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-856">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="59cdc-857">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-857">New cmdlets</span></span> 
        - <span data-ttu-id="59cdc-858">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="59cdc-858">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="59cdc-859">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-859">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="59cdc-860">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-860">New cmdlets</span></span> 
        - <span data-ttu-id="59cdc-861">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="59cdc-861">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="59cdc-862">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="59cdc-862">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="59cdc-863">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="59cdc-863">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="59cdc-864">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-864">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="59cdc-865">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-865">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="59cdc-866">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-866">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="59cdc-867">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-867">New cmdlets</span></span>
        - <span data-ttu-id="59cdc-868">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="59cdc-868">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="59cdc-869">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="59cdc-869">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="59cdc-870">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="59cdc-870">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="59cdc-871">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="59cdc-871">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="59cdc-872">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="59cdc-872">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="59cdc-873">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-873">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="59cdc-874">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-874">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="59cdc-875">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-875">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="59cdc-876">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-876">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="59cdc-877">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-877">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="59cdc-878">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-878">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="59cdc-879">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-879">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="59cdc-880">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-880">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="59cdc-881">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-881">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="59cdc-882">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-882">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="59cdc-883">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-883">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="59cdc-884">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-884">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="59cdc-885">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-885">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="59cdc-886">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="59cdc-886">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="59cdc-887">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-887">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="59cdc-888">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-888">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="59cdc-889">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="59cdc-889">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="59cdc-890">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-890">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="59cdc-891">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-891">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="59cdc-892">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-892">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="59cdc-893">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-893">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="59cdc-894">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-894">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-895">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-895">Az.OperationalInsights</span></span>
* <span data-ttu-id="59cdc-896">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-896">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-897">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-897">Az.Resources</span></span>
* <span data-ttu-id="59cdc-898">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-898">Support for additional Template Export options</span></span>
    - <span data-ttu-id="59cdc-899">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-899">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="59cdc-900">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-900">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="59cdc-901">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-901">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-902">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-902">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-903">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-903">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-904">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-904">Az.Sql</span></span>
* <span data-ttu-id="59cdc-905">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-905">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="59cdc-906">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-906">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="59cdc-907">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-907">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="59cdc-908">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="59cdc-908">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="59cdc-909">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="59cdc-909">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="59cdc-910">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="59cdc-910">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="59cdc-911">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="59cdc-911">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="59cdc-912">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="59cdc-912">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-913">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-913">Az.Storage</span></span>
* <span data-ttu-id="59cdc-914">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-914">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="59cdc-915">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-915">New-AzStorageAccount</span></span>
* <span data-ttu-id="59cdc-916">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-916">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="59cdc-917">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-917">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-918">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-918">Az.Websites</span></span>
* <span data-ttu-id="59cdc-919">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-919">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="59cdc-920">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-920">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="59cdc-921">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-921">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="59cdc-922">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cdc-922">Az.Cdn</span></span>
* <span data-ttu-id="59cdc-923">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-923">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-924">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-924">Az.Compute</span></span>
* <span data-ttu-id="59cdc-925">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-925">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="59cdc-926">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="59cdc-926">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="59cdc-927">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-927">Az.EventHub</span></span>
* <span data-ttu-id="59cdc-928">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-928">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="59cdc-929">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-929">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-930">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-930">Az.Network</span></span>
* <span data-ttu-id="59cdc-931">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-931">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="59cdc-932">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-932">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="59cdc-933">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-933">Az.PolicyInsights</span></span>
* <span data-ttu-id="59cdc-934">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-934">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-935">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-935">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-936">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-936">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="59cdc-937">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cdc-937">Az.ServiceBus</span></span>
* <span data-ttu-id="59cdc-938">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-938">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-939">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-939">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-940">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-940">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="59cdc-941">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-941">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-942">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-942">Az.Sql</span></span>
* <span data-ttu-id="59cdc-943">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-943">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="59cdc-944">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="59cdc-944">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="59cdc-945">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-945">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="59cdc-946">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-946">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-947">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-947">Az.Websites</span></span>
* <span data-ttu-id="59cdc-948">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-948">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="59cdc-949">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-949">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="59cdc-950">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-950">Az.ApiManagement</span></span>
* <span data-ttu-id="59cdc-951">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-951">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="59cdc-952">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="59cdc-952">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="59cdc-953">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-953">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="59cdc-954">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-954">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="59cdc-955">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-955">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="59cdc-956">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-956">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="59cdc-957">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-957">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="59cdc-958">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-958">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="59cdc-959">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-959">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="59cdc-960">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="59cdc-960">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="59cdc-961">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-961">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="59cdc-962">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-962">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="59cdc-963">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-963">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="59cdc-964">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-964">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="59cdc-965">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="59cdc-965">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="59cdc-966">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="59cdc-966">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="59cdc-967">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="59cdc-967">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="59cdc-968">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="59cdc-968">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="59cdc-969">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-969">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="59cdc-970">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="59cdc-970">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="59cdc-971">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-971">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="59cdc-972">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-972">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="59cdc-973">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="59cdc-973">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="59cdc-974">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-974">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="59cdc-975">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-975">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="59cdc-976">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-976">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="59cdc-977">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-977">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="59cdc-978">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-978">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="59cdc-979">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-979">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="59cdc-980">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-980">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="59cdc-981">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-981">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="59cdc-982">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="59cdc-982">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="59cdc-983">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-983">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="59cdc-984">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-984">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="59cdc-985">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="59cdc-985">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="59cdc-986">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="59cdc-986">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="59cdc-987">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="59cdc-987">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="59cdc-988">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-988">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="59cdc-989">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-989">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="59cdc-990">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-990">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="59cdc-991">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="59cdc-991">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="59cdc-992">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="59cdc-992">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="59cdc-993">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="59cdc-993">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="59cdc-994">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-994">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="59cdc-995">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-995">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="59cdc-996">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="59cdc-996">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="59cdc-997">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="59cdc-997">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="59cdc-998">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-998">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="59cdc-999">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-999">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="59cdc-1000">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1000">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="59cdc-1001">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1001">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="59cdc-1002">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1002">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="59cdc-1003">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1003">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="59cdc-1004">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1004">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="59cdc-1005">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1005">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="59cdc-1006">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1006">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="59cdc-1007">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1007">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="59cdc-1008">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1008">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="59cdc-1009">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1009">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="59cdc-1010">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1010">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="59cdc-1011">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1011">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="59cdc-1012">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1012">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="59cdc-1013">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="59cdc-1013">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="59cdc-1014">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1014">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="59cdc-1015">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1015">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="59cdc-1016">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1016">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="59cdc-1017">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="59cdc-1017">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="59cdc-1018">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1018">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="59cdc-1019">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="59cdc-1019">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="59cdc-1020">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1020">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="59cdc-1021">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="59cdc-1021">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="59cdc-1022">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1022">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="59cdc-1023">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1023">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="59cdc-1024">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-1024">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="59cdc-1025">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1025">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="59cdc-1026">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1026">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="59cdc-1027">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="59cdc-1027">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-1028">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1028">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1029">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1029">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="59cdc-1030">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="59cdc-1030">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="59cdc-1031">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="59cdc-1031">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="59cdc-1032">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1032">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="59cdc-1033">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="59cdc-1033">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="59cdc-1034">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1034">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="59cdc-1035">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1035">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1036">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1036">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1037">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1037">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="59cdc-1038">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1038">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1039">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1039">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1040">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1040">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-1041">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1041">Az.Monitor</span></span>
* <span data-ttu-id="59cdc-1042">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1042">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1043">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1043">Az.Network</span></span>
* <span data-ttu-id="59cdc-1044">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1044">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="59cdc-1045">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="59cdc-1045">Updated cmdlet:</span></span>
        - <span data-ttu-id="59cdc-1046">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-1046">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="59cdc-1047">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1047">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1048">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1048">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1049">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1049">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1050">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1050">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1051">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1051">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="59cdc-1052">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1052">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1053">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1053">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1054">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1054">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="59cdc-1055">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1055">Az.CognitiveServices</span></span>
* <span data-ttu-id="59cdc-1056">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1056">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="59cdc-1057">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1057">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1058">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1058">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1059">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1059">Proximity placement group feature.</span></span>
    - <span data-ttu-id="59cdc-1060">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="59cdc-1060">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="59cdc-1061">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-1061">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="59cdc-1062">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1062">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="59cdc-1063">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1063">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="59cdc-1064">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1064">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="59cdc-1065">重大な変更</span><span class="sxs-lookup"><span data-stu-id="59cdc-1065">Breaking changes</span></span>
    - <span data-ttu-id="59cdc-1066">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1066">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="59cdc-1067">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1067">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="59cdc-1068">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="59cdc-1068">Az.DeploymentManager</span></span>
* <span data-ttu-id="59cdc-1069">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-1069">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="59cdc-1070">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="59cdc-1070">Az.Dns</span></span>
* <span data-ttu-id="59cdc-1071">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="59cdc-1071">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="59cdc-1072">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1072">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="59cdc-1073">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1073">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="59cdc-1074">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1074">Az.FrontDoor</span></span>
* <span data-ttu-id="59cdc-1075">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-1075">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="59cdc-1076">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1076">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="59cdc-1077">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="59cdc-1077">Az.HDInsight</span></span>
* <span data-ttu-id="59cdc-1078">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1078">Removed two cmdlets:</span></span>
    - <span data-ttu-id="59cdc-1079">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="59cdc-1079">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="59cdc-1080">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="59cdc-1080">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="59cdc-1081">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1081">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="59cdc-1082">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1082">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="59cdc-1083">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1083">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="59cdc-1084">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1084">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-1085">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1085">Az.Monitor</span></span>
* <span data-ttu-id="59cdc-1086">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="59cdc-1086">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="59cdc-1087">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="59cdc-1087">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="59cdc-1088">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="59cdc-1088">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="59cdc-1089">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="59cdc-1089">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="59cdc-1090">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1090">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="59cdc-1091">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="59cdc-1091">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="59cdc-1092">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="59cdc-1092">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="59cdc-1093">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1093">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="59cdc-1094">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1094">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="59cdc-1095">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1095">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="59cdc-1096">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1096">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="59cdc-1097">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1097">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="59cdc-1098">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="59cdc-1098">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="59cdc-1099">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1099">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1100">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1100">Az.Network</span></span>
* <span data-ttu-id="59cdc-1101">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1101">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="59cdc-1102">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1102">New cmdlets</span></span>
        - <span data-ttu-id="59cdc-1103">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="59cdc-1103">New-AzNatGateway</span></span>
        - <span data-ttu-id="59cdc-1104">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="59cdc-1104">Get-AzNatGateway</span></span>
        - <span data-ttu-id="59cdc-1105">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="59cdc-1105">Set-AzNatGateway</span></span>
        - <span data-ttu-id="59cdc-1106">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="59cdc-1106">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="59cdc-1107">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1107">Updated cmdlets</span></span>
        - <span data-ttu-id="59cdc-1108">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="59cdc-1108">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="59cdc-1109">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="59cdc-1109">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="59cdc-1110">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1110">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="59cdc-1111">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1111">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="59cdc-1112">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1112">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="59cdc-1113">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-1113">Az.PolicyInsights</span></span>
* <span data-ttu-id="59cdc-1114">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1114">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="59cdc-1115">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1115">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="59cdc-1116">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1116">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1117">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1117">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-1118">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1118">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="59cdc-1119">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1119">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="59cdc-1120">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1120">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="59cdc-1121">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1121">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="59cdc-1122">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1122">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="59cdc-1123">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1123">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="59cdc-1124">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="59cdc-1124">Az.Relay</span></span>
* <span data-ttu-id="59cdc-1125">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1125">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="59cdc-1126">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cdc-1126">Az.ServiceBus</span></span>
* <span data-ttu-id="59cdc-1127">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1127">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-1128">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1128">Az.Storage</span></span>
* <span data-ttu-id="59cdc-1129">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="59cdc-1129">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="59cdc-1130">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1130">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="59cdc-1131">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1131">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="59cdc-1132">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-1132">New-AzStorageAccount</span></span>
* <span data-ttu-id="59cdc-1133">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="59cdc-1133">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="59cdc-1134">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-1134">New-AzStorageAccount</span></span>
    - <span data-ttu-id="59cdc-1135">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-1135">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="59cdc-1136">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="59cdc-1136">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1137">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1137">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1138">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="59cdc-1138">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="59cdc-1139">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1139">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="59cdc-1140">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1140">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="59cdc-1141">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="59cdc-1141">Highlights since the last major release</span></span>
* <span data-ttu-id="59cdc-1142">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="59cdc-1142">General availability of `Az` module</span></span>
* <span data-ttu-id="59cdc-1143">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="59cdc-1143">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="59cdc-1144">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="59cdc-1144">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="59cdc-1145">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1145">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="59cdc-1146">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1146">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="59cdc-1147">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1147">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="59cdc-1148">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1148">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1149">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1150">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1150">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="59cdc-1151">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="59cdc-1151">Az.Batch</span></span>
* <span data-ttu-id="59cdc-1152">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1152">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="59cdc-1153">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cdc-1153">Az.Cdn</span></span>
* <span data-ttu-id="59cdc-1154">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1154">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="59cdc-1155">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1155">Az.CognitiveServices</span></span>
* <span data-ttu-id="59cdc-1156">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1156">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1157">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1157">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1158">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1158">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="59cdc-1159">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1159">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="59cdc-1160">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1160">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-1161">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-1161">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-1162">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1162">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1163">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1163">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1164">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1164">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="59cdc-1165">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="59cdc-1165">Az.EventGrid</span></span>
* <span data-ttu-id="59cdc-1166">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1166">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="59cdc-1167">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-1167">Az.EventHub</span></span>
* <span data-ttu-id="59cdc-1168">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1168">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="59cdc-1169">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="59cdc-1169">Az.HDInsight</span></span>
* <span data-ttu-id="59cdc-1170">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1170">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-1171">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-1171">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-1172">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1172">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="59cdc-1173">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cdc-1173">Az.KeyVault</span></span>
* <span data-ttu-id="59cdc-1174">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1174">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="59cdc-1175">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1175">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="59cdc-1176">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="59cdc-1176">Az.MachineLearning</span></span>
* <span data-ttu-id="59cdc-1177">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1177">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="59cdc-1178">Az.Media</span><span class="sxs-lookup"><span data-stu-id="59cdc-1178">Az.Media</span></span>
* <span data-ttu-id="59cdc-1179">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1179">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-1180">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1180">Az.Monitor</span></span>
  * <span data-ttu-id="59cdc-1181">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1181">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="59cdc-1182">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="59cdc-1182">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="59cdc-1183">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="59cdc-1183">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="59cdc-1184">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="59cdc-1184">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="59cdc-1185">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="59cdc-1185">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="59cdc-1186">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="59cdc-1186">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="59cdc-1187">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1187">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1188">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1188">Az.Network</span></span>
* <span data-ttu-id="59cdc-1189">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1189">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="59cdc-1190">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1190">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="59cdc-1191">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="59cdc-1191">Az.NotificationHubs</span></span>
* <span data-ttu-id="59cdc-1192">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1192">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-1193">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-1193">Az.OperationalInsights</span></span>
* <span data-ttu-id="59cdc-1194">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1194">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="59cdc-1195">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="59cdc-1195">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="59cdc-1196">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1196">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1197">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1197">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-1198">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1198">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="59cdc-1199">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1199">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="59cdc-1200">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1200">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="59cdc-1201">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1201">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="59cdc-1202">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="59cdc-1202">Az.RedisCache</span></span>
* <span data-ttu-id="59cdc-1203">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1204">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1204">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1205">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1205">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1206">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1206">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1207">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="59cdc-1207">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="59cdc-1208">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="59cdc-1209">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1209">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="59cdc-1210">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1210">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="59cdc-1211">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1211">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="59cdc-1212">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1212">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="59cdc-1213">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1213">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1214">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1214">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1215">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1215">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="59cdc-1216">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1216">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="59cdc-1217">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1217">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="59cdc-1218">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1218">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="59cdc-1219">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1219">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="59cdc-1220">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="59cdc-1220">Highlights since the last major release</span></span>
* <span data-ttu-id="59cdc-1221">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="59cdc-1221">General availability of `Az` module</span></span>
* <span data-ttu-id="59cdc-1222">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="59cdc-1222">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="59cdc-1223">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="59cdc-1223">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="59cdc-1224">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1224">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="59cdc-1225">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1225">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="59cdc-1226">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1226">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="59cdc-1227">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1227">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1228">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1228">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1229">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1229">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="59cdc-1230">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1230">Az.AnalysisServices</span></span>
* <span data-ttu-id="59cdc-1231">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="59cdc-1231">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="59cdc-1232">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1232">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-1233">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1233">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1234">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1234">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="59cdc-1235">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1235">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="59cdc-1236">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1236">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1237">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1237">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1238">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1238">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="59cdc-1239">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1239">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="59cdc-1240">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1240">Az.ContainerInstance</span></span>
* <span data-ttu-id="59cdc-1241">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1241">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-1242">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-1242">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-1243">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1243">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="59cdc-1244">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1244">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1245">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1245">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1246">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1246">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="59cdc-1247">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1247">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="59cdc-1248">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1248">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="59cdc-1249">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="59cdc-1249">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="59cdc-1250">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1250">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="59cdc-1251">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="59cdc-1251">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1252">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1252">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1253">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1253">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-1254">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1254">Az.Storage</span></span>
* <span data-ttu-id="59cdc-1255">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="59cdc-1255">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="59cdc-1256">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="59cdc-1256">New-AzStorageContext</span></span>
* <span data-ttu-id="59cdc-1257">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1257">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="59cdc-1258">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="59cdc-1258">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="59cdc-1259">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="59cdc-1259">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="59cdc-1260">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1260">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="59cdc-1261">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1261">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="59cdc-1262">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1262">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="59cdc-1263">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-1263">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="59cdc-1264">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-1264">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="59cdc-1265">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-1265">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="59cdc-1266">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="59cdc-1266">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="59cdc-1267">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1267">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="59cdc-1268">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="59cdc-1268">Highlights since the last major release</span></span>
* <span data-ttu-id="59cdc-1269">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="59cdc-1269">General availability of `Az` module</span></span>
* <span data-ttu-id="59cdc-1270">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="59cdc-1270">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="59cdc-1271">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="59cdc-1271">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="59cdc-1272">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1272">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="59cdc-1273">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1273">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="59cdc-1274">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1274">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="59cdc-1275">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1275">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-1276">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1276">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1277">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1277">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="59cdc-1278">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="59cdc-1278">Dynamic grouping</span></span>
    * <span data-ttu-id="59cdc-1279">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="59cdc-1279">Pre-Post script</span></span>
    * <span data-ttu-id="59cdc-1280">再起動設定</span><span class="sxs-lookup"><span data-stu-id="59cdc-1280">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1281">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1282">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1282">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="59cdc-1283">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1283">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="59cdc-1284">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cdc-1284">Az.KeyVault</span></span>
* <span data-ttu-id="59cdc-1285">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1285">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1286">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1286">Az.Network</span></span>
* <span data-ttu-id="59cdc-1287">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1287">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="59cdc-1288">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1288">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1289">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1289">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-1290">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1290">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="59cdc-1291">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1291">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1292">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1292">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1293">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1293">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="59cdc-1294">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1294">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1295">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1295">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1296">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1296">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-1297">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1297">Az.Storage</span></span>
* <span data-ttu-id="59cdc-1298">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-1298">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="59cdc-1299">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1299">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="59cdc-1300">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1300">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="59cdc-1301">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1301">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="59cdc-1302">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="59cdc-1302">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="59cdc-1303">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="59cdc-1303">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="59cdc-1304">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1304">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1305">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1305">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1306">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1306">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="59cdc-1307">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1307">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1308">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1308">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1309">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1309">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="59cdc-1310">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1310">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-1311">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1311">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1312">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1312">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="59cdc-1313">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1313">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="59cdc-1314">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1314">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="59cdc-1315">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cdc-1315">Az.Cdn</span></span>
* <span data-ttu-id="59cdc-1316">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1316">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1317">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1317">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1318">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1318">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-1319">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-1319">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-1320">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1320">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="59cdc-1321">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="59cdc-1321">Az.LogicApp</span></span>
* <span data-ttu-id="59cdc-1322">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1322">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1323">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1323">Az.Network</span></span>
* <span data-ttu-id="59cdc-1324">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1324">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1325">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1325">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-1326">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1326">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="59cdc-1327">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1327">SDK Update</span></span>
* <span data-ttu-id="59cdc-1328">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1328">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="59cdc-1329">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1329">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1330">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1330">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1331">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1331">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="59cdc-1332">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="59cdc-1332">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="59cdc-1333">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1333">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="59cdc-1334">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="59cdc-1334">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="59cdc-1335">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1335">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="59cdc-1336">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="59cdc-1336">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1337">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1337">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1338">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1338">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="59cdc-1339">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1339">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-1340">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1340">Az.Storage</span></span>
* <span data-ttu-id="59cdc-1341">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1341">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="59cdc-1342">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1342">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="59cdc-1343">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1343">Az.AnalysisServices</span></span>
* <span data-ttu-id="59cdc-1344">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1344">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-1345">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1345">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1346">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1346">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="59cdc-1347">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1347">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="59cdc-1348">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1348">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="59cdc-1349">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1349">Az.CognitiveServices</span></span>
* <span data-ttu-id="59cdc-1350">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1350">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1351">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1351">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1352">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1352">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="59cdc-1353">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1353">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="59cdc-1354">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1354">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="59cdc-1355">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1355">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1356">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1356">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1357">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1357">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="59cdc-1358">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-1358">Az.EventHub</span></span>
* <span data-ttu-id="59cdc-1359">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1359">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="59cdc-1360">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cdc-1360">Az.KeyVault</span></span>
* <span data-ttu-id="59cdc-1361">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1361">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="59cdc-1362">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="59cdc-1362">Az.LogicApp</span></span>
* <span data-ttu-id="59cdc-1363">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1363">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="59cdc-1364">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1364">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="59cdc-1365">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1365">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="59cdc-1366">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="59cdc-1366">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="59cdc-1367">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="59cdc-1367">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="59cdc-1368">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="59cdc-1368">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="59cdc-1369">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="59cdc-1369">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="59cdc-1370">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1370">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="59cdc-1371">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cdc-1371">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="59cdc-1372">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cdc-1372">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="59cdc-1373">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cdc-1373">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="59cdc-1374">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cdc-1374">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="59cdc-1375">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1375">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="59cdc-1376">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1376">Az.Monitor</span></span>
* <span data-ttu-id="59cdc-1377">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1377">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1378">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1378">Az.Network</span></span>
* <span data-ttu-id="59cdc-1379">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1379">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-1380">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-1380">Az.OperationalInsights</span></span>
* <span data-ttu-id="59cdc-1381">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1381">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="59cdc-1382">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1382">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="59cdc-1383">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1383">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="59cdc-1384">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1384">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1385">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="59cdc-1385">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="59cdc-1386">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="59cdc-1386">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="59cdc-1387">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="59cdc-1387">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="59cdc-1388">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1388">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1389">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1389">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1390">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1390">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="59cdc-1391">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1391">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1392">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1392">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1393">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1393">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="59cdc-1394">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1394">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1395">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1395">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1396">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1396">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="59cdc-1397">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1397">Az.AnalysisServices</span></span>
<span data-ttu-id="59cdc-1398">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="59cdc-1398">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1399">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1399">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1400">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1400">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="59cdc-1401">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1401">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="59cdc-1402">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1402">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1403">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1403">Az.RecoveryServices</span></span>
<span data-ttu-id="59cdc-1404">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="59cdc-1404">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1405">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1405">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1406">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1406">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="59cdc-1407">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="59cdc-1407">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="59cdc-1408">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1408">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="59cdc-1409">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="59cdc-1409">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1410">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1410">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1411">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1411">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="59cdc-1412">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1412">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="59cdc-1413">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1413">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="59cdc-1414">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1414">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1415">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1415">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1416">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-1416">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="59cdc-1417">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1417">Az.AnalysisServices</span></span>
* <span data-ttu-id="59cdc-1418">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-1418">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1419">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1419">Az.RecoveryServices</span></span>
* <span data-ttu-id="59cdc-1420">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-1420">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="59cdc-1421">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1421">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1422">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1422">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1423">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1423">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="59cdc-1424">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1424">Update incorrect online help URLs</span></span>
* <span data-ttu-id="59cdc-1425">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1425">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="59cdc-1426">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="59cdc-1426">Az.Aks</span></span>
* <span data-ttu-id="59cdc-1427">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1427">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="59cdc-1428">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1428">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1429">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1429">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="59cdc-1430">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1430">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="59cdc-1431">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="59cdc-1431">Az.Cdn</span></span>
* <span data-ttu-id="59cdc-1432">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1432">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1433">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1433">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1434">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1434">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="59cdc-1435">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1435">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="59cdc-1436">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1436">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="59cdc-1437">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="59cdc-1437">Az.ContainerRegistry</span></span>
* <span data-ttu-id="59cdc-1438">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1438">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="59cdc-1439">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="59cdc-1439">Az.DataFactory</span></span>
* <span data-ttu-id="59cdc-1440">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1440">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1441">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1441">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1442">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="59cdc-1442">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="59cdc-1443">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="59cdc-1443">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="59cdc-1444">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1444">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-1445">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-1445">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-1446">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1446">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="59cdc-1447">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cdc-1447">Az.KeyVault</span></span>
* <span data-ttu-id="59cdc-1448">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1448">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1449">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1449">Az.Network</span></span>
* <span data-ttu-id="59cdc-1450">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1450">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1451">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1451">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1452">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1452">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="59cdc-1453">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1453">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="59cdc-1454">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1454">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="59cdc-1455">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="59cdc-1455">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="59cdc-1456">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="59cdc-1456">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="59cdc-1457">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1457">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="59cdc-1458">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="59cdc-1458">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-1459">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-1459">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-1460">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="59cdc-1460">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="59cdc-1461">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1461">Fix some error messages.</span></span>
* <span data-ttu-id="59cdc-1462">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1462">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="59cdc-1463">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1463">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="59cdc-1464">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="59cdc-1464">Az.SignalR</span></span>
* <span data-ttu-id="59cdc-1465">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1465">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1466">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1466">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1467">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1467">Update incorrect online help URLs</span></span>
* <span data-ttu-id="59cdc-1468">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1468">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="59cdc-1469">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1469">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="59cdc-1470">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-1470">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-1471">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1471">Az.Storage</span></span>
* <span data-ttu-id="59cdc-1472">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1472">Update incorrect online help URLs</span></span>
* <span data-ttu-id="59cdc-1473">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="59cdc-1473">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="59cdc-1474">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="59cdc-1474">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="59cdc-1475">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="59cdc-1475">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="59cdc-1476">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="59cdc-1476">Az.TrafficManager</span></span>
* <span data-ttu-id="59cdc-1477">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1477">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1478">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1478">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1479">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1479">Update incorrect online help URLs</span></span>
* <span data-ttu-id="59cdc-1480">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1480">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="59cdc-1481">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="59cdc-1481">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="59cdc-1482">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1482">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="59cdc-1483">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1483">Az.Accounts</span></span>
* <span data-ttu-id="59cdc-1484">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="59cdc-1484">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1485">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1485">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1486">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1486">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="59cdc-1487">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1487">Updated the description of ID in help files</span></span>
* <span data-ttu-id="59cdc-1488">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1488">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1489">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1489">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1490">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1490">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="59cdc-1491">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1491">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="59cdc-1492">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="59cdc-1492">Az.EventGrid</span></span>
* <span data-ttu-id="59cdc-1493">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1493">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="59cdc-1494">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="59cdc-1494">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="59cdc-1495">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="59cdc-1495">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="59cdc-1496">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="59cdc-1496">Event Time-To-Live,</span></span>
        - <span data-ttu-id="59cdc-1497">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="59cdc-1497">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="59cdc-1498">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="59cdc-1498">Dead letter endpoint.</span></span>
    - <span data-ttu-id="59cdc-1499">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="59cdc-1499">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="59cdc-1500">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="59cdc-1500">Event Time-To-Live,</span></span>
        - <span data-ttu-id="59cdc-1501">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="59cdc-1501">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="59cdc-1502">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="59cdc-1502">Dead letter endpoint.</span></span>
* <span data-ttu-id="59cdc-1503">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1503">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="59cdc-1504">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1504">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="59cdc-1505">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="59cdc-1505">Az.IotHub</span></span>
* <span data-ttu-id="59cdc-1506">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1506">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="59cdc-1507">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="59cdc-1507">Az.LogicApp</span></span>
* <span data-ttu-id="59cdc-1508">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="59cdc-1508">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1509">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1509">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1510">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1510">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="59cdc-1511">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="59cdc-1511">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="59cdc-1512">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1512">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="59cdc-1513">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1513">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="59cdc-1514">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1514">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="59cdc-1515">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="59cdc-1515">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="59cdc-1516">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="59cdc-1516">Az.SignalR</span></span>
* <span data-ttu-id="59cdc-1517">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1517">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1518">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1518">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1519">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1519">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="59cdc-1520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1520">Az.Storage</span></span>
* <span data-ttu-id="59cdc-1521">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="59cdc-1521">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="59cdc-1522">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="59cdc-1522">New-AzStorageContext</span></span>
* <span data-ttu-id="59cdc-1523">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1523">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="59cdc-1524">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="59cdc-1524">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1525">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1525">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1526">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1526">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="59cdc-1527">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1527">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="59cdc-1528">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1528">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="59cdc-1529">全般</span><span class="sxs-lookup"><span data-stu-id="59cdc-1529">General</span></span>

- <span data-ttu-id="59cdc-1530">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="59cdc-1530">General Availability of Az Module</span></span>
- <span data-ttu-id="59cdc-1531">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="59cdc-1531">Online help for each module</span></span>
- <span data-ttu-id="59cdc-1532">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1532">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="59cdc-1533">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1533">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="59cdc-1534">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="59cdc-1534">Az.Accounts</span></span>
- <span data-ttu-id="59cdc-1535">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1535">Changed from Az.Profile</span></span>
- <span data-ttu-id="59cdc-1536">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1536">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="59cdc-1537">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-1537">Az.ApiManagement</span></span>
- <span data-ttu-id="59cdc-1538">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="59cdc-1538">Fixes for #7002</span></span>
- <span data-ttu-id="59cdc-1539">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1539">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="59cdc-1540">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="59cdc-1540">Az.Batch</span></span>
- <span data-ttu-id="59cdc-1541">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1541">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="59cdc-1542">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1542">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="59cdc-1543">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1543">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="59cdc-1544">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="59cdc-1544">Az.Billing</span></span>
- <span data-ttu-id="59cdc-1545">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1545">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="59cdc-1546">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1546">Az.CognitivServices</span></span>
- <span data-ttu-id="59cdc-1547">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1547">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="59cdc-1548">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1548">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="59cdc-1549">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1549">Az.ContainerInstance</span></span>
- <span data-ttu-id="59cdc-1550">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1550">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="59cdc-1551">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="59cdc-1551">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="59cdc-1552">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1552">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1553">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1553">Az.DataLakeStore</span></span>
- <span data-ttu-id="59cdc-1554">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1554">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="59cdc-1555">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1555">Az.Monitor</span></span>
- <span data-ttu-id="59cdc-1556">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1556">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="59cdc-1557">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="59cdc-1557">Az.KeyVault</span></span>
- <span data-ttu-id="59cdc-1558">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1558">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="59cdc-1559">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="59cdc-1559">Az.MachineLearning</span></span>
- <span data-ttu-id="59cdc-1560">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1560">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="59cdc-1561">Az.Media</span><span class="sxs-lookup"><span data-stu-id="59cdc-1561">Az.Media</span></span>
- <span data-ttu-id="59cdc-1562">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1562">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="59cdc-1563">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1563">Az.Network</span></span>
<span data-ttu-id="59cdc-1564">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1564">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="59cdc-1565">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-1565">New cmdlets added:</span></span>
        - <span data-ttu-id="59cdc-1566">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-1566">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="59cdc-1567">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-1567">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="59cdc-1568">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-1568">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="59cdc-1569">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-1569">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="59cdc-1570">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-1570">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="59cdc-1571">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1571">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="59cdc-1572">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="59cdc-1572">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="59cdc-1573">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="59cdc-1573">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="59cdc-1574">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1574">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="59cdc-1575">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="59cdc-1575">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="59cdc-1576">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1576">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="59cdc-1577">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="59cdc-1577">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="59cdc-1578">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-1578">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="59cdc-1579">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-1579">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="59cdc-1580">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1580">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="59cdc-1581">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1581">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="59cdc-1582">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="59cdc-1582">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="59cdc-1583">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="59cdc-1583">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="59cdc-1584">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="59cdc-1584">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="59cdc-1585">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1585">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="59cdc-1586">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1586">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="59cdc-1587">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-1587">Az.OperationalInsights</span></span>
- <span data-ttu-id="59cdc-1588">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1588">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="59cdc-1589">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1589">Az.Profile</span></span>
- <span data-ttu-id="59cdc-1590">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1590">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1591">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1591">Az.RecoveryServices</span></span>
- <span data-ttu-id="59cdc-1592">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1592">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="59cdc-1593">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1593">Az.Resources</span></span>
- <span data-ttu-id="59cdc-1594">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1594">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="59cdc-1595">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-1595">Az.ServiceFabric</span></span>
- <span data-ttu-id="59cdc-1596">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="59cdc-1596">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="59cdc-1597">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1597">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="59cdc-1598">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="59cdc-1598">Az.SIgnalR</span></span>
- <span data-ttu-id="59cdc-1599">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="59cdc-1599">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="59cdc-1600">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1600">Az.Sql</span></span>
- <span data-ttu-id="59cdc-1601">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1601">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="59cdc-1602">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1602">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="59cdc-1603">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="59cdc-1604">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1604">Az.Storage</span></span>
- <span data-ttu-id="59cdc-1605">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1605">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="59cdc-1606">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1606">Az.Websites</span></span>
- <span data-ttu-id="59cdc-1607">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="59cdc-1607">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="59cdc-1608">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1608">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="59cdc-1609">全般</span><span class="sxs-lookup"><span data-stu-id="59cdc-1609">General</span></span>

* <span data-ttu-id="59cdc-1610">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="59cdc-1610">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="59cdc-1611">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1611">Az.Compute</span></span>

* <span data-ttu-id="59cdc-1612">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1612">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1613">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1613">Az.DataLakeStore</span></span>

* <span data-ttu-id="59cdc-1614">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1614">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="59cdc-1615">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="59cdc-1615">Az.FrontDoor</span></span>

* <span data-ttu-id="59cdc-1616">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1616">Fixed some broken links</span></span>
    - <span data-ttu-id="59cdc-1617">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1617">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="59cdc-1618">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1618">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="59cdc-1619">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1619">Az.RecoveryServices</span></span>

* <span data-ttu-id="59cdc-1620">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1620">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="59cdc-1621">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1621">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="59cdc-1622">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1622">Az.Resources</span></span>

* <span data-ttu-id="59cdc-1623">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1623">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="59cdc-1624">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1624">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="59cdc-1625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1625">Az.Sql</span></span>

* <span data-ttu-id="59cdc-1626">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="59cdc-1626">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="59cdc-1627">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1627">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="59cdc-1628">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1628">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="59cdc-1629">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1629">Az.Storage</span></span>

* <span data-ttu-id="59cdc-1630">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1630">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="59cdc-1631">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1631">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="59cdc-1632">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1632">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="59cdc-1633">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="59cdc-1633">Support Static Website configuration</span></span>
    - <span data-ttu-id="59cdc-1634">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="59cdc-1634">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="59cdc-1635">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="59cdc-1635">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="59cdc-1636">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1636">Az.Websites</span></span>

* <span data-ttu-id="59cdc-1637">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="59cdc-1637">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="59cdc-1638">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1638">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="59cdc-1639">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="59cdc-1639">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="59cdc-1640">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1640">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="59cdc-1641">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="59cdc-1641">Az.ApiManagement</span></span>
* <span data-ttu-id="59cdc-1642">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1642">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="59cdc-1643">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="59cdc-1643">Az.Automation</span></span>
* <span data-ttu-id="59cdc-1644">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="59cdc-1644">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="59cdc-1645">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1645">Added Update Management cmdlets</span></span>
* <span data-ttu-id="59cdc-1646">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1646">Added Source Control cmdlets</span></span>
* <span data-ttu-id="59cdc-1647">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1647">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="59cdc-1648">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1648">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="59cdc-1649">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1649">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1650">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1650">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="59cdc-1651">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1651">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="59cdc-1652">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1652">Az.ContainerInstance</span></span>
* <span data-ttu-id="59cdc-1653">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1653">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="59cdc-1654">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="59cdc-1654">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="59cdc-1655">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1655">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="59cdc-1656">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1656">Az.Network</span></span>
* <span data-ttu-id="59cdc-1657">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1657">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="59cdc-1658">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1658">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="59cdc-1659">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1659">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="59cdc-1660">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1660">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="59cdc-1661">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="59cdc-1661">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="59cdc-1662">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1662">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="59cdc-1663">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1663">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="59cdc-1664">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="59cdc-1664">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="59cdc-1665">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1665">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="59cdc-1666">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1666">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="59cdc-1667">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="59cdc-1667">Az.Relay</span></span>
* <span data-ttu-id="59cdc-1668">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="59cdc-1668">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="59cdc-1669">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1669">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1670">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1670">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="59cdc-1671">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1671">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="59cdc-1672">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="59cdc-1672">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="59cdc-1673">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-1673">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-1674">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1674">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="59cdc-1675">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1675">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1676">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1676">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="59cdc-1677">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1677">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="59cdc-1678">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1678">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="59cdc-1679">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1679">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="59cdc-1680">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="59cdc-1680">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="59cdc-1681">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="59cdc-1681">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="59cdc-1682">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="59cdc-1682">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="59cdc-1683">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="59cdc-1683">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="59cdc-1684">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="59cdc-1684">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="59cdc-1685">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1685">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="59cdc-1686">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1686">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="59cdc-1687">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1687">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="59cdc-1688">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="59cdc-1688">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="59cdc-1689">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="59cdc-1689">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="59cdc-1690">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="59cdc-1690">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="59cdc-1691">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="59cdc-1691">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="59cdc-1692">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1692">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="59cdc-1693">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1693">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="59cdc-1694">全般</span><span class="sxs-lookup"><span data-stu-id="59cdc-1694">General</span></span>
* <span data-ttu-id="59cdc-1695">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="59cdc-1695">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="59cdc-1696">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1696">Az.Profile</span></span>
* <span data-ttu-id="59cdc-1697">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1697">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="59cdc-1698">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1698">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="59cdc-1699">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1699">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="59cdc-1700">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1700">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="59cdc-1701">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1701">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="59cdc-1702">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1702">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="59cdc-1703">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1703">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="59cdc-1704">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1704">Az.CognitiveServices</span></span>
* <span data-ttu-id="59cdc-1705">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1705">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1706">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1706">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1707">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1707">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="59cdc-1708">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="59cdc-1708">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="59cdc-1709">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1709">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1710">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1710">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1711">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1711">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="59cdc-1712">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1712">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="59cdc-1713">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="59cdc-1713">Az.Insights</span></span>
* <span data-ttu-id="59cdc-1714">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1714">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="59cdc-1715">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1715">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="59cdc-1716">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1716">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="59cdc-1717">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="59cdc-1717">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1718">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1718">Az.Network</span></span>
* <span data-ttu-id="59cdc-1719">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="59cdc-1719">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="59cdc-1720">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-1720">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="59cdc-1721">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-1721">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="59cdc-1722">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="59cdc-1722">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="59cdc-1723">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-1723">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="59cdc-1724">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="59cdc-1724">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="59cdc-1725">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="59cdc-1725">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="59cdc-1726">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="59cdc-1726">Az.PolicyInsights</span></span>
* <span data-ttu-id="59cdc-1727">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1727">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1728">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1728">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1729">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1729">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="59cdc-1730">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1730">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="59cdc-1731">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="59cdc-1731">Az.ServiceBus</span></span>
* <span data-ttu-id="59cdc-1732">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1732">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="59cdc-1733">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="59cdc-1733">Az.ServiceFabric</span></span>
* <span data-ttu-id="59cdc-1734">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1734">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="59cdc-1735">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1735">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="59cdc-1736">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1736">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="59cdc-1737">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1737">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="59cdc-1738">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1738">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="59cdc-1739">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1739">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="59cdc-1740">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1740">Az.Profile</span></span>
* <span data-ttu-id="59cdc-1741">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1741">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="59cdc-1742">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1742">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1743">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1743">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1744">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1744">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="59cdc-1745">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1745">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="59cdc-1746">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="59cdc-1746">Az.DataLakeStore</span></span>
* <span data-ttu-id="59cdc-1747">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1747">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="59cdc-1748">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1748">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="59cdc-1749">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1749">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="59cdc-1750">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1750">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="59cdc-1751">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1751">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1752">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1752">Az.Network</span></span>
* <span data-ttu-id="59cdc-1753">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1753">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="59cdc-1754">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1754">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1755">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1755">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1756">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1756">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="59cdc-1757">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1757">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="59cdc-1758">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1758">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="59cdc-1759">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1759">Azure.Storage</span></span>
* <span data-ttu-id="59cdc-1760">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1760">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="59cdc-1761">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1761">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="59cdc-1762">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="59cdc-1762">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="59cdc-1763">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1763">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="59cdc-1764">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="59cdc-1764">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="59cdc-1765">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="59cdc-1765">Az.CognitiveServices</span></span>
* <span data-ttu-id="59cdc-1766">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1766">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="59cdc-1767">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="59cdc-1767">Az.Compute</span></span>
* <span data-ttu-id="59cdc-1768">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1768">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="59cdc-1769">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1769">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="59cdc-1770">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1770">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="59cdc-1771">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="59cdc-1771">Az.DataFactoryV2</span></span>
* <span data-ttu-id="59cdc-1772">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1772">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="59cdc-1773">Az.Network</span><span class="sxs-lookup"><span data-stu-id="59cdc-1773">Az.Network</span></span>
* <span data-ttu-id="59cdc-1774">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1774">Added NetworkProfile functionality.</span></span> <span data-ttu-id="59cdc-1775">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="59cdc-1775">new cmdlets added</span></span>
    - <span data-ttu-id="59cdc-1776">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1776">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="59cdc-1777">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1777">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="59cdc-1778">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1778">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="59cdc-1779">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="59cdc-1779">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="59cdc-1780">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-1780">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="59cdc-1781">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="59cdc-1781">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="59cdc-1782">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1782">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="59cdc-1783">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1783">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="59cdc-1784">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1784">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="59cdc-1785">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="59cdc-1785">Az.RedisCache</span></span>
* <span data-ttu-id="59cdc-1786">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="59cdc-1786">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="59cdc-1787">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1787">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="59cdc-1788">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="59cdc-1788">Az.Resources</span></span>
* <span data-ttu-id="59cdc-1789">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1789">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="59cdc-1790">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1790">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="59cdc-1791">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="59cdc-1791">Az.Sql</span></span>
* <span data-ttu-id="59cdc-1792">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="59cdc-1792">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="59cdc-1793">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="59cdc-1793">Az.Websites</span></span>
* <span data-ttu-id="59cdc-1794">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="59cdc-1794">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="59cdc-1795">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="59cdc-1795">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="59cdc-1796">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="59cdc-1796">0.2.0 - September 2018</span></span>
 <span data-ttu-id="59cdc-1797">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="59cdc-1797">Initial Release</span></span>
