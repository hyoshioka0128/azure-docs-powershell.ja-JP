---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/30/2019
ms.openlocfilehash: 8a9a399f72ed9e3e9a3cbc09c8a4abaa91339c24
ms.sourcegitcommit: f0f09eee03ef9dd7fe07432252a3dc8ca93e3a7b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2019
ms.locfileid: "71319304"
---
## <a name="180---april-2019"></a><span data-ttu-id="1f87f-103">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-103">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1f87f-104">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="1f87f-104">Highlights since the last major release</span></span>
* <span data-ttu-id="1f87f-105">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="1f87f-105">General availability of `Az` module</span></span>
* <span data-ttu-id="1f87f-106">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1f87f-106">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1f87f-107">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1f87f-107">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1f87f-108">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-108">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1f87f-109">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-109">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1f87f-110">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-110">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1f87f-111">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-111">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1f87f-112">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-112">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-113">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-113">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1f87f-114">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1f87f-114">Az.Batch</span></span>
* <span data-ttu-id="1f87f-115">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-115">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1f87f-116">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1f87f-116">Az.Cdn</span></span>
* <span data-ttu-id="1f87f-117">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-117">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1f87f-118">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-118">Az.CognitiveServices</span></span>
* <span data-ttu-id="1f87f-119">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-119">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-120">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-120">Az.Compute</span></span>
* <span data-ttu-id="1f87f-121">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-121">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="1f87f-122">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-122">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1f87f-123">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-123">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1f87f-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1f87f-124">Az.DataFactory</span></span>
* <span data-ttu-id="1f87f-125">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-125">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-126">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-126">Az.DataLakeStore</span></span>
* <span data-ttu-id="1f87f-127">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-127">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1f87f-128">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1f87f-128">Az.EventGrid</span></span>
* <span data-ttu-id="1f87f-129">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-129">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1f87f-130">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1f87f-130">Az.EventHub</span></span>
* <span data-ttu-id="1f87f-131">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-131">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="1f87f-132">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1f87f-132">Az.HDInsight</span></span>
* <span data-ttu-id="1f87f-133">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-133">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1f87f-134">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1f87f-134">Az.IotHub</span></span>
* <span data-ttu-id="1f87f-135">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-135">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1f87f-136">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f87f-136">Az.KeyVault</span></span>
* <span data-ttu-id="1f87f-137">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-137">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1f87f-138">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-138">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="1f87f-139">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1f87f-139">Az.MachineLearning</span></span>
* <span data-ttu-id="1f87f-140">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-140">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="1f87f-141">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1f87f-141">Az.Media</span></span>
* <span data-ttu-id="1f87f-142">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-142">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1f87f-143">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1f87f-143">Az.Monitor</span></span>
  * <span data-ttu-id="1f87f-144">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-144">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="1f87f-145">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="1f87f-145">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="1f87f-146">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="1f87f-146">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="1f87f-147">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1f87f-147">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1f87f-148">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1f87f-148">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1f87f-149">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1f87f-149">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="1f87f-150">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-150">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-151">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-151">Az.Network</span></span>
* <span data-ttu-id="1f87f-152">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-152">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1f87f-153">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-153">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="1f87f-154">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="1f87f-154">Az.NotificationHubs</span></span>
* <span data-ttu-id="1f87f-155">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-155">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1f87f-156">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1f87f-156">Az.OperationalInsights</span></span>
* <span data-ttu-id="1f87f-157">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-157">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="1f87f-158">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1f87f-158">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="1f87f-159">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-159">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-160">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-160">Az.RecoveryServices</span></span>
* <span data-ttu-id="1f87f-161">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-161">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1f87f-162">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-162">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="1f87f-163">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-163">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="1f87f-164">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-164">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1f87f-165">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1f87f-165">Az.RedisCache</span></span>
* <span data-ttu-id="1f87f-166">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-166">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-167">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-167">Az.Resources</span></span>
* <span data-ttu-id="1f87f-168">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-168">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-169">Az.Sql</span></span>
* <span data-ttu-id="1f87f-170">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="1f87f-170">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="1f87f-171">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-171">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1f87f-172">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-172">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="1f87f-173">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-173">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="1f87f-174">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="1f87f-174">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="1f87f-175">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="1f87f-175">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="1f87f-176">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-176">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1f87f-177">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-177">Az.Websites</span></span>
* <span data-ttu-id="1f87f-178">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-178">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="1f87f-179">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-179">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1f87f-180">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-180">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="1f87f-181">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-181">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="1f87f-182">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-182">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1f87f-183">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="1f87f-183">Highlights since the last major release</span></span>
* <span data-ttu-id="1f87f-184">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="1f87f-184">General availability of `Az` module</span></span>
* <span data-ttu-id="1f87f-185">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1f87f-185">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1f87f-186">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1f87f-186">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1f87f-187">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-187">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1f87f-188">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-188">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1f87f-189">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-189">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1f87f-190">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-190">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1f87f-191">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-191">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-192">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-192">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1f87f-193">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-193">Az.AnalysisServices</span></span>
* <span data-ttu-id="1f87f-194">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="1f87f-194">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="1f87f-195">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-195">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1f87f-196">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1f87f-196">Az.Automation</span></span>
* <span data-ttu-id="1f87f-197">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-197">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="1f87f-198">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-198">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="1f87f-199">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-199">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-200">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-200">Az.Compute</span></span>
* <span data-ttu-id="1f87f-201">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-201">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1f87f-202">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-202">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="1f87f-203">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-203">Az.ContainerInstance</span></span>
* <span data-ttu-id="1f87f-204">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-204">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1f87f-205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1f87f-205">Az.DataFactory</span></span>
* <span data-ttu-id="1f87f-206">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-206">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="1f87f-207">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-207">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-208">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-208">Az.Resources</span></span>
* <span data-ttu-id="1f87f-209">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-209">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="1f87f-210">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-210">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="1f87f-211">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="1f87f-211">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="1f87f-212">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1f87f-212">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="1f87f-213">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-213">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="1f87f-214">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1f87f-214">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-215">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-215">Az.Sql</span></span>
* <span data-ttu-id="1f87f-216">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-216">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1f87f-217">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-217">Az.Storage</span></span>
* <span data-ttu-id="1f87f-218">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="1f87f-218">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="1f87f-219">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1f87f-219">New-AzStorageContext</span></span>
* <span data-ttu-id="1f87f-220">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="1f87f-220">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="1f87f-221">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1f87f-221">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1f87f-222">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1f87f-222">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1f87f-223">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1f87f-223">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="1f87f-224">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1f87f-224">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="1f87f-225">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="1f87f-225">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="1f87f-226">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1f87f-226">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1f87f-227">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1f87f-227">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1f87f-228">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1f87f-228">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="1f87f-229">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1f87f-229">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="1f87f-230">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-230">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1f87f-231">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="1f87f-231">Highlights since the last major release</span></span>
* <span data-ttu-id="1f87f-232">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="1f87f-232">General availability of `Az` module</span></span>
* <span data-ttu-id="1f87f-233">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1f87f-233">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1f87f-234">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1f87f-234">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1f87f-235">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-235">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1f87f-236">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-236">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1f87f-237">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-237">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1f87f-238">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-238">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1f87f-239">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1f87f-239">Az.Automation</span></span>
* <span data-ttu-id="1f87f-240">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-240">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="1f87f-241">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="1f87f-241">Dynamic grouping</span></span>
    * <span data-ttu-id="1f87f-242">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="1f87f-242">Pre-Post script</span></span>
    * <span data-ttu-id="1f87f-243">再起動設定</span><span class="sxs-lookup"><span data-stu-id="1f87f-243">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-244">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-244">Az.Compute</span></span>
* <span data-ttu-id="1f87f-245">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-245">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="1f87f-246">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-246">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1f87f-247">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f87f-247">Az.KeyVault</span></span>
* <span data-ttu-id="1f87f-248">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-248">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-249">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-249">Az.Network</span></span>
* <span data-ttu-id="1f87f-250">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-250">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="1f87f-251">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-251">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-252">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-252">Az.RecoveryServices</span></span>
* <span data-ttu-id="1f87f-253">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-253">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="1f87f-254">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-254">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-255">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-255">Az.Resources</span></span>
* <span data-ttu-id="1f87f-256">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-256">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="1f87f-257">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-257">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-258">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-258">Az.Sql</span></span>
* <span data-ttu-id="1f87f-259">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-259">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1f87f-260">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-260">Az.Storage</span></span>
* <span data-ttu-id="1f87f-261">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="1f87f-261">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="1f87f-262">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1f87f-262">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1f87f-263">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1f87f-263">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1f87f-264">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1f87f-264">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1f87f-265">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="1f87f-265">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="1f87f-266">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="1f87f-266">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="1f87f-267">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="1f87f-267">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1f87f-268">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-268">Az.Websites</span></span>
* <span data-ttu-id="1f87f-269">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-269">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="1f87f-270">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-270">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1f87f-271">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-271">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-272">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-272">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="1f87f-273">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-273">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1f87f-274">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1f87f-274">Az.Automation</span></span>
* <span data-ttu-id="1f87f-275">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-275">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="1f87f-276">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-276">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="1f87f-277">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="1f87f-277">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1f87f-278">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1f87f-278">Az.Cdn</span></span>
* <span data-ttu-id="1f87f-279">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="1f87f-279">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-280">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-280">Az.Compute</span></span>
* <span data-ttu-id="1f87f-281">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-281">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1f87f-282">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1f87f-282">Az.DataFactory</span></span>
* <span data-ttu-id="1f87f-283">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-283">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1f87f-284">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1f87f-284">Az.LogicApp</span></span>
* <span data-ttu-id="1f87f-285">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-285">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-286">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-286">Az.Network</span></span>
* <span data-ttu-id="1f87f-287">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-287">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-288">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-288">Az.RecoveryServices</span></span>
* <span data-ttu-id="1f87f-289">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-289">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="1f87f-290">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-290">SDK Update</span></span>
* <span data-ttu-id="1f87f-291">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-291">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="1f87f-292">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-292">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-293">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-293">Az.Resources</span></span>
* <span data-ttu-id="1f87f-294">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-294">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="1f87f-295">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="1f87f-295">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="1f87f-296">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-296">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="1f87f-297">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="1f87f-297">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="1f87f-298">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-298">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="1f87f-299">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="1f87f-299">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-300">Az.Sql</span></span>
* <span data-ttu-id="1f87f-301">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-301">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="1f87f-302">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-302">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1f87f-303">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-303">Az.Storage</span></span>
* <span data-ttu-id="1f87f-304">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="1f87f-304">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="1f87f-305">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-305">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="1f87f-306">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-306">Az.AnalysisServices</span></span>
* <span data-ttu-id="1f87f-307">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="1f87f-307">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1f87f-308">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1f87f-308">Az.Automation</span></span>
* <span data-ttu-id="1f87f-309">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-309">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="1f87f-310">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-310">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="1f87f-311">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-311">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1f87f-312">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-312">Az.CognitiveServices</span></span>
* <span data-ttu-id="1f87f-313">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1f87f-313">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-314">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-314">Az.Compute</span></span>
* <span data-ttu-id="1f87f-315">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-315">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="1f87f-316">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-316">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="1f87f-317">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-317">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="1f87f-318">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="1f87f-318">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-319">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-319">Az.DataLakeStore</span></span>
* <span data-ttu-id="1f87f-320">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-320">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1f87f-321">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1f87f-321">Az.EventHub</span></span>
* <span data-ttu-id="1f87f-322">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-322">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="1f87f-323">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f87f-323">Az.KeyVault</span></span>
* <span data-ttu-id="1f87f-324">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-324">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1f87f-325">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1f87f-325">Az.LogicApp</span></span>
* <span data-ttu-id="1f87f-326">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-326">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="1f87f-327">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-327">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="1f87f-328">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-328">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="1f87f-329">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1f87f-329">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1f87f-330">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1f87f-330">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1f87f-331">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1f87f-331">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1f87f-332">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1f87f-332">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="1f87f-333">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-333">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="1f87f-334">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f87f-334">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1f87f-335">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f87f-335">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1f87f-336">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f87f-336">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1f87f-337">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f87f-337">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="1f87f-338">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-338">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1f87f-339">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1f87f-339">Az.Monitor</span></span>
* <span data-ttu-id="1f87f-340">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-340">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-341">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-341">Az.Network</span></span>
* <span data-ttu-id="1f87f-342">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-342">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1f87f-343">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1f87f-343">Az.OperationalInsights</span></span>
* <span data-ttu-id="1f87f-344">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-344">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="1f87f-345">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-345">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="1f87f-346">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-346">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="1f87f-347">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-347">Az.Resources</span></span>
* <span data-ttu-id="1f87f-348">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1f87f-348">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1f87f-349">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1f87f-349">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="1f87f-350">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="1f87f-350">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="1f87f-351">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-351">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-352">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-352">Az.Sql</span></span>
* <span data-ttu-id="1f87f-353">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-353">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="1f87f-354">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-354">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1f87f-355">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-355">Az.Websites</span></span>
* <span data-ttu-id="1f87f-356">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-356">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="1f87f-357">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-357">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1f87f-358">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-358">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-359">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-359">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1f87f-360">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-360">Az.AnalysisServices</span></span>
<span data-ttu-id="1f87f-361">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="1f87f-361">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-362">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-362">Az.Compute</span></span>
* <span data-ttu-id="1f87f-363">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-363">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="1f87f-364">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-364">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="1f87f-365">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-365">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-366">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-366">Az.RecoveryServices</span></span>
<span data-ttu-id="1f87f-367">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="1f87f-367">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-368">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-368">Az.Resources</span></span>
* <span data-ttu-id="1f87f-369">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-369">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="1f87f-370">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1f87f-370">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1f87f-371">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-371">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="1f87f-372">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1f87f-372">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-373">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-373">Az.Sql</span></span>
* <span data-ttu-id="1f87f-374">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-374">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="1f87f-375">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-375">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="1f87f-376">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-376">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="1f87f-377">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-377">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1f87f-378">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-378">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-379">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="1f87f-379">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1f87f-380">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-380">Az.AnalysisServices</span></span>
* <span data-ttu-id="1f87f-381">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="1f87f-381">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-382">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-382">Az.RecoveryServices</span></span>
* <span data-ttu-id="1f87f-383">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="1f87f-383">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="1f87f-384">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-384">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1f87f-385">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-385">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-386">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-386">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1f87f-387">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-387">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1f87f-388">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-388">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="1f87f-389">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="1f87f-389">Az.Aks</span></span>
* <span data-ttu-id="1f87f-390">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-390">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1f87f-391">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1f87f-391">Az.Automation</span></span>
* <span data-ttu-id="1f87f-392">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-392">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="1f87f-393">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-393">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1f87f-394">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1f87f-394">Az.Cdn</span></span>
* <span data-ttu-id="1f87f-395">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-395">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-396">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-396">Az.Compute</span></span>
* <span data-ttu-id="1f87f-397">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-397">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="1f87f-398">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-398">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="1f87f-399">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-399">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="1f87f-400">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1f87f-400">Az.ContainerRegistry</span></span>
* <span data-ttu-id="1f87f-401">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-401">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1f87f-402">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1f87f-402">Az.DataFactory</span></span>
* <span data-ttu-id="1f87f-403">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-403">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-404">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-404">Az.DataLakeStore</span></span>
* <span data-ttu-id="1f87f-405">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="1f87f-405">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="1f87f-406">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="1f87f-406">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="1f87f-407">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-407">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1f87f-408">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1f87f-408">Az.IotHub</span></span>
* <span data-ttu-id="1f87f-409">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-409">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1f87f-410">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f87f-410">Az.KeyVault</span></span>
* <span data-ttu-id="1f87f-411">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-411">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-412">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-412">Az.Network</span></span>
* <span data-ttu-id="1f87f-413">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-413">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-414">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-414">Az.Resources</span></span>
* <span data-ttu-id="1f87f-415">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-415">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="1f87f-416">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-416">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="1f87f-417">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-417">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="1f87f-418">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="1f87f-418">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="1f87f-419">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="1f87f-419">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="1f87f-420">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-420">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="1f87f-421">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="1f87f-421">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1f87f-422">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f87f-422">Az.ServiceFabric</span></span>
* <span data-ttu-id="1f87f-423">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="1f87f-423">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="1f87f-424">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-424">Fix some error messages.</span></span>
* <span data-ttu-id="1f87f-425">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-425">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="1f87f-426">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-426">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1f87f-427">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1f87f-427">Az.SignalR</span></span>
* <span data-ttu-id="1f87f-428">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-428">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-429">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-429">Az.Sql</span></span>
* <span data-ttu-id="1f87f-430">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-430">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1f87f-431">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-431">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="1f87f-432">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-432">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="1f87f-433">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="1f87f-433">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1f87f-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-434">Az.Storage</span></span>
* <span data-ttu-id="1f87f-435">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-435">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1f87f-436">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="1f87f-436">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="1f87f-437">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="1f87f-437">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="1f87f-438">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="1f87f-438">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="1f87f-439">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1f87f-439">Az.TrafficManager</span></span>
* <span data-ttu-id="1f87f-440">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-440">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1f87f-441">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-441">Az.Websites</span></span>
* <span data-ttu-id="1f87f-442">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-442">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1f87f-443">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-443">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="1f87f-444">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="1f87f-444">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="1f87f-445">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-445">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1f87f-446">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-446">Az.Accounts</span></span>
* <span data-ttu-id="1f87f-447">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="1f87f-447">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-448">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-448">Az.Compute</span></span>
* <span data-ttu-id="1f87f-449">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-449">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="1f87f-450">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="1f87f-450">Updated the description of ID in help files</span></span>
* <span data-ttu-id="1f87f-451">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-451">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-452">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-452">Az.DataLakeStore</span></span>
* <span data-ttu-id="1f87f-453">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-453">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="1f87f-454">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-454">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1f87f-455">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1f87f-455">Az.EventGrid</span></span>
* <span data-ttu-id="1f87f-456">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-456">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="1f87f-457">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="1f87f-457">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="1f87f-458">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="1f87f-458">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1f87f-459">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="1f87f-459">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1f87f-460">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="1f87f-460">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1f87f-461">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="1f87f-461">Dead letter endpoint.</span></span>
    - <span data-ttu-id="1f87f-462">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="1f87f-462">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1f87f-463">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="1f87f-463">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1f87f-464">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="1f87f-464">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1f87f-465">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="1f87f-465">Dead letter endpoint.</span></span>
* <span data-ttu-id="1f87f-466">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-466">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="1f87f-467">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="1f87f-467">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1f87f-468">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1f87f-468">Az.IotHub</span></span>
* <span data-ttu-id="1f87f-469">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-469">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1f87f-470">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1f87f-470">Az.LogicApp</span></span>
* <span data-ttu-id="1f87f-471">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="1f87f-471">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-472">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-472">Az.Resources</span></span>
* <span data-ttu-id="1f87f-473">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-473">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="1f87f-474">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="1f87f-474">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="1f87f-475">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-475">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1f87f-476">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-476">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="1f87f-477">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="1f87f-477">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="1f87f-478">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="1f87f-478">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1f87f-479">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1f87f-479">Az.SignalR</span></span>
* <span data-ttu-id="1f87f-480">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-480">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-481">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-481">Az.Sql</span></span>
* <span data-ttu-id="1f87f-482">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-482">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1f87f-483">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-483">Az.Storage</span></span>
* <span data-ttu-id="1f87f-484">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="1f87f-484">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="1f87f-485">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1f87f-485">New-AzStorageContext</span></span>
* <span data-ttu-id="1f87f-486">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-486">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="1f87f-487">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="1f87f-487">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1f87f-488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-488">Az.Websites</span></span>
* <span data-ttu-id="1f87f-489">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-489">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="1f87f-490">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-490">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="1f87f-491">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-491">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="1f87f-492">全般</span><span class="sxs-lookup"><span data-stu-id="1f87f-492">General</span></span>

- <span data-ttu-id="1f87f-493">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="1f87f-493">General Availability of Az Module</span></span>
- <span data-ttu-id="1f87f-494">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="1f87f-494">Online help for each module</span></span>
- <span data-ttu-id="1f87f-495">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-495">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="1f87f-496">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-496">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="1f87f-497">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1f87f-497">Az.Accounts</span></span>
- <span data-ttu-id="1f87f-498">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-498">Changed from Az.Profile</span></span>
- <span data-ttu-id="1f87f-499">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-499">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1f87f-500">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1f87f-500">Az.ApiManagement</span></span>
- <span data-ttu-id="1f87f-501">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="1f87f-501">Fixes for #7002</span></span>
- <span data-ttu-id="1f87f-502">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-502">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="1f87f-503">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1f87f-503">Az.Batch</span></span>
- <span data-ttu-id="1f87f-504">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-504">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="1f87f-505">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-505">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="1f87f-506">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-506">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="1f87f-507">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="1f87f-507">Az.Billing</span></span>
- <span data-ttu-id="1f87f-508">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-508">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="1f87f-509">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-509">Az.CognitivServices</span></span>
- <span data-ttu-id="1f87f-510">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-510">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="1f87f-511">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-511">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1f87f-512">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-512">Az.ContainerInstance</span></span>
- <span data-ttu-id="1f87f-513">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-513">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="1f87f-514">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1f87f-514">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="1f87f-515">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-515">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-516">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-516">Az.DataLakeStore</span></span>
- <span data-ttu-id="1f87f-517">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-517">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="1f87f-518">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1f87f-518">Az.Monitor</span></span>
- <span data-ttu-id="1f87f-519">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-519">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="1f87f-520">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1f87f-520">Az.KeyVault</span></span>
- <span data-ttu-id="1f87f-521">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-521">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="1f87f-522">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1f87f-522">Az.MachineLearning</span></span>
- <span data-ttu-id="1f87f-523">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="1f87f-523">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="1f87f-524">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1f87f-524">Az.Media</span></span>
- <span data-ttu-id="1f87f-525">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-525">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1f87f-526">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-526">Az.Network</span></span>
<span data-ttu-id="1f87f-527">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-527">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="1f87f-528">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="1f87f-528">New cmdlets added:</span></span>
        - <span data-ttu-id="1f87f-529">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1f87f-529">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1f87f-530">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1f87f-530">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1f87f-531">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1f87f-531">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1f87f-532">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1f87f-532">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1f87f-533">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1f87f-533">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1f87f-534">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="1f87f-534">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="1f87f-535">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="1f87f-535">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="1f87f-536">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="1f87f-536">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="1f87f-537">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-537">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="1f87f-538">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1f87f-538">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="1f87f-539">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1f87f-539">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1f87f-540">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1f87f-540">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1f87f-541">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1f87f-541">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="1f87f-542">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="1f87f-542">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="1f87f-543">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-543">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="1f87f-544">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-544">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="1f87f-545">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1f87f-545">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1f87f-546">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1f87f-546">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1f87f-547">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1f87f-547">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="1f87f-548">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-548">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="1f87f-549">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-549">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="1f87f-550">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1f87f-550">Az.OperationalInsights</span></span>
- <span data-ttu-id="1f87f-551">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-551">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="1f87f-552">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1f87f-552">Az.Profile</span></span>
- <span data-ttu-id="1f87f-553">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-553">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-554">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-554">Az.RecoveryServices</span></span>
- <span data-ttu-id="1f87f-555">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-555">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="1f87f-556">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-556">Az.Resources</span></span>
- <span data-ttu-id="1f87f-557">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-557">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1f87f-558">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f87f-558">Az.ServiceFabric</span></span>
- <span data-ttu-id="1f87f-559">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="1f87f-559">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="1f87f-560">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-560">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="1f87f-561">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="1f87f-561">Az.SIgnalR</span></span>
- <span data-ttu-id="1f87f-562">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="1f87f-562">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="1f87f-563">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-563">Az.Sql</span></span>
- <span data-ttu-id="1f87f-564">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-564">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="1f87f-565">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-565">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="1f87f-566">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-566">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="1f87f-567">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-567">Az.Storage</span></span>
- <span data-ttu-id="1f87f-568">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-568">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1f87f-569">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-569">Az.Websites</span></span>
- <span data-ttu-id="1f87f-570">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1f87f-570">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="1f87f-571">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-571">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="1f87f-572">全般</span><span class="sxs-lookup"><span data-stu-id="1f87f-572">General</span></span>

* <span data-ttu-id="1f87f-573">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="1f87f-573">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="1f87f-574">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-574">Az.Compute</span></span>

* <span data-ttu-id="1f87f-575">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-575">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-576">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-576">Az.DataLakeStore</span></span>

* <span data-ttu-id="1f87f-577">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-577">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="1f87f-578">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1f87f-578">Az.FrontDoor</span></span>

* <span data-ttu-id="1f87f-579">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-579">Fixed some broken links</span></span>
    - <span data-ttu-id="1f87f-580">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-580">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="1f87f-581">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-581">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1f87f-582">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-582">Az.RecoveryServices</span></span>

* <span data-ttu-id="1f87f-583">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-583">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="1f87f-584">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-584">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="1f87f-585">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-585">Az.Resources</span></span>

* <span data-ttu-id="1f87f-586">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-586">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="1f87f-587">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-587">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="1f87f-588">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-588">Az.Sql</span></span>

* <span data-ttu-id="1f87f-589">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="1f87f-589">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="1f87f-590">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-590">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="1f87f-591">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-591">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="1f87f-592">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-592">Az.Storage</span></span>

* <span data-ttu-id="1f87f-593">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-593">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="1f87f-594">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-594">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="1f87f-595">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1f87f-595">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1f87f-596">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="1f87f-596">Support Static Website configuration</span></span>
    - <span data-ttu-id="1f87f-597">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1f87f-597">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="1f87f-598">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1f87f-598">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1f87f-599">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-599">Az.Websites</span></span>

* <span data-ttu-id="1f87f-600">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="1f87f-600">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="1f87f-601">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-601">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="1f87f-602">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="1f87f-602">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="1f87f-603">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-603">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1f87f-604">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1f87f-604">Az.ApiManagement</span></span>
* <span data-ttu-id="1f87f-605">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-605">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="1f87f-606">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1f87f-606">Az.Automation</span></span>
* <span data-ttu-id="1f87f-607">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="1f87f-607">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="1f87f-608">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-608">Added Update Management cmdlets</span></span>
* <span data-ttu-id="1f87f-609">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-609">Added Source Control cmdlets</span></span>
* <span data-ttu-id="1f87f-610">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-610">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="1f87f-611">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-611">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="1f87f-612">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-612">Az.Compute</span></span>
* <span data-ttu-id="1f87f-613">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-613">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="1f87f-614">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-614">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1f87f-615">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-615">Az.ContainerInstance</span></span>
* <span data-ttu-id="1f87f-616">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-616">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="1f87f-617">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1f87f-617">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="1f87f-618">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-618">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1f87f-619">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-619">Az.Network</span></span>
* <span data-ttu-id="1f87f-620">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-620">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="1f87f-621">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-621">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="1f87f-622">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-622">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="1f87f-623">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-623">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="1f87f-624">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1f87f-624">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1f87f-625">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-625">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="1f87f-626">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-626">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="1f87f-627">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1f87f-627">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="1f87f-628">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-628">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="1f87f-629">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-629">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="1f87f-630">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="1f87f-630">Az.Relay</span></span>
* <span data-ttu-id="1f87f-631">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="1f87f-631">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="1f87f-632">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-632">Az.Resources</span></span>
* <span data-ttu-id="1f87f-633">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-633">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="1f87f-634">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-634">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="1f87f-635">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="1f87f-635">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1f87f-636">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f87f-636">Az.ServiceFabric</span></span>
* <span data-ttu-id="1f87f-637">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-637">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="1f87f-638">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-638">Az.Sql</span></span>
* <span data-ttu-id="1f87f-639">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-639">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="1f87f-640">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-640">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1f87f-641">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-641">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1f87f-642">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-642">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1f87f-643">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1f87f-643">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1f87f-644">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1f87f-644">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1f87f-645">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1f87f-645">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1f87f-646">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1f87f-646">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1f87f-647">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1f87f-647">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="1f87f-648">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="1f87f-648">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="1f87f-649">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-649">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="1f87f-650">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-650">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="1f87f-651">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="1f87f-651">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1f87f-652">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="1f87f-652">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1f87f-653">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="1f87f-653">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="1f87f-654">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="1f87f-654">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="1f87f-655">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-655">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="1f87f-656">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-656">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1f87f-657">全般</span><span class="sxs-lookup"><span data-stu-id="1f87f-657">General</span></span>
* <span data-ttu-id="1f87f-658">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="1f87f-658">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="1f87f-659">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1f87f-659">Az.Profile</span></span>
* <span data-ttu-id="1f87f-660">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-660">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="1f87f-661">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-661">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="1f87f-662">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-662">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="1f87f-663">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-663">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="1f87f-664">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-664">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="1f87f-665">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-665">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="1f87f-666">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-666">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="1f87f-667">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-667">Az.CognitiveServices</span></span>
* <span data-ttu-id="1f87f-668">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-668">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-669">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-669">Az.Compute</span></span>
* <span data-ttu-id="1f87f-670">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-670">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="1f87f-671">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="1f87f-671">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="1f87f-672">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-672">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-673">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-673">Az.DataLakeStore</span></span>
* <span data-ttu-id="1f87f-674">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-674">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="1f87f-675">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-675">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="1f87f-676">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="1f87f-676">Az.Insights</span></span>
* <span data-ttu-id="1f87f-677">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-677">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="1f87f-678">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="1f87f-678">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="1f87f-679">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-679">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="1f87f-680">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="1f87f-680">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-681">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-681">Az.Network</span></span>
* <span data-ttu-id="1f87f-682">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="1f87f-682">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="1f87f-683">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="1f87f-683">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="1f87f-684">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="1f87f-684">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="1f87f-685">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1f87f-685">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="1f87f-686">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="1f87f-686">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="1f87f-687">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="1f87f-687">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="1f87f-688">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1f87f-688">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1f87f-689">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1f87f-689">Az.PolicyInsights</span></span>
* <span data-ttu-id="1f87f-690">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-690">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-691">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-691">Az.Resources</span></span>
* <span data-ttu-id="1f87f-692">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-692">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="1f87f-693">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-693">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1f87f-694">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1f87f-694">Az.ServiceBus</span></span>
* <span data-ttu-id="1f87f-695">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-695">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1f87f-696">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1f87f-696">Az.ServiceFabric</span></span>
* <span data-ttu-id="1f87f-697">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-697">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="1f87f-698">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-698">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="1f87f-699">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="1f87f-699">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="1f87f-700">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="1f87f-700">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="1f87f-701">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-701">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="1f87f-702">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-702">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="1f87f-703">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1f87f-703">Az.Profile</span></span>
* <span data-ttu-id="1f87f-704">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-704">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="1f87f-705">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-705">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-706">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-706">Az.Compute</span></span>
* <span data-ttu-id="1f87f-707">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-707">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="1f87f-708">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-708">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1f87f-709">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1f87f-709">Az.DataLakeStore</span></span>
* <span data-ttu-id="1f87f-710">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-710">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="1f87f-711">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1f87f-711">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="1f87f-712">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="1f87f-712">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1f87f-713">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="1f87f-713">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1f87f-714">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="1f87f-714">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-715">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-715">Az.Network</span></span>
* <span data-ttu-id="1f87f-716">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-716">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="1f87f-717">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-717">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-718">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-718">Az.Resources</span></span>
* <span data-ttu-id="1f87f-719">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-719">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="1f87f-720">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-720">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="1f87f-721">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-721">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="1f87f-722">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1f87f-722">Azure.Storage</span></span>
* <span data-ttu-id="1f87f-723">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-723">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="1f87f-724">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1f87f-724">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="1f87f-725">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1f87f-725">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1f87f-726">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-726">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="1f87f-727">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="1f87f-727">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="1f87f-728">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1f87f-728">Az.CognitiveServices</span></span>
* <span data-ttu-id="1f87f-729">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-729">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1f87f-730">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1f87f-730">Az.Compute</span></span>
* <span data-ttu-id="1f87f-731">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-731">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="1f87f-732">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-732">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="1f87f-733">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-733">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="1f87f-734">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1f87f-734">Az.DataFactoryV2</span></span>
* <span data-ttu-id="1f87f-735">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-735">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1f87f-736">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1f87f-736">Az.Network</span></span>
* <span data-ttu-id="1f87f-737">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1f87f-737">Added NetworkProfile functionality.</span></span> <span data-ttu-id="1f87f-738">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="1f87f-738">new cmdlets added</span></span>
    - <span data-ttu-id="1f87f-739">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1f87f-739">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="1f87f-740">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1f87f-740">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="1f87f-741">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1f87f-741">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="1f87f-742">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1f87f-742">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="1f87f-743">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="1f87f-743">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="1f87f-744">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="1f87f-744">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="1f87f-745">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-745">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="1f87f-746">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-746">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="1f87f-747">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-747">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1f87f-748">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1f87f-748">Az.RedisCache</span></span>
* <span data-ttu-id="1f87f-749">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="1f87f-749">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="1f87f-750">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-750">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="1f87f-751">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1f87f-751">Az.Resources</span></span>
* <span data-ttu-id="1f87f-752">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-752">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1f87f-753">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-753">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="1f87f-754">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1f87f-754">Az.Sql</span></span>
* <span data-ttu-id="1f87f-755">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1f87f-755">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1f87f-756">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1f87f-756">Az.Websites</span></span>
* <span data-ttu-id="1f87f-757">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="1f87f-757">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="1f87f-758">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="1f87f-758">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="1f87f-759">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="1f87f-759">0.2.0 - September 2018</span></span>
 <span data-ttu-id="1f87f-760">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="1f87f-760">Initial Release</span></span>