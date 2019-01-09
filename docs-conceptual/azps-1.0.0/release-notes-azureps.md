## <a name="100---december-2018"></a><span data-ttu-id="7f60f-101">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-101">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="7f60f-102">全般</span><span class="sxs-lookup"><span data-stu-id="7f60f-102">General</span></span>

- <span data-ttu-id="7f60f-103">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="7f60f-103">General Availability of Az Module</span></span>
- <span data-ttu-id="7f60f-104">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="7f60f-104">Online help for each module</span></span>
- <span data-ttu-id="7f60f-105">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-105">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="7f60f-106">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-106">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="7f60f-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="7f60f-107">Az.Accounts</span></span>
- <span data-ttu-id="7f60f-108">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-108">Changed from Az.Profile</span></span>
- <span data-ttu-id="7f60f-109">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-109">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="7f60f-110">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f60f-110">Az.ApiManagement</span></span>
- <span data-ttu-id="7f60f-111">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="7f60f-111">Fixes for #7002</span></span>
- <span data-ttu-id="7f60f-112">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-112">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="7f60f-113">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="7f60f-113">Az.Batch</span></span>
- <span data-ttu-id="7f60f-114">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-114">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="7f60f-115">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-115">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="7f60f-116">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-116">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="7f60f-117">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="7f60f-117">Az.Billing</span></span>
- <span data-ttu-id="7f60f-118">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-118">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="7f60f-119">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="7f60f-119">Az.CognitivServices</span></span>
- <span data-ttu-id="7f60f-120">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-120">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="7f60f-121">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-121">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="7f60f-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7f60f-122">Az.ContainerInstance</span></span>
- <span data-ttu-id="7f60f-123">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-123">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="7f60f-124">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7f60f-124">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="7f60f-125">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-125">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="7f60f-126">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f60f-126">Az.DataLakeStore</span></span>
- <span data-ttu-id="7f60f-127">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-127">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="7f60f-128">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="7f60f-128">Az.Monitor</span></span>
- <span data-ttu-id="7f60f-129">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-129">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="7f60f-130">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7f60f-130">Az.KeyVault</span></span>
- <span data-ttu-id="7f60f-131">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-131">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="7f60f-132">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7f60f-132">Az.MachineLearning</span></span>
- <span data-ttu-id="7f60f-133">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="7f60f-133">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="7f60f-134">Az.Media</span><span class="sxs-lookup"><span data-stu-id="7f60f-134">Az.Media</span></span>
- <span data-ttu-id="7f60f-135">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-135">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="7f60f-136">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f60f-136">Az.Network</span></span>
<span data-ttu-id="7f60f-137">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-137">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="7f60f-138">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="7f60f-138">New cmdlets added:</span></span>
        - <span data-ttu-id="7f60f-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f60f-139">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f60f-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f60f-140">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f60f-141">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f60f-141">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f60f-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f60f-142">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f60f-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="7f60f-143">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="7f60f-144">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="7f60f-144">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="7f60f-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="7f60f-145">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="7f60f-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f60f-146">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="7f60f-147">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="7f60f-147">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="7f60f-148">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="7f60f-148">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="7f60f-149">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="7f60f-149">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="7f60f-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="7f60f-150">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="7f60f-151">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="7f60f-151">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="7f60f-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="7f60f-152">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="7f60f-153">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-153">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="7f60f-154">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="7f60f-154">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="7f60f-155">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="7f60f-155">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="7f60f-156">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="7f60f-156">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="7f60f-157">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="7f60f-157">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="7f60f-158">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="7f60f-158">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="7f60f-159">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-159">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="7f60f-160">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7f60f-160">Az.OperationalInsights</span></span>
- <span data-ttu-id="7f60f-161">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-161">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="7f60f-162">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f60f-162">Az.Profile</span></span>
- <span data-ttu-id="7f60f-163">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-163">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="7f60f-164">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f60f-164">Az.RecoveryServices</span></span>
- <span data-ttu-id="7f60f-165">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-165">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="7f60f-166">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f60f-166">Az.Resources</span></span>
- <span data-ttu-id="7f60f-167">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-167">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="7f60f-168">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f60f-168">Az.ServiceFabric</span></span>
- <span data-ttu-id="7f60f-169">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="7f60f-169">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="7f60f-170">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-170">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="7f60f-171">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="7f60f-171">Az.SIgnalR</span></span>
- <span data-ttu-id="7f60f-172">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="7f60f-172">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="7f60f-173">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f60f-173">Az.Sql</span></span>
- <span data-ttu-id="7f60f-174">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-174">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="7f60f-175">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-175">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="7f60f-176">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-176">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="7f60f-177">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f60f-177">Az.Storage</span></span>
- <span data-ttu-id="7f60f-178">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-178">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="7f60f-179">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f60f-179">Az.Websites</span></span>
- <span data-ttu-id="7f60f-180">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="7f60f-180">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="7f60f-181">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-181">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="7f60f-182">全般</span><span class="sxs-lookup"><span data-stu-id="7f60f-182">General</span></span>

* <span data-ttu-id="7f60f-183">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="7f60f-183">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="7f60f-184">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f60f-184">Az.Compute</span></span>

* <span data-ttu-id="7f60f-185">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-185">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="7f60f-186">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f60f-186">Az.DataLakeStore</span></span>

* <span data-ttu-id="7f60f-187">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-187">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="7f60f-188">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="7f60f-188">Az.FrontDoor</span></span>

* <span data-ttu-id="7f60f-189">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-189">Fixed some broken links</span></span>
    - <span data-ttu-id="7f60f-190">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-190">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="7f60f-191">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-191">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="7f60f-192">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="7f60f-192">Az.RecoveryServices</span></span>

* <span data-ttu-id="7f60f-193">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-193">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="7f60f-194">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-194">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="7f60f-195">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f60f-195">Az.Resources</span></span>

* <span data-ttu-id="7f60f-196">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="7f60f-196">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="7f60f-197">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-197">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="7f60f-198">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f60f-198">Az.Sql</span></span>

* <span data-ttu-id="7f60f-199">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="7f60f-199">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="7f60f-200">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-200">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="7f60f-201">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-201">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="7f60f-202">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="7f60f-202">Az.Storage</span></span>

* <span data-ttu-id="7f60f-203">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-203">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="7f60f-204">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-204">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="7f60f-205">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="7f60f-205">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="7f60f-206">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="7f60f-206">Support Static Website configuration</span></span>
    - <span data-ttu-id="7f60f-207">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="7f60f-207">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="7f60f-208">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="7f60f-208">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="7f60f-209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f60f-209">Az.Websites</span></span>

* <span data-ttu-id="7f60f-210">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="7f60f-210">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="7f60f-211">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-211">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="7f60f-212">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="7f60f-212">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="7f60f-213">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-213">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="7f60f-214">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7f60f-214">Az.ApiManagement</span></span>
* <span data-ttu-id="7f60f-215">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-215">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="7f60f-216">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="7f60f-216">Az.Automation</span></span>
* <span data-ttu-id="7f60f-217">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="7f60f-217">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="7f60f-218">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-218">Added Update Management cmdlets</span></span>
* <span data-ttu-id="7f60f-219">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-219">Added Source Control cmdlets</span></span>
* <span data-ttu-id="7f60f-220">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-220">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="7f60f-221">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-221">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="7f60f-222">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f60f-222">Az.Compute</span></span>
* <span data-ttu-id="7f60f-223">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-223">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="7f60f-224">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-224">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="7f60f-225">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="7f60f-225">Az.ContainerInstance</span></span>
* <span data-ttu-id="7f60f-226">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-226">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="7f60f-227">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="7f60f-227">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="7f60f-228">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-228">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="7f60f-229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f60f-229">Az.Network</span></span>
* <span data-ttu-id="7f60f-230">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-230">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="7f60f-231">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-231">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="7f60f-232">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-232">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="7f60f-233">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-233">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="7f60f-234">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="7f60f-234">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="7f60f-235">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-235">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="7f60f-236">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-236">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="7f60f-237">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="7f60f-237">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="7f60f-238">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-238">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="7f60f-239">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-239">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="7f60f-240">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="7f60f-240">Az.Relay</span></span>
* <span data-ttu-id="7f60f-241">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="7f60f-241">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="7f60f-242">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f60f-242">Az.Resources</span></span>
* <span data-ttu-id="7f60f-243">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-243">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="7f60f-244">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-244">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="7f60f-245">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="7f60f-245">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="7f60f-246">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f60f-246">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f60f-247">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-247">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="7f60f-248">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f60f-248">Az.Sql</span></span>
* <span data-ttu-id="7f60f-249">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-249">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="7f60f-250">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f60f-250">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f60f-251">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f60f-251">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f60f-252">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f60f-252">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f60f-253">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="7f60f-253">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="7f60f-254">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f60f-254">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="7f60f-255">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f60f-255">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="7f60f-256">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f60f-256">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="7f60f-257">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="7f60f-257">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="7f60f-258">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="7f60f-258">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="7f60f-259">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-259">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="7f60f-260">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-260">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="7f60f-261">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="7f60f-261">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="7f60f-262">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="7f60f-262">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="7f60f-263">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="7f60f-263">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="7f60f-264">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="7f60f-264">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="7f60f-265">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-265">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="7f60f-266">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-266">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="7f60f-267">全般</span><span class="sxs-lookup"><span data-stu-id="7f60f-267">General</span></span>
* <span data-ttu-id="7f60f-268">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="7f60f-268">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="7f60f-269">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f60f-269">Az.Profile</span></span>
* <span data-ttu-id="7f60f-270">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-270">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="7f60f-271">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-271">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="7f60f-272">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-272">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="7f60f-273">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-273">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="7f60f-274">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-274">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="7f60f-275">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-275">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="7f60f-276">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-276">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="7f60f-277">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f60f-277">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f60f-278">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-278">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f60f-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f60f-279">Az.Compute</span></span>
* <span data-ttu-id="7f60f-280">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-280">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="7f60f-281">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="7f60f-281">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="7f60f-282">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-282">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f60f-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f60f-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f60f-284">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-284">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="7f60f-285">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-285">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="7f60f-286">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="7f60f-286">Az.Insights</span></span>
* <span data-ttu-id="7f60f-287">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-287">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="7f60f-288">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="7f60f-288">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="7f60f-289">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-289">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="7f60f-290">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="7f60f-290">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f60f-291">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f60f-291">Az.Network</span></span>
* <span data-ttu-id="7f60f-292">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="7f60f-292">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="7f60f-293">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f60f-293">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="7f60f-294">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="7f60f-294">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="7f60f-295">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7f60f-295">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="7f60f-296">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="7f60f-296">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="7f60f-297">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="7f60f-297">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="7f60f-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="7f60f-298">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="7f60f-299">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="7f60f-299">Az.PolicyInsights</span></span>
* <span data-ttu-id="7f60f-300">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-300">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f60f-301">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f60f-301">Az.Resources</span></span>
* <span data-ttu-id="7f60f-302">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="7f60f-302">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="7f60f-303">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-303">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="7f60f-304">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="7f60f-304">Az.ServiceBus</span></span>
* <span data-ttu-id="7f60f-305">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-305">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="7f60f-306">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7f60f-306">Az.ServiceFabric</span></span>
* <span data-ttu-id="7f60f-307">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-307">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="7f60f-308">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-308">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="7f60f-309">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="7f60f-309">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="7f60f-310">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="7f60f-310">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="7f60f-311">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-311">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="7f60f-312">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-312">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="7f60f-313">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="7f60f-313">Az.Profile</span></span>
* <span data-ttu-id="7f60f-314">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-314">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="7f60f-315">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-315">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f60f-316">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f60f-316">Az.Compute</span></span>
* <span data-ttu-id="7f60f-317">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-317">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="7f60f-318">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-318">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="7f60f-319">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7f60f-319">Az.DataLakeStore</span></span>
* <span data-ttu-id="7f60f-320">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-320">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="7f60f-321">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="7f60f-321">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="7f60f-322">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="7f60f-322">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="7f60f-323">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="7f60f-323">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="7f60f-324">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="7f60f-324">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f60f-325">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f60f-325">Az.Network</span></span>
* <span data-ttu-id="7f60f-326">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-326">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="7f60f-327">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-327">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f60f-328">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f60f-328">Az.Resources</span></span>
* <span data-ttu-id="7f60f-329">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-329">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="7f60f-330">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-330">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="7f60f-331">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-331">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="7f60f-332">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7f60f-332">Azure.Storage</span></span>
* <span data-ttu-id="7f60f-333">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-333">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="7f60f-334">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="7f60f-334">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="7f60f-335">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="7f60f-335">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="7f60f-336">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-336">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="7f60f-337">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="7f60f-337">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="7f60f-338">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="7f60f-338">Az.CognitiveServices</span></span>
* <span data-ttu-id="7f60f-339">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-339">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="7f60f-340">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="7f60f-340">Az.Compute</span></span>
* <span data-ttu-id="7f60f-341">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-341">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="7f60f-342">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-342">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="7f60f-343">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-343">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="7f60f-344">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7f60f-344">Az.DataFactoryV2</span></span>
* <span data-ttu-id="7f60f-345">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-345">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="7f60f-346">Az.Network</span><span class="sxs-lookup"><span data-stu-id="7f60f-346">Az.Network</span></span>
* <span data-ttu-id="7f60f-347">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="7f60f-347">Added NetworkProfile functionality.</span></span> <span data-ttu-id="7f60f-348">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="7f60f-348">new cmdlets added</span></span>
    - <span data-ttu-id="7f60f-349">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f60f-349">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f60f-350">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f60f-350">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f60f-351">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f60f-351">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f60f-352">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="7f60f-352">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="7f60f-353">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="7f60f-353">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="7f60f-354">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="7f60f-354">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="7f60f-355">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-355">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="7f60f-356">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-356">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="7f60f-357">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-357">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="7f60f-358">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7f60f-358">Az.RedisCache</span></span>
* <span data-ttu-id="7f60f-359">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="7f60f-359">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="7f60f-360">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-360">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="7f60f-361">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="7f60f-361">Az.Resources</span></span>
* <span data-ttu-id="7f60f-362">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-362">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="7f60f-363">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-363">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="7f60f-364">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="7f60f-364">Az.Sql</span></span>
* <span data-ttu-id="7f60f-365">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7f60f-365">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="7f60f-366">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="7f60f-366">Az.Websites</span></span>
* <span data-ttu-id="7f60f-367">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="7f60f-367">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="7f60f-368">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="7f60f-368">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="7f60f-369">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="7f60f-369">0.2.0 - September 2018</span></span>
 <span data-ttu-id="7f60f-370">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="7f60f-370">Initial Release</span></span>