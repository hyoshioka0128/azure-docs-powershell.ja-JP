---
ms.openlocfilehash: 3848f7fb8e298d137c747405f32a0776c1a8f029
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048633"
---
## <a name="200---may-2019"></a><span data-ttu-id="96af7-101">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="96af7-101">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="96af7-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-102">Az.Accounts</span></span>
* <span data-ttu-id="96af7-103">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-103">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="96af7-104">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="96af7-104">Az.CognitiveServices</span></span>
* <span data-ttu-id="96af7-105">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="96af7-105">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="96af7-106">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-106">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-107">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-107">Az.Compute</span></span>
* <span data-ttu-id="96af7-108">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="96af7-108">Proximity placement group feature.</span></span>
    - <span data-ttu-id="96af7-109">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="96af7-109">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="96af7-110">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="96af7-110">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="96af7-111">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-111">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="96af7-112">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-112">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="96af7-113">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-113">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="96af7-114">重大な変更</span><span class="sxs-lookup"><span data-stu-id="96af7-114">Breaking changes</span></span>
    - <span data-ttu-id="96af7-115">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="96af7-115">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="96af7-116">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="96af7-116">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="96af7-117">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="96af7-117">Az.DeploymentManager</span></span>
* <span data-ttu-id="96af7-118">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="96af7-118">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="96af7-119">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="96af7-119">Az.Dns</span></span>
* <span data-ttu-id="96af7-120">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="96af7-120">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="96af7-121">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="96af7-121">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="96af7-122">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-122">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="96af7-123">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="96af7-123">Az.FrontDoor</span></span>
* <span data-ttu-id="96af7-124">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="96af7-124">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="96af7-125">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="96af7-125">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="96af7-126">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="96af7-126">Az.HDInsight</span></span>
* <span data-ttu-id="96af7-127">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-127">Removed two cmdlets:</span></span>
    - <span data-ttu-id="96af7-128">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="96af7-128">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="96af7-129">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="96af7-129">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="96af7-130">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-130">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="96af7-131">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-131">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="96af7-132">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="96af7-132">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="96af7-133">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="96af7-133">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="96af7-134">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="96af7-134">Az.Monitor</span></span>
* <span data-ttu-id="96af7-135">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="96af7-135">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="96af7-136">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="96af7-136">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="96af7-137">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="96af7-137">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="96af7-138">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="96af7-138">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="96af7-139">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="96af7-139">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="96af7-140">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="96af7-140">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="96af7-141">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="96af7-141">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="96af7-142">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="96af7-142">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="96af7-143">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="96af7-143">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="96af7-144">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="96af7-144">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="96af7-145">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="96af7-145">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="96af7-146">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="96af7-146">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="96af7-147">SQR API に関する[詳細](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="96af7-147">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="96af7-148">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-148">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-149">Az.Network</span></span>
* <span data-ttu-id="96af7-150">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-150">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="96af7-151">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-151">New cmdlets</span></span>
        - <span data-ttu-id="96af7-152">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="96af7-152">New-AzNatGateway</span></span>
        - <span data-ttu-id="96af7-153">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="96af7-153">Get-AzNatGateway</span></span>
        - <span data-ttu-id="96af7-154">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="96af7-154">Set-AzNatGateway</span></span>
        - <span data-ttu-id="96af7-155">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="96af7-155">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="96af7-156">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-156">Updated cmdlets</span></span>
        - <span data-ttu-id="96af7-157">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="96af7-157">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="96af7-158">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="96af7-158">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="96af7-159">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="96af7-159">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="96af7-160">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-160">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="96af7-161">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-161">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="96af7-162">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="96af7-162">Az.PolicyInsights</span></span>
* <span data-ttu-id="96af7-163">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="96af7-163">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="96af7-164">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-164">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="96af7-165">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="96af7-165">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-166">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-166">Az.RecoveryServices</span></span>
* <span data-ttu-id="96af7-167">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="96af7-167">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="96af7-168">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="96af7-168">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="96af7-169">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="96af7-169">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="96af7-170">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="96af7-170">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="96af7-171">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="96af7-171">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="96af7-172">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="96af7-172">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="96af7-173">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="96af7-173">Az.Relay</span></span>
* <span data-ttu-id="96af7-174">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-174">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="96af7-175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96af7-175">Az.ServiceBus</span></span>
* <span data-ttu-id="96af7-176">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-176">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="96af7-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-177">Az.Storage</span></span>
* <span data-ttu-id="96af7-178">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage.*" から "Microsoft.Azure.Storage.*" に変更されています)</span><span class="sxs-lookup"><span data-stu-id="96af7-178">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="96af7-179">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="96af7-179">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="96af7-180">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="96af7-180">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="96af7-181">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96af7-181">New-AzStorageAccount</span></span>
* <span data-ttu-id="96af7-182">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="96af7-182">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="96af7-183">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96af7-183">New-AzStorageAccount</span></span>
    - <span data-ttu-id="96af7-184">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96af7-184">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="96af7-185">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96af7-185">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-186">Az.Websites</span></span>
* <span data-ttu-id="96af7-187">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="96af7-187">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="96af7-188">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="96af7-188">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="96af7-189">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="96af7-189">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="96af7-190">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="96af7-190">Highlights since the last major release</span></span>
* <span data-ttu-id="96af7-191">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="96af7-191">General availability of `Az` module</span></span>
* <span data-ttu-id="96af7-192">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="96af7-192">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="96af7-193">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="96af7-193">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="96af7-194">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-194">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="96af7-195">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="96af7-195">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="96af7-196">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-196">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="96af7-197">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-197">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="96af7-198">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-198">Az.Accounts</span></span>
* <span data-ttu-id="96af7-199">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-199">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="96af7-200">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="96af7-200">Az.Batch</span></span>
* <span data-ttu-id="96af7-201">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-201">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="96af7-202">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="96af7-202">Az.Cdn</span></span>
* <span data-ttu-id="96af7-203">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-203">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="96af7-204">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="96af7-204">Az.CognitiveServices</span></span>
* <span data-ttu-id="96af7-205">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-205">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-206">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-206">Az.Compute</span></span>
* <span data-ttu-id="96af7-207">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-207">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="96af7-208">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-208">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="96af7-209">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-209">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="96af7-210">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="96af7-210">Az.DataFactory</span></span>
* <span data-ttu-id="96af7-211">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-211">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="96af7-212">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-212">Az.DataLakeStore</span></span>
* <span data-ttu-id="96af7-213">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-213">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="96af7-214">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="96af7-214">Az.EventGrid</span></span>
* <span data-ttu-id="96af7-215">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-215">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="96af7-216">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="96af7-216">Az.EventHub</span></span>
* <span data-ttu-id="96af7-217">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-217">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="96af7-218">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="96af7-218">Az.HDInsight</span></span>
* <span data-ttu-id="96af7-219">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-219">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="96af7-220">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="96af7-220">Az.IotHub</span></span>
* <span data-ttu-id="96af7-221">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-221">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="96af7-222">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96af7-222">Az.KeyVault</span></span>
* <span data-ttu-id="96af7-223">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-223">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="96af7-224">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-224">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="96af7-225">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="96af7-225">Az.MachineLearning</span></span>
* <span data-ttu-id="96af7-226">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-226">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="96af7-227">Az.Media</span><span class="sxs-lookup"><span data-stu-id="96af7-227">Az.Media</span></span>
* <span data-ttu-id="96af7-228">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-228">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="96af7-229">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="96af7-229">Az.Monitor</span></span>
  * <span data-ttu-id="96af7-230">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-230">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="96af7-231">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="96af7-231">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="96af7-232">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="96af7-232">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="96af7-233">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="96af7-233">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="96af7-234">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="96af7-234">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="96af7-235">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="96af7-235">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="96af7-236">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-236">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-237">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-237">Az.Network</span></span>
* <span data-ttu-id="96af7-238">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-238">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="96af7-239">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-239">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="96af7-240">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="96af7-240">Az.NotificationHubs</span></span>
* <span data-ttu-id="96af7-241">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-241">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="96af7-242">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="96af7-242">Az.OperationalInsights</span></span>
* <span data-ttu-id="96af7-243">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-243">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="96af7-244">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="96af7-244">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="96af7-245">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-245">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-246">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-246">Az.RecoveryServices</span></span>
* <span data-ttu-id="96af7-247">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-247">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="96af7-248">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-248">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="96af7-249">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-249">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="96af7-250">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-250">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="96af7-251">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="96af7-251">Az.RedisCache</span></span>
* <span data-ttu-id="96af7-252">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-252">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-253">Az.Resources</span></span>
* <span data-ttu-id="96af7-254">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-254">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-255">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-255">Az.Sql</span></span>
* <span data-ttu-id="96af7-256">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="96af7-256">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="96af7-257">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-257">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="96af7-258">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-258">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="96af7-259">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="96af7-259">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="96af7-260">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="96af7-260">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="96af7-261">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="96af7-261">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="96af7-262">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-262">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-263">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-263">Az.Websites</span></span>
* <span data-ttu-id="96af7-264">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-264">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="96af7-265">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-265">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="96af7-266">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-266">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="96af7-267">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-267">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="96af7-268">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="96af7-268">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="96af7-269">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="96af7-269">Highlights since the last major release</span></span>
* <span data-ttu-id="96af7-270">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="96af7-270">General availability of `Az` module</span></span>
* <span data-ttu-id="96af7-271">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="96af7-271">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="96af7-272">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="96af7-272">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="96af7-273">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-273">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="96af7-274">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="96af7-274">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="96af7-275">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-275">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="96af7-276">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-276">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="96af7-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-277">Az.Accounts</span></span>
* <span data-ttu-id="96af7-278">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-278">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="96af7-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96af7-279">Az.AnalysisServices</span></span>
* <span data-ttu-id="96af7-280">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="96af7-280">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="96af7-281">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="96af7-281">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="96af7-282">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="96af7-282">Az.Automation</span></span>
* <span data-ttu-id="96af7-283">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-283">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="96af7-284">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-284">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="96af7-285">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-285">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-286">Az.Compute</span></span>
* <span data-ttu-id="96af7-287">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-287">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="96af7-288">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-288">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="96af7-289">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-289">Az.ContainerInstance</span></span>
* <span data-ttu-id="96af7-290">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-290">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="96af7-291">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="96af7-291">Az.DataFactory</span></span>
* <span data-ttu-id="96af7-292">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-292">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="96af7-293">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-293">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-294">Az.Resources</span></span>
* <span data-ttu-id="96af7-295">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="96af7-295">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="96af7-296">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="96af7-296">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="96af7-297">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="96af7-297">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="96af7-298">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="96af7-298">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="96af7-299">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-299">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="96af7-300">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="96af7-300">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-301">Az.Sql</span></span>
* <span data-ttu-id="96af7-302">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="96af7-302">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="96af7-303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-303">Az.Storage</span></span>
* <span data-ttu-id="96af7-304">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="96af7-304">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="96af7-305">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="96af7-305">New-AzStorageContext</span></span>
* <span data-ttu-id="96af7-306">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="96af7-306">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="96af7-307">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="96af7-307">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="96af7-308">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="96af7-308">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="96af7-309">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="96af7-309">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="96af7-310">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="96af7-310">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="96af7-311">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="96af7-311">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="96af7-312">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="96af7-312">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="96af7-313">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="96af7-313">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="96af7-314">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="96af7-314">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="96af7-315">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="96af7-315">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="96af7-316">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="96af7-316">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="96af7-317">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="96af7-317">Highlights since the last major release</span></span>
* <span data-ttu-id="96af7-318">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="96af7-318">General availability of `Az` module</span></span>
* <span data-ttu-id="96af7-319">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="96af7-319">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="96af7-320">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="96af7-320">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="96af7-321">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-321">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="96af7-322">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="96af7-322">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="96af7-323">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-323">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="96af7-324">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-324">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="96af7-325">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="96af7-325">Az.Automation</span></span>
* <span data-ttu-id="96af7-326">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="96af7-326">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="96af7-327">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="96af7-327">Dynamic grouping</span></span>
    * <span data-ttu-id="96af7-328">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="96af7-328">Pre-Post script</span></span>
    * <span data-ttu-id="96af7-329">再起動設定</span><span class="sxs-lookup"><span data-stu-id="96af7-329">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-330">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-330">Az.Compute</span></span>
* <span data-ttu-id="96af7-331">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-331">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="96af7-332">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-332">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="96af7-333">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96af7-333">Az.KeyVault</span></span>
* <span data-ttu-id="96af7-334">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-334">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-335">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-335">Az.Network</span></span>
* <span data-ttu-id="96af7-336">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-336">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="96af7-337">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-337">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-338">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-338">Az.RecoveryServices</span></span>
* <span data-ttu-id="96af7-339">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-339">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="96af7-340">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-340">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-341">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-341">Az.Resources</span></span>
* <span data-ttu-id="96af7-342">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="96af7-342">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="96af7-343">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-343">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-344">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-344">Az.Sql</span></span>
* <span data-ttu-id="96af7-345">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-345">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="96af7-346">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-346">Az.Storage</span></span>
* <span data-ttu-id="96af7-347">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="96af7-347">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="96af7-348">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="96af7-348">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="96af7-349">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="96af7-349">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="96af7-350">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="96af7-350">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="96af7-351">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="96af7-351">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="96af7-352">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="96af7-352">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="96af7-353">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="96af7-353">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-354">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-354">Az.Websites</span></span>
* <span data-ttu-id="96af7-355">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-355">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="96af7-356">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="96af7-356">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="96af7-357">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-357">Az.Accounts</span></span>
* <span data-ttu-id="96af7-358">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-358">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="96af7-359">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-359">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="96af7-360">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="96af7-360">Az.Automation</span></span>
* <span data-ttu-id="96af7-361">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-361">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="96af7-362">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-362">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="96af7-363">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="96af7-363">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="96af7-364">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="96af7-364">Az.Cdn</span></span>
* <span data-ttu-id="96af7-365">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="96af7-365">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-366">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-366">Az.Compute</span></span>
* <span data-ttu-id="96af7-367">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-367">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="96af7-368">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="96af7-368">Az.DataFactory</span></span>
* <span data-ttu-id="96af7-369">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-369">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="96af7-370">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="96af7-370">Az.LogicApp</span></span>
* <span data-ttu-id="96af7-371">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-371">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-372">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-372">Az.Network</span></span>
* <span data-ttu-id="96af7-373">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-373">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-374">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-374">Az.RecoveryServices</span></span>
* <span data-ttu-id="96af7-375">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-375">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="96af7-376">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="96af7-376">SDK Update</span></span>
* <span data-ttu-id="96af7-377">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="96af7-377">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="96af7-378">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-378">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-379">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-379">Az.Resources</span></span>
* <span data-ttu-id="96af7-380">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-380">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="96af7-381">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="96af7-381">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="96af7-382">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-382">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="96af7-383">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="96af7-383">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="96af7-384">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-384">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="96af7-385">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="96af7-385">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-386">Az.Sql</span></span>
* <span data-ttu-id="96af7-387">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-387">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="96af7-388">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-388">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="96af7-389">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-389">Az.Storage</span></span>
* <span data-ttu-id="96af7-390">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="96af7-390">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="96af7-391">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="96af7-391">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="96af7-392">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96af7-392">Az.AnalysisServices</span></span>
* <span data-ttu-id="96af7-393">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="96af7-393">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="96af7-394">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="96af7-394">Az.Automation</span></span>
* <span data-ttu-id="96af7-395">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-395">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="96af7-396">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-396">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="96af7-397">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="96af7-397">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="96af7-398">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="96af7-398">Az.CognitiveServices</span></span>
* <span data-ttu-id="96af7-399">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="96af7-399">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-400">Az.Compute</span></span>
* <span data-ttu-id="96af7-401">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-401">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="96af7-402">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-402">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="96af7-403">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-403">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="96af7-404">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="96af7-404">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="96af7-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="96af7-406">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-406">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="96af7-407">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="96af7-407">Az.EventHub</span></span>
* <span data-ttu-id="96af7-408">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-408">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="96af7-409">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96af7-409">Az.KeyVault</span></span>
* <span data-ttu-id="96af7-410">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-410">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="96af7-411">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="96af7-411">Az.LogicApp</span></span>
* <span data-ttu-id="96af7-412">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-412">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="96af7-413">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-413">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="96af7-414">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-414">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="96af7-415">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="96af7-415">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="96af7-416">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="96af7-416">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="96af7-417">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="96af7-417">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="96af7-418">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="96af7-418">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="96af7-419">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-419">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="96af7-420">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="96af7-420">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="96af7-421">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="96af7-421">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="96af7-422">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="96af7-422">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="96af7-423">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="96af7-423">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="96af7-424">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-424">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="96af7-425">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="96af7-425">Az.Monitor</span></span>
* <span data-ttu-id="96af7-426">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-426">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-427">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-427">Az.Network</span></span>
* <span data-ttu-id="96af7-428">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-428">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="96af7-429">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="96af7-429">Az.OperationalInsights</span></span>
* <span data-ttu-id="96af7-430">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-430">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="96af7-431">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-431">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="96af7-432">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-432">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="96af7-433">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-433">Az.Resources</span></span>
* <span data-ttu-id="96af7-434">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="96af7-434">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="96af7-435">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="96af7-435">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="96af7-436">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="96af7-436">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="96af7-437">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-437">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-438">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-438">Az.Sql</span></span>
* <span data-ttu-id="96af7-439">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-439">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="96af7-440">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-440">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-441">Az.Websites</span></span>
* <span data-ttu-id="96af7-442">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-442">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="96af7-443">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="96af7-443">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="96af7-444">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-444">Az.Accounts</span></span>
* <span data-ttu-id="96af7-445">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="96af7-445">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="96af7-446">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96af7-446">Az.AnalysisServices</span></span>
<span data-ttu-id="96af7-447">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="96af7-447">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-448">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-448">Az.Compute</span></span>
* <span data-ttu-id="96af7-449">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-449">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="96af7-450">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-450">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="96af7-451">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-451">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-452">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-452">Az.RecoveryServices</span></span>
<span data-ttu-id="96af7-453">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="96af7-453">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-454">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-454">Az.Resources</span></span>
* <span data-ttu-id="96af7-455">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-455">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="96af7-456">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="96af7-456">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="96af7-457">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-457">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="96af7-458">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="96af7-458">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-459">Az.Sql</span></span>
* <span data-ttu-id="96af7-460">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="96af7-460">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="96af7-461">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-461">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="96af7-462">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-462">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="96af7-463">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="96af7-463">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="96af7-464">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-464">Az.Accounts</span></span>
* <span data-ttu-id="96af7-465">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="96af7-465">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="96af7-466">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96af7-466">Az.AnalysisServices</span></span>
* <span data-ttu-id="96af7-467">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="96af7-467">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-468">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-468">Az.RecoveryServices</span></span>
* <span data-ttu-id="96af7-469">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="96af7-469">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="96af7-470">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="96af7-470">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="96af7-471">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-471">Az.Accounts</span></span>
* <span data-ttu-id="96af7-472">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="96af7-472">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="96af7-473">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-473">Update incorrect online help URLs</span></span>
* <span data-ttu-id="96af7-474">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-474">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="96af7-475">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="96af7-475">Az.Aks</span></span>
* <span data-ttu-id="96af7-476">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-476">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="96af7-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="96af7-477">Az.Automation</span></span>
* <span data-ttu-id="96af7-478">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-478">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="96af7-479">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-479">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="96af7-480">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="96af7-480">Az.Cdn</span></span>
* <span data-ttu-id="96af7-481">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-481">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-482">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-482">Az.Compute</span></span>
* <span data-ttu-id="96af7-483">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="96af7-483">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="96af7-484">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="96af7-484">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="96af7-485">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-485">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="96af7-486">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="96af7-486">Az.ContainerRegistry</span></span>
* <span data-ttu-id="96af7-487">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-487">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="96af7-488">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="96af7-488">Az.DataFactory</span></span>
* <span data-ttu-id="96af7-489">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="96af7-489">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="96af7-490">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-490">Az.DataLakeStore</span></span>
* <span data-ttu-id="96af7-491">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="96af7-491">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="96af7-492">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="96af7-492">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="96af7-493">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-493">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="96af7-494">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="96af7-494">Az.IotHub</span></span>
* <span data-ttu-id="96af7-495">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="96af7-495">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="96af7-496">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96af7-496">Az.KeyVault</span></span>
* <span data-ttu-id="96af7-497">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-497">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-498">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-498">Az.Network</span></span>
* <span data-ttu-id="96af7-499">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-499">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-500">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-500">Az.Resources</span></span>
* <span data-ttu-id="96af7-501">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-501">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="96af7-502">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-502">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="96af7-503">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-503">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="96af7-504">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="96af7-504">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="96af7-505">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="96af7-505">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="96af7-506">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-506">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="96af7-507">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="96af7-507">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="96af7-508">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96af7-508">Az.ServiceFabric</span></span>
* <span data-ttu-id="96af7-509">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="96af7-509">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="96af7-510">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="96af7-510">Fix some error messages.</span></span>
* <span data-ttu-id="96af7-511">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-511">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="96af7-512">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-512">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="96af7-513">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="96af7-513">Az.SignalR</span></span>
* <span data-ttu-id="96af7-514">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-514">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-515">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-515">Az.Sql</span></span>
* <span data-ttu-id="96af7-516">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-516">Update incorrect online help URLs</span></span>
* <span data-ttu-id="96af7-517">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-517">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="96af7-518">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-518">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="96af7-519">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="96af7-519">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="96af7-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-520">Az.Storage</span></span>
* <span data-ttu-id="96af7-521">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-521">Update incorrect online help URLs</span></span>
* <span data-ttu-id="96af7-522">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="96af7-522">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="96af7-523">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="96af7-523">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="96af7-524">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="96af7-524">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="96af7-525">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="96af7-525">Az.TrafficManager</span></span>
* <span data-ttu-id="96af7-526">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-526">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-527">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-527">Az.Websites</span></span>
* <span data-ttu-id="96af7-528">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="96af7-528">Update incorrect online help URLs</span></span>
* <span data-ttu-id="96af7-529">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-529">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="96af7-530">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="96af7-530">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="96af7-531">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="96af7-531">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="96af7-532">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-532">Az.Accounts</span></span>
* <span data-ttu-id="96af7-533">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="96af7-533">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-534">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-534">Az.Compute</span></span>
* <span data-ttu-id="96af7-535">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-535">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="96af7-536">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="96af7-536">Updated the description of ID in help files</span></span>
* <span data-ttu-id="96af7-537">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-537">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="96af7-538">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-538">Az.DataLakeStore</span></span>
* <span data-ttu-id="96af7-539">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-539">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="96af7-540">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-540">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="96af7-541">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="96af7-541">Az.EventGrid</span></span>
* <span data-ttu-id="96af7-542">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-542">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="96af7-543">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="96af7-543">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="96af7-544">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="96af7-544">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="96af7-545">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="96af7-545">Event Time-To-Live,</span></span>
        - <span data-ttu-id="96af7-546">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="96af7-546">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="96af7-547">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="96af7-547">Dead letter endpoint.</span></span>
    - <span data-ttu-id="96af7-548">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="96af7-548">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="96af7-549">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="96af7-549">Event Time-To-Live,</span></span>
        - <span data-ttu-id="96af7-550">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="96af7-550">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="96af7-551">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="96af7-551">Dead letter endpoint.</span></span>
* <span data-ttu-id="96af7-552">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-552">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="96af7-553">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="96af7-553">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="96af7-554">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="96af7-554">Az.IotHub</span></span>
* <span data-ttu-id="96af7-555">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-555">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="96af7-556">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="96af7-556">Az.LogicApp</span></span>
* <span data-ttu-id="96af7-557">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="96af7-557">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-558">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-558">Az.Resources</span></span>
* <span data-ttu-id="96af7-559">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-559">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="96af7-560">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="96af7-560">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="96af7-561">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-561">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="96af7-562">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-562">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="96af7-563">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="96af7-563">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="96af7-564">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="96af7-564">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="96af7-565">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="96af7-565">Az.SignalR</span></span>
* <span data-ttu-id="96af7-566">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-566">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-567">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-567">Az.Sql</span></span>
* <span data-ttu-id="96af7-568">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="96af7-568">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="96af7-569">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-569">Az.Storage</span></span>
* <span data-ttu-id="96af7-570">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="96af7-570">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="96af7-571">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="96af7-571">New-AzStorageContext</span></span>
* <span data-ttu-id="96af7-572">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-572">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="96af7-573">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="96af7-573">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-574">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-574">Az.Websites</span></span>
* <span data-ttu-id="96af7-575">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-575">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="96af7-576">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-576">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="96af7-577">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="96af7-577">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="96af7-578">全般</span><span class="sxs-lookup"><span data-stu-id="96af7-578">General</span></span>

- <span data-ttu-id="96af7-579">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="96af7-579">General Availability of Az Module</span></span>
- <span data-ttu-id="96af7-580">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="96af7-580">Online help for each module</span></span>
- <span data-ttu-id="96af7-581">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-581">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="96af7-582">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-582">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="96af7-583">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="96af7-583">Az.Accounts</span></span>
- <span data-ttu-id="96af7-584">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="96af7-584">Changed from Az.Profile</span></span>
- <span data-ttu-id="96af7-585">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-585">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="96af7-586">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="96af7-586">Az.ApiManagement</span></span>
- <span data-ttu-id="96af7-587">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="96af7-587">Fixes for #7002</span></span>
- <span data-ttu-id="96af7-588">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-588">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="96af7-589">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="96af7-589">Az.Batch</span></span>
- <span data-ttu-id="96af7-590">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-590">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="96af7-591">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-591">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="96af7-592">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-592">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="96af7-593">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="96af7-593">Az.Billing</span></span>
- <span data-ttu-id="96af7-594">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-594">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="96af7-595">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="96af7-595">Az.CognitivServices</span></span>
- <span data-ttu-id="96af7-596">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-596">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="96af7-597">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="96af7-597">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="96af7-598">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-598">Az.ContainerInstance</span></span>
- <span data-ttu-id="96af7-599">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-599">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="96af7-600">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="96af7-600">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="96af7-601">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-601">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="96af7-602">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-602">Az.DataLakeStore</span></span>
- <span data-ttu-id="96af7-603">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-603">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="96af7-604">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="96af7-604">Az.Monitor</span></span>
- <span data-ttu-id="96af7-605">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-605">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="96af7-606">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96af7-606">Az.KeyVault</span></span>
- <span data-ttu-id="96af7-607">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="96af7-607">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="96af7-608">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="96af7-608">Az.MachineLearning</span></span>
- <span data-ttu-id="96af7-609">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="96af7-609">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="96af7-610">Az.Media</span><span class="sxs-lookup"><span data-stu-id="96af7-610">Az.Media</span></span>
- <span data-ttu-id="96af7-611">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="96af7-611">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="96af7-612">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-612">Az.Network</span></span>
<span data-ttu-id="96af7-613">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-613">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="96af7-614">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="96af7-614">New cmdlets added:</span></span>
        - <span data-ttu-id="96af7-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="96af7-615">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="96af7-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="96af7-616">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="96af7-617">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="96af7-617">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="96af7-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="96af7-618">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="96af7-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="96af7-619">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="96af7-620">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="96af7-620">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="96af7-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="96af7-621">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="96af7-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="96af7-622">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="96af7-623">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-623">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="96af7-624">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="96af7-624">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="96af7-625">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="96af7-625">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="96af7-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="96af7-626">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="96af7-627">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="96af7-627">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="96af7-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="96af7-628">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="96af7-629">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-629">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="96af7-630">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-630">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="96af7-631">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="96af7-631">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="96af7-632">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="96af7-632">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="96af7-633">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="96af7-633">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="96af7-634">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-634">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="96af7-635">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-635">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="96af7-636">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="96af7-636">Az.OperationalInsights</span></span>
- <span data-ttu-id="96af7-637">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-637">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="96af7-638">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="96af7-638">Az.Profile</span></span>
- <span data-ttu-id="96af7-639">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="96af7-639">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-640">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-640">Az.RecoveryServices</span></span>
- <span data-ttu-id="96af7-641">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-641">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="96af7-642">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-642">Az.Resources</span></span>
- <span data-ttu-id="96af7-643">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-643">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="96af7-644">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96af7-644">Az.ServiceFabric</span></span>
- <span data-ttu-id="96af7-645">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="96af7-645">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="96af7-646">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-646">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="96af7-647">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="96af7-647">Az.SIgnalR</span></span>
- <span data-ttu-id="96af7-648">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="96af7-648">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="96af7-649">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-649">Az.Sql</span></span>
- <span data-ttu-id="96af7-650">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-650">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="96af7-651">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-651">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="96af7-652">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-652">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="96af7-653">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-653">Az.Storage</span></span>
- <span data-ttu-id="96af7-654">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="96af7-655">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-655">Az.Websites</span></span>
- <span data-ttu-id="96af7-656">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="96af7-656">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="96af7-657">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="96af7-657">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="96af7-658">全般</span><span class="sxs-lookup"><span data-stu-id="96af7-658">General</span></span>

* <span data-ttu-id="96af7-659">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="96af7-659">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="96af7-660">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-660">Az.Compute</span></span>

* <span data-ttu-id="96af7-661">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-661">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="96af7-662">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-662">Az.DataLakeStore</span></span>

* <span data-ttu-id="96af7-663">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-663">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="96af7-664">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="96af7-664">Az.FrontDoor</span></span>

* <span data-ttu-id="96af7-665">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-665">Fixed some broken links</span></span>
    - <span data-ttu-id="96af7-666">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-666">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="96af7-667">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-667">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="96af7-668">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96af7-668">Az.RecoveryServices</span></span>

* <span data-ttu-id="96af7-669">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-669">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="96af7-670">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="96af7-670">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="96af7-671">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-671">Az.Resources</span></span>

* <span data-ttu-id="96af7-672">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="96af7-672">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="96af7-673">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-673">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="96af7-674">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-674">Az.Sql</span></span>

* <span data-ttu-id="96af7-675">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="96af7-675">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="96af7-676">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-676">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="96af7-677">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="96af7-677">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="96af7-678">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-678">Az.Storage</span></span>

* <span data-ttu-id="96af7-679">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-679">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="96af7-680">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-680">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="96af7-681">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="96af7-681">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="96af7-682">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="96af7-682">Support Static Website configuration</span></span>
    - <span data-ttu-id="96af7-683">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="96af7-683">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="96af7-684">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="96af7-684">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="96af7-685">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-685">Az.Websites</span></span>

* <span data-ttu-id="96af7-686">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="96af7-686">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="96af7-687">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-687">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="96af7-688">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="96af7-688">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="96af7-689">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="96af7-689">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="96af7-690">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="96af7-690">Az.ApiManagement</span></span>
* <span data-ttu-id="96af7-691">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-691">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="96af7-692">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="96af7-692">Az.Automation</span></span>
* <span data-ttu-id="96af7-693">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="96af7-693">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="96af7-694">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-694">Added Update Management cmdlets</span></span>
* <span data-ttu-id="96af7-695">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-695">Added Source Control cmdlets</span></span>
* <span data-ttu-id="96af7-696">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-696">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="96af7-697">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-697">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="96af7-698">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-698">Az.Compute</span></span>
* <span data-ttu-id="96af7-699">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-699">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="96af7-700">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-700">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="96af7-701">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-701">Az.ContainerInstance</span></span>
* <span data-ttu-id="96af7-702">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-702">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="96af7-703">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="96af7-703">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="96af7-704">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-704">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="96af7-705">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-705">Az.Network</span></span>
* <span data-ttu-id="96af7-706">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-706">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="96af7-707">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-707">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="96af7-708">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-708">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="96af7-709">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-709">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="96af7-710">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="96af7-710">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="96af7-711">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-711">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="96af7-712">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="96af7-712">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="96af7-713">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="96af7-713">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="96af7-714">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-714">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="96af7-715">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-715">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="96af7-716">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="96af7-716">Az.Relay</span></span>
* <span data-ttu-id="96af7-717">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="96af7-717">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="96af7-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-718">Az.Resources</span></span>
* <span data-ttu-id="96af7-719">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-719">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="96af7-720">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-720">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="96af7-721">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="96af7-721">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="96af7-722">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96af7-722">Az.ServiceFabric</span></span>
* <span data-ttu-id="96af7-723">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-723">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="96af7-724">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-724">Az.Sql</span></span>
* <span data-ttu-id="96af7-725">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-725">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="96af7-726">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-726">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="96af7-727">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-727">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="96af7-728">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-728">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="96af7-729">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="96af7-729">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="96af7-730">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="96af7-730">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="96af7-731">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="96af7-731">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="96af7-732">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="96af7-732">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="96af7-733">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="96af7-733">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="96af7-734">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="96af7-734">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="96af7-735">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-735">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="96af7-736">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="96af7-736">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="96af7-737">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="96af7-737">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="96af7-738">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="96af7-738">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="96af7-739">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="96af7-739">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="96af7-740">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="96af7-740">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="96af7-741">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-741">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="96af7-742">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="96af7-742">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="96af7-743">全般</span><span class="sxs-lookup"><span data-stu-id="96af7-743">General</span></span>
* <span data-ttu-id="96af7-744">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="96af7-744">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="96af7-745">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="96af7-745">Az.Profile</span></span>
* <span data-ttu-id="96af7-746">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-746">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="96af7-747">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-747">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="96af7-748">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="96af7-748">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="96af7-749">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-749">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="96af7-750">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-750">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="96af7-751">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-751">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="96af7-752">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-752">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="96af7-753">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="96af7-753">Az.CognitiveServices</span></span>
* <span data-ttu-id="96af7-754">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-754">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-755">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-755">Az.Compute</span></span>
* <span data-ttu-id="96af7-756">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-756">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="96af7-757">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="96af7-757">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="96af7-758">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-758">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="96af7-759">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-759">Az.DataLakeStore</span></span>
* <span data-ttu-id="96af7-760">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="96af7-760">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="96af7-761">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-761">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="96af7-762">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="96af7-762">Az.Insights</span></span>
* <span data-ttu-id="96af7-763">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-763">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="96af7-764">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="96af7-764">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="96af7-765">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-765">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="96af7-766">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="96af7-766">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-767">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-767">Az.Network</span></span>
* <span data-ttu-id="96af7-768">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="96af7-768">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="96af7-769">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="96af7-769">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="96af7-770">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="96af7-770">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="96af7-771">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="96af7-771">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="96af7-772">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="96af7-772">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="96af7-773">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="96af7-773">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="96af7-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="96af7-774">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="96af7-775">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="96af7-775">Az.PolicyInsights</span></span>
* <span data-ttu-id="96af7-776">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-776">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-777">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-777">Az.Resources</span></span>
* <span data-ttu-id="96af7-778">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="96af7-778">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="96af7-779">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="96af7-779">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="96af7-780">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96af7-780">Az.ServiceBus</span></span>
* <span data-ttu-id="96af7-781">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-781">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="96af7-782">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96af7-782">Az.ServiceFabric</span></span>
* <span data-ttu-id="96af7-783">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-783">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="96af7-784">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-784">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="96af7-785">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="96af7-785">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="96af7-786">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="96af7-786">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="96af7-787">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-787">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="96af7-788">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="96af7-788">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="96af7-789">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="96af7-789">Az.Profile</span></span>
* <span data-ttu-id="96af7-790">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-790">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="96af7-791">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-791">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-792">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-792">Az.Compute</span></span>
* <span data-ttu-id="96af7-793">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-793">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="96af7-794">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-794">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="96af7-795">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96af7-795">Az.DataLakeStore</span></span>
* <span data-ttu-id="96af7-796">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-796">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="96af7-797">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="96af7-797">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="96af7-798">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="96af7-798">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="96af7-799">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="96af7-799">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="96af7-800">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="96af7-800">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-801">Az.Network</span></span>
* <span data-ttu-id="96af7-802">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-802">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="96af7-803">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-803">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-804">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-804">Az.Resources</span></span>
* <span data-ttu-id="96af7-805">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-805">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="96af7-806">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-806">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="96af7-807">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="96af7-807">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="96af7-808">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="96af7-808">Azure.Storage</span></span>
* <span data-ttu-id="96af7-809">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-809">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="96af7-810">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="96af7-810">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="96af7-811">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="96af7-811">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="96af7-812">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-812">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="96af7-813">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="96af7-813">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="96af7-814">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="96af7-814">Az.CognitiveServices</span></span>
* <span data-ttu-id="96af7-815">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="96af7-815">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="96af7-816">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="96af7-816">Az.Compute</span></span>
* <span data-ttu-id="96af7-817">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-817">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="96af7-818">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-818">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="96af7-819">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-819">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="96af7-820">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="96af7-820">Az.DataFactoryV2</span></span>
* <span data-ttu-id="96af7-821">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-821">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="96af7-822">Az.Network</span><span class="sxs-lookup"><span data-stu-id="96af7-822">Az.Network</span></span>
* <span data-ttu-id="96af7-823">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96af7-823">Added NetworkProfile functionality.</span></span> <span data-ttu-id="96af7-824">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="96af7-824">new cmdlets added</span></span>
    - <span data-ttu-id="96af7-825">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="96af7-825">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="96af7-826">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="96af7-826">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="96af7-827">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="96af7-827">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="96af7-828">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="96af7-828">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="96af7-829">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="96af7-829">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="96af7-830">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="96af7-830">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="96af7-831">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-831">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="96af7-832">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-832">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="96af7-833">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-833">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="96af7-834">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="96af7-834">Az.RedisCache</span></span>
* <span data-ttu-id="96af7-835">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="96af7-835">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="96af7-836">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-836">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="96af7-837">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="96af7-837">Az.Resources</span></span>
* <span data-ttu-id="96af7-838">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="96af7-838">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="96af7-839">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-839">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="96af7-840">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="96af7-840">Az.Sql</span></span>
* <span data-ttu-id="96af7-841">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96af7-841">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="96af7-842">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="96af7-842">Az.Websites</span></span>
* <span data-ttu-id="96af7-843">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="96af7-843">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="96af7-844">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="96af7-844">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="96af7-845">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="96af7-845">0.2.0 - September 2018</span></span>
 <span data-ttu-id="96af7-846">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="96af7-846">Initial Release</span></span>