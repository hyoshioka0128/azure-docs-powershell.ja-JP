---
ms.openlocfilehash: 96e6d7bc0cc29adc1c0e49ba344d27349454c214
ms.sourcegitcommit: 92722d603b60dc769660e7517da60110133d9959
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2019
ms.locfileid: "71226441"
---
## <a name="270---september-2019"></a><span data-ttu-id="f7830-101">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="f7830-101">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="f7830-102">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f7830-102">Az.ApiManagement</span></span>
* <span data-ttu-id="f7830-103">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-103">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="f7830-104">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-104">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="f7830-105">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="f7830-105">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-106">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-106">Az.Automation</span></span>
* <span data-ttu-id="f7830-107">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-107">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="f7830-108">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-108">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="f7830-109">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-109">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-110">Az.Compute</span></span>
* <span data-ttu-id="f7830-111">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="f7830-111">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="f7830-112">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="f7830-112">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="f7830-113">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="f7830-113">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="f7830-114">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="f7830-114">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="f7830-115">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="f7830-115">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="f7830-116">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="f7830-116">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="f7830-117">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="f7830-117">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="f7830-118">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="f7830-118">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="f7830-119">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="f7830-119">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-120">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-120">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-121">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="f7830-121">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="f7830-122">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-122">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="f7830-123">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="f7830-123">Az.HDInsight</span></span>
* <span data-ttu-id="f7830-124">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="f7830-124">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="f7830-125">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="f7830-125">Az.IotHub</span></span>
* <span data-ttu-id="f7830-126">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="f7830-126">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="f7830-127">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="f7830-127">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="f7830-128">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f7830-128">New cmdlets are:</span></span>
    - <span data-ttu-id="f7830-129">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="f7830-129">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="f7830-130">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="f7830-130">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="f7830-131">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="f7830-131">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="f7830-132">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="f7830-132">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="f7830-133">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-133">Az.Monitor</span></span>
* <span data-ttu-id="f7830-134">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="f7830-134">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="f7830-135">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f7830-135">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="f7830-136">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="f7830-136">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="f7830-137">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="f7830-137">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="f7830-138">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-138">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="f7830-139">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-139">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="f7830-140">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="f7830-140">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="f7830-141">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="f7830-141">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="f7830-142">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-142">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="f7830-143">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="f7830-143">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="f7830-144">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-144">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="f7830-145">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="f7830-145">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="f7830-146">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-146">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="f7830-147">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="f7830-147">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="f7830-148">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="f7830-148">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="f7830-149">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="f7830-149">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="f7830-150">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="f7830-150">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="f7830-151">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="f7830-151">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="f7830-152">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-152">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="f7830-153">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="f7830-153">Overall improved help files</span></span>
* <span data-ttu-id="f7830-154">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="f7830-154">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-155">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-155">Az.Network</span></span>
* <span data-ttu-id="f7830-156">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="f7830-156">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="f7830-157">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="f7830-157">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="f7830-158">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="f7830-158">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="f7830-159">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="f7830-159">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="f7830-160">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="f7830-160">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="f7830-161">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-161">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="f7830-162">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-162">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="f7830-163">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-163">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="f7830-164">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-164">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="f7830-165">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-165">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="f7830-166">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-166">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="f7830-167">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-167">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="f7830-168">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-168">New cmdlets</span></span>
        - <span data-ttu-id="f7830-169">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="f7830-169">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="f7830-170">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-170">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="f7830-171">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="f7830-171">Updated cmdlet:</span></span>
        - <span data-ttu-id="f7830-172">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="f7830-172">New-VpnSite</span></span>
        - <span data-ttu-id="f7830-173">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="f7830-173">Update-VpnSite</span></span>
        - <span data-ttu-id="f7830-174">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-174">New-VpnConnection</span></span>
        - <span data-ttu-id="f7830-175">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-175">Update-VpnConnection</span></span>
* <span data-ttu-id="f7830-176">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-176">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-177">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-177">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-178">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-178">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="f7830-179">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-179">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-180">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-180">Az.Resources</span></span>
* <span data-ttu-id="f7830-181">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-181">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="f7830-182">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-182">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-183">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-183">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="f7830-184">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="f7830-184">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="f7830-185">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="f7830-185">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="f7830-186">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="f7830-186">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="f7830-187">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="f7830-187">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="f7830-188">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="f7830-188">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="f7830-189">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="f7830-189">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="f7830-190">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="f7830-190">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="f7830-191">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="f7830-191">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="f7830-192">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="f7830-192">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="f7830-193">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="f7830-193">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="f7830-194">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="f7830-194">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="f7830-195">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="f7830-195">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="f7830-196">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="f7830-196">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="f7830-197">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="f7830-197">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="f7830-198">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="f7830-198">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="f7830-199">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="f7830-199">Az.SignalR</span></span>
* <span data-ttu-id="f7830-200">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="f7830-200">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-201">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-201">Az.Sql</span></span>
* <span data-ttu-id="f7830-202">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="f7830-202">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="f7830-203">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-203">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="f7830-204">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="f7830-204">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="f7830-205">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-205">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="f7830-206">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="f7830-206">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-207">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-207">Az.Storage</span></span>
* <span data-ttu-id="f7830-208">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-208">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="f7830-209">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="f7830-209">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="f7830-210">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="f7830-210">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="f7830-211">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="f7830-211">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="f7830-212">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="f7830-212">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="f7830-213">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="f7830-213">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="f7830-214">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="f7830-214">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="f7830-215">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="f7830-215">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="f7830-216">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="f7830-216">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="f7830-217">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="f7830-217">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="f7830-218">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="f7830-218">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-219">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-219">Az.Websites</span></span>
* <span data-ttu-id="f7830-220">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="f7830-220">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="f7830-221">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="f7830-221">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="f7830-222">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="f7830-222">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="f7830-223">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="f7830-223">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="f7830-224">全般</span><span class="sxs-lookup"><span data-stu-id="f7830-224">General</span></span>
* <span data-ttu-id="f7830-225">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-225">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="f7830-226">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-226">Az.Accounts</span></span>
* <span data-ttu-id="f7830-227">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="f7830-227">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="f7830-228">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="f7830-228">Az.Aks</span></span>
* <span data-ttu-id="f7830-229">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-229">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="f7830-230">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="f7830-230">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="f7830-231">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f7830-231">Az.ApiManagement</span></span>
* <span data-ttu-id="f7830-232">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="f7830-232">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="f7830-233">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="f7830-233">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="f7830-234">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-234">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="f7830-235">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="f7830-235">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="f7830-236">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-236">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="f7830-237">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="f7830-237">Az.Batch</span></span>
* <span data-ttu-id="f7830-238">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-238">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="f7830-239">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="f7830-239">Az.Cdn</span></span>
* <span data-ttu-id="f7830-240">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-240">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-241">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-241">Az.Compute</span></span>
* <span data-ttu-id="f7830-242">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-242">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="f7830-243">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-243">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="f7830-244">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-244">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="f7830-245">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-245">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="f7830-246">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="f7830-246">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="f7830-247">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="f7830-247">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="f7830-248">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-248">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="f7830-249">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-249">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-250">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-250">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-251">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-251">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="f7830-252">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-252">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="f7830-253">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="f7830-253">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="f7830-254">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-254">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-255">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-255">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-256">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-256">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="f7830-257">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="f7830-257">Az.EventHub</span></span>
* <span data-ttu-id="f7830-258">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="f7830-258">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="f7830-259">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="f7830-259">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="f7830-260">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-260">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="f7830-261">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="f7830-261">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="f7830-262">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="f7830-262">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="f7830-263">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-263">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="f7830-264">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-264">Az.Monitor</span></span>
* <span data-ttu-id="f7830-265">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-265">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-266">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-266">Az.Network</span></span>
* <span data-ttu-id="f7830-267">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-267">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="f7830-268">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="f7830-268">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="f7830-269">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-269">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="f7830-270">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-270">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="f7830-271">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="f7830-271">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="f7830-272">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-272">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="f7830-273">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-273">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-274">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-274">Az.OperationalInsights</span></span>
* <span data-ttu-id="f7830-275">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-275">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="f7830-276">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-276">Added example</span></span>
    - <span data-ttu-id="f7830-277">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-277">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="f7830-278">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-278">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="f7830-279">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-279">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-280">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-280">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-281">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-281">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-282">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-282">Az.Resources</span></span>
* <span data-ttu-id="f7830-283">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-283">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="f7830-284">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-284">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="f7830-285">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="f7830-285">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="f7830-286">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-286">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f7830-287">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f7830-287">Az.ServiceBus</span></span>
* <span data-ttu-id="f7830-288">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="f7830-288">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="f7830-289">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="f7830-289">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="f7830-290">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-290">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="f7830-291">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-291">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-292">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-292">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="f7830-293">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="f7830-293">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="f7830-294">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="f7830-294">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="f7830-295">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-295">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="f7830-296">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="f7830-296">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="f7830-297">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-297">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-298">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-298">Az.Sql</span></span>
* <span data-ttu-id="f7830-299">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-299">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-300">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-300">Az.Storage</span></span>
* <span data-ttu-id="f7830-301">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-301">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="f7830-302">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="f7830-302">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="f7830-303">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="f7830-303">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="f7830-304">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="f7830-304">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="f7830-305">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="f7830-305">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="f7830-306">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="f7830-306">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-307">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-307">Az.Websites</span></span>
* <span data-ttu-id="f7830-308">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-308">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="f7830-309">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="f7830-309">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-310">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-310">Az.Accounts</span></span>
* <span data-ttu-id="f7830-311">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-311">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="f7830-312">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-312">Az.ApplicationInsights</span></span>
* <span data-ttu-id="f7830-313">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-313">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="f7830-314">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-314">Az.Automation</span></span>
* <span data-ttu-id="f7830-315">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-315">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="f7830-316">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f7830-316">Az.CognitiveServices</span></span>
* <span data-ttu-id="f7830-317">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-317">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-318">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-318">Az.Compute</span></span>
* <span data-ttu-id="f7830-319">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-319">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="f7830-320">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="f7830-320">Az.ContainerRegistry</span></span>
* <span data-ttu-id="f7830-321">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-321">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="f7830-322">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="f7830-322">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-323">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-323">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-324">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-324">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="f7830-325">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-325">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="f7830-326">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="f7830-326">Az.EventHub</span></span>
* <span data-ttu-id="f7830-327">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="f7830-327">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="f7830-328">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-328">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="f7830-329">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7830-329">Az.KeyVault</span></span>
* <span data-ttu-id="f7830-330">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-330">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="f7830-331">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="f7830-331">Az.LogicApp</span></span>
* <span data-ttu-id="f7830-332">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-332">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="f7830-333">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-333">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="f7830-334">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="f7830-334">Az.ManagedServices</span></span>
* <span data-ttu-id="f7830-335">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-335">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-336">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-336">Az.Network</span></span>
* <span data-ttu-id="f7830-337">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-337">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="f7830-338">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-338">New cmdlets</span></span>
        - <span data-ttu-id="f7830-339">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="f7830-339">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="f7830-340">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="f7830-340">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="f7830-341">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-341">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="f7830-342">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-342">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="f7830-343">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-343">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="f7830-344">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-344">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="f7830-345">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="f7830-345">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="f7830-346">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="f7830-346">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="f7830-347">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="f7830-347">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="f7830-348">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-348">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="f7830-349">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-349">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="f7830-350">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-350">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="f7830-351">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="f7830-351">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="f7830-352">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-352">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="f7830-353">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-353">Updated cmdlets</span></span>
        - <span data-ttu-id="f7830-354">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-354">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="f7830-355">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-355">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="f7830-356">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-356">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="f7830-357">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-357">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="f7830-358">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-358">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="f7830-359">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="f7830-359">Updated cmdlet:</span></span>
        - <span data-ttu-id="f7830-360">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-360">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="f7830-361">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-361">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="f7830-362">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-362">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="f7830-363">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="f7830-363">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="f7830-364">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-364">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="f7830-365">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f7830-365">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-366">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-366">Az.OperationalInsights</span></span>
* <span data-ttu-id="f7830-367">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-367">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="f7830-368">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-368">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-369">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-369">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-370">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-370">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="f7830-371">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-371">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="f7830-372">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-372">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="f7830-373">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-373">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="f7830-374">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-374">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="f7830-375">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-375">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="f7830-376">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-376">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="f7830-377">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-377">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="f7830-378">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-378">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="f7830-379">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-379">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-380">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-380">Az.Resources</span></span>
- <span data-ttu-id="f7830-381">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="f7830-381">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="f7830-382">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-382">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f7830-383">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f7830-383">Az.ServiceBus</span></span>
* <span data-ttu-id="f7830-384">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="f7830-384">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="f7830-385">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-385">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-386">Az.Sql</span></span>
* <span data-ttu-id="f7830-387">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-387">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="f7830-388">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-388">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="f7830-389">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-389">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-390">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-390">Az.Storage</span></span>
* <span data-ttu-id="f7830-391">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-391">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="f7830-392">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="f7830-392">Az.StorageSync</span></span>
* <span data-ttu-id="f7830-393">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-393">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="f7830-394">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-394">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-395">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-395">Az.Websites</span></span>
* <span data-ttu-id="f7830-396">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-396">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="f7830-397">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-397">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="f7830-398">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-398">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="f7830-399">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="f7830-399">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-400">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-400">Az.Accounts</span></span>
* <span data-ttu-id="f7830-401">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="f7830-401">Add support for profile cmdlets</span></span>
* <span data-ttu-id="f7830-402">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="f7830-402">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="f7830-403">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="f7830-403">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="f7830-404">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="f7830-404">Az.Advisor</span></span>
* <span data-ttu-id="f7830-405">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="f7830-405">GA release of Az.Advisor</span></span>
* <span data-ttu-id="f7830-406">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="f7830-406">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="f7830-407">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f7830-407">Az.ApiManagement</span></span>
* <span data-ttu-id="f7830-408">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="f7830-408">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="f7830-409">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="f7830-409">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="f7830-410">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-410">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="f7830-411">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-411">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="f7830-412">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-412">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="f7830-413">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="f7830-413">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="f7830-414">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-414">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-415">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-415">Az.Automation</span></span>
* <span data-ttu-id="f7830-416">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-416">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-417">Az.Compute</span></span>
* <span data-ttu-id="f7830-418">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="f7830-418">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-419">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-419">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-420">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="f7830-420">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="f7830-421">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f7830-421">Az.EventGrid</span></span>
* <span data-ttu-id="f7830-422">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-422">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="f7830-423">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="f7830-423">Az.IotHub</span></span>
* <span data-ttu-id="f7830-424">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-424">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-425">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-425">Az.Network</span></span>
* <span data-ttu-id="f7830-426">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-426">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="f7830-427">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="f7830-427">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="f7830-428">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-428">Az.PolicyInsights</span></span>
* <span data-ttu-id="f7830-429">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-429">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="f7830-430">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="f7830-430">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-431">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-431">Az.OperationalInsights</span></span>
* <span data-ttu-id="f7830-432">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-432">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-433">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-433">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-434">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-434">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-435">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-435">Az.Resources</span></span>
    - <span data-ttu-id="f7830-436">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-436">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="f7830-437">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-437">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="f7830-438">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-438">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="f7830-439">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-439">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f7830-440">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f7830-440">Az.ServiceBus</span></span>
* <span data-ttu-id="f7830-441">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="f7830-441">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-442">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-442">Az.Sql</span></span>
* <span data-ttu-id="f7830-443">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-443">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="f7830-444">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-444">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="f7830-445">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="f7830-445">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="f7830-446">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="f7830-446">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="f7830-447">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="f7830-447">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="f7830-448">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="f7830-448">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="f7830-449">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="f7830-449">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="f7830-450">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="f7830-450">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="f7830-451">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="f7830-451">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-452">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-452">Az.Storage</span></span>
* <span data-ttu-id="f7830-453">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-453">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="f7830-454">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="f7830-454">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="f7830-455">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-455">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="f7830-456">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="f7830-456">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="f7830-457">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-457">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="f7830-458">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-458">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="f7830-459">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-459">Set-AzStorageAccount</span></span>
* <span data-ttu-id="f7830-460">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-460">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="f7830-461">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="f7830-461">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="f7830-462">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="f7830-462">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="f7830-463">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="f7830-463">Az.StorageSync</span></span>
* <span data-ttu-id="f7830-464">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="f7830-464">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="f7830-465">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="f7830-465">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-466">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-466">Az.Accounts</span></span>
* <span data-ttu-id="f7830-467">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-467">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="f7830-468">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="f7830-468">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="f7830-469">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-469">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="f7830-470">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="f7830-470">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="f7830-471">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="f7830-471">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-472">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-472">Az.Compute</span></span>
* <span data-ttu-id="f7830-473">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-473">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="f7830-474">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-474">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="f7830-475">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="f7830-475">Az.Dns</span></span>
* <span data-ttu-id="f7830-476">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-476">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="f7830-477">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f7830-477">Az.EventGrid</span></span>
* <span data-ttu-id="f7830-478">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-478">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="f7830-479">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="f7830-479">New cmdlets:</span></span>
    - <span data-ttu-id="f7830-480">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="f7830-480">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="f7830-481">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="f7830-481">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="f7830-482">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="f7830-482">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="f7830-483">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f7830-483">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="f7830-484">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="f7830-484">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="f7830-485">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="f7830-485">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="f7830-486">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="f7830-486">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="f7830-487">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="f7830-487">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="f7830-488">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="f7830-488">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="f7830-489">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="f7830-489">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="f7830-490">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="f7830-490">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="f7830-491">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="f7830-491">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="f7830-492">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="f7830-492">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="f7830-493">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f7830-493">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="f7830-494">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="f7830-494">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="f7830-495">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="f7830-495">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="f7830-496">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="f7830-496">Updated cmdlets:</span></span>
    - <span data-ttu-id="f7830-497">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="f7830-497">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="f7830-498">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-498">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="f7830-499">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-499">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="f7830-500">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="f7830-500">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="f7830-501">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="f7830-501">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="f7830-502">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="f7830-502">Event subscription expiration date,</span></span>
            - <span data-ttu-id="f7830-503">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="f7830-503">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="f7830-504">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-504">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="f7830-505">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="f7830-505">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="f7830-506">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="f7830-506">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="f7830-507">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-507">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="f7830-508">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="f7830-508">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="f7830-509">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-509">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="f7830-510">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-510">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="f7830-511">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="f7830-511">Az.FrontDoor</span></span>
* <span data-ttu-id="f7830-512">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="f7830-512">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="f7830-513">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-513">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="f7830-514">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="f7830-514">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="f7830-515">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-515">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-516">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-516">Az.Network</span></span>
* <span data-ttu-id="f7830-517">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-517">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="f7830-518">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-518">New cmdlets</span></span>
        - <span data-ttu-id="f7830-519">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="f7830-519">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="f7830-520">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-520">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="f7830-521">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-521">New cmdlets</span></span> 
        - <span data-ttu-id="f7830-522">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="f7830-522">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="f7830-523">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-523">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="f7830-524">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-524">New cmdlets</span></span> 
        - <span data-ttu-id="f7830-525">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="f7830-525">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="f7830-526">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="f7830-526">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="f7830-527">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="f7830-527">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="f7830-528">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-528">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="f7830-529">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-529">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="f7830-530">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-530">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="f7830-531">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-531">New cmdlets</span></span>
        - <span data-ttu-id="f7830-532">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="f7830-532">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="f7830-533">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="f7830-533">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="f7830-534">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="f7830-534">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="f7830-535">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="f7830-535">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="f7830-536">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="f7830-536">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="f7830-537">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-537">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="f7830-538">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-538">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="f7830-539">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-539">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="f7830-540">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-540">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="f7830-541">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-541">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="f7830-542">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-542">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="f7830-543">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-543">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="f7830-544">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-544">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="f7830-545">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-545">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="f7830-546">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-546">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="f7830-547">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-547">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="f7830-548">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-548">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="f7830-549">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-549">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="f7830-550">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="f7830-550">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="f7830-551">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-551">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="f7830-552">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-552">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="f7830-553">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="f7830-553">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="f7830-554">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="f7830-554">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="f7830-555">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-555">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="f7830-556">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-556">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="f7830-557">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-557">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="f7830-558">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-558">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-559">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-559">Az.OperationalInsights</span></span>
* <span data-ttu-id="f7830-560">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="f7830-560">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-561">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-561">Az.Resources</span></span>
* <span data-ttu-id="f7830-562">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="f7830-562">Support for additional Template Export options</span></span>
    - <span data-ttu-id="f7830-563">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-563">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="f7830-564">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-564">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="f7830-565">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-565">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="f7830-566">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-566">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-567">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-567">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-568">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-568">Az.Sql</span></span>
* <span data-ttu-id="f7830-569">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-569">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="f7830-570">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-570">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="f7830-571">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="f7830-571">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="f7830-572">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="f7830-572">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="f7830-573">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="f7830-573">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="f7830-574">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="f7830-574">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="f7830-575">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="f7830-575">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="f7830-576">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="f7830-576">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-577">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-577">Az.Storage</span></span>
* <span data-ttu-id="f7830-578">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-578">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="f7830-579">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-579">New-AzStorageAccount</span></span>
* <span data-ttu-id="f7830-580">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="f7830-580">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="f7830-581">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="f7830-581">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-582">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-582">Az.Websites</span></span>
* <span data-ttu-id="f7830-583">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="f7830-583">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="f7830-584">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-584">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="f7830-585">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="f7830-585">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="f7830-586">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="f7830-586">Az.Cdn</span></span>
* <span data-ttu-id="f7830-587">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-587">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-588">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-588">Az.Compute</span></span>
* <span data-ttu-id="f7830-589">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-589">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="f7830-590">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="f7830-590">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="f7830-591">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="f7830-591">Az.EventHub</span></span>
* <span data-ttu-id="f7830-592">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-592">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="f7830-593">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-593">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-594">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-594">Az.Network</span></span>
* <span data-ttu-id="f7830-595">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-595">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="f7830-596">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-596">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="f7830-597">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-597">Az.PolicyInsights</span></span>
* <span data-ttu-id="f7830-598">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-598">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-599">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-599">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-600">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-600">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f7830-601">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f7830-601">Az.ServiceBus</span></span>
* <span data-ttu-id="f7830-602">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-602">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="f7830-603">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-603">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-604">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-604">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="f7830-605">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-605">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-606">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-606">Az.Sql</span></span>
* <span data-ttu-id="f7830-607">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-607">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="f7830-608">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="f7830-608">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="f7830-609">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-609">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="f7830-610">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-610">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-611">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-611">Az.Websites</span></span>
* <span data-ttu-id="f7830-612">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-612">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="f7830-613">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="f7830-613">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="f7830-614">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f7830-614">Az.ApiManagement</span></span>
* <span data-ttu-id="f7830-615">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="f7830-615">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="f7830-616">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="f7830-616">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="f7830-617">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="f7830-617">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="f7830-618">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="f7830-618">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="f7830-619">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="f7830-619">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="f7830-620">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="f7830-620">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="f7830-621">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="f7830-621">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="f7830-622">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="f7830-622">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="f7830-623">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="f7830-623">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="f7830-624">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="f7830-624">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="f7830-625">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="f7830-625">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="f7830-626">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="f7830-626">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="f7830-627">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="f7830-627">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="f7830-628">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-628">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="f7830-629">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="f7830-629">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="f7830-630">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="f7830-630">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="f7830-631">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="f7830-631">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="f7830-632">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="f7830-632">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="f7830-633">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-633">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="f7830-634">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="f7830-634">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="f7830-635">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="f7830-635">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="f7830-636">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="f7830-636">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="f7830-637">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="f7830-637">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="f7830-638">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-638">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="f7830-639">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-639">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="f7830-640">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-640">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="f7830-641">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="f7830-641">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="f7830-642">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="f7830-642">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="f7830-643">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-643">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="f7830-644">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-644">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="f7830-645">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-645">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="f7830-646">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="f7830-646">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="f7830-647">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-647">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="f7830-648">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-648">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="f7830-649">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="f7830-649">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="f7830-650">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="f7830-650">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="f7830-651">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="f7830-651">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="f7830-652">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-652">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="f7830-653">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-653">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="f7830-654">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-654">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="f7830-655">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="f7830-655">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="f7830-656">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="f7830-656">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="f7830-657">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="f7830-657">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="f7830-658">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-658">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="f7830-659">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-659">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="f7830-660">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="f7830-660">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="f7830-661">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="f7830-661">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="f7830-662">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-662">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="f7830-663">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-663">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="f7830-664">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="f7830-664">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="f7830-665">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="f7830-665">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="f7830-666">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="f7830-666">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="f7830-667">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="f7830-667">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="f7830-668">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-668">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="f7830-669">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="f7830-669">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="f7830-670">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="f7830-670">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="f7830-671">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-671">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="f7830-672">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="f7830-672">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="f7830-673">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="f7830-673">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="f7830-674">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-674">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="f7830-675">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-675">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="f7830-676">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="f7830-676">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="f7830-677">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="f7830-677">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="f7830-678">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-678">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="f7830-679">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-679">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="f7830-680">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="f7830-680">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="f7830-681">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="f7830-681">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="f7830-682">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="f7830-682">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="f7830-683">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="f7830-683">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="f7830-684">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="f7830-684">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="f7830-685">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="f7830-685">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="f7830-686">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="f7830-686">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="f7830-687">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="f7830-687">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="f7830-688">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="f7830-688">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="f7830-689">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="f7830-689">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="f7830-690">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="f7830-690">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="f7830-691">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="f7830-691">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-692">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-692">Az.Automation</span></span>
* <span data-ttu-id="f7830-693">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-693">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="f7830-694">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="f7830-694">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="f7830-695">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="f7830-695">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="f7830-696">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-696">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="f7830-697">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="f7830-697">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="f7830-698">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-698">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="f7830-699">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-699">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-700">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-700">Az.Compute</span></span>
* <span data-ttu-id="f7830-701">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-701">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="f7830-702">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="f7830-702">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-703">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-703">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-704">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-704">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="f7830-705">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-705">Az.Monitor</span></span>
* <span data-ttu-id="f7830-706">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-706">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-707">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-707">Az.Network</span></span>
* <span data-ttu-id="f7830-708">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-708">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="f7830-709">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="f7830-709">Updated cmdlet:</span></span>
        - <span data-ttu-id="f7830-710">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="f7830-710">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="f7830-711">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-711">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-712">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-712">Az.Resources</span></span>
* <span data-ttu-id="f7830-713">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-713">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-714">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-714">Az.Sql</span></span>
* <span data-ttu-id="f7830-715">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-715">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="f7830-716">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="f7830-716">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-717">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-717">Az.Accounts</span></span>
* <span data-ttu-id="f7830-718">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-718">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="f7830-719">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f7830-719">Az.CognitiveServices</span></span>
* <span data-ttu-id="f7830-720">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="f7830-720">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="f7830-721">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-721">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-722">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-722">Az.Compute</span></span>
* <span data-ttu-id="f7830-723">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="f7830-723">Proximity placement group feature.</span></span>
    - <span data-ttu-id="f7830-724">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="f7830-724">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="f7830-725">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-725">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="f7830-726">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-726">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="f7830-727">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-727">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="f7830-728">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-728">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="f7830-729">重大な変更</span><span class="sxs-lookup"><span data-stu-id="f7830-729">Breaking changes</span></span>
    - <span data-ttu-id="f7830-730">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="f7830-730">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="f7830-731">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="f7830-731">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="f7830-732">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="f7830-732">Az.DeploymentManager</span></span>
* <span data-ttu-id="f7830-733">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="f7830-733">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="f7830-734">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="f7830-734">Az.Dns</span></span>
* <span data-ttu-id="f7830-735">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="f7830-735">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="f7830-736">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="f7830-736">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="f7830-737">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-737">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="f7830-738">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="f7830-738">Az.FrontDoor</span></span>
* <span data-ttu-id="f7830-739">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="f7830-739">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="f7830-740">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="f7830-740">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="f7830-741">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="f7830-741">Az.HDInsight</span></span>
* <span data-ttu-id="f7830-742">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-742">Removed two cmdlets:</span></span>
    - <span data-ttu-id="f7830-743">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="f7830-743">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="f7830-744">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="f7830-744">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="f7830-745">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-745">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="f7830-746">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-746">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="f7830-747">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="f7830-747">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="f7830-748">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="f7830-748">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="f7830-749">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-749">Az.Monitor</span></span>
* <span data-ttu-id="f7830-750">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="f7830-750">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="f7830-751">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="f7830-751">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="f7830-752">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="f7830-752">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="f7830-753">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="f7830-753">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="f7830-754">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="f7830-754">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="f7830-755">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="f7830-755">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="f7830-756">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="f7830-756">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="f7830-757">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="f7830-757">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="f7830-758">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="f7830-758">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="f7830-759">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="f7830-759">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="f7830-760">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="f7830-760">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="f7830-761">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="f7830-761">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="f7830-762">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="f7830-762">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="f7830-763">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-763">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-764">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-764">Az.Network</span></span>
* <span data-ttu-id="f7830-765">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-765">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="f7830-766">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-766">New cmdlets</span></span>
        - <span data-ttu-id="f7830-767">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="f7830-767">New-AzNatGateway</span></span>
        - <span data-ttu-id="f7830-768">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="f7830-768">Get-AzNatGateway</span></span>
        - <span data-ttu-id="f7830-769">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="f7830-769">Set-AzNatGateway</span></span>
        - <span data-ttu-id="f7830-770">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="f7830-770">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="f7830-771">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-771">Updated cmdlets</span></span>
        - <span data-ttu-id="f7830-772">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="f7830-772">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="f7830-773">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="f7830-773">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="f7830-774">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="f7830-774">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="f7830-775">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-775">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="f7830-776">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-776">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="f7830-777">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-777">Az.PolicyInsights</span></span>
* <span data-ttu-id="f7830-778">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="f7830-778">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="f7830-779">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-779">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="f7830-780">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="f7830-780">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-781">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-781">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-782">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="f7830-782">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="f7830-783">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="f7830-783">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="f7830-784">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="f7830-784">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="f7830-785">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="f7830-785">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="f7830-786">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="f7830-786">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="f7830-787">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="f7830-787">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="f7830-788">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="f7830-788">Az.Relay</span></span>
* <span data-ttu-id="f7830-789">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-789">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f7830-790">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f7830-790">Az.ServiceBus</span></span>
* <span data-ttu-id="f7830-791">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-791">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-792">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-792">Az.Storage</span></span>
* <span data-ttu-id="f7830-793">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="f7830-793">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="f7830-794">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="f7830-794">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="f7830-795">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-795">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="f7830-796">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-796">New-AzStorageAccount</span></span>
* <span data-ttu-id="f7830-797">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="f7830-797">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="f7830-798">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-798">New-AzStorageAccount</span></span>
    - <span data-ttu-id="f7830-799">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-799">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="f7830-800">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="f7830-800">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-801">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-801">Az.Websites</span></span>
* <span data-ttu-id="f7830-802">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="f7830-802">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="f7830-803">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="f7830-803">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="f7830-804">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="f7830-804">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="f7830-805">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="f7830-805">Highlights since the last major release</span></span>
* <span data-ttu-id="f7830-806">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="f7830-806">General availability of `Az` module</span></span>
* <span data-ttu-id="f7830-807">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="f7830-807">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="f7830-808">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="f7830-808">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="f7830-809">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-809">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="f7830-810">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="f7830-810">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="f7830-811">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-811">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="f7830-812">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-812">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="f7830-813">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-813">Az.Accounts</span></span>
* <span data-ttu-id="f7830-814">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-814">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="f7830-815">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="f7830-815">Az.Batch</span></span>
* <span data-ttu-id="f7830-816">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-816">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="f7830-817">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="f7830-817">Az.Cdn</span></span>
* <span data-ttu-id="f7830-818">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-818">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="f7830-819">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f7830-819">Az.CognitiveServices</span></span>
* <span data-ttu-id="f7830-820">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-820">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-821">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-821">Az.Compute</span></span>
* <span data-ttu-id="f7830-822">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-822">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="f7830-823">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-823">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="f7830-824">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-824">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-825">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-825">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-826">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-826">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-827">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-827">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-828">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-828">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="f7830-829">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f7830-829">Az.EventGrid</span></span>
* <span data-ttu-id="f7830-830">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-830">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="f7830-831">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="f7830-831">Az.EventHub</span></span>
* <span data-ttu-id="f7830-832">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-832">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="f7830-833">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="f7830-833">Az.HDInsight</span></span>
* <span data-ttu-id="f7830-834">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-834">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="f7830-835">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="f7830-835">Az.IotHub</span></span>
* <span data-ttu-id="f7830-836">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-836">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="f7830-837">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7830-837">Az.KeyVault</span></span>
* <span data-ttu-id="f7830-838">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-838">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="f7830-839">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-839">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="f7830-840">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="f7830-840">Az.MachineLearning</span></span>
* <span data-ttu-id="f7830-841">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-841">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="f7830-842">Az.Media</span><span class="sxs-lookup"><span data-stu-id="f7830-842">Az.Media</span></span>
* <span data-ttu-id="f7830-843">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-843">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="f7830-844">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-844">Az.Monitor</span></span>
  * <span data-ttu-id="f7830-845">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-845">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="f7830-846">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="f7830-846">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="f7830-847">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="f7830-847">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="f7830-848">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="f7830-848">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="f7830-849">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="f7830-849">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="f7830-850">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="f7830-850">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="f7830-851">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-851">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-852">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-852">Az.Network</span></span>
* <span data-ttu-id="f7830-853">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-853">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="f7830-854">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-854">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="f7830-855">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="f7830-855">Az.NotificationHubs</span></span>
* <span data-ttu-id="f7830-856">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-856">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-857">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-857">Az.OperationalInsights</span></span>
* <span data-ttu-id="f7830-858">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-858">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="f7830-859">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="f7830-859">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="f7830-860">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-860">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-861">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-861">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-862">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-862">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="f7830-863">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-863">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="f7830-864">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-864">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="f7830-865">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-865">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="f7830-866">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="f7830-866">Az.RedisCache</span></span>
* <span data-ttu-id="f7830-867">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-867">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-868">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-868">Az.Resources</span></span>
* <span data-ttu-id="f7830-869">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-869">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-870">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-870">Az.Sql</span></span>
* <span data-ttu-id="f7830-871">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="f7830-871">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="f7830-872">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-872">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="f7830-873">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-873">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="f7830-874">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="f7830-874">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="f7830-875">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="f7830-875">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="f7830-876">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="f7830-876">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="f7830-877">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-877">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-878">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-878">Az.Websites</span></span>
* <span data-ttu-id="f7830-879">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-879">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="f7830-880">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-880">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="f7830-881">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-881">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="f7830-882">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-882">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="f7830-883">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="f7830-883">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="f7830-884">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="f7830-884">Highlights since the last major release</span></span>
* <span data-ttu-id="f7830-885">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="f7830-885">General availability of `Az` module</span></span>
* <span data-ttu-id="f7830-886">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="f7830-886">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="f7830-887">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="f7830-887">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="f7830-888">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-888">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="f7830-889">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="f7830-889">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="f7830-890">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-890">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="f7830-891">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-891">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="f7830-892">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-892">Az.Accounts</span></span>
* <span data-ttu-id="f7830-893">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-893">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="f7830-894">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f7830-894">Az.AnalysisServices</span></span>
* <span data-ttu-id="f7830-895">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="f7830-895">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="f7830-896">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="f7830-896">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-897">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-897">Az.Automation</span></span>
* <span data-ttu-id="f7830-898">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-898">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="f7830-899">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-899">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="f7830-900">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-900">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-901">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-901">Az.Compute</span></span>
* <span data-ttu-id="f7830-902">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-902">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="f7830-903">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-903">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="f7830-904">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-904">Az.ContainerInstance</span></span>
* <span data-ttu-id="f7830-905">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-905">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-906">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-906">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-907">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-907">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="f7830-908">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-908">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-909">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-909">Az.Resources</span></span>
* <span data-ttu-id="f7830-910">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="f7830-910">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="f7830-911">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="f7830-911">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="f7830-912">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="f7830-912">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="f7830-913">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="f7830-913">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="f7830-914">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-914">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="f7830-915">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="f7830-915">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-916">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-916">Az.Sql</span></span>
* <span data-ttu-id="f7830-917">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="f7830-917">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-918">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-918">Az.Storage</span></span>
* <span data-ttu-id="f7830-919">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="f7830-919">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="f7830-920">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="f7830-920">New-AzStorageContext</span></span>
* <span data-ttu-id="f7830-921">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="f7830-921">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="f7830-922">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="f7830-922">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="f7830-923">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="f7830-923">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="f7830-924">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="f7830-924">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="f7830-925">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="f7830-925">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="f7830-926">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="f7830-926">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="f7830-927">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="f7830-927">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="f7830-928">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="f7830-928">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="f7830-929">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="f7830-929">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="f7830-930">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="f7830-930">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="f7830-931">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="f7830-931">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="f7830-932">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="f7830-932">Highlights since the last major release</span></span>
* <span data-ttu-id="f7830-933">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="f7830-933">General availability of `Az` module</span></span>
* <span data-ttu-id="f7830-934">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="f7830-934">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="f7830-935">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="f7830-935">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="f7830-936">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-936">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="f7830-937">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="f7830-937">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="f7830-938">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-938">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="f7830-939">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-939">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-940">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-940">Az.Automation</span></span>
* <span data-ttu-id="f7830-941">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-941">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="f7830-942">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="f7830-942">Dynamic grouping</span></span>
    * <span data-ttu-id="f7830-943">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="f7830-943">Pre-Post script</span></span>
    * <span data-ttu-id="f7830-944">再起動設定</span><span class="sxs-lookup"><span data-stu-id="f7830-944">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-945">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-945">Az.Compute</span></span>
* <span data-ttu-id="f7830-946">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-946">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="f7830-947">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-947">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="f7830-948">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7830-948">Az.KeyVault</span></span>
* <span data-ttu-id="f7830-949">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-949">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-950">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-950">Az.Network</span></span>
* <span data-ttu-id="f7830-951">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-951">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="f7830-952">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-952">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-953">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-953">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-954">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-954">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="f7830-955">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-955">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-956">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-956">Az.Resources</span></span>
* <span data-ttu-id="f7830-957">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="f7830-957">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="f7830-958">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-958">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-959">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-959">Az.Sql</span></span>
* <span data-ttu-id="f7830-960">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-960">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-961">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-961">Az.Storage</span></span>
* <span data-ttu-id="f7830-962">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-962">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="f7830-963">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f7830-963">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="f7830-964">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f7830-964">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="f7830-965">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="f7830-965">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="f7830-966">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="f7830-966">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="f7830-967">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="f7830-967">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="f7830-968">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="f7830-968">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-969">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-969">Az.Websites</span></span>
* <span data-ttu-id="f7830-970">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-970">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="f7830-971">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="f7830-971">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-972">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-972">Az.Accounts</span></span>
* <span data-ttu-id="f7830-973">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-973">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="f7830-974">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-974">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-975">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-975">Az.Automation</span></span>
* <span data-ttu-id="f7830-976">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-976">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="f7830-977">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-977">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="f7830-978">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="f7830-978">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="f7830-979">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="f7830-979">Az.Cdn</span></span>
* <span data-ttu-id="f7830-980">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-980">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-981">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-981">Az.Compute</span></span>
* <span data-ttu-id="f7830-982">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-982">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-983">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-983">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-984">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-984">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="f7830-985">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="f7830-985">Az.LogicApp</span></span>
* <span data-ttu-id="f7830-986">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-986">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-987">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-987">Az.Network</span></span>
* <span data-ttu-id="f7830-988">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-988">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-989">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-989">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-990">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-990">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="f7830-991">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="f7830-991">SDK Update</span></span>
* <span data-ttu-id="f7830-992">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="f7830-992">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="f7830-993">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-993">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-994">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-994">Az.Resources</span></span>
* <span data-ttu-id="f7830-995">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-995">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="f7830-996">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="f7830-996">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="f7830-997">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-997">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="f7830-998">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="f7830-998">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="f7830-999">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-999">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="f7830-1000">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="f7830-1000">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-1001">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1001">Az.Sql</span></span>
* <span data-ttu-id="f7830-1002">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1002">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="f7830-1003">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1003">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-1004">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-1004">Az.Storage</span></span>
* <span data-ttu-id="f7830-1005">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="f7830-1005">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="f7830-1006">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1006">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="f7830-1007">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1007">Az.AnalysisServices</span></span>
* <span data-ttu-id="f7830-1008">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-1008">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-1009">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-1009">Az.Automation</span></span>
* <span data-ttu-id="f7830-1010">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1010">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="f7830-1011">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1011">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="f7830-1012">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1012">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="f7830-1013">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1013">Az.CognitiveServices</span></span>
* <span data-ttu-id="f7830-1014">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="f7830-1014">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1015">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1015">Az.Compute</span></span>
* <span data-ttu-id="f7830-1016">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1016">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="f7830-1017">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1017">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="f7830-1018">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1018">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="f7830-1019">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="f7830-1019">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1020">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1020">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-1021">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1021">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="f7830-1022">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="f7830-1022">Az.EventHub</span></span>
* <span data-ttu-id="f7830-1023">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1023">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="f7830-1024">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7830-1024">Az.KeyVault</span></span>
* <span data-ttu-id="f7830-1025">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1025">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="f7830-1026">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="f7830-1026">Az.LogicApp</span></span>
* <span data-ttu-id="f7830-1027">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1027">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="f7830-1028">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1028">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="f7830-1029">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-1029">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="f7830-1030">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="f7830-1030">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="f7830-1031">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="f7830-1031">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="f7830-1032">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="f7830-1032">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="f7830-1033">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="f7830-1033">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="f7830-1034">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-1034">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="f7830-1035">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7830-1035">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="f7830-1036">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7830-1036">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="f7830-1037">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7830-1037">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="f7830-1038">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7830-1038">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="f7830-1039">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1039">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="f7830-1040">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-1040">Az.Monitor</span></span>
* <span data-ttu-id="f7830-1041">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1041">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-1042">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1042">Az.Network</span></span>
* <span data-ttu-id="f7830-1043">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1043">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-1044">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-1044">Az.OperationalInsights</span></span>
* <span data-ttu-id="f7830-1045">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1045">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="f7830-1046">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1046">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="f7830-1047">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1047">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="f7830-1048">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1048">Az.Resources</span></span>
* <span data-ttu-id="f7830-1049">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="f7830-1049">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="f7830-1050">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="f7830-1050">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="f7830-1051">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="f7830-1051">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="f7830-1052">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1052">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-1053">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1053">Az.Sql</span></span>
* <span data-ttu-id="f7830-1054">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1054">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="f7830-1055">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1055">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-1056">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-1056">Az.Websites</span></span>
* <span data-ttu-id="f7830-1057">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1057">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="f7830-1058">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1058">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-1059">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-1059">Az.Accounts</span></span>
* <span data-ttu-id="f7830-1060">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1060">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="f7830-1061">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1061">Az.AnalysisServices</span></span>
<span data-ttu-id="f7830-1062">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="f7830-1062">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1063">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1063">Az.Compute</span></span>
* <span data-ttu-id="f7830-1064">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1064">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="f7830-1065">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1065">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="f7830-1066">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1066">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-1067">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1067">Az.RecoveryServices</span></span>
<span data-ttu-id="f7830-1068">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="f7830-1068">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-1069">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1069">Az.Resources</span></span>
* <span data-ttu-id="f7830-1070">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1070">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="f7830-1071">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="f7830-1071">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="f7830-1072">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1072">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="f7830-1073">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="f7830-1073">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-1074">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1074">Az.Sql</span></span>
* <span data-ttu-id="f7830-1075">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1075">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="f7830-1076">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1076">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="f7830-1077">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1077">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="f7830-1078">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1078">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-1079">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-1079">Az.Accounts</span></span>
* <span data-ttu-id="f7830-1080">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="f7830-1080">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="f7830-1081">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1081">Az.AnalysisServices</span></span>
* <span data-ttu-id="f7830-1082">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="f7830-1082">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-1083">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1083">Az.RecoveryServices</span></span>
* <span data-ttu-id="f7830-1084">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="f7830-1084">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="f7830-1085">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1085">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-1086">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-1086">Az.Accounts</span></span>
* <span data-ttu-id="f7830-1087">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1087">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="f7830-1088">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1088">Update incorrect online help URLs</span></span>
* <span data-ttu-id="f7830-1089">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1089">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="f7830-1090">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="f7830-1090">Az.Aks</span></span>
* <span data-ttu-id="f7830-1091">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1091">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="f7830-1092">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-1092">Az.Automation</span></span>
* <span data-ttu-id="f7830-1093">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1093">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="f7830-1094">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1094">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="f7830-1095">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="f7830-1095">Az.Cdn</span></span>
* <span data-ttu-id="f7830-1096">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1096">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1097">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1097">Az.Compute</span></span>
* <span data-ttu-id="f7830-1098">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1098">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="f7830-1099">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1099">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="f7830-1100">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1100">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="f7830-1101">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="f7830-1101">Az.ContainerRegistry</span></span>
* <span data-ttu-id="f7830-1102">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1102">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="f7830-1103">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="f7830-1103">Az.DataFactory</span></span>
* <span data-ttu-id="f7830-1104">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1104">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1105">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1105">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-1106">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="f7830-1106">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="f7830-1107">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="f7830-1107">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="f7830-1108">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1108">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="f7830-1109">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="f7830-1109">Az.IotHub</span></span>
* <span data-ttu-id="f7830-1110">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1110">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="f7830-1111">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7830-1111">Az.KeyVault</span></span>
* <span data-ttu-id="f7830-1112">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1112">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-1113">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1113">Az.Network</span></span>
* <span data-ttu-id="f7830-1114">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1114">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-1115">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1115">Az.Resources</span></span>
* <span data-ttu-id="f7830-1116">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1116">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="f7830-1117">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1117">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="f7830-1118">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1118">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="f7830-1119">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="f7830-1119">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="f7830-1120">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="f7830-1120">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="f7830-1121">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1121">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="f7830-1122">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="f7830-1122">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="f7830-1123">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-1123">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-1124">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="f7830-1124">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="f7830-1125">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1125">Fix some error messages.</span></span>
* <span data-ttu-id="f7830-1126">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1126">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="f7830-1127">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1127">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="f7830-1128">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="f7830-1128">Az.SignalR</span></span>
* <span data-ttu-id="f7830-1129">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1129">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-1130">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1130">Az.Sql</span></span>
* <span data-ttu-id="f7830-1131">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1131">Update incorrect online help URLs</span></span>
* <span data-ttu-id="f7830-1132">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1132">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="f7830-1133">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1133">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="f7830-1134">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-1134">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-1135">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-1135">Az.Storage</span></span>
* <span data-ttu-id="f7830-1136">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1136">Update incorrect online help URLs</span></span>
* <span data-ttu-id="f7830-1137">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="f7830-1137">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="f7830-1138">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="f7830-1138">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="f7830-1139">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="f7830-1139">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="f7830-1140">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="f7830-1140">Az.TrafficManager</span></span>
* <span data-ttu-id="f7830-1141">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1141">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-1142">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-1142">Az.Websites</span></span>
* <span data-ttu-id="f7830-1143">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1143">Update incorrect online help URLs</span></span>
* <span data-ttu-id="f7830-1144">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1144">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="f7830-1145">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="f7830-1145">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="f7830-1146">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1146">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="f7830-1147">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-1147">Az.Accounts</span></span>
* <span data-ttu-id="f7830-1148">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="f7830-1148">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1149">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1149">Az.Compute</span></span>
* <span data-ttu-id="f7830-1150">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1150">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="f7830-1151">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="f7830-1151">Updated the description of ID in help files</span></span>
* <span data-ttu-id="f7830-1152">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1152">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1153">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1153">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-1154">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1154">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="f7830-1155">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1155">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="f7830-1156">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="f7830-1156">Az.EventGrid</span></span>
* <span data-ttu-id="f7830-1157">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1157">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="f7830-1158">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="f7830-1158">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="f7830-1159">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="f7830-1159">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="f7830-1160">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="f7830-1160">Event Time-To-Live,</span></span>
        - <span data-ttu-id="f7830-1161">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="f7830-1161">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="f7830-1162">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="f7830-1162">Dead letter endpoint.</span></span>
    - <span data-ttu-id="f7830-1163">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="f7830-1163">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="f7830-1164">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="f7830-1164">Event Time-To-Live,</span></span>
        - <span data-ttu-id="f7830-1165">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="f7830-1165">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="f7830-1166">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="f7830-1166">Dead letter endpoint.</span></span>
* <span data-ttu-id="f7830-1167">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1167">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="f7830-1168">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="f7830-1168">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="f7830-1169">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="f7830-1169">Az.IotHub</span></span>
* <span data-ttu-id="f7830-1170">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1170">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="f7830-1171">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="f7830-1171">Az.LogicApp</span></span>
* <span data-ttu-id="f7830-1172">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="f7830-1172">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-1173">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1173">Az.Resources</span></span>
* <span data-ttu-id="f7830-1174">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1174">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="f7830-1175">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="f7830-1175">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="f7830-1176">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1176">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="f7830-1177">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1177">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="f7830-1178">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="f7830-1178">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="f7830-1179">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="f7830-1179">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="f7830-1180">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="f7830-1180">Az.SignalR</span></span>
* <span data-ttu-id="f7830-1181">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1181">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-1182">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1182">Az.Sql</span></span>
* <span data-ttu-id="f7830-1183">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1183">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="f7830-1184">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-1184">Az.Storage</span></span>
* <span data-ttu-id="f7830-1185">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="f7830-1185">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="f7830-1186">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="f7830-1186">New-AzStorageContext</span></span>
* <span data-ttu-id="f7830-1187">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1187">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="f7830-1188">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="f7830-1188">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-1189">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-1189">Az.Websites</span></span>
* <span data-ttu-id="f7830-1190">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1190">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="f7830-1191">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1191">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="f7830-1192">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1192">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="f7830-1193">全般</span><span class="sxs-lookup"><span data-stu-id="f7830-1193">General</span></span>

- <span data-ttu-id="f7830-1194">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="f7830-1194">General Availability of Az Module</span></span>
- <span data-ttu-id="f7830-1195">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="f7830-1195">Online help for each module</span></span>
- <span data-ttu-id="f7830-1196">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1196">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="f7830-1197">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1197">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="f7830-1198">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="f7830-1198">Az.Accounts</span></span>
- <span data-ttu-id="f7830-1199">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1199">Changed from Az.Profile</span></span>
- <span data-ttu-id="f7830-1200">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1200">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="f7830-1201">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f7830-1201">Az.ApiManagement</span></span>
- <span data-ttu-id="f7830-1202">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="f7830-1202">Fixes for #7002</span></span>
- <span data-ttu-id="f7830-1203">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1203">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="f7830-1204">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="f7830-1204">Az.Batch</span></span>
- <span data-ttu-id="f7830-1205">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1205">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="f7830-1206">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1206">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="f7830-1207">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1207">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="f7830-1208">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="f7830-1208">Az.Billing</span></span>
- <span data-ttu-id="f7830-1209">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1209">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="f7830-1210">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1210">Az.CognitivServices</span></span>
- <span data-ttu-id="f7830-1211">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1211">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="f7830-1212">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1212">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="f7830-1213">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-1213">Az.ContainerInstance</span></span>
- <span data-ttu-id="f7830-1214">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1214">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="f7830-1215">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="f7830-1215">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="f7830-1216">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1216">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1217">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1217">Az.DataLakeStore</span></span>
- <span data-ttu-id="f7830-1218">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1218">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="f7830-1219">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="f7830-1219">Az.Monitor</span></span>
- <span data-ttu-id="f7830-1220">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1220">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="f7830-1221">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="f7830-1221">Az.KeyVault</span></span>
- <span data-ttu-id="f7830-1222">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1222">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="f7830-1223">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="f7830-1223">Az.MachineLearning</span></span>
- <span data-ttu-id="f7830-1224">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="f7830-1224">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="f7830-1225">Az.Media</span><span class="sxs-lookup"><span data-stu-id="f7830-1225">Az.Media</span></span>
- <span data-ttu-id="f7830-1226">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1226">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="f7830-1227">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1227">Az.Network</span></span>
<span data-ttu-id="f7830-1228">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1228">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="f7830-1229">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="f7830-1229">New cmdlets added:</span></span>
        - <span data-ttu-id="f7830-1230">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f7830-1230">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f7830-1231">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f7830-1231">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f7830-1232">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f7830-1232">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f7830-1233">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f7830-1233">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f7830-1234">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="f7830-1234">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="f7830-1235">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="f7830-1235">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="f7830-1236">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="f7830-1236">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="f7830-1237">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7830-1237">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="f7830-1238">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-1238">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="f7830-1239">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="f7830-1239">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="f7830-1240">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="f7830-1240">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="f7830-1241">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="f7830-1241">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="f7830-1242">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-1242">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="f7830-1243">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-1243">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="f7830-1244">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1244">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="f7830-1245">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-1245">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="f7830-1246">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="f7830-1246">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="f7830-1247">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="f7830-1247">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="f7830-1248">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="f7830-1248">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="f7830-1249">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-1249">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="f7830-1250">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1250">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="f7830-1251">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-1251">Az.OperationalInsights</span></span>
- <span data-ttu-id="f7830-1252">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1252">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="f7830-1253">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f7830-1253">Az.Profile</span></span>
- <span data-ttu-id="f7830-1254">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1254">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-1255">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1255">Az.RecoveryServices</span></span>
- <span data-ttu-id="f7830-1256">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1256">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="f7830-1257">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1257">Az.Resources</span></span>
- <span data-ttu-id="f7830-1258">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1258">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="f7830-1259">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-1259">Az.ServiceFabric</span></span>
- <span data-ttu-id="f7830-1260">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="f7830-1260">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="f7830-1261">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1261">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="f7830-1262">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="f7830-1262">Az.SIgnalR</span></span>
- <span data-ttu-id="f7830-1263">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="f7830-1263">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="f7830-1264">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1264">Az.Sql</span></span>
- <span data-ttu-id="f7830-1265">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1265">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="f7830-1266">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1266">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="f7830-1267">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1267">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="f7830-1268">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-1268">Az.Storage</span></span>
- <span data-ttu-id="f7830-1269">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1269">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="f7830-1270">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-1270">Az.Websites</span></span>
- <span data-ttu-id="f7830-1271">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="f7830-1271">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="f7830-1272">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1272">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="f7830-1273">全般</span><span class="sxs-lookup"><span data-stu-id="f7830-1273">General</span></span>

* <span data-ttu-id="f7830-1274">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="f7830-1274">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="f7830-1275">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1275">Az.Compute</span></span>

* <span data-ttu-id="f7830-1276">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1276">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1277">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1277">Az.DataLakeStore</span></span>

* <span data-ttu-id="f7830-1278">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1278">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="f7830-1279">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="f7830-1279">Az.FrontDoor</span></span>

* <span data-ttu-id="f7830-1280">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1280">Fixed some broken links</span></span>
    - <span data-ttu-id="f7830-1281">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1281">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="f7830-1282">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1282">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="f7830-1283">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1283">Az.RecoveryServices</span></span>

* <span data-ttu-id="f7830-1284">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1284">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="f7830-1285">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1285">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="f7830-1286">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1286">Az.Resources</span></span>

* <span data-ttu-id="f7830-1287">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1287">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="f7830-1288">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1288">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="f7830-1289">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1289">Az.Sql</span></span>

* <span data-ttu-id="f7830-1290">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="f7830-1290">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="f7830-1291">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1291">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="f7830-1292">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1292">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="f7830-1293">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-1293">Az.Storage</span></span>

* <span data-ttu-id="f7830-1294">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1294">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="f7830-1295">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1295">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="f7830-1296">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="f7830-1296">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="f7830-1297">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="f7830-1297">Support Static Website configuration</span></span>
    - <span data-ttu-id="f7830-1298">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="f7830-1298">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="f7830-1299">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="f7830-1299">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="f7830-1300">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-1300">Az.Websites</span></span>

* <span data-ttu-id="f7830-1301">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="f7830-1301">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="f7830-1302">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1302">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="f7830-1303">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="f7830-1303">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="f7830-1304">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1304">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="f7830-1305">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="f7830-1305">Az.ApiManagement</span></span>
* <span data-ttu-id="f7830-1306">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1306">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="f7830-1307">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="f7830-1307">Az.Automation</span></span>
* <span data-ttu-id="f7830-1308">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="f7830-1308">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="f7830-1309">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1309">Added Update Management cmdlets</span></span>
* <span data-ttu-id="f7830-1310">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1310">Added Source Control cmdlets</span></span>
* <span data-ttu-id="f7830-1311">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1311">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="f7830-1312">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1312">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="f7830-1313">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1313">Az.Compute</span></span>
* <span data-ttu-id="f7830-1314">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1314">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="f7830-1315">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1315">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="f7830-1316">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-1316">Az.ContainerInstance</span></span>
* <span data-ttu-id="f7830-1317">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1317">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="f7830-1318">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="f7830-1318">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="f7830-1319">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1319">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="f7830-1320">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1320">Az.Network</span></span>
* <span data-ttu-id="f7830-1321">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1321">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="f7830-1322">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1322">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="f7830-1323">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1323">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="f7830-1324">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1324">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="f7830-1325">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="f7830-1325">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="f7830-1326">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1326">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="f7830-1327">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1327">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="f7830-1328">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="f7830-1328">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="f7830-1329">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1329">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="f7830-1330">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1330">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="f7830-1331">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="f7830-1331">Az.Relay</span></span>
* <span data-ttu-id="f7830-1332">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="f7830-1332">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="f7830-1333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1333">Az.Resources</span></span>
* <span data-ttu-id="f7830-1334">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1334">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="f7830-1335">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1335">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="f7830-1336">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="f7830-1336">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="f7830-1337">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-1337">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-1338">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1338">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="f7830-1339">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1339">Az.Sql</span></span>
* <span data-ttu-id="f7830-1340">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1340">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="f7830-1341">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-1341">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f7830-1342">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-1342">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f7830-1343">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-1343">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f7830-1344">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="f7830-1344">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="f7830-1345">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f7830-1345">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="f7830-1346">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f7830-1346">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="f7830-1347">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f7830-1347">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="f7830-1348">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="f7830-1348">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="f7830-1349">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="f7830-1349">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="f7830-1350">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1350">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="f7830-1351">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1351">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="f7830-1352">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="f7830-1352">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="f7830-1353">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="f7830-1353">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="f7830-1354">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="f7830-1354">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="f7830-1355">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="f7830-1355">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="f7830-1356">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1356">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="f7830-1357">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1357">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="f7830-1358">全般</span><span class="sxs-lookup"><span data-stu-id="f7830-1358">General</span></span>
* <span data-ttu-id="f7830-1359">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="f7830-1359">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="f7830-1360">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f7830-1360">Az.Profile</span></span>
* <span data-ttu-id="f7830-1361">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1361">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="f7830-1362">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1362">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="f7830-1363">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1363">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="f7830-1364">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1364">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="f7830-1365">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1365">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="f7830-1366">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1366">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="f7830-1367">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1367">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="f7830-1368">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1368">Az.CognitiveServices</span></span>
* <span data-ttu-id="f7830-1369">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1369">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1370">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1370">Az.Compute</span></span>
* <span data-ttu-id="f7830-1371">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1371">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="f7830-1372">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="f7830-1372">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="f7830-1373">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1373">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1374">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1374">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-1375">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1375">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="f7830-1376">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1376">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="f7830-1377">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="f7830-1377">Az.Insights</span></span>
* <span data-ttu-id="f7830-1378">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1378">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="f7830-1379">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="f7830-1379">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="f7830-1380">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1380">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="f7830-1381">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="f7830-1381">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-1382">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1382">Az.Network</span></span>
* <span data-ttu-id="f7830-1383">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="f7830-1383">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="f7830-1384">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="f7830-1384">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="f7830-1385">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="f7830-1385">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="f7830-1386">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="f7830-1386">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="f7830-1387">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="f7830-1387">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="f7830-1388">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="f7830-1388">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="f7830-1389">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="f7830-1389">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="f7830-1390">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="f7830-1390">Az.PolicyInsights</span></span>
* <span data-ttu-id="f7830-1391">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1391">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-1392">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1392">Az.Resources</span></span>
* <span data-ttu-id="f7830-1393">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1393">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="f7830-1394">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1394">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="f7830-1395">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="f7830-1395">Az.ServiceBus</span></span>
* <span data-ttu-id="f7830-1396">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1396">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="f7830-1397">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="f7830-1397">Az.ServiceFabric</span></span>
* <span data-ttu-id="f7830-1398">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1398">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="f7830-1399">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1399">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="f7830-1400">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="f7830-1400">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="f7830-1401">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="f7830-1401">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="f7830-1402">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1402">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="f7830-1403">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1403">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="f7830-1404">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="f7830-1404">Az.Profile</span></span>
* <span data-ttu-id="f7830-1405">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1405">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="f7830-1406">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1406">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1407">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1407">Az.Compute</span></span>
* <span data-ttu-id="f7830-1408">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1408">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="f7830-1409">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1409">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="f7830-1410">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="f7830-1410">Az.DataLakeStore</span></span>
* <span data-ttu-id="f7830-1411">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1411">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="f7830-1412">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="f7830-1412">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="f7830-1413">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="f7830-1413">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="f7830-1414">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="f7830-1414">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="f7830-1415">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="f7830-1415">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-1416">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1416">Az.Network</span></span>
* <span data-ttu-id="f7830-1417">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1417">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="f7830-1418">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1418">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-1419">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1419">Az.Resources</span></span>
* <span data-ttu-id="f7830-1420">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1420">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="f7830-1421">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1421">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="f7830-1422">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1422">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="f7830-1423">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="f7830-1423">Azure.Storage</span></span>
* <span data-ttu-id="f7830-1424">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1424">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="f7830-1425">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="f7830-1425">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="f7830-1426">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="f7830-1426">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="f7830-1427">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1427">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="f7830-1428">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="f7830-1428">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="f7830-1429">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="f7830-1429">Az.CognitiveServices</span></span>
* <span data-ttu-id="f7830-1430">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1430">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="f7830-1431">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="f7830-1431">Az.Compute</span></span>
* <span data-ttu-id="f7830-1432">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1432">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="f7830-1433">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1433">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="f7830-1434">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1434">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="f7830-1435">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="f7830-1435">Az.DataFactoryV2</span></span>
* <span data-ttu-id="f7830-1436">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1436">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="f7830-1437">Az.Network</span><span class="sxs-lookup"><span data-stu-id="f7830-1437">Az.Network</span></span>
* <span data-ttu-id="f7830-1438">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="f7830-1438">Added NetworkProfile functionality.</span></span> <span data-ttu-id="f7830-1439">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="f7830-1439">new cmdlets added</span></span>
    - <span data-ttu-id="f7830-1440">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f7830-1440">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="f7830-1441">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f7830-1441">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="f7830-1442">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f7830-1442">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="f7830-1443">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="f7830-1443">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="f7830-1444">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-1444">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="f7830-1445">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="f7830-1445">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="f7830-1446">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1446">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="f7830-1447">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1447">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="f7830-1448">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1448">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="f7830-1449">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="f7830-1449">Az.RedisCache</span></span>
* <span data-ttu-id="f7830-1450">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="f7830-1450">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="f7830-1451">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1451">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="f7830-1452">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="f7830-1452">Az.Resources</span></span>
* <span data-ttu-id="f7830-1453">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1453">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="f7830-1454">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1454">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="f7830-1455">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="f7830-1455">Az.Sql</span></span>
* <span data-ttu-id="f7830-1456">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="f7830-1456">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="f7830-1457">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="f7830-1457">Az.Websites</span></span>
* <span data-ttu-id="f7830-1458">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="f7830-1458">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="f7830-1459">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="f7830-1459">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="f7830-1460">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="f7830-1460">0.2.0 - September 2018</span></span>
 <span data-ttu-id="f7830-1461">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="f7830-1461">Initial Release</span></span>