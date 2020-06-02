---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/30/2019
ms.openlocfilehash: 34b21292ccc47bb53b6609cd637ef18338a45cd3
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2020
ms.locfileid: "84121453"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="1bcbb-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="1bcbb-103">Azure PowerShell release notes</span></span>
## <a name="180---april-2019"></a><span data-ttu-id="1bcbb-104">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-104">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1bcbb-105">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="1bcbb-105">Highlights since the last major release</span></span>
* <span data-ttu-id="1bcbb-106">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="1bcbb-106">General availability of `Az` module</span></span>
* <span data-ttu-id="1bcbb-107">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1bcbb-107">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1bcbb-108">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1bcbb-108">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1bcbb-109">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-109">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1bcbb-110">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-110">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1bcbb-111">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-111">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1bcbb-112">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-112">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-113">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-113">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-114">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-114">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="1bcbb-115">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1bcbb-115">Az.Batch</span></span>
* <span data-ttu-id="1bcbb-116">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-116">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1bcbb-117">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1bcbb-117">Az.Cdn</span></span>
* <span data-ttu-id="1bcbb-118">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-118">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1bcbb-119">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-119">Az.CognitiveServices</span></span>
* <span data-ttu-id="1bcbb-120">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-120">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-121">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-121">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-122">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-122">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="1bcbb-123">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-123">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1bcbb-124">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-124">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1bcbb-125">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1bcbb-125">Az.DataFactory</span></span>
* <span data-ttu-id="1bcbb-126">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-126">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-127">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-127">Az.DataLakeStore</span></span>
* <span data-ttu-id="1bcbb-128">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-128">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1bcbb-129">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1bcbb-129">Az.EventGrid</span></span>
* <span data-ttu-id="1bcbb-130">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-130">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1bcbb-131">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1bcbb-131">Az.EventHub</span></span>
* <span data-ttu-id="1bcbb-132">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-132">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="1bcbb-133">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="1bcbb-133">Az.HDInsight</span></span>
* <span data-ttu-id="1bcbb-134">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-134">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1bcbb-135">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1bcbb-135">Az.IotHub</span></span>
* <span data-ttu-id="1bcbb-136">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-136">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1bcbb-137">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1bcbb-137">Az.KeyVault</span></span>
* <span data-ttu-id="1bcbb-138">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-138">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1bcbb-139">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-139">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="1bcbb-140">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1bcbb-140">Az.MachineLearning</span></span>
* <span data-ttu-id="1bcbb-141">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-141">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="1bcbb-142">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1bcbb-142">Az.Media</span></span>
* <span data-ttu-id="1bcbb-143">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-143">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1bcbb-144">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1bcbb-144">Az.Monitor</span></span>
  * <span data-ttu-id="1bcbb-145">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-145">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="1bcbb-146">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="1bcbb-146">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="1bcbb-147">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="1bcbb-147">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="1bcbb-148">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1bcbb-148">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1bcbb-149">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1bcbb-149">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="1bcbb-150">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="1bcbb-150">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="1bcbb-151">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-151">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-152">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-152">Az.Network</span></span>
* <span data-ttu-id="1bcbb-153">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-153">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1bcbb-154">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-154">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="1bcbb-155">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="1bcbb-155">Az.NotificationHubs</span></span>
* <span data-ttu-id="1bcbb-156">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-156">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1bcbb-157">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1bcbb-157">Az.OperationalInsights</span></span>
* <span data-ttu-id="1bcbb-158">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-158">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="1bcbb-159">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="1bcbb-159">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="1bcbb-160">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-160">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-161">Az.RecoveryServices</span></span>
* <span data-ttu-id="1bcbb-162">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-162">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1bcbb-163">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-163">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="1bcbb-164">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-164">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="1bcbb-165">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-165">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1bcbb-166">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1bcbb-166">Az.RedisCache</span></span>
* <span data-ttu-id="1bcbb-167">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-167">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-168">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-168">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-169">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-169">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-170">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-170">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-171">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="1bcbb-171">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="1bcbb-172">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-172">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1bcbb-173">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-173">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="1bcbb-174">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-174">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="1bcbb-175">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-175">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="1bcbb-176">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-176">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="1bcbb-177">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-177">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1bcbb-178">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-178">Az.Websites</span></span>
* <span data-ttu-id="1bcbb-179">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-179">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="1bcbb-180">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-180">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="1bcbb-181">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-181">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="1bcbb-182">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-182">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="1bcbb-183">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-183">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1bcbb-184">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="1bcbb-184">Highlights since the last major release</span></span>
* <span data-ttu-id="1bcbb-185">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="1bcbb-185">General availability of `Az` module</span></span>
* <span data-ttu-id="1bcbb-186">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1bcbb-186">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1bcbb-187">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1bcbb-187">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1bcbb-188">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-188">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1bcbb-189">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-189">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1bcbb-190">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-190">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1bcbb-191">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-191">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-192">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-192">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-193">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-193">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1bcbb-194">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-194">Az.AnalysisServices</span></span>
* <span data-ttu-id="1bcbb-195">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="1bcbb-195">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="1bcbb-196">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-196">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1bcbb-197">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1bcbb-197">Az.Automation</span></span>
* <span data-ttu-id="1bcbb-198">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-198">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="1bcbb-199">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-199">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="1bcbb-200">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-200">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-201">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-201">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-202">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-202">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="1bcbb-203">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-203">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="1bcbb-204">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-204">Az.ContainerInstance</span></span>
* <span data-ttu-id="1bcbb-205">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-205">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1bcbb-206">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1bcbb-206">Az.DataFactory</span></span>
* <span data-ttu-id="1bcbb-207">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-207">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="1bcbb-208">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-208">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-209">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-209">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-210">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-210">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="1bcbb-211">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-211">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="1bcbb-212">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-212">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="1bcbb-213">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1bcbb-213">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="1bcbb-214">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-214">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="1bcbb-215">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="1bcbb-215">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-216">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-216">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-217">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-217">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1bcbb-218">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-218">Az.Storage</span></span>
* <span data-ttu-id="1bcbb-219">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="1bcbb-219">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="1bcbb-220">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1bcbb-220">New-AzStorageContext</span></span>
* <span data-ttu-id="1bcbb-221">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-221">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="1bcbb-222">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1bcbb-222">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1bcbb-223">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="1bcbb-223">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="1bcbb-224">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-224">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="1bcbb-225">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-225">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="1bcbb-226">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-226">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="1bcbb-227">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1bcbb-227">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1bcbb-228">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="1bcbb-228">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="1bcbb-229">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1bcbb-229">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="1bcbb-230">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="1bcbb-230">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="1bcbb-231">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-231">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="1bcbb-232">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="1bcbb-232">Highlights since the last major release</span></span>
* <span data-ttu-id="1bcbb-233">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="1bcbb-233">General availability of `Az` module</span></span>
* <span data-ttu-id="1bcbb-234">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="1bcbb-234">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="1bcbb-235">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="1bcbb-235">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="1bcbb-236">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-236">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="1bcbb-237">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-237">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1bcbb-238">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-238">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="1bcbb-239">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-239">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1bcbb-240">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1bcbb-240">Az.Automation</span></span>
* <span data-ttu-id="1bcbb-241">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-241">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="1bcbb-242">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="1bcbb-242">Dynamic grouping</span></span>
    * <span data-ttu-id="1bcbb-243">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="1bcbb-243">Pre-Post script</span></span>
    * <span data-ttu-id="1bcbb-244">再起動設定</span><span class="sxs-lookup"><span data-stu-id="1bcbb-244">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-245">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-245">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-246">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-246">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="1bcbb-247">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-247">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1bcbb-248">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1bcbb-248">Az.KeyVault</span></span>
* <span data-ttu-id="1bcbb-249">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-249">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-250">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-250">Az.Network</span></span>
* <span data-ttu-id="1bcbb-251">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-251">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="1bcbb-252">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-252">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="1bcbb-254">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-254">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="1bcbb-255">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-255">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-256">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-256">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-257">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-257">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="1bcbb-258">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-258">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-259">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-259">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-260">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-260">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1bcbb-261">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-261">Az.Storage</span></span>
* <span data-ttu-id="1bcbb-262">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="1bcbb-262">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="1bcbb-263">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-263">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1bcbb-264">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-264">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1bcbb-265">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-265">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="1bcbb-266">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="1bcbb-266">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="1bcbb-267">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="1bcbb-267">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="1bcbb-268">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="1bcbb-268">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1bcbb-269">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-269">Az.Websites</span></span>
* <span data-ttu-id="1bcbb-270">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-270">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="1bcbb-271">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-271">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-272">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-272">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-273">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-273">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="1bcbb-274">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-274">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1bcbb-275">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1bcbb-275">Az.Automation</span></span>
* <span data-ttu-id="1bcbb-276">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-276">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="1bcbb-277">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-277">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="1bcbb-278">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-278">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1bcbb-279">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1bcbb-279">Az.Cdn</span></span>
* <span data-ttu-id="1bcbb-280">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-280">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-281">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-282">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-282">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1bcbb-283">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1bcbb-283">Az.DataFactory</span></span>
* <span data-ttu-id="1bcbb-284">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-284">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1bcbb-285">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1bcbb-285">Az.LogicApp</span></span>
* <span data-ttu-id="1bcbb-286">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-286">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-287">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-287">Az.Network</span></span>
* <span data-ttu-id="1bcbb-288">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-288">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-289">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-289">Az.RecoveryServices</span></span>
* <span data-ttu-id="1bcbb-290">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-290">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="1bcbb-291">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-291">SDK Update</span></span>
* <span data-ttu-id="1bcbb-292">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-292">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="1bcbb-293">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-293">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-294">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-294">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-295">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-295">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="1bcbb-296">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="1bcbb-296">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="1bcbb-297">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-297">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="1bcbb-298">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="1bcbb-298">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="1bcbb-299">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-299">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="1bcbb-300">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="1bcbb-300">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-301">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-301">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-302">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-302">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="1bcbb-303">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-303">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1bcbb-304">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-304">Az.Storage</span></span>
* <span data-ttu-id="1bcbb-305">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-305">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="1bcbb-306">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-306">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="1bcbb-307">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-307">Az.AnalysisServices</span></span>
* <span data-ttu-id="1bcbb-308">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-308">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1bcbb-309">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1bcbb-309">Az.Automation</span></span>
* <span data-ttu-id="1bcbb-310">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-310">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="1bcbb-311">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-311">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="1bcbb-312">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-312">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1bcbb-313">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-313">Az.CognitiveServices</span></span>
* <span data-ttu-id="1bcbb-314">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-314">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-315">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-316">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-316">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="1bcbb-317">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-317">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="1bcbb-318">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-318">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="1bcbb-319">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-319">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-320">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-320">Az.DataLakeStore</span></span>
* <span data-ttu-id="1bcbb-321">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-321">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="1bcbb-322">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="1bcbb-322">Az.EventHub</span></span>
* <span data-ttu-id="1bcbb-323">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-323">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1bcbb-324">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1bcbb-324">Az.KeyVault</span></span>
* <span data-ttu-id="1bcbb-325">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-325">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1bcbb-326">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1bcbb-326">Az.LogicApp</span></span>
* <span data-ttu-id="1bcbb-327">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-327">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="1bcbb-328">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-328">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="1bcbb-329">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-329">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="1bcbb-330">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1bcbb-330">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1bcbb-331">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1bcbb-331">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1bcbb-332">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1bcbb-332">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="1bcbb-333">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="1bcbb-333">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="1bcbb-334">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-334">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="1bcbb-335">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bcbb-335">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1bcbb-336">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bcbb-336">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1bcbb-337">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bcbb-337">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="1bcbb-338">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bcbb-338">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="1bcbb-339">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-339">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="1bcbb-340">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1bcbb-340">Az.Monitor</span></span>
* <span data-ttu-id="1bcbb-341">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-341">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-342">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-342">Az.Network</span></span>
* <span data-ttu-id="1bcbb-343">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-343">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="1bcbb-344">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1bcbb-344">Az.OperationalInsights</span></span>
* <span data-ttu-id="1bcbb-345">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-345">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="1bcbb-346">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-346">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="1bcbb-347">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-347">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-348">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-348">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-349">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1bcbb-349">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1bcbb-350">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1bcbb-350">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="1bcbb-351">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="1bcbb-351">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="1bcbb-352">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-352">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-353">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-353">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-354">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-354">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="1bcbb-355">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-355">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1bcbb-356">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-356">Az.Websites</span></span>
* <span data-ttu-id="1bcbb-357">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-357">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="1bcbb-358">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-358">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-359">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-359">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-360">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-360">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1bcbb-361">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-361">Az.AnalysisServices</span></span>
<span data-ttu-id="1bcbb-362">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="1bcbb-362">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-363">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-363">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-364">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-364">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="1bcbb-365">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-365">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="1bcbb-366">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-366">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-367">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-367">Az.RecoveryServices</span></span>
<span data-ttu-id="1bcbb-368">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="1bcbb-368">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-369">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-369">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-370">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-370">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="1bcbb-371">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="1bcbb-371">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="1bcbb-372">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-372">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="1bcbb-373">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="1bcbb-373">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-374">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-374">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-375">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-375">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="1bcbb-376">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-376">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="1bcbb-377">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-377">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="1bcbb-378">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-378">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-379">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-379">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-380">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="1bcbb-380">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="1bcbb-381">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-381">Az.AnalysisServices</span></span>
* <span data-ttu-id="1bcbb-382">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="1bcbb-382">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-383">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-383">Az.RecoveryServices</span></span>
* <span data-ttu-id="1bcbb-384">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="1bcbb-384">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="1bcbb-385">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-385">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-386">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-386">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-387">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-387">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="1bcbb-388">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-388">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1bcbb-389">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-389">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="1bcbb-390">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="1bcbb-390">Az.Aks</span></span>
* <span data-ttu-id="1bcbb-391">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-391">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="1bcbb-392">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1bcbb-392">Az.Automation</span></span>
* <span data-ttu-id="1bcbb-393">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-393">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="1bcbb-394">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-394">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="1bcbb-395">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="1bcbb-395">Az.Cdn</span></span>
* <span data-ttu-id="1bcbb-396">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-396">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-397">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-397">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-398">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-398">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="1bcbb-399">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-399">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="1bcbb-400">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-400">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="1bcbb-401">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="1bcbb-401">Az.ContainerRegistry</span></span>
* <span data-ttu-id="1bcbb-402">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-402">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="1bcbb-403">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="1bcbb-403">Az.DataFactory</span></span>
* <span data-ttu-id="1bcbb-404">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-404">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="1bcbb-406">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="1bcbb-406">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="1bcbb-407">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="1bcbb-407">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="1bcbb-408">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-408">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1bcbb-409">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1bcbb-409">Az.IotHub</span></span>
* <span data-ttu-id="1bcbb-410">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-410">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="1bcbb-411">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1bcbb-411">Az.KeyVault</span></span>
* <span data-ttu-id="1bcbb-412">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-412">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-413">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-413">Az.Network</span></span>
* <span data-ttu-id="1bcbb-414">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-414">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-415">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-415">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-416">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-416">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="1bcbb-417">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-417">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="1bcbb-418">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-418">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="1bcbb-419">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="1bcbb-419">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="1bcbb-420">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="1bcbb-420">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="1bcbb-421">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-421">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="1bcbb-422">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="1bcbb-422">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1bcbb-423">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1bcbb-423">Az.ServiceFabric</span></span>
* <span data-ttu-id="1bcbb-424">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="1bcbb-424">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="1bcbb-425">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-425">Fix some error messages.</span></span>
* <span data-ttu-id="1bcbb-426">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-426">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="1bcbb-427">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-427">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1bcbb-428">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1bcbb-428">Az.SignalR</span></span>
* <span data-ttu-id="1bcbb-429">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-429">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-430">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-430">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-431">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-431">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1bcbb-432">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-432">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="1bcbb-433">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-433">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="1bcbb-434">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="1bcbb-434">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1bcbb-435">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-435">Az.Storage</span></span>
* <span data-ttu-id="1bcbb-436">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-436">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1bcbb-437">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="1bcbb-437">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="1bcbb-438">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="1bcbb-438">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="1bcbb-439">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="1bcbb-439">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="1bcbb-440">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="1bcbb-440">Az.TrafficManager</span></span>
* <span data-ttu-id="1bcbb-441">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-441">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1bcbb-442">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-442">Az.Websites</span></span>
* <span data-ttu-id="1bcbb-443">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-443">Update incorrect online help URLs</span></span>
* <span data-ttu-id="1bcbb-444">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-444">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="1bcbb-445">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="1bcbb-445">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="1bcbb-446">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-446">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="1bcbb-447">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-447">Az.Accounts</span></span>
* <span data-ttu-id="1bcbb-448">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="1bcbb-448">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-449">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-449">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-450">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-450">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="1bcbb-451">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-451">Updated the description of ID in help files</span></span>
* <span data-ttu-id="1bcbb-452">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-452">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-453">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-453">Az.DataLakeStore</span></span>
* <span data-ttu-id="1bcbb-454">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-454">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="1bcbb-455">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-455">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="1bcbb-456">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="1bcbb-456">Az.EventGrid</span></span>
* <span data-ttu-id="1bcbb-457">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-457">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="1bcbb-458">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="1bcbb-458">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="1bcbb-459">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="1bcbb-459">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1bcbb-460">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="1bcbb-460">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1bcbb-461">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="1bcbb-461">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1bcbb-462">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="1bcbb-462">Dead letter endpoint.</span></span>
    - <span data-ttu-id="1bcbb-463">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="1bcbb-463">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="1bcbb-464">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="1bcbb-464">Event Time-To-Live,</span></span>
        - <span data-ttu-id="1bcbb-465">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="1bcbb-465">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="1bcbb-466">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="1bcbb-466">Dead letter endpoint.</span></span>
* <span data-ttu-id="1bcbb-467">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-467">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="1bcbb-468">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-468">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="1bcbb-469">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="1bcbb-469">Az.IotHub</span></span>
* <span data-ttu-id="1bcbb-470">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-470">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="1bcbb-471">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="1bcbb-471">Az.LogicApp</span></span>
* <span data-ttu-id="1bcbb-472">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="1bcbb-472">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-473">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-473">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-474">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-474">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="1bcbb-475">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="1bcbb-475">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="1bcbb-476">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-476">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1bcbb-477">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-477">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="1bcbb-478">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-478">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="1bcbb-479">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="1bcbb-479">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="1bcbb-480">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="1bcbb-480">Az.SignalR</span></span>
* <span data-ttu-id="1bcbb-481">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-481">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-482">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-482">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-483">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-483">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="1bcbb-484">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-484">Az.Storage</span></span>
* <span data-ttu-id="1bcbb-485">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="1bcbb-485">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="1bcbb-486">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="1bcbb-486">New-AzStorageContext</span></span>
* <span data-ttu-id="1bcbb-487">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-487">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="1bcbb-488">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="1bcbb-488">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1bcbb-489">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-489">Az.Websites</span></span>
* <span data-ttu-id="1bcbb-490">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-490">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="1bcbb-491">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-491">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="1bcbb-492">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-492">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="1bcbb-493">全般</span><span class="sxs-lookup"><span data-stu-id="1bcbb-493">General</span></span>

- <span data-ttu-id="1bcbb-494">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="1bcbb-494">General Availability of Az Module</span></span>
- <span data-ttu-id="1bcbb-495">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="1bcbb-495">Online help for each module</span></span>
- <span data-ttu-id="1bcbb-496">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-496">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="1bcbb-497">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-497">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="1bcbb-498">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="1bcbb-498">Az.Accounts</span></span>
- <span data-ttu-id="1bcbb-499">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-499">Changed from Az.Profile</span></span>
- <span data-ttu-id="1bcbb-500">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-500">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1bcbb-501">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1bcbb-501">Az.ApiManagement</span></span>
- <span data-ttu-id="1bcbb-502">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="1bcbb-502">Fixes for #7002</span></span>
- <span data-ttu-id="1bcbb-503">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-503">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="1bcbb-504">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="1bcbb-504">Az.Batch</span></span>
- <span data-ttu-id="1bcbb-505">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-505">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="1bcbb-506">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-506">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="1bcbb-507">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-507">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="1bcbb-508">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="1bcbb-508">Az.Billing</span></span>
- <span data-ttu-id="1bcbb-509">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-509">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="1bcbb-510">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-510">Az.CognitivServices</span></span>
- <span data-ttu-id="1bcbb-511">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-511">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="1bcbb-512">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-512">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1bcbb-513">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-513">Az.ContainerInstance</span></span>
- <span data-ttu-id="1bcbb-514">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-514">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="1bcbb-515">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="1bcbb-515">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="1bcbb-516">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-516">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-517">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-517">Az.DataLakeStore</span></span>
- <span data-ttu-id="1bcbb-518">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-518">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="1bcbb-519">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="1bcbb-519">Az.Monitor</span></span>
- <span data-ttu-id="1bcbb-520">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-520">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="1bcbb-521">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="1bcbb-521">Az.KeyVault</span></span>
- <span data-ttu-id="1bcbb-522">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-522">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="1bcbb-523">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="1bcbb-523">Az.MachineLearning</span></span>
- <span data-ttu-id="1bcbb-524">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-524">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="1bcbb-525">Az.Media</span><span class="sxs-lookup"><span data-stu-id="1bcbb-525">Az.Media</span></span>
- <span data-ttu-id="1bcbb-526">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-526">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1bcbb-527">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-527">Az.Network</span></span>
<span data-ttu-id="1bcbb-528">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-528">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="1bcbb-529">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="1bcbb-529">New cmdlets added:</span></span>
        - <span data-ttu-id="1bcbb-530">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1bcbb-530">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1bcbb-531">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1bcbb-531">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1bcbb-532">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1bcbb-532">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1bcbb-533">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1bcbb-533">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1bcbb-534">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="1bcbb-534">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="1bcbb-535">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="1bcbb-535">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="1bcbb-536">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="1bcbb-536">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="1bcbb-537">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="1bcbb-537">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="1bcbb-538">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-538">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="1bcbb-539">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="1bcbb-539">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="1bcbb-540">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1bcbb-540">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1bcbb-541">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="1bcbb-541">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="1bcbb-542">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="1bcbb-542">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="1bcbb-543">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="1bcbb-543">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="1bcbb-544">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-544">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="1bcbb-545">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-545">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="1bcbb-546">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1bcbb-546">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1bcbb-547">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1bcbb-547">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="1bcbb-548">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="1bcbb-548">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="1bcbb-549">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-549">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="1bcbb-550">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-550">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="1bcbb-551">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="1bcbb-551">Az.OperationalInsights</span></span>
- <span data-ttu-id="1bcbb-552">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-552">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="1bcbb-553">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-553">Az.Profile</span></span>
- <span data-ttu-id="1bcbb-554">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-554">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-555">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-555">Az.RecoveryServices</span></span>
- <span data-ttu-id="1bcbb-556">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-556">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="1bcbb-557">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-557">Az.Resources</span></span>
- <span data-ttu-id="1bcbb-558">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-558">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1bcbb-559">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1bcbb-559">Az.ServiceFabric</span></span>
- <span data-ttu-id="1bcbb-560">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="1bcbb-560">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="1bcbb-561">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-561">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="1bcbb-562">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="1bcbb-562">Az.SIgnalR</span></span>
- <span data-ttu-id="1bcbb-563">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="1bcbb-563">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="1bcbb-564">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-564">Az.Sql</span></span>
- <span data-ttu-id="1bcbb-565">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-565">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="1bcbb-566">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-566">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="1bcbb-567">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-567">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="1bcbb-568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-568">Az.Storage</span></span>
- <span data-ttu-id="1bcbb-569">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-569">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1bcbb-570">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-570">Az.Websites</span></span>
- <span data-ttu-id="1bcbb-571">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="1bcbb-571">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="1bcbb-572">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-572">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="1bcbb-573">全般</span><span class="sxs-lookup"><span data-stu-id="1bcbb-573">General</span></span>

* <span data-ttu-id="1bcbb-574">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="1bcbb-574">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="1bcbb-575">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-575">Az.Compute</span></span>

* <span data-ttu-id="1bcbb-576">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-576">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-577">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-577">Az.DataLakeStore</span></span>

* <span data-ttu-id="1bcbb-578">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-578">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="1bcbb-579">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="1bcbb-579">Az.FrontDoor</span></span>

* <span data-ttu-id="1bcbb-580">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-580">Fixed some broken links</span></span>
    - <span data-ttu-id="1bcbb-581">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-581">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="1bcbb-582">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-582">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="1bcbb-583">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-583">Az.RecoveryServices</span></span>

* <span data-ttu-id="1bcbb-584">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-584">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="1bcbb-585">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-585">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="1bcbb-586">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-586">Az.Resources</span></span>

* <span data-ttu-id="1bcbb-587">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-587">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="1bcbb-588">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-588">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="1bcbb-589">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-589">Az.Sql</span></span>

* <span data-ttu-id="1bcbb-590">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="1bcbb-590">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="1bcbb-591">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-591">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="1bcbb-592">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-592">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="1bcbb-593">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-593">Az.Storage</span></span>

* <span data-ttu-id="1bcbb-594">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-594">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="1bcbb-595">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-595">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="1bcbb-596">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-596">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1bcbb-597">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="1bcbb-597">Support Static Website configuration</span></span>
    - <span data-ttu-id="1bcbb-598">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1bcbb-598">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="1bcbb-599">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="1bcbb-599">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="1bcbb-600">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-600">Az.Websites</span></span>

* <span data-ttu-id="1bcbb-601">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="1bcbb-601">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="1bcbb-602">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-602">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="1bcbb-603">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="1bcbb-603">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="1bcbb-604">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-604">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="1bcbb-605">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="1bcbb-605">Az.ApiManagement</span></span>
* <span data-ttu-id="1bcbb-606">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-606">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="1bcbb-607">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="1bcbb-607">Az.Automation</span></span>
* <span data-ttu-id="1bcbb-608">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="1bcbb-608">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="1bcbb-609">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-609">Added Update Management cmdlets</span></span>
* <span data-ttu-id="1bcbb-610">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-610">Added Source Control cmdlets</span></span>
* <span data-ttu-id="1bcbb-611">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-611">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="1bcbb-612">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-612">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="1bcbb-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-613">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-614">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-614">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="1bcbb-615">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-615">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="1bcbb-616">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-616">Az.ContainerInstance</span></span>
* <span data-ttu-id="1bcbb-617">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-617">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="1bcbb-618">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="1bcbb-618">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="1bcbb-619">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-619">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="1bcbb-620">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-620">Az.Network</span></span>
* <span data-ttu-id="1bcbb-621">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-621">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="1bcbb-622">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-622">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="1bcbb-623">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-623">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="1bcbb-624">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-624">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="1bcbb-625">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="1bcbb-625">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="1bcbb-626">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-626">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="1bcbb-627">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-627">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="1bcbb-628">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="1bcbb-628">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="1bcbb-629">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-629">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="1bcbb-630">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-630">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="1bcbb-631">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="1bcbb-631">Az.Relay</span></span>
* <span data-ttu-id="1bcbb-632">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="1bcbb-632">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="1bcbb-633">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-633">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-634">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-634">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="1bcbb-635">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-635">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="1bcbb-636">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="1bcbb-636">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="1bcbb-637">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1bcbb-637">Az.ServiceFabric</span></span>
* <span data-ttu-id="1bcbb-638">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-638">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="1bcbb-639">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-639">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-640">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-640">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="1bcbb-641">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-641">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1bcbb-642">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-642">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1bcbb-643">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-643">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1bcbb-644">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="1bcbb-644">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="1bcbb-645">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1bcbb-645">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1bcbb-646">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1bcbb-646">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1bcbb-647">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1bcbb-647">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="1bcbb-648">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="1bcbb-648">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="1bcbb-649">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-649">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="1bcbb-650">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-650">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="1bcbb-651">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-651">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="1bcbb-652">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="1bcbb-652">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1bcbb-653">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="1bcbb-653">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="1bcbb-654">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="1bcbb-654">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="1bcbb-655">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="1bcbb-655">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="1bcbb-656">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-656">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="1bcbb-657">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-657">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="1bcbb-658">全般</span><span class="sxs-lookup"><span data-stu-id="1bcbb-658">General</span></span>
* <span data-ttu-id="1bcbb-659">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="1bcbb-659">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="1bcbb-660">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-660">Az.Profile</span></span>
* <span data-ttu-id="1bcbb-661">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-661">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="1bcbb-662">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-662">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="1bcbb-663">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-663">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="1bcbb-664">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-664">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="1bcbb-665">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-665">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="1bcbb-666">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-666">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="1bcbb-667">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-667">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="1bcbb-668">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-668">Az.CognitiveServices</span></span>
* <span data-ttu-id="1bcbb-669">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-669">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-670">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-670">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-671">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-671">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="1bcbb-672">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="1bcbb-672">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="1bcbb-673">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-673">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-674">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-674">Az.DataLakeStore</span></span>
* <span data-ttu-id="1bcbb-675">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-675">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="1bcbb-676">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-676">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="1bcbb-677">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="1bcbb-677">Az.Insights</span></span>
* <span data-ttu-id="1bcbb-678">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-678">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="1bcbb-679">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-679">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="1bcbb-680">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-680">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="1bcbb-681">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="1bcbb-681">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-682">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-682">Az.Network</span></span>
* <span data-ttu-id="1bcbb-683">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="1bcbb-683">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="1bcbb-684">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="1bcbb-684">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="1bcbb-685">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="1bcbb-685">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="1bcbb-686">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1bcbb-686">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="1bcbb-687">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="1bcbb-687">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="1bcbb-688">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="1bcbb-688">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="1bcbb-689">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="1bcbb-689">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="1bcbb-690">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="1bcbb-690">Az.PolicyInsights</span></span>
* <span data-ttu-id="1bcbb-691">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-691">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-692">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-692">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-693">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-693">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="1bcbb-694">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-694">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="1bcbb-695">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="1bcbb-695">Az.ServiceBus</span></span>
* <span data-ttu-id="1bcbb-696">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-696">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="1bcbb-697">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="1bcbb-697">Az.ServiceFabric</span></span>
* <span data-ttu-id="1bcbb-698">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-698">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="1bcbb-699">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-699">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="1bcbb-700">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-700">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="1bcbb-701">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-701">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="1bcbb-702">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-702">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="1bcbb-703">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-703">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="1bcbb-704">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-704">Az.Profile</span></span>
* <span data-ttu-id="1bcbb-705">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-705">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="1bcbb-706">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-706">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-707">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-707">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-708">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-708">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="1bcbb-709">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-709">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="1bcbb-710">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="1bcbb-710">Az.DataLakeStore</span></span>
* <span data-ttu-id="1bcbb-711">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-711">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="1bcbb-712">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-712">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="1bcbb-713">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-713">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1bcbb-714">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-714">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="1bcbb-715">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-715">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-716">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-716">Az.Network</span></span>
* <span data-ttu-id="1bcbb-717">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-717">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="1bcbb-718">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-718">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-719">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-719">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-720">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-720">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="1bcbb-721">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-721">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="1bcbb-722">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-722">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="1bcbb-723">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-723">Azure.Storage</span></span>
* <span data-ttu-id="1bcbb-724">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-724">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="1bcbb-725">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-725">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="1bcbb-726">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="1bcbb-726">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="1bcbb-727">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-727">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="1bcbb-728">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="1bcbb-728">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="1bcbb-729">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="1bcbb-729">Az.CognitiveServices</span></span>
* <span data-ttu-id="1bcbb-730">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-730">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="1bcbb-731">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="1bcbb-731">Az.Compute</span></span>
* <span data-ttu-id="1bcbb-732">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-732">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="1bcbb-733">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-733">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="1bcbb-734">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-734">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="1bcbb-735">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="1bcbb-735">Az.DataFactoryV2</span></span>
* <span data-ttu-id="1bcbb-736">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-736">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="1bcbb-737">Az.Network</span><span class="sxs-lookup"><span data-stu-id="1bcbb-737">Az.Network</span></span>
* <span data-ttu-id="1bcbb-738">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-738">Added NetworkProfile functionality.</span></span> <span data-ttu-id="1bcbb-739">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="1bcbb-739">new cmdlets added</span></span>
    - <span data-ttu-id="1bcbb-740">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-740">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="1bcbb-741">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-741">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="1bcbb-742">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-742">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="1bcbb-743">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="1bcbb-743">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="1bcbb-744">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="1bcbb-744">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="1bcbb-745">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="1bcbb-745">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="1bcbb-746">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-746">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="1bcbb-747">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-747">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="1bcbb-748">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-748">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="1bcbb-749">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="1bcbb-749">Az.RedisCache</span></span>
* <span data-ttu-id="1bcbb-750">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="1bcbb-750">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="1bcbb-751">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-751">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="1bcbb-752">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="1bcbb-752">Az.Resources</span></span>
* <span data-ttu-id="1bcbb-753">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-753">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="1bcbb-754">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-754">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="1bcbb-755">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="1bcbb-755">Az.Sql</span></span>
* <span data-ttu-id="1bcbb-756">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="1bcbb-756">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="1bcbb-757">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="1bcbb-757">Az.Websites</span></span>
* <span data-ttu-id="1bcbb-758">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="1bcbb-758">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="1bcbb-759">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="1bcbb-759">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="1bcbb-760">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="1bcbb-760">0.2.0 - September 2018</span></span>
 <span data-ttu-id="1bcbb-761">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="1bcbb-761">Initial Release</span></span>
