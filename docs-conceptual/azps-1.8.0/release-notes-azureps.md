---
ms.openlocfilehash: ffeba2cff2e157e7ec0fb7639f9d4075c359c85e
ms.sourcegitcommit: 0b644bfecf4224b2ea83520d1a6a956734d9fba4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "67863837"
---
## <a name="180---april-2019"></a><span data-ttu-id="cec6f-101">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-101">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cec6f-102">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cec6f-102">Highlights since the last major release</span></span>
* <span data-ttu-id="cec6f-103">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="cec6f-103">General availability of `Az` module</span></span>
* <span data-ttu-id="cec6f-104">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="cec6f-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cec6f-105">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="cec6f-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cec6f-106">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cec6f-107">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cec6f-108">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cec6f-109">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cec6f-110">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-110">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-111">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-111">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="cec6f-112">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cec6f-112">Az.Batch</span></span>
* <span data-ttu-id="cec6f-113">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-113">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cec6f-114">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cec6f-114">Az.Cdn</span></span>
* <span data-ttu-id="cec6f-115">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-115">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cec6f-116">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-116">Az.CognitiveServices</span></span>
* <span data-ttu-id="cec6f-117">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-117">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-118">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-118">Az.Compute</span></span>
* <span data-ttu-id="cec6f-119">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-119">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="cec6f-120">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-120">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cec6f-121">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-121">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cec6f-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cec6f-122">Az.DataFactory</span></span>
* <span data-ttu-id="cec6f-123">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-123">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-124">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-124">Az.DataLakeStore</span></span>
* <span data-ttu-id="cec6f-125">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-125">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cec6f-126">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cec6f-126">Az.EventGrid</span></span>
* <span data-ttu-id="cec6f-127">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-127">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cec6f-128">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cec6f-128">Az.EventHub</span></span>
* <span data-ttu-id="cec6f-129">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-129">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="cec6f-130">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cec6f-130">Az.HDInsight</span></span>
* <span data-ttu-id="cec6f-131">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-131">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cec6f-132">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cec6f-132">Az.IotHub</span></span>
* <span data-ttu-id="cec6f-133">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-133">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cec6f-134">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cec6f-134">Az.KeyVault</span></span>
* <span data-ttu-id="cec6f-135">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-135">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cec6f-136">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-136">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="cec6f-137">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cec6f-137">Az.MachineLearning</span></span>
* <span data-ttu-id="cec6f-138">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-138">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="cec6f-139">Az.Media</span><span class="sxs-lookup"><span data-stu-id="cec6f-139">Az.Media</span></span>
* <span data-ttu-id="cec6f-140">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-140">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cec6f-141">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cec6f-141">Az.Monitor</span></span>
  * <span data-ttu-id="cec6f-142">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-142">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="cec6f-143">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="cec6f-143">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="cec6f-144">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="cec6f-144">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="cec6f-145">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="cec6f-145">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="cec6f-146">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="cec6f-146">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="cec6f-147">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="cec6f-147">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="cec6f-148">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-148">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-149">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-149">Az.Network</span></span>
* <span data-ttu-id="cec6f-150">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-150">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cec6f-151">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-151">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="cec6f-152">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="cec6f-152">Az.NotificationHubs</span></span>
* <span data-ttu-id="cec6f-153">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-153">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cec6f-154">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cec6f-154">Az.OperationalInsights</span></span>
* <span data-ttu-id="cec6f-155">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-155">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="cec6f-156">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="cec6f-156">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="cec6f-157">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-157">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-158">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-158">Az.RecoveryServices</span></span>
* <span data-ttu-id="cec6f-159">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-159">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cec6f-160">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-160">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="cec6f-161">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-161">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="cec6f-162">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-162">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cec6f-163">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cec6f-163">Az.RedisCache</span></span>
* <span data-ttu-id="cec6f-164">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-164">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-165">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-165">Az.Resources</span></span>
* <span data-ttu-id="cec6f-166">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-166">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-167">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-167">Az.Sql</span></span>
* <span data-ttu-id="cec6f-168">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="cec6f-168">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="cec6f-169">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-169">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cec6f-170">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-170">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="cec6f-171">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-171">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="cec6f-172">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="cec6f-172">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="cec6f-173">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="cec6f-173">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="cec6f-174">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-174">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cec6f-175">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-175">Az.Websites</span></span>
* <span data-ttu-id="cec6f-176">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-176">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="cec6f-177">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-177">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cec6f-178">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-178">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="cec6f-179">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-179">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="cec6f-180">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-180">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cec6f-181">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cec6f-181">Highlights since the last major release</span></span>
* <span data-ttu-id="cec6f-182">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="cec6f-182">General availability of `Az` module</span></span>
* <span data-ttu-id="cec6f-183">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="cec6f-183">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cec6f-184">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="cec6f-184">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cec6f-185">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-185">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cec6f-186">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-186">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cec6f-187">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-187">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cec6f-188">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-188">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cec6f-189">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-189">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-190">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-190">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cec6f-191">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-191">Az.AnalysisServices</span></span>
* <span data-ttu-id="cec6f-192">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="cec6f-192">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="cec6f-193">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-193">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cec6f-194">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cec6f-194">Az.Automation</span></span>
* <span data-ttu-id="cec6f-195">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-195">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="cec6f-196">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-196">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="cec6f-197">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-197">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-198">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-198">Az.Compute</span></span>
* <span data-ttu-id="cec6f-199">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-199">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="cec6f-200">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-200">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="cec6f-201">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-201">Az.ContainerInstance</span></span>
* <span data-ttu-id="cec6f-202">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-202">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cec6f-203">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cec6f-203">Az.DataFactory</span></span>
* <span data-ttu-id="cec6f-204">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-204">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="cec6f-205">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-205">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-206">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-206">Az.Resources</span></span>
* <span data-ttu-id="cec6f-207">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-207">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="cec6f-208">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-208">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="cec6f-209">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="cec6f-209">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="cec6f-210">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="cec6f-210">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="cec6f-211">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-211">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="cec6f-212">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="cec6f-212">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-213">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-213">Az.Sql</span></span>
* <span data-ttu-id="cec6f-214">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-214">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cec6f-215">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-215">Az.Storage</span></span>
* <span data-ttu-id="cec6f-216">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="cec6f-216">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="cec6f-217">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cec6f-217">New-AzStorageContext</span></span>
* <span data-ttu-id="cec6f-218">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="cec6f-218">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="cec6f-219">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="cec6f-219">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="cec6f-220">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="cec6f-220">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="cec6f-221">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="cec6f-221">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="cec6f-222">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="cec6f-222">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="cec6f-223">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="cec6f-223">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="cec6f-224">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cec6f-224">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="cec6f-225">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cec6f-225">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="cec6f-226">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cec6f-226">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="cec6f-227">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cec6f-227">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="cec6f-228">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-228">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cec6f-229">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cec6f-229">Highlights since the last major release</span></span>
* <span data-ttu-id="cec6f-230">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="cec6f-230">General availability of `Az` module</span></span>
* <span data-ttu-id="cec6f-231">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="cec6f-231">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cec6f-232">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="cec6f-232">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cec6f-233">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-233">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cec6f-234">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-234">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cec6f-235">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-235">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cec6f-236">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-236">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cec6f-237">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cec6f-237">Az.Automation</span></span>
* <span data-ttu-id="cec6f-238">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-238">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="cec6f-239">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="cec6f-239">Dynamic grouping</span></span>
    * <span data-ttu-id="cec6f-240">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="cec6f-240">Pre-Post script</span></span>
    * <span data-ttu-id="cec6f-241">再起動設定</span><span class="sxs-lookup"><span data-stu-id="cec6f-241">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-242">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-242">Az.Compute</span></span>
* <span data-ttu-id="cec6f-243">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-243">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="cec6f-244">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-244">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cec6f-245">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cec6f-245">Az.KeyVault</span></span>
* <span data-ttu-id="cec6f-246">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-246">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-247">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-247">Az.Network</span></span>
* <span data-ttu-id="cec6f-248">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-248">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="cec6f-249">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-249">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-250">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-250">Az.RecoveryServices</span></span>
* <span data-ttu-id="cec6f-251">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-251">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="cec6f-252">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-252">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-253">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-253">Az.Resources</span></span>
* <span data-ttu-id="cec6f-254">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-254">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="cec6f-255">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-255">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-256">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-256">Az.Sql</span></span>
* <span data-ttu-id="cec6f-257">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-257">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cec6f-258">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-258">Az.Storage</span></span>
* <span data-ttu-id="cec6f-259">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="cec6f-259">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="cec6f-260">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cec6f-260">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cec6f-261">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cec6f-261">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cec6f-262">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cec6f-262">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cec6f-263">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="cec6f-263">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="cec6f-264">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="cec6f-264">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="cec6f-265">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="cec6f-265">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cec6f-266">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-266">Az.Websites</span></span>
* <span data-ttu-id="cec6f-267">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-267">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="cec6f-268">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-268">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cec6f-269">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-269">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-270">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-270">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="cec6f-271">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-271">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cec6f-272">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cec6f-272">Az.Automation</span></span>
* <span data-ttu-id="cec6f-273">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-273">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="cec6f-274">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-274">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="cec6f-275">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="cec6f-275">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cec6f-276">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cec6f-276">Az.Cdn</span></span>
* <span data-ttu-id="cec6f-277">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="cec6f-277">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-278">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-278">Az.Compute</span></span>
* <span data-ttu-id="cec6f-279">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-279">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cec6f-280">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cec6f-280">Az.DataFactory</span></span>
* <span data-ttu-id="cec6f-281">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-281">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cec6f-282">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cec6f-282">Az.LogicApp</span></span>
* <span data-ttu-id="cec6f-283">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-283">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-284">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-284">Az.Network</span></span>
* <span data-ttu-id="cec6f-285">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-285">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-286">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-286">Az.RecoveryServices</span></span>
* <span data-ttu-id="cec6f-287">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-287">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="cec6f-288">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-288">SDK Update</span></span>
* <span data-ttu-id="cec6f-289">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-289">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="cec6f-290">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-290">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-291">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-291">Az.Resources</span></span>
* <span data-ttu-id="cec6f-292">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-292">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="cec6f-293">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="cec6f-293">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="cec6f-294">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-294">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="cec6f-295">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="cec6f-295">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="cec6f-296">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-296">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="cec6f-297">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="cec6f-297">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-298">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-298">Az.Sql</span></span>
* <span data-ttu-id="cec6f-299">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-299">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="cec6f-300">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-300">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cec6f-301">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-301">Az.Storage</span></span>
* <span data-ttu-id="cec6f-302">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="cec6f-302">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="cec6f-303">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-303">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="cec6f-304">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-304">Az.AnalysisServices</span></span>
* <span data-ttu-id="cec6f-305">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="cec6f-305">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cec6f-306">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cec6f-306">Az.Automation</span></span>
* <span data-ttu-id="cec6f-307">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-307">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="cec6f-308">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-308">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="cec6f-309">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-309">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cec6f-310">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-310">Az.CognitiveServices</span></span>
* <span data-ttu-id="cec6f-311">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="cec6f-311">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-312">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-312">Az.Compute</span></span>
* <span data-ttu-id="cec6f-313">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-313">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="cec6f-314">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-314">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="cec6f-315">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-315">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="cec6f-316">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="cec6f-316">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-317">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-317">Az.DataLakeStore</span></span>
* <span data-ttu-id="cec6f-318">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-318">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cec6f-319">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cec6f-319">Az.EventHub</span></span>
* <span data-ttu-id="cec6f-320">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-320">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="cec6f-321">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cec6f-321">Az.KeyVault</span></span>
* <span data-ttu-id="cec6f-322">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-322">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cec6f-323">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cec6f-323">Az.LogicApp</span></span>
* <span data-ttu-id="cec6f-324">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-324">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="cec6f-325">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-325">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="cec6f-326">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-326">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="cec6f-327">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cec6f-327">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cec6f-328">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cec6f-328">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cec6f-329">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cec6f-329">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cec6f-330">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cec6f-330">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="cec6f-331">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-331">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="cec6f-332">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cec6f-332">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cec6f-333">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cec6f-333">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cec6f-334">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cec6f-334">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cec6f-335">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cec6f-335">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="cec6f-336">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-336">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cec6f-337">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cec6f-337">Az.Monitor</span></span>
* <span data-ttu-id="cec6f-338">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-338">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-339">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-339">Az.Network</span></span>
* <span data-ttu-id="cec6f-340">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-340">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cec6f-341">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cec6f-341">Az.OperationalInsights</span></span>
* <span data-ttu-id="cec6f-342">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-342">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="cec6f-343">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-343">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="cec6f-344">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-344">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="cec6f-345">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-345">Az.Resources</span></span>
* <span data-ttu-id="cec6f-346">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="cec6f-346">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cec6f-347">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="cec6f-347">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="cec6f-348">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="cec6f-348">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="cec6f-349">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-349">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-350">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-350">Az.Sql</span></span>
* <span data-ttu-id="cec6f-351">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-351">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="cec6f-352">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-352">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cec6f-353">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-353">Az.Websites</span></span>
* <span data-ttu-id="cec6f-354">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-354">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="cec6f-355">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-355">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cec6f-356">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-356">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-357">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-357">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cec6f-358">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-358">Az.AnalysisServices</span></span>
<span data-ttu-id="cec6f-359">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="cec6f-359">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-360">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-360">Az.Compute</span></span>
* <span data-ttu-id="cec6f-361">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-361">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="cec6f-362">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-362">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="cec6f-363">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-363">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-364">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-364">Az.RecoveryServices</span></span>
<span data-ttu-id="cec6f-365">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="cec6f-365">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-366">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-366">Az.Resources</span></span>
* <span data-ttu-id="cec6f-367">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-367">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="cec6f-368">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="cec6f-368">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cec6f-369">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-369">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="cec6f-370">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="cec6f-370">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-371">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-371">Az.Sql</span></span>
* <span data-ttu-id="cec6f-372">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-372">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="cec6f-373">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-373">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="cec6f-374">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-374">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="cec6f-375">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-375">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cec6f-376">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-376">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-377">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="cec6f-377">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cec6f-378">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-378">Az.AnalysisServices</span></span>
* <span data-ttu-id="cec6f-379">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="cec6f-379">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-380">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-380">Az.RecoveryServices</span></span>
* <span data-ttu-id="cec6f-381">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="cec6f-381">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="cec6f-382">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-382">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cec6f-383">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-383">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-384">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-384">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cec6f-385">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-385">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cec6f-386">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-386">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="cec6f-387">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="cec6f-387">Az.Aks</span></span>
* <span data-ttu-id="cec6f-388">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-388">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cec6f-389">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cec6f-389">Az.Automation</span></span>
* <span data-ttu-id="cec6f-390">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-390">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="cec6f-391">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-391">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cec6f-392">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cec6f-392">Az.Cdn</span></span>
* <span data-ttu-id="cec6f-393">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-393">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-394">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-394">Az.Compute</span></span>
* <span data-ttu-id="cec6f-395">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-395">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="cec6f-396">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-396">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="cec6f-397">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-397">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="cec6f-398">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="cec6f-398">Az.ContainerRegistry</span></span>
* <span data-ttu-id="cec6f-399">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-399">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cec6f-400">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cec6f-400">Az.DataFactory</span></span>
* <span data-ttu-id="cec6f-401">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-401">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-402">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-402">Az.DataLakeStore</span></span>
* <span data-ttu-id="cec6f-403">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="cec6f-403">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="cec6f-404">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="cec6f-404">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="cec6f-405">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-405">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cec6f-406">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cec6f-406">Az.IotHub</span></span>
* <span data-ttu-id="cec6f-407">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-407">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cec6f-408">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cec6f-408">Az.KeyVault</span></span>
* <span data-ttu-id="cec6f-409">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-409">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-410">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-410">Az.Network</span></span>
* <span data-ttu-id="cec6f-411">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-411">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-412">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-412">Az.Resources</span></span>
* <span data-ttu-id="cec6f-413">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-413">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="cec6f-414">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-414">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="cec6f-415">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-415">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="cec6f-416">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="cec6f-416">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="cec6f-417">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="cec6f-417">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="cec6f-418">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-418">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="cec6f-419">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="cec6f-419">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cec6f-420">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cec6f-420">Az.ServiceFabric</span></span>
* <span data-ttu-id="cec6f-421">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="cec6f-421">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="cec6f-422">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-422">Fix some error messages.</span></span>
* <span data-ttu-id="cec6f-423">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-423">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="cec6f-424">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-424">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cec6f-425">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cec6f-425">Az.SignalR</span></span>
* <span data-ttu-id="cec6f-426">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-426">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-427">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-427">Az.Sql</span></span>
* <span data-ttu-id="cec6f-428">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-428">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cec6f-429">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-429">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="cec6f-430">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-430">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="cec6f-431">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="cec6f-431">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cec6f-432">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-432">Az.Storage</span></span>
* <span data-ttu-id="cec6f-433">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-433">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cec6f-434">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="cec6f-434">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="cec6f-435">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="cec6f-435">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="cec6f-436">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="cec6f-436">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="cec6f-437">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="cec6f-437">Az.TrafficManager</span></span>
* <span data-ttu-id="cec6f-438">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-438">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cec6f-439">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-439">Az.Websites</span></span>
* <span data-ttu-id="cec6f-440">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-440">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cec6f-441">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-441">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="cec6f-442">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="cec6f-442">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="cec6f-443">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-443">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cec6f-444">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-444">Az.Accounts</span></span>
* <span data-ttu-id="cec6f-445">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="cec6f-445">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-446">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-446">Az.Compute</span></span>
* <span data-ttu-id="cec6f-447">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-447">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="cec6f-448">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="cec6f-448">Updated the description of ID in help files</span></span>
* <span data-ttu-id="cec6f-449">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-449">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-450">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-450">Az.DataLakeStore</span></span>
* <span data-ttu-id="cec6f-451">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-451">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="cec6f-452">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-452">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cec6f-453">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cec6f-453">Az.EventGrid</span></span>
* <span data-ttu-id="cec6f-454">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-454">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="cec6f-455">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="cec6f-455">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="cec6f-456">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="cec6f-456">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cec6f-457">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="cec6f-457">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cec6f-458">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="cec6f-458">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cec6f-459">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="cec6f-459">Dead letter endpoint.</span></span>
    - <span data-ttu-id="cec6f-460">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="cec6f-460">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cec6f-461">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="cec6f-461">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cec6f-462">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="cec6f-462">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cec6f-463">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="cec6f-463">Dead letter endpoint.</span></span>
* <span data-ttu-id="cec6f-464">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-464">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="cec6f-465">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="cec6f-465">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cec6f-466">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cec6f-466">Az.IotHub</span></span>
* <span data-ttu-id="cec6f-467">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-467">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cec6f-468">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cec6f-468">Az.LogicApp</span></span>
* <span data-ttu-id="cec6f-469">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="cec6f-469">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-470">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-470">Az.Resources</span></span>
* <span data-ttu-id="cec6f-471">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-471">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="cec6f-472">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="cec6f-472">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="cec6f-473">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-473">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cec6f-474">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-474">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="cec6f-475">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="cec6f-475">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="cec6f-476">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="cec6f-476">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cec6f-477">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cec6f-477">Az.SignalR</span></span>
* <span data-ttu-id="cec6f-478">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-478">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-479">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-479">Az.Sql</span></span>
* <span data-ttu-id="cec6f-480">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-480">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cec6f-481">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-481">Az.Storage</span></span>
* <span data-ttu-id="cec6f-482">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="cec6f-482">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="cec6f-483">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cec6f-483">New-AzStorageContext</span></span>
* <span data-ttu-id="cec6f-484">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-484">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="cec6f-485">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="cec6f-485">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cec6f-486">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-486">Az.Websites</span></span>
* <span data-ttu-id="cec6f-487">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-487">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="cec6f-488">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-488">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="cec6f-489">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-489">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="cec6f-490">全般</span><span class="sxs-lookup"><span data-stu-id="cec6f-490">General</span></span>

- <span data-ttu-id="cec6f-491">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="cec6f-491">General Availability of Az Module</span></span>
- <span data-ttu-id="cec6f-492">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="cec6f-492">Online help for each module</span></span>
- <span data-ttu-id="cec6f-493">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-493">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="cec6f-494">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-494">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="cec6f-495">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cec6f-495">Az.Accounts</span></span>
- <span data-ttu-id="cec6f-496">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-496">Changed from Az.Profile</span></span>
- <span data-ttu-id="cec6f-497">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-497">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cec6f-498">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cec6f-498">Az.ApiManagement</span></span>
- <span data-ttu-id="cec6f-499">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="cec6f-499">Fixes for #7002</span></span>
- <span data-ttu-id="cec6f-500">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-500">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="cec6f-501">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cec6f-501">Az.Batch</span></span>
- <span data-ttu-id="cec6f-502">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-502">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="cec6f-503">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-503">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="cec6f-504">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-504">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="cec6f-505">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="cec6f-505">Az.Billing</span></span>
- <span data-ttu-id="cec6f-506">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-506">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="cec6f-507">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-507">Az.CognitivServices</span></span>
- <span data-ttu-id="cec6f-508">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-508">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="cec6f-509">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-509">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cec6f-510">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-510">Az.ContainerInstance</span></span>
- <span data-ttu-id="cec6f-511">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-511">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="cec6f-512">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="cec6f-512">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="cec6f-513">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-513">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-514">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-514">Az.DataLakeStore</span></span>
- <span data-ttu-id="cec6f-515">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-515">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="cec6f-516">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cec6f-516">Az.Monitor</span></span>
- <span data-ttu-id="cec6f-517">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-517">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="cec6f-518">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cec6f-518">Az.KeyVault</span></span>
- <span data-ttu-id="cec6f-519">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-519">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="cec6f-520">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cec6f-520">Az.MachineLearning</span></span>
- <span data-ttu-id="cec6f-521">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="cec6f-521">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="cec6f-522">Az.Media</span><span class="sxs-lookup"><span data-stu-id="cec6f-522">Az.Media</span></span>
- <span data-ttu-id="cec6f-523">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-523">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cec6f-524">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-524">Az.Network</span></span>
<span data-ttu-id="cec6f-525">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-525">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="cec6f-526">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cec6f-526">New cmdlets added:</span></span>
        - <span data-ttu-id="cec6f-527">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cec6f-527">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cec6f-528">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cec6f-528">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cec6f-529">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cec6f-529">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cec6f-530">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cec6f-530">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cec6f-531">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cec6f-531">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cec6f-532">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="cec6f-532">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="cec6f-533">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="cec6f-533">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="cec6f-534">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="cec6f-534">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="cec6f-535">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-535">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="cec6f-536">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="cec6f-536">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="cec6f-537">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cec6f-537">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cec6f-538">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cec6f-538">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cec6f-539">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cec6f-539">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="cec6f-540">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="cec6f-540">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="cec6f-541">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-541">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="cec6f-542">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-542">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="cec6f-543">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cec6f-543">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cec6f-544">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cec6f-544">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cec6f-545">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cec6f-545">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="cec6f-546">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-546">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="cec6f-547">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-547">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="cec6f-548">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cec6f-548">Az.OperationalInsights</span></span>
- <span data-ttu-id="cec6f-549">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-549">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="cec6f-550">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cec6f-550">Az.Profile</span></span>
- <span data-ttu-id="cec6f-551">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-551">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-552">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-552">Az.RecoveryServices</span></span>
- <span data-ttu-id="cec6f-553">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-553">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="cec6f-554">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-554">Az.Resources</span></span>
- <span data-ttu-id="cec6f-555">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-555">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cec6f-556">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cec6f-556">Az.ServiceFabric</span></span>
- <span data-ttu-id="cec6f-557">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="cec6f-557">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="cec6f-558">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-558">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="cec6f-559">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="cec6f-559">Az.SIgnalR</span></span>
- <span data-ttu-id="cec6f-560">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="cec6f-560">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="cec6f-561">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-561">Az.Sql</span></span>
- <span data-ttu-id="cec6f-562">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-562">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="cec6f-563">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-563">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="cec6f-564">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-564">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="cec6f-565">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-565">Az.Storage</span></span>
- <span data-ttu-id="cec6f-566">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-566">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cec6f-567">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-567">Az.Websites</span></span>
- <span data-ttu-id="cec6f-568">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cec6f-568">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="cec6f-569">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-569">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="cec6f-570">全般</span><span class="sxs-lookup"><span data-stu-id="cec6f-570">General</span></span>

* <span data-ttu-id="cec6f-571">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="cec6f-571">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="cec6f-572">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-572">Az.Compute</span></span>

* <span data-ttu-id="cec6f-573">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-573">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-574">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-574">Az.DataLakeStore</span></span>

* <span data-ttu-id="cec6f-575">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-575">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="cec6f-576">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cec6f-576">Az.FrontDoor</span></span>

* <span data-ttu-id="cec6f-577">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-577">Fixed some broken links</span></span>
    - <span data-ttu-id="cec6f-578">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-578">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="cec6f-579">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-579">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cec6f-580">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-580">Az.RecoveryServices</span></span>

* <span data-ttu-id="cec6f-581">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-581">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="cec6f-582">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-582">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="cec6f-583">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-583">Az.Resources</span></span>

* <span data-ttu-id="cec6f-584">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-584">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="cec6f-585">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-585">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="cec6f-586">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-586">Az.Sql</span></span>

* <span data-ttu-id="cec6f-587">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="cec6f-587">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="cec6f-588">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-588">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="cec6f-589">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-589">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="cec6f-590">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-590">Az.Storage</span></span>

* <span data-ttu-id="cec6f-591">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-591">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="cec6f-592">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-592">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="cec6f-593">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cec6f-593">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cec6f-594">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="cec6f-594">Support Static Website configuration</span></span>
    - <span data-ttu-id="cec6f-595">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cec6f-595">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="cec6f-596">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cec6f-596">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cec6f-597">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-597">Az.Websites</span></span>

* <span data-ttu-id="cec6f-598">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="cec6f-598">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="cec6f-599">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-599">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="cec6f-600">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="cec6f-600">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="cec6f-601">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-601">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cec6f-602">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cec6f-602">Az.ApiManagement</span></span>
* <span data-ttu-id="cec6f-603">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-603">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="cec6f-604">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cec6f-604">Az.Automation</span></span>
* <span data-ttu-id="cec6f-605">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="cec6f-605">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="cec6f-606">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-606">Added Update Management cmdlets</span></span>
* <span data-ttu-id="cec6f-607">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-607">Added Source Control cmdlets</span></span>
* <span data-ttu-id="cec6f-608">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-608">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="cec6f-609">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-609">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="cec6f-610">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-610">Az.Compute</span></span>
* <span data-ttu-id="cec6f-611">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-611">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="cec6f-612">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-612">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cec6f-613">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-613">Az.ContainerInstance</span></span>
* <span data-ttu-id="cec6f-614">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-614">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="cec6f-615">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="cec6f-615">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="cec6f-616">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-616">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cec6f-617">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-617">Az.Network</span></span>
* <span data-ttu-id="cec6f-618">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-618">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="cec6f-619">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-619">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="cec6f-620">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-620">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="cec6f-621">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-621">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="cec6f-622">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="cec6f-622">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="cec6f-623">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-623">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="cec6f-624">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-624">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="cec6f-625">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="cec6f-625">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="cec6f-626">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-626">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="cec6f-627">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-627">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="cec6f-628">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="cec6f-628">Az.Relay</span></span>
* <span data-ttu-id="cec6f-629">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="cec6f-629">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="cec6f-630">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-630">Az.Resources</span></span>
* <span data-ttu-id="cec6f-631">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-631">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="cec6f-632">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-632">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="cec6f-633">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="cec6f-633">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cec6f-634">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cec6f-634">Az.ServiceFabric</span></span>
* <span data-ttu-id="cec6f-635">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-635">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="cec6f-636">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-636">Az.Sql</span></span>
* <span data-ttu-id="cec6f-637">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-637">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="cec6f-638">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-638">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cec6f-639">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-639">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cec6f-640">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-640">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cec6f-641">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cec6f-641">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cec6f-642">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cec6f-642">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cec6f-643">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cec6f-643">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cec6f-644">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cec6f-644">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cec6f-645">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cec6f-645">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="cec6f-646">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="cec6f-646">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="cec6f-647">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-647">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="cec6f-648">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-648">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="cec6f-649">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="cec6f-649">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cec6f-650">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="cec6f-650">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cec6f-651">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="cec6f-651">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="cec6f-652">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="cec6f-652">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="cec6f-653">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-653">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="cec6f-654">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-654">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="cec6f-655">全般</span><span class="sxs-lookup"><span data-stu-id="cec6f-655">General</span></span>
* <span data-ttu-id="cec6f-656">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="cec6f-656">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="cec6f-657">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cec6f-657">Az.Profile</span></span>
* <span data-ttu-id="cec6f-658">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-658">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="cec6f-659">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-659">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="cec6f-660">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-660">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="cec6f-661">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-661">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="cec6f-662">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-662">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="cec6f-663">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-663">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="cec6f-664">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-664">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="cec6f-665">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-665">Az.CognitiveServices</span></span>
* <span data-ttu-id="cec6f-666">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-666">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-667">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-667">Az.Compute</span></span>
* <span data-ttu-id="cec6f-668">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-668">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="cec6f-669">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="cec6f-669">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="cec6f-670">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-670">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-671">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-671">Az.DataLakeStore</span></span>
* <span data-ttu-id="cec6f-672">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-672">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="cec6f-673">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-673">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="cec6f-674">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="cec6f-674">Az.Insights</span></span>
* <span data-ttu-id="cec6f-675">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-675">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="cec6f-676">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="cec6f-676">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="cec6f-677">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-677">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="cec6f-678">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="cec6f-678">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-679">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-679">Az.Network</span></span>
* <span data-ttu-id="cec6f-680">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="cec6f-680">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="cec6f-681">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="cec6f-681">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="cec6f-682">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="cec6f-682">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="cec6f-683">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cec6f-683">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="cec6f-684">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="cec6f-684">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="cec6f-685">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="cec6f-685">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="cec6f-686">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cec6f-686">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cec6f-687">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cec6f-687">Az.PolicyInsights</span></span>
* <span data-ttu-id="cec6f-688">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-688">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-689">Az.Resources</span></span>
* <span data-ttu-id="cec6f-690">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-690">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="cec6f-691">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-691">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cec6f-692">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cec6f-692">Az.ServiceBus</span></span>
* <span data-ttu-id="cec6f-693">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-693">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cec6f-694">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cec6f-694">Az.ServiceFabric</span></span>
* <span data-ttu-id="cec6f-695">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-695">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="cec6f-696">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-696">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="cec6f-697">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="cec6f-697">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="cec6f-698">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="cec6f-698">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="cec6f-699">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-699">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="cec6f-700">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-700">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="cec6f-701">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cec6f-701">Az.Profile</span></span>
* <span data-ttu-id="cec6f-702">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-702">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="cec6f-703">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-703">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-704">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-704">Az.Compute</span></span>
* <span data-ttu-id="cec6f-705">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-705">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="cec6f-706">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-706">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cec6f-707">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cec6f-707">Az.DataLakeStore</span></span>
* <span data-ttu-id="cec6f-708">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-708">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="cec6f-709">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cec6f-709">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="cec6f-710">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="cec6f-710">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cec6f-711">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="cec6f-711">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cec6f-712">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="cec6f-712">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-713">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-713">Az.Network</span></span>
* <span data-ttu-id="cec6f-714">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-714">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="cec6f-715">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-715">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-716">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-716">Az.Resources</span></span>
* <span data-ttu-id="cec6f-717">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-717">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="cec6f-718">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-718">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="cec6f-719">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-719">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="cec6f-720">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="cec6f-720">Azure.Storage</span></span>
* <span data-ttu-id="cec6f-721">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-721">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="cec6f-722">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="cec6f-722">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="cec6f-723">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cec6f-723">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cec6f-724">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-724">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="cec6f-725">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="cec6f-725">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="cec6f-726">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cec6f-726">Az.CognitiveServices</span></span>
* <span data-ttu-id="cec6f-727">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-727">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cec6f-728">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cec6f-728">Az.Compute</span></span>
* <span data-ttu-id="cec6f-729">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-729">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="cec6f-730">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-730">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="cec6f-731">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-731">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="cec6f-732">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="cec6f-732">Az.DataFactoryV2</span></span>
* <span data-ttu-id="cec6f-733">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-733">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cec6f-734">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cec6f-734">Az.Network</span></span>
* <span data-ttu-id="cec6f-735">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cec6f-735">Added NetworkProfile functionality.</span></span> <span data-ttu-id="cec6f-736">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cec6f-736">new cmdlets added</span></span>
    - <span data-ttu-id="cec6f-737">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cec6f-737">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="cec6f-738">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cec6f-738">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="cec6f-739">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cec6f-739">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="cec6f-740">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cec6f-740">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="cec6f-741">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="cec6f-741">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="cec6f-742">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="cec6f-742">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="cec6f-743">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-743">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="cec6f-744">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-744">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="cec6f-745">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-745">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cec6f-746">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cec6f-746">Az.RedisCache</span></span>
* <span data-ttu-id="cec6f-747">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="cec6f-747">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="cec6f-748">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-748">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="cec6f-749">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cec6f-749">Az.Resources</span></span>
* <span data-ttu-id="cec6f-750">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-750">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cec6f-751">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-751">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="cec6f-752">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cec6f-752">Az.Sql</span></span>
* <span data-ttu-id="cec6f-753">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cec6f-753">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cec6f-754">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cec6f-754">Az.Websites</span></span>
* <span data-ttu-id="cec6f-755">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="cec6f-755">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="cec6f-756">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="cec6f-756">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="cec6f-757">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="cec6f-757">0.2.0 - September 2018</span></span>
 <span data-ttu-id="cec6f-758">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="cec6f-758">Initial Release</span></span>