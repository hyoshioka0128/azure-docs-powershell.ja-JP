---
ms.openlocfilehash: f357a17f698d68c1a29dcb78f83671973fd6ecad
ms.sourcegitcommit: 0b644bfecf4224b2ea83520d1a6a956734d9fba4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2019
ms.locfileid: "67863736"
---
## <a name="240---july-2019"></a><span data-ttu-id="8d38a-101">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-101">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-102">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-103">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-103">Add support for profile cmdlets</span></span>
* <span data-ttu-id="8d38a-104">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-104">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="8d38a-105">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-105">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8d38a-106">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8d38a-106">Az.Advisor</span></span>
* <span data-ttu-id="8d38a-107">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-107">GA release of Az.Advisor</span></span>
* <span data-ttu-id="8d38a-108">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-108">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d38a-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d38a-109">Az.ApiManagement</span></span>
* <span data-ttu-id="8d38a-110">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="8d38a-110">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="8d38a-111">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8d38a-111">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="8d38a-112">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-112">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="8d38a-113">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-113">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="8d38a-114">https://github.com/Azure/azure-powershell/issues/9307 と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-114">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="8d38a-115">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8d38a-115">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="8d38a-116">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-116">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-117">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-117">Az.Automation</span></span>
* <span data-ttu-id="8d38a-118">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-118">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-119">Az.Compute</span></span>
* <span data-ttu-id="8d38a-120">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-120">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d38a-121">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d38a-121">Az.DataFactory</span></span>
* <span data-ttu-id="8d38a-122">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-122">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d38a-123">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d38a-123">Az.EventGrid</span></span>
* <span data-ttu-id="8d38a-124">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-124">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d38a-125">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-125">Az.IotHub</span></span>
* <span data-ttu-id="8d38a-126">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-126">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-127">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-127">Az.Network</span></span>
* <span data-ttu-id="8d38a-128">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-128">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="8d38a-129">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-129">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d38a-130">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-130">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d38a-131">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-131">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="8d38a-132">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="8d38a-132">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d38a-133">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-133">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d38a-134">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-134">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-135">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-135">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-136">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-136">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-137">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-137">Az.Resources</span></span>
    - <span data-ttu-id="8d38a-138">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-138">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="8d38a-139">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-139">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="8d38a-140">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-140">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="8d38a-141">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-141">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d38a-142">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d38a-142">Az.ServiceBus</span></span>
* <span data-ttu-id="8d38a-143">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="8d38a-143">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-144">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-144">Az.Sql</span></span>
* <span data-ttu-id="8d38a-145">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-145">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="8d38a-146">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="8d38a-146">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="8d38a-147">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d38a-147">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d38a-148">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d38a-148">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d38a-149">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d38a-149">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d38a-150">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d38a-150">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8d38a-151">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d38a-151">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8d38a-152">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d38a-152">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="8d38a-153">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-153">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-154">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-154">Az.Storage</span></span>
* <span data-ttu-id="8d38a-155">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-155">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="8d38a-156">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d38a-156">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="8d38a-157">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-157">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="8d38a-158">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="8d38a-158">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="8d38a-159">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="8d38a-159">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="8d38a-160">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-160">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8d38a-161">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-161">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8d38a-162">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="8d38a-162">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="8d38a-163">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d38a-163">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="8d38a-164">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d38a-164">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d38a-165">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d38a-165">Az.StorageSync</span></span>
* <span data-ttu-id="8d38a-166">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-166">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="8d38a-167">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-167">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-168">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-168">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-169">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-169">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="8d38a-170">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="8d38a-170">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="8d38a-171">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-171">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="8d38a-172">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="8d38a-172">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="8d38a-173">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="8d38a-173">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-174">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-174">Az.Compute</span></span>
* <span data-ttu-id="8d38a-175">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-175">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="8d38a-176">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-176">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="8d38a-177">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8d38a-177">Az.Dns</span></span>
* <span data-ttu-id="8d38a-178">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-178">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d38a-179">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d38a-179">Az.EventGrid</span></span>
* <span data-ttu-id="8d38a-180">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-180">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="8d38a-181">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d38a-181">New cmdlets:</span></span>
    - <span data-ttu-id="8d38a-182">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d38a-182">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d38a-183">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-183">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d38a-184">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d38a-184">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d38a-185">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-185">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="8d38a-186">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d38a-186">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d38a-187">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-187">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d38a-188">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8d38a-188">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8d38a-189">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-189">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d38a-190">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8d38a-190">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8d38a-191">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-191">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="8d38a-192">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8d38a-192">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8d38a-193">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-193">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="8d38a-194">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="8d38a-194">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="8d38a-195">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-195">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="8d38a-196">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8d38a-196">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8d38a-197">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-197">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="8d38a-198">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d38a-198">Updated cmdlets:</span></span>
    - <span data-ttu-id="8d38a-199">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8d38a-199">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="8d38a-200">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-200">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8d38a-201">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-201">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8d38a-202">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="8d38a-202">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="8d38a-203">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8d38a-203">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="8d38a-204">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="8d38a-204">Event subscription expiration date,</span></span>
            - <span data-ttu-id="8d38a-205">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="8d38a-205">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="8d38a-206">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-206">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="8d38a-207">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="8d38a-207">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="8d38a-208">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8d38a-208">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="8d38a-209">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-209">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="8d38a-210">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8d38a-210">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="8d38a-211">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-211">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="8d38a-212">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-212">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d38a-213">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d38a-213">Az.FrontDoor</span></span>
* <span data-ttu-id="8d38a-214">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="8d38a-214">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="8d38a-215">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-215">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="8d38a-216">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="8d38a-216">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="8d38a-217">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-217">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-218">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-218">Az.Network</span></span>
* <span data-ttu-id="8d38a-219">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-219">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="8d38a-220">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-220">New cmdlets</span></span>
        - <span data-ttu-id="8d38a-221">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="8d38a-221">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="8d38a-222">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-222">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="8d38a-223">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-223">New cmdlets</span></span> 
        - <span data-ttu-id="8d38a-224">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8d38a-224">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="8d38a-225">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-225">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="8d38a-226">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-226">New cmdlets</span></span> 
        - <span data-ttu-id="8d38a-227">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d38a-227">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="8d38a-228">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d38a-228">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d38a-229">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d38a-229">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d38a-230">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d38a-230">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="8d38a-231">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d38a-231">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8d38a-232">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-232">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="8d38a-233">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-233">New cmdlets</span></span>
        - <span data-ttu-id="8d38a-234">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d38a-234">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d38a-235">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d38a-235">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d38a-236">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d38a-236">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d38a-237">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="8d38a-237">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="8d38a-238">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="8d38a-238">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="8d38a-239">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-239">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="8d38a-240">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-240">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="8d38a-241">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-241">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="8d38a-242">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-242">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="8d38a-243">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-243">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="8d38a-244">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-244">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="8d38a-245">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-245">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="8d38a-246">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-246">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="8d38a-247">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-247">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="8d38a-248">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-248">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="8d38a-249">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-249">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="8d38a-250">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-250">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="8d38a-251">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-251">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="8d38a-252">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="8d38a-252">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8d38a-253">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-253">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="8d38a-254">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-254">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="8d38a-255">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="8d38a-255">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="8d38a-256">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-256">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="8d38a-257">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-257">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="8d38a-258">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-258">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8d38a-259">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-259">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8d38a-260">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-260">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d38a-261">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-261">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d38a-262">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-262">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-263">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-263">Az.Resources</span></span>
* <span data-ttu-id="8d38a-264">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d38a-264">Support for additional Template Export options</span></span>
    - <span data-ttu-id="8d38a-265">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-265">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8d38a-266">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-266">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8d38a-267">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-267">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d38a-268">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-268">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d38a-269">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-269">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-270">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-270">Az.Sql</span></span>
* <span data-ttu-id="8d38a-271">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-271">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="8d38a-272">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-272">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="8d38a-273">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-273">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="8d38a-274">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d38a-274">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d38a-275">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d38a-275">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d38a-276">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d38a-276">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d38a-277">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8d38a-277">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="8d38a-278">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8d38a-278">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-279">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-279">Az.Storage</span></span>
* <span data-ttu-id="8d38a-280">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-280">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="8d38a-281">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-281">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d38a-282">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-282">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="8d38a-283">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8d38a-283">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-284">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-284">Az.Websites</span></span>
* <span data-ttu-id="8d38a-285">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-285">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="8d38a-286">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-286">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="8d38a-287">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-287">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="8d38a-288">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d38a-288">Az.Cdn</span></span>
* <span data-ttu-id="8d38a-289">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-289">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-290">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-290">Az.Compute</span></span>
* <span data-ttu-id="8d38a-291">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-291">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="8d38a-292">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d38a-292">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d38a-293">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-293">Az.EventHub</span></span>
* <span data-ttu-id="8d38a-294">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-294">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="8d38a-295">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-295">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-296">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-296">Az.Network</span></span>
* <span data-ttu-id="8d38a-297">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-297">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="8d38a-298">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-298">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d38a-299">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-299">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d38a-300">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-300">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-301">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-301">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-302">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-302">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d38a-303">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d38a-303">Az.ServiceBus</span></span>
* <span data-ttu-id="8d38a-304">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-304">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d38a-305">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-305">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d38a-306">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-306">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="8d38a-307">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-307">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-308">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-308">Az.Sql</span></span>
* <span data-ttu-id="8d38a-309">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-309">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="8d38a-310">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="8d38a-310">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8d38a-311">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-311">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="8d38a-312">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-312">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-313">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-313">Az.Websites</span></span>
* <span data-ttu-id="8d38a-314">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-314">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="8d38a-315">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-315">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8d38a-316">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d38a-316">Az.ApiManagement</span></span>
* <span data-ttu-id="8d38a-317">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-317">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="8d38a-318">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="8d38a-318">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="8d38a-319">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="8d38a-319">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="8d38a-320">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8d38a-320">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="8d38a-321">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-321">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="8d38a-322">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8d38a-322">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="8d38a-323">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="8d38a-323">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="8d38a-324">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="8d38a-324">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="8d38a-325">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-325">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="8d38a-326">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="8d38a-326">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="8d38a-327">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="8d38a-327">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="8d38a-328">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="8d38a-328">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="8d38a-329">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="8d38a-329">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="8d38a-330">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-330">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="8d38a-331">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="8d38a-331">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="8d38a-332">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="8d38a-332">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="8d38a-333">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="8d38a-333">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="8d38a-334">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="8d38a-334">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="8d38a-335">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-335">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="8d38a-336">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="8d38a-336">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="8d38a-337">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-337">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="8d38a-338">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-338">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="8d38a-339">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="8d38a-339">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="8d38a-340">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-340">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="8d38a-341">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-341">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="8d38a-342">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-342">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="8d38a-343">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="8d38a-343">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="8d38a-344">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="8d38a-344">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="8d38a-345">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-345">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="8d38a-346">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-346">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="8d38a-347">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-347">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="8d38a-348">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="8d38a-348">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="8d38a-349">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-349">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="8d38a-350">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-350">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d38a-351">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="8d38a-351">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="8d38a-352">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8d38a-352">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="8d38a-353">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8d38a-353">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="8d38a-354">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-354">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="8d38a-355">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-355">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="8d38a-356">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-356">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="8d38a-357">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8d38a-357">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8d38a-358">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="8d38a-358">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8d38a-359">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="8d38a-359">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="8d38a-360">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-360">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8d38a-361">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-361">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d38a-362">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8d38a-362">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8d38a-363">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="8d38a-363">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="8d38a-364">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-364">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8d38a-365">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-365">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="8d38a-366">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="8d38a-366">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="8d38a-367">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="8d38a-367">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="8d38a-368">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="8d38a-368">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="8d38a-369">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8d38a-369">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="8d38a-370">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-370">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="8d38a-371">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="8d38a-371">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="8d38a-372">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="8d38a-372">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="8d38a-373">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-373">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8d38a-374">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8d38a-374">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8d38a-375">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8d38a-375">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8d38a-376">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-376">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8d38a-377">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-377">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8d38a-378">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8d38a-378">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8d38a-379">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8d38a-379">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8d38a-380">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-380">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8d38a-381">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-381">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="8d38a-382">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="8d38a-382">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="8d38a-383">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="8d38a-383">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="8d38a-384">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="8d38a-384">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="8d38a-385">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="8d38a-385">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="8d38a-386">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8d38a-386">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="8d38a-387">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="8d38a-387">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="8d38a-388">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="8d38a-388">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="8d38a-389">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="8d38a-389">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="8d38a-390">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-390">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="8d38a-391">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="8d38a-391">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="8d38a-392">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8d38a-392">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="8d38a-393">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="8d38a-393">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-394">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-394">Az.Automation</span></span>
* <span data-ttu-id="8d38a-395">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-395">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="8d38a-396">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="8d38a-396">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="8d38a-397">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="8d38a-397">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="8d38a-398">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-398">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="8d38a-399">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="8d38a-399">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="8d38a-400">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-400">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="8d38a-401">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-401">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-402">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-402">Az.Compute</span></span>
* <span data-ttu-id="8d38a-403">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-403">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="8d38a-404">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-404">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-406">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-406">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d38a-407">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d38a-407">Az.Monitor</span></span>
* <span data-ttu-id="8d38a-408">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-408">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-409">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-409">Az.Network</span></span>
* <span data-ttu-id="8d38a-410">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-410">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="8d38a-411">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d38a-411">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d38a-412">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d38a-412">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="8d38a-413">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-413">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-414">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-414">Az.Resources</span></span>
* <span data-ttu-id="8d38a-415">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-415">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-416">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-416">Az.Sql</span></span>
* <span data-ttu-id="8d38a-417">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8d38a-417">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="8d38a-418">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-418">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-419">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-419">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-420">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-420">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d38a-421">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-421">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d38a-422">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-422">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="8d38a-423">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-423">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-424">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-424">Az.Compute</span></span>
* <span data-ttu-id="8d38a-425">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="8d38a-425">Proximity placement group feature.</span></span>
    - <span data-ttu-id="8d38a-426">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="8d38a-426">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="8d38a-427">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="8d38a-427">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="8d38a-428">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-428">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="8d38a-429">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-429">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="8d38a-430">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-430">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="8d38a-431">重大な変更</span><span class="sxs-lookup"><span data-stu-id="8d38a-431">Breaking changes</span></span>
    - <span data-ttu-id="8d38a-432">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8d38a-432">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="8d38a-433">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8d38a-433">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8d38a-434">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8d38a-434">Az.DeploymentManager</span></span>
* <span data-ttu-id="8d38a-435">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-435">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="8d38a-436">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8d38a-436">Az.Dns</span></span>
* <span data-ttu-id="8d38a-437">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="8d38a-437">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="8d38a-438">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="8d38a-438">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="8d38a-439">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-439">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d38a-440">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d38a-440">Az.FrontDoor</span></span>
* <span data-ttu-id="8d38a-441">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-441">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="8d38a-442">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="8d38a-442">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="8d38a-443">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d38a-443">Az.HDInsight</span></span>
* <span data-ttu-id="8d38a-444">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-444">Removed two cmdlets:</span></span>
    - <span data-ttu-id="8d38a-445">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d38a-445">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="8d38a-446">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d38a-446">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8d38a-447">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-447">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8d38a-448">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-448">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="8d38a-449">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-449">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="8d38a-450">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="8d38a-450">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d38a-451">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d38a-451">Az.Monitor</span></span>
* <span data-ttu-id="8d38a-452">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="8d38a-452">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="8d38a-453">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="8d38a-453">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="8d38a-454">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="8d38a-454">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="8d38a-455">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="8d38a-455">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="8d38a-456">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="8d38a-456">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="8d38a-457">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="8d38a-457">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="8d38a-458">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="8d38a-458">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="8d38a-459">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-459">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d38a-460">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-460">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d38a-461">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-461">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d38a-462">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-462">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d38a-463">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-463">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d38a-464">SQR API に関する[詳細](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="8d38a-464">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="8d38a-465">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-465">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-466">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-466">Az.Network</span></span>
* <span data-ttu-id="8d38a-467">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-467">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="8d38a-468">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-468">New cmdlets</span></span>
        - <span data-ttu-id="8d38a-469">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d38a-469">New-AzNatGateway</span></span>
        - <span data-ttu-id="8d38a-470">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d38a-470">Get-AzNatGateway</span></span>
        - <span data-ttu-id="8d38a-471">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d38a-471">Set-AzNatGateway</span></span>
        - <span data-ttu-id="8d38a-472">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d38a-472">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="8d38a-473">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-473">Updated cmdlets</span></span>
        - <span data-ttu-id="8d38a-474">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8d38a-474">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="8d38a-475">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8d38a-475">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="8d38a-476">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="8d38a-476">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="8d38a-477">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-477">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="8d38a-478">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-478">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d38a-479">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-479">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d38a-480">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="8d38a-480">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="8d38a-481">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-481">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="8d38a-482">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8d38a-482">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-483">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-483">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-484">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="8d38a-484">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="8d38a-485">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="8d38a-485">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="8d38a-486">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="8d38a-486">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="8d38a-487">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8d38a-487">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="8d38a-488">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8d38a-488">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="8d38a-489">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="8d38a-489">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="8d38a-490">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8d38a-490">Az.Relay</span></span>
* <span data-ttu-id="8d38a-491">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-491">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d38a-492">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d38a-492">Az.ServiceBus</span></span>
* <span data-ttu-id="8d38a-493">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-493">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-494">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-494">Az.Storage</span></span>
* <span data-ttu-id="8d38a-495">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="8d38a-495">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="8d38a-496">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-496">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="8d38a-497">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-497">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="8d38a-498">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-498">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d38a-499">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="8d38a-499">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="8d38a-500">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-500">New-AzStorageAccount</span></span>
    - <span data-ttu-id="8d38a-501">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-501">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="8d38a-502">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d38a-502">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-503">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-503">Az.Websites</span></span>
* <span data-ttu-id="8d38a-504">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8d38a-504">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="8d38a-505">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="8d38a-505">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="8d38a-506">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-506">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d38a-507">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8d38a-507">Highlights since the last major release</span></span>
* <span data-ttu-id="8d38a-508">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8d38a-508">General availability of `Az` module</span></span>
* <span data-ttu-id="8d38a-509">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d38a-509">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d38a-510">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d38a-510">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d38a-511">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-511">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d38a-512">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-512">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d38a-513">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-513">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d38a-514">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-514">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d38a-515">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-515">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-516">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-516">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d38a-517">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d38a-517">Az.Batch</span></span>
* <span data-ttu-id="8d38a-518">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-518">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d38a-519">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d38a-519">Az.Cdn</span></span>
* <span data-ttu-id="8d38a-520">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-520">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d38a-521">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-521">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d38a-522">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-522">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-523">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-523">Az.Compute</span></span>
* <span data-ttu-id="8d38a-524">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-524">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="8d38a-525">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-525">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d38a-526">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-526">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d38a-527">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d38a-527">Az.DataFactory</span></span>
* <span data-ttu-id="8d38a-528">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-528">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-529">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-529">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-530">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-530">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d38a-531">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d38a-531">Az.EventGrid</span></span>
* <span data-ttu-id="8d38a-532">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-532">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d38a-533">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-533">Az.EventHub</span></span>
* <span data-ttu-id="8d38a-534">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-534">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="8d38a-535">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d38a-535">Az.HDInsight</span></span>
* <span data-ttu-id="8d38a-536">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-536">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d38a-537">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-537">Az.IotHub</span></span>
* <span data-ttu-id="8d38a-538">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-538">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d38a-539">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d38a-539">Az.KeyVault</span></span>
* <span data-ttu-id="8d38a-540">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-540">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d38a-541">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-541">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8d38a-542">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d38a-542">Az.MachineLearning</span></span>
* <span data-ttu-id="8d38a-543">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-543">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="8d38a-544">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8d38a-544">Az.Media</span></span>
* <span data-ttu-id="8d38a-545">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-545">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d38a-546">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d38a-546">Az.Monitor</span></span>
  * <span data-ttu-id="8d38a-547">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-547">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="8d38a-548">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="8d38a-548">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="8d38a-549">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="8d38a-549">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="8d38a-550">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d38a-550">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8d38a-551">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d38a-551">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8d38a-552">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d38a-552">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="8d38a-553">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-553">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-554">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-554">Az.Network</span></span>
* <span data-ttu-id="8d38a-555">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-555">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d38a-556">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-556">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="8d38a-557">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8d38a-557">Az.NotificationHubs</span></span>
* <span data-ttu-id="8d38a-558">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-558">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d38a-559">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-559">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d38a-560">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-560">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8d38a-561">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8d38a-561">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8d38a-562">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-562">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-563">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-563">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-564">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-564">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d38a-565">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-565">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="8d38a-566">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-566">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="8d38a-567">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-567">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d38a-568">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d38a-568">Az.RedisCache</span></span>
* <span data-ttu-id="8d38a-569">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-569">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-570">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-570">Az.Resources</span></span>
* <span data-ttu-id="8d38a-571">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-571">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-572">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-572">Az.Sql</span></span>
* <span data-ttu-id="8d38a-573">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="8d38a-573">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="8d38a-574">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-574">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d38a-575">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-575">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="8d38a-576">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-576">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="8d38a-577">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="8d38a-577">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="8d38a-578">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="8d38a-578">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="8d38a-579">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-579">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-580">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-580">Az.Websites</span></span>
* <span data-ttu-id="8d38a-581">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-581">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="8d38a-582">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-582">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d38a-583">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-583">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="8d38a-584">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-584">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="8d38a-585">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-585">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d38a-586">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8d38a-586">Highlights since the last major release</span></span>
* <span data-ttu-id="8d38a-587">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8d38a-587">General availability of `Az` module</span></span>
* <span data-ttu-id="8d38a-588">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d38a-588">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d38a-589">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d38a-589">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d38a-590">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-590">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d38a-591">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-591">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d38a-592">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-592">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d38a-593">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-593">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d38a-594">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-594">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-595">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-595">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d38a-596">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-596">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d38a-597">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="8d38a-597">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="8d38a-598">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-598">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-599">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-599">Az.Automation</span></span>
* <span data-ttu-id="8d38a-600">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-600">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="8d38a-601">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-601">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="8d38a-602">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-602">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-603">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-603">Az.Compute</span></span>
* <span data-ttu-id="8d38a-604">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-604">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8d38a-605">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-605">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="8d38a-606">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-606">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d38a-607">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-607">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d38a-608">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d38a-608">Az.DataFactory</span></span>
* <span data-ttu-id="8d38a-609">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-609">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="8d38a-610">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-610">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-611">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-611">Az.Resources</span></span>
* <span data-ttu-id="8d38a-612">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-612">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="8d38a-613">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-613">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8d38a-614">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="8d38a-614">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="8d38a-615">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8d38a-615">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="8d38a-616">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-616">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="8d38a-617">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8d38a-617">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-618">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-618">Az.Sql</span></span>
* <span data-ttu-id="8d38a-619">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-619">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-620">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-620">Az.Storage</span></span>
* <span data-ttu-id="8d38a-621">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="8d38a-621">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="8d38a-622">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8d38a-622">New-AzStorageContext</span></span>
* <span data-ttu-id="8d38a-623">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d38a-623">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="8d38a-624">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8d38a-624">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8d38a-625">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8d38a-625">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8d38a-626">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d38a-626">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8d38a-627">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d38a-627">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="8d38a-628">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d38a-628">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="8d38a-629">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d38a-629">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8d38a-630">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d38a-630">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8d38a-631">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d38a-631">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="8d38a-632">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d38a-632">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="8d38a-633">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-633">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d38a-634">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8d38a-634">Highlights since the last major release</span></span>
* <span data-ttu-id="8d38a-635">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8d38a-635">General availability of `Az` module</span></span>
* <span data-ttu-id="8d38a-636">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d38a-636">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d38a-637">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d38a-637">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d38a-638">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-638">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d38a-639">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-639">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d38a-640">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-640">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d38a-641">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-641">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-642">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-642">Az.Automation</span></span>
* <span data-ttu-id="8d38a-643">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-643">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="8d38a-644">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="8d38a-644">Dynamic grouping</span></span>
    * <span data-ttu-id="8d38a-645">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="8d38a-645">Pre-Post script</span></span>
    * <span data-ttu-id="8d38a-646">再起動設定</span><span class="sxs-lookup"><span data-stu-id="8d38a-646">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-647">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-647">Az.Compute</span></span>
* <span data-ttu-id="8d38a-648">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-648">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="8d38a-649">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-649">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d38a-650">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d38a-650">Az.KeyVault</span></span>
* <span data-ttu-id="8d38a-651">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-651">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-652">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-652">Az.Network</span></span>
* <span data-ttu-id="8d38a-653">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-653">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="8d38a-654">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-654">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-655">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-655">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-656">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-656">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="8d38a-657">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-657">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-658">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-658">Az.Resources</span></span>
* <span data-ttu-id="8d38a-659">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-659">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="8d38a-660">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-660">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-661">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-661">Az.Sql</span></span>
* <span data-ttu-id="8d38a-662">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-662">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-663">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-663">Az.Storage</span></span>
* <span data-ttu-id="8d38a-664">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="8d38a-664">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="8d38a-665">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d38a-665">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d38a-666">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d38a-666">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d38a-667">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d38a-667">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d38a-668">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="8d38a-668">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="8d38a-669">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="8d38a-669">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="8d38a-670">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-670">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-671">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-671">Az.Websites</span></span>
* <span data-ttu-id="8d38a-672">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-672">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="8d38a-673">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-673">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-674">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-674">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-675">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-675">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="8d38a-676">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-676">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-677">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-677">Az.Automation</span></span>
* <span data-ttu-id="8d38a-678">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-678">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="8d38a-679">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-679">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="8d38a-680">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-680">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d38a-681">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d38a-681">Az.Cdn</span></span>
* <span data-ttu-id="8d38a-682">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8d38a-682">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-683">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-683">Az.Compute</span></span>
* <span data-ttu-id="8d38a-684">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-684">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d38a-685">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d38a-685">Az.DataFactory</span></span>
* <span data-ttu-id="8d38a-686">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-686">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d38a-687">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d38a-687">Az.LogicApp</span></span>
* <span data-ttu-id="8d38a-688">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-688">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-689">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-689">Az.Network</span></span>
* <span data-ttu-id="8d38a-690">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-690">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-691">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-691">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-692">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-692">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="8d38a-693">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-693">SDK Update</span></span>
* <span data-ttu-id="8d38a-694">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-694">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="8d38a-695">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-695">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-696">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-696">Az.Resources</span></span>
* <span data-ttu-id="8d38a-697">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-697">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="8d38a-698">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="8d38a-698">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="8d38a-699">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-699">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="8d38a-700">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="8d38a-700">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="8d38a-701">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-701">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="8d38a-702">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="8d38a-702">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-703">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-703">Az.Sql</span></span>
* <span data-ttu-id="8d38a-704">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-704">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="8d38a-705">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-705">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-706">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-706">Az.Storage</span></span>
* <span data-ttu-id="8d38a-707">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d38a-707">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="8d38a-708">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-708">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="8d38a-709">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-709">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d38a-710">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8d38a-710">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-711">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-711">Az.Automation</span></span>
* <span data-ttu-id="8d38a-712">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-712">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="8d38a-713">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-713">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="8d38a-714">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-714">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d38a-715">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-715">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d38a-716">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-716">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-717">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-717">Az.Compute</span></span>
* <span data-ttu-id="8d38a-718">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-718">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="8d38a-719">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-719">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="8d38a-720">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-720">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="8d38a-721">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="8d38a-721">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-722">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-722">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-723">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-723">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d38a-724">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-724">Az.EventHub</span></span>
* <span data-ttu-id="8d38a-725">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-725">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="8d38a-726">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d38a-726">Az.KeyVault</span></span>
* <span data-ttu-id="8d38a-727">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-727">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d38a-728">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d38a-728">Az.LogicApp</span></span>
* <span data-ttu-id="8d38a-729">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-729">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="8d38a-730">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-730">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="8d38a-731">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-731">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="8d38a-732">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d38a-732">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d38a-733">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d38a-733">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d38a-734">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d38a-734">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d38a-735">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d38a-735">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="8d38a-736">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-736">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="8d38a-737">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d38a-737">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d38a-738">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d38a-738">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d38a-739">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d38a-739">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d38a-740">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d38a-740">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="8d38a-741">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-741">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d38a-742">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d38a-742">Az.Monitor</span></span>
* <span data-ttu-id="8d38a-743">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-743">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-744">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-744">Az.Network</span></span>
* <span data-ttu-id="8d38a-745">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-745">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d38a-746">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-746">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d38a-747">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-747">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="8d38a-748">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-748">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="8d38a-749">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-749">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="8d38a-750">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-750">Az.Resources</span></span>
* <span data-ttu-id="8d38a-751">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8d38a-751">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8d38a-752">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8d38a-752">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="8d38a-753">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="8d38a-753">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="8d38a-754">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-754">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-755">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-755">Az.Sql</span></span>
* <span data-ttu-id="8d38a-756">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-756">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="8d38a-757">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-757">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-758">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-758">Az.Websites</span></span>
* <span data-ttu-id="8d38a-759">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-759">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="8d38a-760">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-760">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-761">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-761">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-762">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-762">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d38a-763">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-763">Az.AnalysisServices</span></span>
<span data-ttu-id="8d38a-764">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8d38a-764">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-765">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-765">Az.Compute</span></span>
* <span data-ttu-id="8d38a-766">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-766">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="8d38a-767">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-767">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="8d38a-768">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-768">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-769">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-769">Az.RecoveryServices</span></span>
<span data-ttu-id="8d38a-770">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8d38a-770">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-771">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-771">Az.Resources</span></span>
* <span data-ttu-id="8d38a-772">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-772">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="8d38a-773">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8d38a-773">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8d38a-774">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-774">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="8d38a-775">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8d38a-775">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-776">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-776">Az.Sql</span></span>
* <span data-ttu-id="8d38a-777">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-777">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="8d38a-778">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-778">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="8d38a-779">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-779">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="8d38a-780">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-780">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-781">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-781">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-782">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-782">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d38a-783">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-783">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d38a-784">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-784">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-785">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-785">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d38a-786">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-786">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="8d38a-787">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-787">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-788">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-788">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-789">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-789">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d38a-790">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-790">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d38a-791">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-791">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="8d38a-792">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8d38a-792">Az.Aks</span></span>
* <span data-ttu-id="8d38a-793">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-793">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d38a-794">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-794">Az.Automation</span></span>
* <span data-ttu-id="8d38a-795">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-795">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="8d38a-796">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-796">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d38a-797">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d38a-797">Az.Cdn</span></span>
* <span data-ttu-id="8d38a-798">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-798">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-799">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-799">Az.Compute</span></span>
* <span data-ttu-id="8d38a-800">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-800">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="8d38a-801">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-801">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="8d38a-802">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-802">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8d38a-803">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8d38a-803">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8d38a-804">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-804">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d38a-805">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d38a-805">Az.DataFactory</span></span>
* <span data-ttu-id="8d38a-806">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-806">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-807">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-807">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-808">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="8d38a-808">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="8d38a-809">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="8d38a-809">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="8d38a-810">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-810">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d38a-811">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-811">Az.IotHub</span></span>
* <span data-ttu-id="8d38a-812">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-812">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d38a-813">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d38a-813">Az.KeyVault</span></span>
* <span data-ttu-id="8d38a-814">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-814">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-815">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-815">Az.Network</span></span>
* <span data-ttu-id="8d38a-816">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-816">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-817">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-817">Az.Resources</span></span>
* <span data-ttu-id="8d38a-818">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-818">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="8d38a-819">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-819">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="8d38a-820">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-820">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="8d38a-821">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="8d38a-821">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="8d38a-822">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="8d38a-822">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="8d38a-823">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-823">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="8d38a-824">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="8d38a-824">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d38a-825">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-825">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d38a-826">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="8d38a-826">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="8d38a-827">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-827">Fix some error messages.</span></span>
* <span data-ttu-id="8d38a-828">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-828">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="8d38a-829">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-829">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d38a-830">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d38a-830">Az.SignalR</span></span>
* <span data-ttu-id="8d38a-831">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-831">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-832">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-832">Az.Sql</span></span>
* <span data-ttu-id="8d38a-833">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-833">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d38a-834">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-834">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="8d38a-835">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-835">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="8d38a-836">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="8d38a-836">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-837">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-837">Az.Storage</span></span>
* <span data-ttu-id="8d38a-838">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-838">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d38a-839">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="8d38a-839">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="8d38a-840">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="8d38a-840">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="8d38a-841">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="8d38a-841">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8d38a-842">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8d38a-842">Az.TrafficManager</span></span>
* <span data-ttu-id="8d38a-843">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-843">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-844">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-844">Az.Websites</span></span>
* <span data-ttu-id="8d38a-845">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-845">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d38a-846">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-846">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="8d38a-847">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8d38a-847">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="8d38a-848">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-848">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d38a-849">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-849">Az.Accounts</span></span>
* <span data-ttu-id="8d38a-850">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="8d38a-850">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-851">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-851">Az.Compute</span></span>
* <span data-ttu-id="8d38a-852">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-852">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="8d38a-853">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="8d38a-853">Updated the description of ID in help files</span></span>
* <span data-ttu-id="8d38a-854">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-854">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-855">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-855">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-856">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-856">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="8d38a-857">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-857">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d38a-858">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d38a-858">Az.EventGrid</span></span>
* <span data-ttu-id="8d38a-859">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-859">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="8d38a-860">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="8d38a-860">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="8d38a-861">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8d38a-861">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8d38a-862">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8d38a-862">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8d38a-863">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8d38a-863">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8d38a-864">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8d38a-864">Dead letter endpoint.</span></span>
    - <span data-ttu-id="8d38a-865">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8d38a-865">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8d38a-866">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8d38a-866">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8d38a-867">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8d38a-867">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8d38a-868">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8d38a-868">Dead letter endpoint.</span></span>
* <span data-ttu-id="8d38a-869">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-869">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="8d38a-870">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-870">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d38a-871">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d38a-871">Az.IotHub</span></span>
* <span data-ttu-id="8d38a-872">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-872">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d38a-873">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d38a-873">Az.LogicApp</span></span>
* <span data-ttu-id="8d38a-874">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="8d38a-874">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-875">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-875">Az.Resources</span></span>
* <span data-ttu-id="8d38a-876">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-876">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="8d38a-877">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="8d38a-877">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="8d38a-878">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-878">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8d38a-879">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-879">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="8d38a-880">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="8d38a-880">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="8d38a-881">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="8d38a-881">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d38a-882">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d38a-882">Az.SignalR</span></span>
* <span data-ttu-id="8d38a-883">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-883">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-884">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-884">Az.Sql</span></span>
* <span data-ttu-id="8d38a-885">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-885">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d38a-886">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-886">Az.Storage</span></span>
* <span data-ttu-id="8d38a-887">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="8d38a-887">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="8d38a-888">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8d38a-888">New-AzStorageContext</span></span>
* <span data-ttu-id="8d38a-889">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-889">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="8d38a-890">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8d38a-890">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-891">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-891">Az.Websites</span></span>
* <span data-ttu-id="8d38a-892">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-892">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8d38a-893">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-893">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="8d38a-894">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-894">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="8d38a-895">全般</span><span class="sxs-lookup"><span data-stu-id="8d38a-895">General</span></span>

- <span data-ttu-id="8d38a-896">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="8d38a-896">General Availability of Az Module</span></span>
- <span data-ttu-id="8d38a-897">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="8d38a-897">Online help for each module</span></span>
- <span data-ttu-id="8d38a-898">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-898">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="8d38a-899">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-899">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="8d38a-900">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d38a-900">Az.Accounts</span></span>
- <span data-ttu-id="8d38a-901">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-901">Changed from Az.Profile</span></span>
- <span data-ttu-id="8d38a-902">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-902">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8d38a-903">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d38a-903">Az.ApiManagement</span></span>
- <span data-ttu-id="8d38a-904">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="8d38a-904">Fixes for #7002</span></span>
- <span data-ttu-id="8d38a-905">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-905">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="8d38a-906">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d38a-906">Az.Batch</span></span>
- <span data-ttu-id="8d38a-907">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-907">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="8d38a-908">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-908">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="8d38a-909">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-909">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="8d38a-910">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8d38a-910">Az.Billing</span></span>
- <span data-ttu-id="8d38a-911">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-911">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="8d38a-912">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-912">Az.CognitivServices</span></span>
- <span data-ttu-id="8d38a-913">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-913">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="8d38a-914">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-914">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8d38a-915">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-915">Az.ContainerInstance</span></span>
- <span data-ttu-id="8d38a-916">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-916">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="8d38a-917">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8d38a-917">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="8d38a-918">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-918">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-919">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-919">Az.DataLakeStore</span></span>
- <span data-ttu-id="8d38a-920">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-920">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="8d38a-921">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d38a-921">Az.Monitor</span></span>
- <span data-ttu-id="8d38a-922">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-922">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="8d38a-923">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d38a-923">Az.KeyVault</span></span>
- <span data-ttu-id="8d38a-924">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-924">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="8d38a-925">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d38a-925">Az.MachineLearning</span></span>
- <span data-ttu-id="8d38a-926">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="8d38a-926">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="8d38a-927">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8d38a-927">Az.Media</span></span>
- <span data-ttu-id="8d38a-928">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-928">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8d38a-929">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-929">Az.Network</span></span>
<span data-ttu-id="8d38a-930">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-930">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="8d38a-931">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8d38a-931">New cmdlets added:</span></span>
        - <span data-ttu-id="8d38a-932">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d38a-932">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d38a-933">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d38a-933">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d38a-934">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d38a-934">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d38a-935">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d38a-935">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d38a-936">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d38a-936">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d38a-937">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-937">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="8d38a-938">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8d38a-938">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="8d38a-939">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d38a-939">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="8d38a-940">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-940">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="8d38a-941">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="8d38a-941">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="8d38a-942">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-942">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8d38a-943">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8d38a-943">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8d38a-944">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d38a-944">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="8d38a-945">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="8d38a-945">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="8d38a-946">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-946">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="8d38a-947">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-947">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="8d38a-948">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d38a-948">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8d38a-949">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d38a-949">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8d38a-950">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d38a-950">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="8d38a-951">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-951">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="8d38a-952">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-952">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="8d38a-953">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-953">Az.OperationalInsights</span></span>
- <span data-ttu-id="8d38a-954">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-954">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="8d38a-955">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d38a-955">Az.Profile</span></span>
- <span data-ttu-id="8d38a-956">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-956">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-957">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-957">Az.RecoveryServices</span></span>
- <span data-ttu-id="8d38a-958">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-958">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="8d38a-959">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-959">Az.Resources</span></span>
- <span data-ttu-id="8d38a-960">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-960">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8d38a-961">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-961">Az.ServiceFabric</span></span>
- <span data-ttu-id="8d38a-962">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="8d38a-962">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="8d38a-963">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-963">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="8d38a-964">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="8d38a-964">Az.SIgnalR</span></span>
- <span data-ttu-id="8d38a-965">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="8d38a-965">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="8d38a-966">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-966">Az.Sql</span></span>
- <span data-ttu-id="8d38a-967">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-967">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="8d38a-968">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-968">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="8d38a-969">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-969">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="8d38a-970">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-970">Az.Storage</span></span>
- <span data-ttu-id="8d38a-971">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-971">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8d38a-972">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-972">Az.Websites</span></span>
- <span data-ttu-id="8d38a-973">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d38a-973">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="8d38a-974">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-974">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="8d38a-975">全般</span><span class="sxs-lookup"><span data-stu-id="8d38a-975">General</span></span>

* <span data-ttu-id="8d38a-976">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8d38a-976">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="8d38a-977">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-977">Az.Compute</span></span>

* <span data-ttu-id="8d38a-978">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-978">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-979">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-979">Az.DataLakeStore</span></span>

* <span data-ttu-id="8d38a-980">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-980">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="8d38a-981">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d38a-981">Az.FrontDoor</span></span>

* <span data-ttu-id="8d38a-982">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-982">Fixed some broken links</span></span>
    - <span data-ttu-id="8d38a-983">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-983">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="8d38a-984">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-984">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8d38a-985">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-985">Az.RecoveryServices</span></span>

* <span data-ttu-id="8d38a-986">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-986">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="8d38a-987">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-987">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="8d38a-988">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-988">Az.Resources</span></span>

* <span data-ttu-id="8d38a-989">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-989">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="8d38a-990">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-990">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="8d38a-991">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-991">Az.Sql</span></span>

* <span data-ttu-id="8d38a-992">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8d38a-992">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="8d38a-993">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-993">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="8d38a-994">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-994">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="8d38a-995">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-995">Az.Storage</span></span>

* <span data-ttu-id="8d38a-996">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-996">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="8d38a-997">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-997">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="8d38a-998">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8d38a-998">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8d38a-999">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="8d38a-999">Support Static Website configuration</span></span>
    - <span data-ttu-id="8d38a-1000">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d38a-1000">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="8d38a-1001">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d38a-1001">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8d38a-1002">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-1002">Az.Websites</span></span>

* <span data-ttu-id="8d38a-1003">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8d38a-1003">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="8d38a-1004">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1004">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="8d38a-1005">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="8d38a-1005">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="8d38a-1006">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-1006">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8d38a-1007">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d38a-1007">Az.ApiManagement</span></span>
* <span data-ttu-id="8d38a-1008">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1008">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="8d38a-1009">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d38a-1009">Az.Automation</span></span>
* <span data-ttu-id="8d38a-1010">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d38a-1010">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="8d38a-1011">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1011">Added Update Management cmdlets</span></span>
* <span data-ttu-id="8d38a-1012">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1012">Added Source Control cmdlets</span></span>
* <span data-ttu-id="8d38a-1013">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1013">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="8d38a-1014">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1014">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="8d38a-1015">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-1015">Az.Compute</span></span>
* <span data-ttu-id="8d38a-1016">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1016">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="8d38a-1017">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1017">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8d38a-1018">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-1018">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d38a-1019">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1019">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="8d38a-1020">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8d38a-1020">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8d38a-1021">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1021">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8d38a-1022">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-1022">Az.Network</span></span>
* <span data-ttu-id="8d38a-1023">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1023">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="8d38a-1024">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1024">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="8d38a-1025">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1025">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="8d38a-1026">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1026">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="8d38a-1027">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8d38a-1027">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8d38a-1028">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1028">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="8d38a-1029">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1029">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="8d38a-1030">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8d38a-1030">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8d38a-1031">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1031">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="8d38a-1032">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1032">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="8d38a-1033">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8d38a-1033">Az.Relay</span></span>
* <span data-ttu-id="8d38a-1034">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8d38a-1034">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="8d38a-1035">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-1035">Az.Resources</span></span>
* <span data-ttu-id="8d38a-1036">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1036">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="8d38a-1037">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1037">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="8d38a-1038">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="8d38a-1038">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8d38a-1039">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-1039">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d38a-1040">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1040">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="8d38a-1041">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-1041">Az.Sql</span></span>
* <span data-ttu-id="8d38a-1042">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1042">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="8d38a-1043">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-1043">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d38a-1044">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-1044">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d38a-1045">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-1045">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d38a-1046">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d38a-1046">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d38a-1047">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d38a-1047">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d38a-1048">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d38a-1048">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d38a-1049">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d38a-1049">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d38a-1050">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d38a-1050">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="8d38a-1051">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1051">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="8d38a-1052">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1052">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="8d38a-1053">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1053">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="8d38a-1054">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8d38a-1054">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8d38a-1055">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8d38a-1055">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8d38a-1056">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8d38a-1056">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="8d38a-1057">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8d38a-1057">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="8d38a-1058">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1058">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="8d38a-1059">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-1059">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="8d38a-1060">全般</span><span class="sxs-lookup"><span data-stu-id="8d38a-1060">General</span></span>
* <span data-ttu-id="8d38a-1061">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="8d38a-1061">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="8d38a-1062">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d38a-1062">Az.Profile</span></span>
* <span data-ttu-id="8d38a-1063">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1063">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="8d38a-1064">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1064">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="8d38a-1065">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1065">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="8d38a-1066">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1066">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="8d38a-1067">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1067">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="8d38a-1068">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1068">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="8d38a-1069">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1069">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d38a-1070">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-1070">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d38a-1071">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1071">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-1072">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-1072">Az.Compute</span></span>
* <span data-ttu-id="8d38a-1073">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1073">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="8d38a-1074">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="8d38a-1074">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="8d38a-1075">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1075">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-1076">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-1076">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-1077">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1077">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="8d38a-1078">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1078">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="8d38a-1079">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="8d38a-1079">Az.Insights</span></span>
* <span data-ttu-id="8d38a-1080">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1080">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="8d38a-1081">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1081">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="8d38a-1082">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1082">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="8d38a-1083">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="8d38a-1083">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-1084">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-1084">Az.Network</span></span>
* <span data-ttu-id="8d38a-1085">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="8d38a-1085">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="8d38a-1086">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d38a-1086">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="8d38a-1087">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="8d38a-1087">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="8d38a-1088">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8d38a-1088">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="8d38a-1089">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="8d38a-1089">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="8d38a-1090">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d38a-1090">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="8d38a-1091">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8d38a-1091">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d38a-1092">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d38a-1092">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d38a-1093">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1093">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-1094">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-1094">Az.Resources</span></span>
* <span data-ttu-id="8d38a-1095">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1095">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="8d38a-1096">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1096">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d38a-1097">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d38a-1097">Az.ServiceBus</span></span>
* <span data-ttu-id="8d38a-1098">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1098">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d38a-1099">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d38a-1099">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d38a-1100">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1100">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="8d38a-1101">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1101">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="8d38a-1102">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1102">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="8d38a-1103">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1103">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="8d38a-1104">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1104">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="8d38a-1105">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-1105">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="8d38a-1106">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d38a-1106">Az.Profile</span></span>
* <span data-ttu-id="8d38a-1107">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1107">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="8d38a-1108">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1108">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-1109">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-1109">Az.Compute</span></span>
* <span data-ttu-id="8d38a-1110">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1110">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="8d38a-1111">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1111">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d38a-1112">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d38a-1112">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d38a-1113">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1113">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="8d38a-1114">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1114">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="8d38a-1115">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1115">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8d38a-1116">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1116">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8d38a-1117">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1117">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-1118">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-1118">Az.Network</span></span>
* <span data-ttu-id="8d38a-1119">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1119">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="8d38a-1120">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1120">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-1121">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-1121">Az.Resources</span></span>
* <span data-ttu-id="8d38a-1122">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1122">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="8d38a-1123">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1123">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="8d38a-1124">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-1124">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="8d38a-1125">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8d38a-1125">Azure.Storage</span></span>
* <span data-ttu-id="8d38a-1126">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1126">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="8d38a-1127">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8d38a-1127">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="8d38a-1128">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8d38a-1128">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8d38a-1129">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1129">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="8d38a-1130">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="8d38a-1130">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="8d38a-1131">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d38a-1131">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d38a-1132">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1132">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d38a-1133">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d38a-1133">Az.Compute</span></span>
* <span data-ttu-id="8d38a-1134">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1134">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="8d38a-1135">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1135">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="8d38a-1136">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1136">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="8d38a-1137">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8d38a-1137">Az.DataFactoryV2</span></span>
* <span data-ttu-id="8d38a-1138">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1138">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d38a-1139">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d38a-1139">Az.Network</span></span>
* <span data-ttu-id="8d38a-1140">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1140">Added NetworkProfile functionality.</span></span> <span data-ttu-id="8d38a-1141">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8d38a-1141">new cmdlets added</span></span>
    - <span data-ttu-id="8d38a-1142">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d38a-1142">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d38a-1143">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d38a-1143">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d38a-1144">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d38a-1144">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d38a-1145">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d38a-1145">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d38a-1146">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="8d38a-1146">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="8d38a-1147">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d38a-1147">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="8d38a-1148">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1148">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="8d38a-1149">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1149">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="8d38a-1150">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1150">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d38a-1151">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d38a-1151">Az.RedisCache</span></span>
* <span data-ttu-id="8d38a-1152">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="8d38a-1152">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="8d38a-1153">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1153">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d38a-1154">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d38a-1154">Az.Resources</span></span>
* <span data-ttu-id="8d38a-1155">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1155">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8d38a-1156">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1156">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d38a-1157">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d38a-1157">Az.Sql</span></span>
* <span data-ttu-id="8d38a-1158">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d38a-1158">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d38a-1159">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d38a-1159">Az.Websites</span></span>
* <span data-ttu-id="8d38a-1160">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="8d38a-1160">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="8d38a-1161">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="8d38a-1161">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="8d38a-1162">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="8d38a-1162">0.2.0 - September 2018</span></span>
 <span data-ttu-id="8d38a-1163">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="8d38a-1163">Initial Release</span></span>