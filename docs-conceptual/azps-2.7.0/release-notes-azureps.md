---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/25/2019
ms.openlocfilehash: b879d970d3237098e481dba0419ee65efa8d51cd
ms.sourcegitcommit: f0f09eee03ef9dd7fe07432252a3dc8ca93e3a7b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "71319325"
---
## <a name="270---september-2019"></a><span data-ttu-id="af749-103">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="af749-103">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="af749-104">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af749-104">Az.ApiManagement</span></span>
* <span data-ttu-id="af749-105">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-105">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="af749-106">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="af749-106">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="af749-107">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="af749-107">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-108">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-108">Az.Automation</span></span>
* <span data-ttu-id="af749-109">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-109">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="af749-110">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-110">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="af749-111">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-111">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-112">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-112">Az.Compute</span></span>
* <span data-ttu-id="af749-113">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="af749-113">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="af749-114">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="af749-114">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="af749-115">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="af749-115">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="af749-116">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="af749-116">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="af749-117">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="af749-117">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="af749-118">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="af749-118">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="af749-119">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="af749-119">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="af749-120">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="af749-120">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="af749-121">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="af749-121">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-122">Az.DataFactory</span></span>
* <span data-ttu-id="af749-123">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="af749-123">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="af749-124">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-124">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="af749-125">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="af749-125">Az.HDInsight</span></span>
* <span data-ttu-id="af749-126">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="af749-126">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="af749-127">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="af749-127">Az.IotHub</span></span>
* <span data-ttu-id="af749-128">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="af749-128">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="af749-129">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="af749-129">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="af749-130">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="af749-130">New cmdlets are:</span></span>
    - <span data-ttu-id="af749-131">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="af749-131">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="af749-132">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="af749-132">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="af749-133">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="af749-133">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="af749-134">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="af749-134">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="af749-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-135">Az.Monitor</span></span>
* <span data-ttu-id="af749-136">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="af749-136">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="af749-137">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="af749-137">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="af749-138">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="af749-138">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="af749-139">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="af749-139">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="af749-140">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="af749-140">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="af749-141">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="af749-141">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="af749-142">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="af749-142">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="af749-143">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="af749-143">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="af749-144">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="af749-144">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="af749-145">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="af749-145">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="af749-146">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="af749-146">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="af749-147">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="af749-147">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="af749-148">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="af749-148">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="af749-149">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="af749-149">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="af749-150">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="af749-150">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="af749-151">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="af749-151">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="af749-152">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="af749-152">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="af749-153">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="af749-153">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="af749-154">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-154">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="af749-155">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="af749-155">Overall improved help files</span></span>
* <span data-ttu-id="af749-156">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="af749-156">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-157">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-157">Az.Network</span></span>
* <span data-ttu-id="af749-158">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="af749-158">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="af749-159">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="af749-159">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="af749-160">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="af749-160">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="af749-161">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="af749-161">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="af749-162">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="af749-162">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="af749-163">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-163">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="af749-164">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-164">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="af749-165">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-165">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="af749-166">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-166">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="af749-167">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-167">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="af749-168">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-168">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="af749-169">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="af749-169">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="af749-170">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-170">New cmdlets</span></span>
        - <span data-ttu-id="af749-171">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="af749-171">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="af749-172">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="af749-172">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="af749-173">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="af749-173">Updated cmdlet:</span></span>
        - <span data-ttu-id="af749-174">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="af749-174">New-VpnSite</span></span>
        - <span data-ttu-id="af749-175">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="af749-175">Update-VpnSite</span></span>
        - <span data-ttu-id="af749-176">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="af749-176">New-VpnConnection</span></span>
        - <span data-ttu-id="af749-177">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="af749-177">Update-VpnConnection</span></span>
* <span data-ttu-id="af749-178">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-178">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-179">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-179">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-180">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-180">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="af749-181">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-181">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-182">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-182">Az.Resources</span></span>
* <span data-ttu-id="af749-183">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-183">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="af749-184">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-184">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-185">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-185">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="af749-186">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="af749-186">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="af749-187">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="af749-187">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="af749-188">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="af749-188">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="af749-189">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="af749-189">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="af749-190">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="af749-190">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="af749-191">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="af749-191">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="af749-192">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="af749-192">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="af749-193">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="af749-193">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="af749-194">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="af749-194">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="af749-195">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="af749-195">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="af749-196">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="af749-196">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="af749-197">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="af749-197">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="af749-198">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="af749-198">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="af749-199">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="af749-199">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="af749-200">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="af749-200">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="af749-201">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="af749-201">Az.SignalR</span></span>
* <span data-ttu-id="af749-202">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="af749-202">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-203">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-203">Az.Sql</span></span>
* <span data-ttu-id="af749-204">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="af749-204">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="af749-205">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-205">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="af749-206">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="af749-206">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="af749-207">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-207">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="af749-208">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="af749-208">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-209">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-209">Az.Storage</span></span>
* <span data-ttu-id="af749-210">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-210">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="af749-211">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="af749-211">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="af749-212">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="af749-212">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="af749-213">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="af749-213">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="af749-214">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="af749-214">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="af749-215">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="af749-215">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="af749-216">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="af749-216">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="af749-217">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="af749-217">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="af749-218">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="af749-218">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="af749-219">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="af749-219">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="af749-220">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="af749-220">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-221">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-221">Az.Websites</span></span>
* <span data-ttu-id="af749-222">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="af749-222">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="af749-223">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="af749-223">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="af749-224">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="af749-224">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="af749-225">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="af749-225">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="af749-226">全般</span><span class="sxs-lookup"><span data-stu-id="af749-226">General</span></span>
* <span data-ttu-id="af749-227">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-227">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="af749-228">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-228">Az.Accounts</span></span>
* <span data-ttu-id="af749-229">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="af749-229">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="af749-230">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="af749-230">Az.Aks</span></span>
* <span data-ttu-id="af749-231">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-231">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="af749-232">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="af749-232">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="af749-233">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af749-233">Az.ApiManagement</span></span>
* <span data-ttu-id="af749-234">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="af749-234">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="af749-235">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="af749-235">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="af749-236">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-236">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="af749-237">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="af749-237">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="af749-238">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-238">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="af749-239">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="af749-239">Az.Batch</span></span>
* <span data-ttu-id="af749-240">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="af749-240">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="af749-241">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="af749-241">Az.Cdn</span></span>
* <span data-ttu-id="af749-242">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-242">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-243">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-243">Az.Compute</span></span>
* <span data-ttu-id="af749-244">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-244">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="af749-245">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-245">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="af749-246">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-246">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="af749-247">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-247">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="af749-248">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="af749-248">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="af749-249">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="af749-249">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="af749-250">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-250">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="af749-251">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-251">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-252">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-252">Az.DataFactory</span></span>
* <span data-ttu-id="af749-253">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-253">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="af749-254">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-254">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="af749-255">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="af749-255">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="af749-256">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-256">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-257">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-257">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-258">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-258">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="af749-259">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="af749-259">Az.EventHub</span></span>
* <span data-ttu-id="af749-260">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="af749-260">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="af749-261">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="af749-261">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="af749-262">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-262">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="af749-263">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="af749-263">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="af749-264">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="af749-264">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="af749-265">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-265">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="af749-266">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-266">Az.Monitor</span></span>
* <span data-ttu-id="af749-267">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-267">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-268">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-268">Az.Network</span></span>
* <span data-ttu-id="af749-269">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-269">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="af749-270">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="af749-270">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="af749-271">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-271">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="af749-272">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-272">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="af749-273">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="af749-273">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="af749-274">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-274">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="af749-275">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-275">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="af749-276">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-276">Az.OperationalInsights</span></span>
* <span data-ttu-id="af749-277">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-277">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="af749-278">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-278">Added example</span></span>
    - <span data-ttu-id="af749-279">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-279">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="af749-280">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-280">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="af749-281">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-281">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-282">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-282">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-283">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-283">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-284">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-284">Az.Resources</span></span>
* <span data-ttu-id="af749-285">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-285">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="af749-286">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-286">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="af749-287">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="af749-287">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="af749-288">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-288">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="af749-289">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="af749-289">Az.ServiceBus</span></span>
* <span data-ttu-id="af749-290">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="af749-290">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="af749-291">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="af749-291">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="af749-292">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-292">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="af749-293">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-293">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-294">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-294">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="af749-295">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="af749-295">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="af749-296">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="af749-296">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="af749-297">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-297">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="af749-298">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="af749-298">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="af749-299">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="af749-299">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-300">Az.Sql</span></span>
* <span data-ttu-id="af749-301">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-301">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-302">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-302">Az.Storage</span></span>
* <span data-ttu-id="af749-303">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-303">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="af749-304">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="af749-304">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="af749-305">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="af749-305">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="af749-306">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="af749-306">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="af749-307">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="af749-307">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="af749-308">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="af749-308">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-309">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-309">Az.Websites</span></span>
* <span data-ttu-id="af749-310">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-310">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="af749-311">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="af749-311">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-312">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-312">Az.Accounts</span></span>
* <span data-ttu-id="af749-313">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-313">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="af749-314">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="af749-314">Az.ApplicationInsights</span></span>
* <span data-ttu-id="af749-315">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-315">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="af749-316">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-316">Az.Automation</span></span>
* <span data-ttu-id="af749-317">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-317">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="af749-318">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="af749-318">Az.CognitiveServices</span></span>
* <span data-ttu-id="af749-319">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-319">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-320">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-320">Az.Compute</span></span>
* <span data-ttu-id="af749-321">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-321">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="af749-322">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="af749-322">Az.ContainerRegistry</span></span>
* <span data-ttu-id="af749-323">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-323">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="af749-324">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="af749-324">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-325">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-325">Az.DataFactory</span></span>
* <span data-ttu-id="af749-326">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-326">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="af749-327">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-327">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="af749-328">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="af749-328">Az.EventHub</span></span>
* <span data-ttu-id="af749-329">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="af749-329">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="af749-330">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-330">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="af749-331">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af749-331">Az.KeyVault</span></span>
* <span data-ttu-id="af749-332">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-332">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="af749-333">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="af749-333">Az.LogicApp</span></span>
* <span data-ttu-id="af749-334">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-334">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="af749-335">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-335">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="af749-336">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="af749-336">Az.ManagedServices</span></span>
* <span data-ttu-id="af749-337">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-337">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-338">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-338">Az.Network</span></span>
* <span data-ttu-id="af749-339">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-339">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="af749-340">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-340">New cmdlets</span></span>
        - <span data-ttu-id="af749-341">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="af749-341">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="af749-342">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="af749-342">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="af749-343">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="af749-343">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="af749-344">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="af749-344">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="af749-345">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="af749-345">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="af749-346">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="af749-346">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="af749-347">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="af749-347">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="af749-348">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="af749-348">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="af749-349">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="af749-349">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="af749-350">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-350">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="af749-351">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-351">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="af749-352">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-352">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="af749-353">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="af749-353">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="af749-354">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="af749-354">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="af749-355">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-355">Updated cmdlets</span></span>
        - <span data-ttu-id="af749-356">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="af749-356">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="af749-357">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="af749-357">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="af749-358">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="af749-358">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="af749-359">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-359">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="af749-360">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-360">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="af749-361">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="af749-361">Updated cmdlet:</span></span>
        - <span data-ttu-id="af749-362">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="af749-362">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="af749-363">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="af749-363">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="af749-364">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="af749-364">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="af749-365">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="af749-365">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="af749-366">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-366">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="af749-367">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="af749-367">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="af749-368">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-368">Az.OperationalInsights</span></span>
* <span data-ttu-id="af749-369">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-369">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="af749-370">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-370">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-371">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-371">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-372">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-372">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="af749-373">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-373">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="af749-374">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-374">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="af749-375">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-375">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="af749-376">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-376">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="af749-377">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-377">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="af749-378">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-378">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="af749-379">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-379">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="af749-380">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-380">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="af749-381">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-381">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-382">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-382">Az.Resources</span></span>
- <span data-ttu-id="af749-383">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="af749-383">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="af749-384">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-384">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="af749-385">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="af749-385">Az.ServiceBus</span></span>
* <span data-ttu-id="af749-386">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="af749-386">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="af749-387">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-387">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-388">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-388">Az.Sql</span></span>
* <span data-ttu-id="af749-389">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-389">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="af749-390">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-390">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="af749-391">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-391">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-392">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-392">Az.Storage</span></span>
* <span data-ttu-id="af749-393">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-393">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="af749-394">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="af749-394">Az.StorageSync</span></span>
* <span data-ttu-id="af749-395">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-395">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="af749-396">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-396">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-397">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-397">Az.Websites</span></span>
* <span data-ttu-id="af749-398">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-398">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="af749-399">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-399">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="af749-400">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-400">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="af749-401">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="af749-401">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-402">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-402">Az.Accounts</span></span>
* <span data-ttu-id="af749-403">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="af749-403">Add support for profile cmdlets</span></span>
* <span data-ttu-id="af749-404">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="af749-404">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="af749-405">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="af749-405">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="af749-406">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="af749-406">Az.Advisor</span></span>
* <span data-ttu-id="af749-407">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="af749-407">GA release of Az.Advisor</span></span>
* <span data-ttu-id="af749-408">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="af749-408">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="af749-409">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af749-409">Az.ApiManagement</span></span>
* <span data-ttu-id="af749-410">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="af749-410">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="af749-411">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="af749-411">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="af749-412">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-412">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="af749-413">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-413">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="af749-414">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="af749-414">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="af749-415">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="af749-415">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="af749-416">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-416">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-417">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-417">Az.Automation</span></span>
* <span data-ttu-id="af749-418">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-418">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-419">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-419">Az.Compute</span></span>
* <span data-ttu-id="af749-420">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="af749-420">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-421">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-421">Az.DataFactory</span></span>
* <span data-ttu-id="af749-422">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="af749-422">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="af749-423">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="af749-423">Az.EventGrid</span></span>
* <span data-ttu-id="af749-424">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="af749-424">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="af749-425">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="af749-425">Az.IotHub</span></span>
* <span data-ttu-id="af749-426">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-426">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-427">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-427">Az.Network</span></span>
* <span data-ttu-id="af749-428">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-428">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="af749-429">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="af749-429">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="af749-430">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="af749-430">Az.PolicyInsights</span></span>
* <span data-ttu-id="af749-431">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-431">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="af749-432">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="af749-432">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="af749-433">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-433">Az.OperationalInsights</span></span>
* <span data-ttu-id="af749-434">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-434">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-435">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-435">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-436">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-436">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-437">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-437">Az.Resources</span></span>
    - <span data-ttu-id="af749-438">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-438">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="af749-439">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-439">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="af749-440">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-440">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="af749-441">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-441">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="af749-442">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="af749-442">Az.ServiceBus</span></span>
* <span data-ttu-id="af749-443">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="af749-443">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-444">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-444">Az.Sql</span></span>
* <span data-ttu-id="af749-445">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-445">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="af749-446">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="af749-446">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="af749-447">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="af749-447">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="af749-448">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="af749-448">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="af749-449">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="af749-449">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="af749-450">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="af749-450">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="af749-451">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="af749-451">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="af749-452">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="af749-452">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="af749-453">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="af749-453">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-454">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-454">Az.Storage</span></span>
* <span data-ttu-id="af749-455">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="af749-455">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="af749-456">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="af749-456">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="af749-457">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-457">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="af749-458">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="af749-458">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="af749-459">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="af749-459">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="af749-460">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-460">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="af749-461">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-461">Set-AzStorageAccount</span></span>
* <span data-ttu-id="af749-462">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="af749-462">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="af749-463">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="af749-463">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="af749-464">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="af749-464">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="af749-465">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="af749-465">Az.StorageSync</span></span>
* <span data-ttu-id="af749-466">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="af749-466">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="af749-467">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="af749-467">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-468">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-468">Az.Accounts</span></span>
* <span data-ttu-id="af749-469">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-469">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="af749-470">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="af749-470">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="af749-471">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-471">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="af749-472">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="af749-472">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="af749-473">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="af749-473">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-474">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-474">Az.Compute</span></span>
* <span data-ttu-id="af749-475">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-475">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="af749-476">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-476">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="af749-477">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="af749-477">Az.Dns</span></span>
* <span data-ttu-id="af749-478">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-478">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="af749-479">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="af749-479">Az.EventGrid</span></span>
* <span data-ttu-id="af749-480">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-480">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="af749-481">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="af749-481">New cmdlets:</span></span>
    - <span data-ttu-id="af749-482">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="af749-482">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="af749-483">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="af749-483">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="af749-484">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="af749-484">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="af749-485">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="af749-485">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="af749-486">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="af749-486">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="af749-487">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="af749-487">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="af749-488">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="af749-488">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="af749-489">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="af749-489">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="af749-490">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="af749-490">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="af749-491">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="af749-491">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="af749-492">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="af749-492">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="af749-493">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="af749-493">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="af749-494">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="af749-494">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="af749-495">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="af749-495">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="af749-496">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="af749-496">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="af749-497">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="af749-497">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="af749-498">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="af749-498">Updated cmdlets:</span></span>
    - <span data-ttu-id="af749-499">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="af749-499">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="af749-500">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-500">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="af749-501">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-501">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="af749-502">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="af749-502">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="af749-503">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="af749-503">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="af749-504">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="af749-504">Event subscription expiration date,</span></span>
            - <span data-ttu-id="af749-505">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="af749-505">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="af749-506">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-506">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="af749-507">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="af749-507">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="af749-508">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="af749-508">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="af749-509">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-509">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="af749-510">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="af749-510">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="af749-511">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-511">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="af749-512">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-512">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="af749-513">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="af749-513">Az.FrontDoor</span></span>
* <span data-ttu-id="af749-514">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="af749-514">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="af749-515">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-515">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="af749-516">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="af749-516">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="af749-517">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-517">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-518">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-518">Az.Network</span></span>
* <span data-ttu-id="af749-519">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-519">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="af749-520">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-520">New cmdlets</span></span>
        - <span data-ttu-id="af749-521">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="af749-521">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="af749-522">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-522">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="af749-523">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-523">New cmdlets</span></span> 
        - <span data-ttu-id="af749-524">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="af749-524">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="af749-525">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-525">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="af749-526">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-526">New cmdlets</span></span> 
        - <span data-ttu-id="af749-527">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="af749-527">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="af749-528">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="af749-528">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="af749-529">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="af749-529">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="af749-530">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="af749-530">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="af749-531">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="af749-531">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="af749-532">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-532">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="af749-533">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-533">New cmdlets</span></span>
        - <span data-ttu-id="af749-534">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="af749-534">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="af749-535">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="af749-535">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="af749-536">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="af749-536">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="af749-537">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="af749-537">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="af749-538">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="af749-538">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="af749-539">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-539">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="af749-540">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-540">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="af749-541">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-541">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="af749-542">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-542">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="af749-543">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-543">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="af749-544">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-544">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="af749-545">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-545">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="af749-546">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-546">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="af749-547">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-547">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="af749-548">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-548">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="af749-549">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-549">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="af749-550">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-550">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="af749-551">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-551">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="af749-552">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="af749-552">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="af749-553">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-553">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="af749-554">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-554">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="af749-555">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="af749-555">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="af749-556">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="af749-556">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="af749-557">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="af749-557">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="af749-558">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-558">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="af749-559">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-559">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="af749-560">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-560">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="af749-561">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-561">Az.OperationalInsights</span></span>
* <span data-ttu-id="af749-562">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="af749-562">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-563">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-563">Az.Resources</span></span>
* <span data-ttu-id="af749-564">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="af749-564">Support for additional Template Export options</span></span>
    - <span data-ttu-id="af749-565">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-565">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="af749-566">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-566">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="af749-567">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-567">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="af749-568">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-568">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-569">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-569">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-570">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-570">Az.Sql</span></span>
* <span data-ttu-id="af749-571">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-571">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="af749-572">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-572">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="af749-573">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="af749-573">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="af749-574">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="af749-574">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="af749-575">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="af749-575">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="af749-576">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="af749-576">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="af749-577">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="af749-577">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="af749-578">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="af749-578">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-579">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-579">Az.Storage</span></span>
* <span data-ttu-id="af749-580">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-580">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="af749-581">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-581">New-AzStorageAccount</span></span>
* <span data-ttu-id="af749-582">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="af749-582">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="af749-583">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="af749-583">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-584">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-584">Az.Websites</span></span>
* <span data-ttu-id="af749-585">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="af749-585">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="af749-586">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-586">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="af749-587">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="af749-587">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="af749-588">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="af749-588">Az.Cdn</span></span>
* <span data-ttu-id="af749-589">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-589">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-590">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-590">Az.Compute</span></span>
* <span data-ttu-id="af749-591">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-591">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="af749-592">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="af749-592">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="af749-593">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="af749-593">Az.EventHub</span></span>
* <span data-ttu-id="af749-594">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-594">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="af749-595">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-595">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-596">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-596">Az.Network</span></span>
* <span data-ttu-id="af749-597">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-597">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="af749-598">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-598">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="af749-599">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="af749-599">Az.PolicyInsights</span></span>
* <span data-ttu-id="af749-600">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-600">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-601">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-601">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-602">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-602">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="af749-603">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="af749-603">Az.ServiceBus</span></span>
* <span data-ttu-id="af749-604">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-604">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="af749-605">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-605">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-606">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-606">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="af749-607">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-607">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-608">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-608">Az.Sql</span></span>
* <span data-ttu-id="af749-609">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-609">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="af749-610">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="af749-610">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="af749-611">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-611">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="af749-612">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-612">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-613">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-613">Az.Websites</span></span>
* <span data-ttu-id="af749-614">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-614">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="af749-615">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="af749-615">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="af749-616">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af749-616">Az.ApiManagement</span></span>
* <span data-ttu-id="af749-617">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="af749-617">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="af749-618">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="af749-618">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="af749-619">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="af749-619">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="af749-620">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="af749-620">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="af749-621">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="af749-621">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="af749-622">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="af749-622">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="af749-623">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="af749-623">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="af749-624">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="af749-624">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="af749-625">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="af749-625">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="af749-626">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="af749-626">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="af749-627">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="af749-627">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="af749-628">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="af749-628">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="af749-629">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="af749-629">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="af749-630">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-630">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="af749-631">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="af749-631">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="af749-632">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="af749-632">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="af749-633">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="af749-633">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="af749-634">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="af749-634">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="af749-635">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="af749-635">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="af749-636">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="af749-636">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="af749-637">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="af749-637">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="af749-638">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="af749-638">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="af749-639">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="af749-639">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="af749-640">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-640">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="af749-641">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-641">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="af749-642">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-642">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="af749-643">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="af749-643">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="af749-644">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="af749-644">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="af749-645">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-645">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="af749-646">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-646">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="af749-647">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-647">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="af749-648">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="af749-648">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="af749-649">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-649">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="af749-650">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-650">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="af749-651">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="af749-651">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="af749-652">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="af749-652">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="af749-653">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="af749-653">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="af749-654">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-654">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="af749-655">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-655">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="af749-656">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-656">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="af749-657">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="af749-657">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="af749-658">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="af749-658">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="af749-659">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="af749-659">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="af749-660">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-660">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="af749-661">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-661">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="af749-662">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="af749-662">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="af749-663">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="af749-663">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="af749-664">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-664">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="af749-665">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-665">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="af749-666">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="af749-666">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="af749-667">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="af749-667">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="af749-668">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="af749-668">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="af749-669">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="af749-669">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="af749-670">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-670">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="af749-671">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="af749-671">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="af749-672">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="af749-672">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="af749-673">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-673">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="af749-674">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="af749-674">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="af749-675">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="af749-675">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="af749-676">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-676">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="af749-677">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-677">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="af749-678">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="af749-678">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="af749-679">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="af749-679">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="af749-680">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-680">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="af749-681">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-681">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="af749-682">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="af749-682">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="af749-683">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="af749-683">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="af749-684">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="af749-684">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="af749-685">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="af749-685">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="af749-686">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="af749-686">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="af749-687">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="af749-687">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="af749-688">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="af749-688">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="af749-689">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="af749-689">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="af749-690">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="af749-690">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="af749-691">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="af749-691">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="af749-692">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="af749-692">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="af749-693">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="af749-693">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-694">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-694">Az.Automation</span></span>
* <span data-ttu-id="af749-695">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-695">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="af749-696">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="af749-696">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="af749-697">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="af749-697">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="af749-698">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="af749-698">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="af749-699">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="af749-699">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="af749-700">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-700">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="af749-701">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-701">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-702">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-702">Az.Compute</span></span>
* <span data-ttu-id="af749-703">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-703">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="af749-704">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="af749-704">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-705">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-705">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-706">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-706">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="af749-707">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-707">Az.Monitor</span></span>
* <span data-ttu-id="af749-708">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-708">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-709">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-709">Az.Network</span></span>
* <span data-ttu-id="af749-710">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-710">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="af749-711">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="af749-711">Updated cmdlet:</span></span>
        - <span data-ttu-id="af749-712">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="af749-712">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="af749-713">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-713">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-714">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-714">Az.Resources</span></span>
* <span data-ttu-id="af749-715">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-715">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-716">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-716">Az.Sql</span></span>
* <span data-ttu-id="af749-717">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="af749-717">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="af749-718">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="af749-718">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-719">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-719">Az.Accounts</span></span>
* <span data-ttu-id="af749-720">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-720">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="af749-721">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="af749-721">Az.CognitiveServices</span></span>
* <span data-ttu-id="af749-722">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="af749-722">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="af749-723">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="af749-723">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-724">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-724">Az.Compute</span></span>
* <span data-ttu-id="af749-725">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="af749-725">Proximity placement group feature.</span></span>
    - <span data-ttu-id="af749-726">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="af749-726">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="af749-727">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="af749-727">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="af749-728">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-728">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="af749-729">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-729">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="af749-730">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-730">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="af749-731">重大な変更</span><span class="sxs-lookup"><span data-stu-id="af749-731">Breaking changes</span></span>
    - <span data-ttu-id="af749-732">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="af749-732">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="af749-733">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="af749-733">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="af749-734">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="af749-734">Az.DeploymentManager</span></span>
* <span data-ttu-id="af749-735">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="af749-735">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="af749-736">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="af749-736">Az.Dns</span></span>
* <span data-ttu-id="af749-737">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="af749-737">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="af749-738">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="af749-738">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="af749-739">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-739">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="af749-740">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="af749-740">Az.FrontDoor</span></span>
* <span data-ttu-id="af749-741">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="af749-741">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="af749-742">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="af749-742">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="af749-743">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="af749-743">Az.HDInsight</span></span>
* <span data-ttu-id="af749-744">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="af749-744">Removed two cmdlets:</span></span>
    - <span data-ttu-id="af749-745">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="af749-745">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="af749-746">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="af749-746">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="af749-747">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-747">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="af749-748">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-748">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="af749-749">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="af749-749">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="af749-750">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="af749-750">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="af749-751">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-751">Az.Monitor</span></span>
* <span data-ttu-id="af749-752">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="af749-752">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="af749-753">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="af749-753">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="af749-754">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="af749-754">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="af749-755">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="af749-755">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="af749-756">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="af749-756">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="af749-757">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="af749-757">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="af749-758">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="af749-758">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="af749-759">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="af749-759">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="af749-760">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="af749-760">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="af749-761">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="af749-761">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="af749-762">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="af749-762">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="af749-763">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="af749-763">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="af749-764">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="af749-764">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="af749-765">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-765">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-766">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-766">Az.Network</span></span>
* <span data-ttu-id="af749-767">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-767">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="af749-768">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-768">New cmdlets</span></span>
        - <span data-ttu-id="af749-769">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="af749-769">New-AzNatGateway</span></span>
        - <span data-ttu-id="af749-770">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="af749-770">Get-AzNatGateway</span></span>
        - <span data-ttu-id="af749-771">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="af749-771">Set-AzNatGateway</span></span>
        - <span data-ttu-id="af749-772">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="af749-772">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="af749-773">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-773">Updated cmdlets</span></span>
        - <span data-ttu-id="af749-774">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="af749-774">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="af749-775">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="af749-775">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="af749-776">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="af749-776">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="af749-777">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-777">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="af749-778">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-778">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="af749-779">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="af749-779">Az.PolicyInsights</span></span>
* <span data-ttu-id="af749-780">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="af749-780">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="af749-781">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-781">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="af749-782">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="af749-782">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-783">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-783">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-784">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="af749-784">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="af749-785">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="af749-785">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="af749-786">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="af749-786">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="af749-787">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="af749-787">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="af749-788">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="af749-788">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="af749-789">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="af749-789">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="af749-790">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="af749-790">Az.Relay</span></span>
* <span data-ttu-id="af749-791">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-791">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="af749-792">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="af749-792">Az.ServiceBus</span></span>
* <span data-ttu-id="af749-793">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-793">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-794">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-794">Az.Storage</span></span>
* <span data-ttu-id="af749-795">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="af749-795">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="af749-796">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="af749-796">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="af749-797">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-797">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="af749-798">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-798">New-AzStorageAccount</span></span>
* <span data-ttu-id="af749-799">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="af749-799">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="af749-800">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-800">New-AzStorageAccount</span></span>
    - <span data-ttu-id="af749-801">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-801">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="af749-802">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="af749-802">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-803">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-803">Az.Websites</span></span>
* <span data-ttu-id="af749-804">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="af749-804">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="af749-805">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="af749-805">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="af749-806">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="af749-806">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="af749-807">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="af749-807">Highlights since the last major release</span></span>
* <span data-ttu-id="af749-808">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="af749-808">General availability of `Az` module</span></span>
* <span data-ttu-id="af749-809">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="af749-809">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="af749-810">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="af749-810">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="af749-811">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-811">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="af749-812">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="af749-812">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="af749-813">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-813">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="af749-814">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-814">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="af749-815">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-815">Az.Accounts</span></span>
* <span data-ttu-id="af749-816">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="af749-816">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="af749-817">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="af749-817">Az.Batch</span></span>
* <span data-ttu-id="af749-818">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-818">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="af749-819">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="af749-819">Az.Cdn</span></span>
* <span data-ttu-id="af749-820">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-820">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="af749-821">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="af749-821">Az.CognitiveServices</span></span>
* <span data-ttu-id="af749-822">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-822">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-823">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-823">Az.Compute</span></span>
* <span data-ttu-id="af749-824">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="af749-824">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="af749-825">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-825">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="af749-826">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="af749-826">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-827">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-827">Az.DataFactory</span></span>
* <span data-ttu-id="af749-828">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-828">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-829">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-829">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-830">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-830">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="af749-831">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="af749-831">Az.EventGrid</span></span>
* <span data-ttu-id="af749-832">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-832">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="af749-833">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="af749-833">Az.EventHub</span></span>
* <span data-ttu-id="af749-834">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-834">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="af749-835">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="af749-835">Az.HDInsight</span></span>
* <span data-ttu-id="af749-836">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-836">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="af749-837">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="af749-837">Az.IotHub</span></span>
* <span data-ttu-id="af749-838">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-838">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="af749-839">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af749-839">Az.KeyVault</span></span>
* <span data-ttu-id="af749-840">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-840">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="af749-841">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="af749-841">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="af749-842">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="af749-842">Az.MachineLearning</span></span>
* <span data-ttu-id="af749-843">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-843">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="af749-844">Az.Media</span><span class="sxs-lookup"><span data-stu-id="af749-844">Az.Media</span></span>
* <span data-ttu-id="af749-845">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-845">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="af749-846">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-846">Az.Monitor</span></span>
  * <span data-ttu-id="af749-847">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-847">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="af749-848">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="af749-848">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="af749-849">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="af749-849">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="af749-850">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="af749-850">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="af749-851">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="af749-851">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="af749-852">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="af749-852">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="af749-853">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-853">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-854">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-854">Az.Network</span></span>
* <span data-ttu-id="af749-855">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-855">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="af749-856">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="af749-856">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="af749-857">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="af749-857">Az.NotificationHubs</span></span>
* <span data-ttu-id="af749-858">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-858">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="af749-859">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-859">Az.OperationalInsights</span></span>
* <span data-ttu-id="af749-860">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-860">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="af749-861">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="af749-861">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="af749-862">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-862">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-863">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-863">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-864">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-864">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="af749-865">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-865">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="af749-866">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-866">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="af749-867">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-867">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="af749-868">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="af749-868">Az.RedisCache</span></span>
* <span data-ttu-id="af749-869">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-869">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-870">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-870">Az.Resources</span></span>
* <span data-ttu-id="af749-871">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="af749-871">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-872">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-872">Az.Sql</span></span>
* <span data-ttu-id="af749-873">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="af749-873">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="af749-874">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-874">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="af749-875">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="af749-875">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="af749-876">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="af749-876">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="af749-877">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="af749-877">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="af749-878">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="af749-878">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="af749-879">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="af749-879">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-880">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-880">Az.Websites</span></span>
* <span data-ttu-id="af749-881">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="af749-881">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="af749-882">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-882">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="af749-883">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-883">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="af749-884">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="af749-884">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="af749-885">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="af749-885">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="af749-886">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="af749-886">Highlights since the last major release</span></span>
* <span data-ttu-id="af749-887">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="af749-887">General availability of `Az` module</span></span>
* <span data-ttu-id="af749-888">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="af749-888">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="af749-889">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="af749-889">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="af749-890">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-890">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="af749-891">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="af749-891">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="af749-892">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-892">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="af749-893">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-893">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="af749-894">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-894">Az.Accounts</span></span>
* <span data-ttu-id="af749-895">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-895">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="af749-896">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="af749-896">Az.AnalysisServices</span></span>
* <span data-ttu-id="af749-897">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="af749-897">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="af749-898">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="af749-898">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-899">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-899">Az.Automation</span></span>
* <span data-ttu-id="af749-900">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-900">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="af749-901">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-901">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="af749-902">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-902">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-903">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-903">Az.Compute</span></span>
* <span data-ttu-id="af749-904">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-904">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="af749-905">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-905">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="af749-906">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="af749-906">Az.ContainerInstance</span></span>
* <span data-ttu-id="af749-907">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-907">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-908">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-908">Az.DataFactory</span></span>
* <span data-ttu-id="af749-909">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-909">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="af749-910">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-910">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-911">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-911">Az.Resources</span></span>
* <span data-ttu-id="af749-912">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="af749-912">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="af749-913">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="af749-913">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="af749-914">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="af749-914">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="af749-915">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="af749-915">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="af749-916">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-916">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="af749-917">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="af749-917">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-918">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-918">Az.Sql</span></span>
* <span data-ttu-id="af749-919">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="af749-919">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-920">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-920">Az.Storage</span></span>
* <span data-ttu-id="af749-921">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="af749-921">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="af749-922">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="af749-922">New-AzStorageContext</span></span>
* <span data-ttu-id="af749-923">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="af749-923">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="af749-924">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="af749-924">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="af749-925">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="af749-925">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="af749-926">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="af749-926">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="af749-927">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="af749-927">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="af749-928">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="af749-928">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="af749-929">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="af749-929">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="af749-930">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="af749-930">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="af749-931">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="af749-931">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="af749-932">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="af749-932">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="af749-933">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="af749-933">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="af749-934">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="af749-934">Highlights since the last major release</span></span>
* <span data-ttu-id="af749-935">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="af749-935">General availability of `Az` module</span></span>
* <span data-ttu-id="af749-936">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="af749-936">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="af749-937">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="af749-937">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="af749-938">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-938">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="af749-939">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="af749-939">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="af749-940">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-940">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="af749-941">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-941">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-942">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-942">Az.Automation</span></span>
* <span data-ttu-id="af749-943">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="af749-943">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="af749-944">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="af749-944">Dynamic grouping</span></span>
    * <span data-ttu-id="af749-945">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="af749-945">Pre-Post script</span></span>
    * <span data-ttu-id="af749-946">再起動設定</span><span class="sxs-lookup"><span data-stu-id="af749-946">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-947">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-947">Az.Compute</span></span>
* <span data-ttu-id="af749-948">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-948">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="af749-949">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-949">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="af749-950">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af749-950">Az.KeyVault</span></span>
* <span data-ttu-id="af749-951">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-951">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-952">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-952">Az.Network</span></span>
* <span data-ttu-id="af749-953">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-953">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="af749-954">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-954">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-955">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-955">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-956">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-956">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="af749-957">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-957">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-958">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-958">Az.Resources</span></span>
* <span data-ttu-id="af749-959">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="af749-959">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="af749-960">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="af749-960">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-961">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-961">Az.Sql</span></span>
* <span data-ttu-id="af749-962">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="af749-962">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-963">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-963">Az.Storage</span></span>
* <span data-ttu-id="af749-964">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="af749-964">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="af749-965">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="af749-965">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="af749-966">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="af749-966">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="af749-967">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="af749-967">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="af749-968">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="af749-968">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="af749-969">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="af749-969">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="af749-970">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="af749-970">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-971">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-971">Az.Websites</span></span>
* <span data-ttu-id="af749-972">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="af749-972">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="af749-973">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="af749-973">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-974">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-974">Az.Accounts</span></span>
* <span data-ttu-id="af749-975">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-975">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="af749-976">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-976">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-977">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-977">Az.Automation</span></span>
* <span data-ttu-id="af749-978">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-978">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="af749-979">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-979">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="af749-980">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="af749-980">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="af749-981">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="af749-981">Az.Cdn</span></span>
* <span data-ttu-id="af749-982">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="af749-982">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-983">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-983">Az.Compute</span></span>
* <span data-ttu-id="af749-984">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-984">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-985">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-985">Az.DataFactory</span></span>
* <span data-ttu-id="af749-986">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-986">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="af749-987">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="af749-987">Az.LogicApp</span></span>
* <span data-ttu-id="af749-988">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-988">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-989">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-989">Az.Network</span></span>
* <span data-ttu-id="af749-990">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-990">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-991">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-991">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-992">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-992">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="af749-993">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="af749-993">SDK Update</span></span>
* <span data-ttu-id="af749-994">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="af749-994">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="af749-995">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-995">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-996">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-996">Az.Resources</span></span>
* <span data-ttu-id="af749-997">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-997">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="af749-998">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="af749-998">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="af749-999">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-999">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="af749-1000">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="af749-1000">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="af749-1001">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1001">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="af749-1002">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="af749-1002">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-1003">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1003">Az.Sql</span></span>
* <span data-ttu-id="af749-1004">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1004">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="af749-1005">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1005">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-1006">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-1006">Az.Storage</span></span>
* <span data-ttu-id="af749-1007">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="af749-1007">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="af749-1008">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="af749-1008">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="af749-1009">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="af749-1009">Az.AnalysisServices</span></span>
* <span data-ttu-id="af749-1010">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="af749-1010">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-1011">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-1011">Az.Automation</span></span>
* <span data-ttu-id="af749-1012">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1012">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="af749-1013">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1013">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="af749-1014">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="af749-1014">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="af749-1015">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="af749-1015">Az.CognitiveServices</span></span>
* <span data-ttu-id="af749-1016">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="af749-1016">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1017">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1017">Az.Compute</span></span>
* <span data-ttu-id="af749-1018">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1018">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="af749-1019">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1019">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="af749-1020">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1020">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="af749-1021">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="af749-1021">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-1022">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1022">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-1023">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1023">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="af749-1024">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="af749-1024">Az.EventHub</span></span>
* <span data-ttu-id="af749-1025">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1025">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="af749-1026">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af749-1026">Az.KeyVault</span></span>
* <span data-ttu-id="af749-1027">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1027">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="af749-1028">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="af749-1028">Az.LogicApp</span></span>
* <span data-ttu-id="af749-1029">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1029">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="af749-1030">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1030">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="af749-1031">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-1031">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="af749-1032">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="af749-1032">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="af749-1033">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="af749-1033">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="af749-1034">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="af749-1034">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="af749-1035">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="af749-1035">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="af749-1036">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-1036">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="af749-1037">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="af749-1037">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="af749-1038">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="af749-1038">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="af749-1039">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="af749-1039">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="af749-1040">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="af749-1040">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="af749-1041">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1041">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="af749-1042">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-1042">Az.Monitor</span></span>
* <span data-ttu-id="af749-1043">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1043">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-1044">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1044">Az.Network</span></span>
* <span data-ttu-id="af749-1045">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1045">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="af749-1046">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-1046">Az.OperationalInsights</span></span>
* <span data-ttu-id="af749-1047">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1047">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="af749-1048">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1048">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="af749-1049">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1049">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="af749-1050">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1050">Az.Resources</span></span>
* <span data-ttu-id="af749-1051">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="af749-1051">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="af749-1052">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="af749-1052">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="af749-1053">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="af749-1053">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="af749-1054">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1054">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-1055">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1055">Az.Sql</span></span>
* <span data-ttu-id="af749-1056">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1056">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="af749-1057">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1057">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-1058">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-1058">Az.Websites</span></span>
* <span data-ttu-id="af749-1059">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1059">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="af749-1060">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="af749-1060">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-1061">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-1061">Az.Accounts</span></span>
* <span data-ttu-id="af749-1062">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="af749-1062">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="af749-1063">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="af749-1063">Az.AnalysisServices</span></span>
<span data-ttu-id="af749-1064">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="af749-1064">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1065">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1065">Az.Compute</span></span>
* <span data-ttu-id="af749-1066">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-1066">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="af749-1067">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1067">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="af749-1068">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1068">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-1069">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-1069">Az.RecoveryServices</span></span>
<span data-ttu-id="af749-1070">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="af749-1070">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-1071">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1071">Az.Resources</span></span>
* <span data-ttu-id="af749-1072">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="af749-1072">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="af749-1073">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="af749-1073">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="af749-1074">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1074">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="af749-1075">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="af749-1075">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-1076">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1076">Az.Sql</span></span>
* <span data-ttu-id="af749-1077">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="af749-1077">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="af749-1078">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1078">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="af749-1079">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1079">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="af749-1080">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="af749-1080">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-1081">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-1081">Az.Accounts</span></span>
* <span data-ttu-id="af749-1082">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="af749-1082">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="af749-1083">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="af749-1083">Az.AnalysisServices</span></span>
* <span data-ttu-id="af749-1084">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="af749-1084">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="af749-1085">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-1085">Az.RecoveryServices</span></span>
* <span data-ttu-id="af749-1086">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="af749-1086">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="af749-1087">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="af749-1087">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-1088">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-1088">Az.Accounts</span></span>
* <span data-ttu-id="af749-1089">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="af749-1089">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="af749-1090">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1090">Update incorrect online help URLs</span></span>
* <span data-ttu-id="af749-1091">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="af749-1091">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="af749-1092">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="af749-1092">Az.Aks</span></span>
* <span data-ttu-id="af749-1093">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1093">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="af749-1094">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-1094">Az.Automation</span></span>
* <span data-ttu-id="af749-1095">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="af749-1095">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="af749-1096">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1096">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="af749-1097">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="af749-1097">Az.Cdn</span></span>
* <span data-ttu-id="af749-1098">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1098">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1099">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1099">Az.Compute</span></span>
* <span data-ttu-id="af749-1100">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="af749-1100">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="af749-1101">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="af749-1101">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="af749-1102">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="af749-1102">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="af749-1103">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="af749-1103">Az.ContainerRegistry</span></span>
* <span data-ttu-id="af749-1104">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1104">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="af749-1105">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="af749-1105">Az.DataFactory</span></span>
* <span data-ttu-id="af749-1106">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="af749-1106">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-1107">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1107">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-1108">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="af749-1108">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="af749-1109">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="af749-1109">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="af749-1110">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1110">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="af749-1111">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="af749-1111">Az.IotHub</span></span>
* <span data-ttu-id="af749-1112">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="af749-1112">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="af749-1113">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af749-1113">Az.KeyVault</span></span>
* <span data-ttu-id="af749-1114">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1114">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-1115">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1115">Az.Network</span></span>
* <span data-ttu-id="af749-1116">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1116">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-1117">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1117">Az.Resources</span></span>
* <span data-ttu-id="af749-1118">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1118">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="af749-1119">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1119">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="af749-1120">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="af749-1120">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="af749-1121">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="af749-1121">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="af749-1122">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="af749-1122">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="af749-1123">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1123">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="af749-1124">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="af749-1124">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="af749-1125">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-1125">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-1126">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="af749-1126">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="af749-1127">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="af749-1127">Fix some error messages.</span></span>
* <span data-ttu-id="af749-1128">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1128">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="af749-1129">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1129">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="af749-1130">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="af749-1130">Az.SignalR</span></span>
* <span data-ttu-id="af749-1131">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1131">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-1132">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1132">Az.Sql</span></span>
* <span data-ttu-id="af749-1133">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1133">Update incorrect online help URLs</span></span>
* <span data-ttu-id="af749-1134">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1134">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="af749-1135">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1135">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="af749-1136">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="af749-1136">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-1137">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-1137">Az.Storage</span></span>
* <span data-ttu-id="af749-1138">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1138">Update incorrect online help URLs</span></span>
* <span data-ttu-id="af749-1139">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="af749-1139">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="af749-1140">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="af749-1140">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="af749-1141">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="af749-1141">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="af749-1142">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="af749-1142">Az.TrafficManager</span></span>
* <span data-ttu-id="af749-1143">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1143">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-1144">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-1144">Az.Websites</span></span>
* <span data-ttu-id="af749-1145">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="af749-1145">Update incorrect online help URLs</span></span>
* <span data-ttu-id="af749-1146">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1146">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="af749-1147">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="af749-1147">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="af749-1148">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="af749-1148">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="af749-1149">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-1149">Az.Accounts</span></span>
* <span data-ttu-id="af749-1150">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="af749-1150">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1151">Az.Compute</span></span>
* <span data-ttu-id="af749-1152">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-1152">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="af749-1153">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="af749-1153">Updated the description of ID in help files</span></span>
* <span data-ttu-id="af749-1154">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1154">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-1155">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1155">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-1156">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1156">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="af749-1157">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1157">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="af749-1158">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="af749-1158">Az.EventGrid</span></span>
* <span data-ttu-id="af749-1159">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1159">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="af749-1160">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="af749-1160">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="af749-1161">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="af749-1161">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="af749-1162">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="af749-1162">Event Time-To-Live,</span></span>
        - <span data-ttu-id="af749-1163">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="af749-1163">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="af749-1164">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="af749-1164">Dead letter endpoint.</span></span>
    - <span data-ttu-id="af749-1165">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="af749-1165">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="af749-1166">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="af749-1166">Event Time-To-Live,</span></span>
        - <span data-ttu-id="af749-1167">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="af749-1167">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="af749-1168">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="af749-1168">Dead letter endpoint.</span></span>
* <span data-ttu-id="af749-1169">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1169">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="af749-1170">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="af749-1170">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="af749-1171">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="af749-1171">Az.IotHub</span></span>
* <span data-ttu-id="af749-1172">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1172">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="af749-1173">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="af749-1173">Az.LogicApp</span></span>
* <span data-ttu-id="af749-1174">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="af749-1174">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-1175">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1175">Az.Resources</span></span>
* <span data-ttu-id="af749-1176">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1176">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="af749-1177">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="af749-1177">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="af749-1178">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1178">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="af749-1179">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1179">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="af749-1180">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="af749-1180">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="af749-1181">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="af749-1181">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="af749-1182">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="af749-1182">Az.SignalR</span></span>
* <span data-ttu-id="af749-1183">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1183">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-1184">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1184">Az.Sql</span></span>
* <span data-ttu-id="af749-1185">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="af749-1185">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="af749-1186">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-1186">Az.Storage</span></span>
* <span data-ttu-id="af749-1187">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="af749-1187">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="af749-1188">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="af749-1188">New-AzStorageContext</span></span>
* <span data-ttu-id="af749-1189">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1189">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="af749-1190">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="af749-1190">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-1191">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-1191">Az.Websites</span></span>
* <span data-ttu-id="af749-1192">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1192">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="af749-1193">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1193">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="af749-1194">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="af749-1194">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="af749-1195">全般</span><span class="sxs-lookup"><span data-stu-id="af749-1195">General</span></span>

- <span data-ttu-id="af749-1196">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="af749-1196">General Availability of Az Module</span></span>
- <span data-ttu-id="af749-1197">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="af749-1197">Online help for each module</span></span>
- <span data-ttu-id="af749-1198">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1198">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="af749-1199">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1199">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="af749-1200">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="af749-1200">Az.Accounts</span></span>
- <span data-ttu-id="af749-1201">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-1201">Changed from Az.Profile</span></span>
- <span data-ttu-id="af749-1202">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1202">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="af749-1203">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af749-1203">Az.ApiManagement</span></span>
- <span data-ttu-id="af749-1204">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="af749-1204">Fixes for #7002</span></span>
- <span data-ttu-id="af749-1205">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1205">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="af749-1206">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="af749-1206">Az.Batch</span></span>
- <span data-ttu-id="af749-1207">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1207">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="af749-1208">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="af749-1208">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="af749-1209">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1209">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="af749-1210">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="af749-1210">Az.Billing</span></span>
- <span data-ttu-id="af749-1211">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1211">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="af749-1212">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="af749-1212">Az.CognitivServices</span></span>
- <span data-ttu-id="af749-1213">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1213">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="af749-1214">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="af749-1214">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="af749-1215">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="af749-1215">Az.ContainerInstance</span></span>
- <span data-ttu-id="af749-1216">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1216">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="af749-1217">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="af749-1217">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="af749-1218">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1218">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="af749-1219">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1219">Az.DataLakeStore</span></span>
- <span data-ttu-id="af749-1220">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1220">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="af749-1221">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="af749-1221">Az.Monitor</span></span>
- <span data-ttu-id="af749-1222">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1222">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="af749-1223">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="af749-1223">Az.KeyVault</span></span>
- <span data-ttu-id="af749-1224">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="af749-1224">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="af749-1225">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="af749-1225">Az.MachineLearning</span></span>
- <span data-ttu-id="af749-1226">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="af749-1226">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="af749-1227">Az.Media</span><span class="sxs-lookup"><span data-stu-id="af749-1227">Az.Media</span></span>
- <span data-ttu-id="af749-1228">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="af749-1228">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="af749-1229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1229">Az.Network</span></span>
<span data-ttu-id="af749-1230">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1230">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="af749-1231">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="af749-1231">New cmdlets added:</span></span>
        - <span data-ttu-id="af749-1232">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="af749-1232">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="af749-1233">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="af749-1233">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="af749-1234">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="af749-1234">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="af749-1235">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="af749-1235">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="af749-1236">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="af749-1236">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="af749-1237">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="af749-1237">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="af749-1238">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="af749-1238">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="af749-1239">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="af749-1239">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="af749-1240">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-1240">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="af749-1241">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="af749-1241">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="af749-1242">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="af749-1242">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="af749-1243">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="af749-1243">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="af749-1244">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="af749-1244">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="af749-1245">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="af749-1245">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="af749-1246">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1246">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="af749-1247">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-1247">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="af749-1248">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="af749-1248">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="af749-1249">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="af749-1249">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="af749-1250">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="af749-1250">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="af749-1251">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-1251">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="af749-1252">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1252">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="af749-1253">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="af749-1253">Az.OperationalInsights</span></span>
- <span data-ttu-id="af749-1254">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1254">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="af749-1255">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="af749-1255">Az.Profile</span></span>
- <span data-ttu-id="af749-1256">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-1256">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="af749-1257">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-1257">Az.RecoveryServices</span></span>
- <span data-ttu-id="af749-1258">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1258">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="af749-1259">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1259">Az.Resources</span></span>
- <span data-ttu-id="af749-1260">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1260">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="af749-1261">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-1261">Az.ServiceFabric</span></span>
- <span data-ttu-id="af749-1262">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="af749-1262">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="af749-1263">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1263">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="af749-1264">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="af749-1264">Az.SIgnalR</span></span>
- <span data-ttu-id="af749-1265">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="af749-1265">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="af749-1266">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1266">Az.Sql</span></span>
- <span data-ttu-id="af749-1267">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1267">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="af749-1268">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1268">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="af749-1269">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1269">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="af749-1270">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-1270">Az.Storage</span></span>
- <span data-ttu-id="af749-1271">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1271">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="af749-1272">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-1272">Az.Websites</span></span>
- <span data-ttu-id="af749-1273">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="af749-1273">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="af749-1274">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="af749-1274">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="af749-1275">全般</span><span class="sxs-lookup"><span data-stu-id="af749-1275">General</span></span>

* <span data-ttu-id="af749-1276">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="af749-1276">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="af749-1277">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1277">Az.Compute</span></span>

* <span data-ttu-id="af749-1278">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1278">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="af749-1279">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1279">Az.DataLakeStore</span></span>

* <span data-ttu-id="af749-1280">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1280">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="af749-1281">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="af749-1281">Az.FrontDoor</span></span>

* <span data-ttu-id="af749-1282">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1282">Fixed some broken links</span></span>
    - <span data-ttu-id="af749-1283">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1283">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="af749-1284">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1284">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="af749-1285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="af749-1285">Az.RecoveryServices</span></span>

* <span data-ttu-id="af749-1286">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1286">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="af749-1287">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="af749-1287">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="af749-1288">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1288">Az.Resources</span></span>

* <span data-ttu-id="af749-1289">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1289">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="af749-1290">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1290">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="af749-1291">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1291">Az.Sql</span></span>

* <span data-ttu-id="af749-1292">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="af749-1292">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="af749-1293">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1293">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="af749-1294">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-1294">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="af749-1295">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-1295">Az.Storage</span></span>

* <span data-ttu-id="af749-1296">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1296">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="af749-1297">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1297">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="af749-1298">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="af749-1298">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="af749-1299">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="af749-1299">Support Static Website configuration</span></span>
    - <span data-ttu-id="af749-1300">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="af749-1300">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="af749-1301">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="af749-1301">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="af749-1302">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-1302">Az.Websites</span></span>

* <span data-ttu-id="af749-1303">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="af749-1303">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="af749-1304">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1304">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="af749-1305">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="af749-1305">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="af749-1306">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="af749-1306">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="af749-1307">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="af749-1307">Az.ApiManagement</span></span>
* <span data-ttu-id="af749-1308">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1308">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="af749-1309">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="af749-1309">Az.Automation</span></span>
* <span data-ttu-id="af749-1310">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="af749-1310">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="af749-1311">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1311">Added Update Management cmdlets</span></span>
* <span data-ttu-id="af749-1312">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1312">Added Source Control cmdlets</span></span>
* <span data-ttu-id="af749-1313">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1313">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="af749-1314">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1314">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="af749-1315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1315">Az.Compute</span></span>
* <span data-ttu-id="af749-1316">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1316">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="af749-1317">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1317">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="af749-1318">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="af749-1318">Az.ContainerInstance</span></span>
* <span data-ttu-id="af749-1319">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1319">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="af749-1320">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="af749-1320">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="af749-1321">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1321">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="af749-1322">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1322">Az.Network</span></span>
* <span data-ttu-id="af749-1323">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1323">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="af749-1324">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1324">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="af749-1325">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1325">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="af749-1326">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1326">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="af749-1327">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="af749-1327">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="af749-1328">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1328">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="af749-1329">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="af749-1329">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="af749-1330">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="af749-1330">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="af749-1331">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1331">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="af749-1332">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1332">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="af749-1333">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="af749-1333">Az.Relay</span></span>
* <span data-ttu-id="af749-1334">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="af749-1334">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="af749-1335">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1335">Az.Resources</span></span>
* <span data-ttu-id="af749-1336">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1336">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="af749-1337">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1337">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="af749-1338">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="af749-1338">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="af749-1339">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-1339">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-1340">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1340">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="af749-1341">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1341">Az.Sql</span></span>
* <span data-ttu-id="af749-1342">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1342">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="af749-1343">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="af749-1343">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="af749-1344">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="af749-1344">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="af749-1345">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="af749-1345">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="af749-1346">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="af749-1346">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="af749-1347">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="af749-1347">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="af749-1348">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="af749-1348">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="af749-1349">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="af749-1349">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="af749-1350">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="af749-1350">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="af749-1351">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="af749-1351">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="af749-1352">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1352">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="af749-1353">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="af749-1353">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="af749-1354">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="af749-1354">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="af749-1355">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="af749-1355">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="af749-1356">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="af749-1356">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="af749-1357">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="af749-1357">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="af749-1358">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1358">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="af749-1359">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="af749-1359">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="af749-1360">全般</span><span class="sxs-lookup"><span data-stu-id="af749-1360">General</span></span>
* <span data-ttu-id="af749-1361">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="af749-1361">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="af749-1362">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="af749-1362">Az.Profile</span></span>
* <span data-ttu-id="af749-1363">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1363">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="af749-1364">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1364">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="af749-1365">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="af749-1365">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="af749-1366">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1366">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="af749-1367">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1367">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="af749-1368">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1368">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="af749-1369">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1369">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="af749-1370">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="af749-1370">Az.CognitiveServices</span></span>
* <span data-ttu-id="af749-1371">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1371">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1372">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1372">Az.Compute</span></span>
* <span data-ttu-id="af749-1373">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1373">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="af749-1374">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="af749-1374">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="af749-1375">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1375">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-1376">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1376">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-1377">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="af749-1377">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="af749-1378">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1378">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="af749-1379">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="af749-1379">Az.Insights</span></span>
* <span data-ttu-id="af749-1380">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1380">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="af749-1381">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="af749-1381">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="af749-1382">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1382">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="af749-1383">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="af749-1383">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-1384">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1384">Az.Network</span></span>
* <span data-ttu-id="af749-1385">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="af749-1385">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="af749-1386">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="af749-1386">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="af749-1387">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="af749-1387">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="af749-1388">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="af749-1388">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="af749-1389">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="af749-1389">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="af749-1390">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="af749-1390">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="af749-1391">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="af749-1391">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="af749-1392">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="af749-1392">Az.PolicyInsights</span></span>
* <span data-ttu-id="af749-1393">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1393">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-1394">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1394">Az.Resources</span></span>
* <span data-ttu-id="af749-1395">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1395">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="af749-1396">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="af749-1396">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="af749-1397">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="af749-1397">Az.ServiceBus</span></span>
* <span data-ttu-id="af749-1398">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1398">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="af749-1399">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="af749-1399">Az.ServiceFabric</span></span>
* <span data-ttu-id="af749-1400">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1400">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="af749-1401">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1401">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="af749-1402">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="af749-1402">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="af749-1403">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="af749-1403">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="af749-1404">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1404">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="af749-1405">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="af749-1405">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="af749-1406">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="af749-1406">Az.Profile</span></span>
* <span data-ttu-id="af749-1407">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1407">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="af749-1408">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1408">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1409">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1409">Az.Compute</span></span>
* <span data-ttu-id="af749-1410">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1410">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="af749-1411">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1411">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="af749-1412">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="af749-1412">Az.DataLakeStore</span></span>
* <span data-ttu-id="af749-1413">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1413">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="af749-1414">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="af749-1414">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="af749-1415">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="af749-1415">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="af749-1416">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="af749-1416">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="af749-1417">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="af749-1417">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-1418">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1418">Az.Network</span></span>
* <span data-ttu-id="af749-1419">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1419">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="af749-1420">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1420">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-1421">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1421">Az.Resources</span></span>
* <span data-ttu-id="af749-1422">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1422">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="af749-1423">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1423">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="af749-1424">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="af749-1424">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="af749-1425">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="af749-1425">Azure.Storage</span></span>
* <span data-ttu-id="af749-1426">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1426">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="af749-1427">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="af749-1427">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="af749-1428">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="af749-1428">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="af749-1429">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1429">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="af749-1430">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="af749-1430">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="af749-1431">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="af749-1431">Az.CognitiveServices</span></span>
* <span data-ttu-id="af749-1432">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="af749-1432">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="af749-1433">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="af749-1433">Az.Compute</span></span>
* <span data-ttu-id="af749-1434">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1434">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="af749-1435">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1435">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="af749-1436">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1436">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="af749-1437">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="af749-1437">Az.DataFactoryV2</span></span>
* <span data-ttu-id="af749-1438">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1438">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="af749-1439">Az.Network</span><span class="sxs-lookup"><span data-stu-id="af749-1439">Az.Network</span></span>
* <span data-ttu-id="af749-1440">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="af749-1440">Added NetworkProfile functionality.</span></span> <span data-ttu-id="af749-1441">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="af749-1441">new cmdlets added</span></span>
    - <span data-ttu-id="af749-1442">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="af749-1442">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="af749-1443">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="af749-1443">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="af749-1444">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="af749-1444">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="af749-1445">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="af749-1445">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="af749-1446">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="af749-1446">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="af749-1447">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="af749-1447">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="af749-1448">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1448">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="af749-1449">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1449">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="af749-1450">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1450">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="af749-1451">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="af749-1451">Az.RedisCache</span></span>
* <span data-ttu-id="af749-1452">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="af749-1452">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="af749-1453">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1453">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="af749-1454">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="af749-1454">Az.Resources</span></span>
* <span data-ttu-id="af749-1455">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="af749-1455">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="af749-1456">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1456">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="af749-1457">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="af749-1457">Az.Sql</span></span>
* <span data-ttu-id="af749-1458">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="af749-1458">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="af749-1459">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="af749-1459">Az.Websites</span></span>
* <span data-ttu-id="af749-1460">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="af749-1460">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="af749-1461">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="af749-1461">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="af749-1462">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="af749-1462">0.2.0 - September 2018</span></span>
 <span data-ttu-id="af749-1463">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="af749-1463">Initial Release</span></span>