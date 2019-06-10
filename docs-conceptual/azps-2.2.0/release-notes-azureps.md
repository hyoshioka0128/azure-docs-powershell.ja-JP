---
ms.openlocfilehash: 911e1f7ff56feab2735f397a0128aab4aa7757c7
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498677"
---
## <a name="220---june-2019"></a><span data-ttu-id="62ea2-101">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-101">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="62ea2-102">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="62ea2-102">Az.Cdn</span></span>
* <span data-ttu-id="62ea2-103">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-103">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-104">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-104">Az.Compute</span></span>
* <span data-ttu-id="62ea2-105">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-105">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="62ea2-106">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="62ea2-106">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="62ea2-107">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="62ea2-107">Az.EventHub</span></span>
* <span data-ttu-id="62ea2-108">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-108">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="62ea2-109">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-109">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-110">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-110">Az.Network</span></span>
* <span data-ttu-id="62ea2-111">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-111">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="62ea2-112">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-112">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="62ea2-113">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="62ea2-113">Az.PolicyInsights</span></span>
* <span data-ttu-id="62ea2-114">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-114">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-115">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-115">Az.RecoveryServices</span></span>
* <span data-ttu-id="62ea2-116">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-116">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="62ea2-117">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="62ea2-117">Az.ServiceBus</span></span>
* <span data-ttu-id="62ea2-118">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-118">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="62ea2-119">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="62ea2-119">Az.ServiceFabric</span></span>
* <span data-ttu-id="62ea2-120">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-120">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="62ea2-121">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-121">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-122">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-122">Az.Sql</span></span>
* <span data-ttu-id="62ea2-123">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-123">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="62ea2-124">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="62ea2-124">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="62ea2-125">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-125">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="62ea2-126">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-126">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-127">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-127">Az.Websites</span></span>
* <span data-ttu-id="62ea2-128">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-128">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="62ea2-129">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-129">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="62ea2-130">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="62ea2-130">Az.ApiManagement</span></span>
* <span data-ttu-id="62ea2-131">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-131">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="62ea2-132">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="62ea2-132">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="62ea2-133">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="62ea2-133">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="62ea2-134">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="62ea2-134">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="62ea2-135">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-135">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="62ea2-136">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="62ea2-136">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="62ea2-137">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="62ea2-137">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="62ea2-138">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="62ea2-138">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="62ea2-139">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-139">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="62ea2-140">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="62ea2-140">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="62ea2-141">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="62ea2-141">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="62ea2-142">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="62ea2-142">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="62ea2-143">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="62ea2-143">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="62ea2-144">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-144">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="62ea2-145">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="62ea2-145">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="62ea2-146">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="62ea2-146">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="62ea2-147">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="62ea2-147">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="62ea2-148">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="62ea2-148">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="62ea2-149">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-149">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="62ea2-150">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="62ea2-150">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="62ea2-151">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-151">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="62ea2-152">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-152">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="62ea2-153">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="62ea2-153">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="62ea2-154">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-154">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="62ea2-155">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-155">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="62ea2-156">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-156">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="62ea2-157">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="62ea2-157">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="62ea2-158">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="62ea2-158">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="62ea2-159">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-159">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="62ea2-160">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-160">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="62ea2-161">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-161">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="62ea2-162">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="62ea2-162">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="62ea2-163">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-163">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="62ea2-164">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-164">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="62ea2-165">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="62ea2-165">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="62ea2-166">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="62ea2-166">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="62ea2-167">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="62ea2-167">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="62ea2-168">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-168">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="62ea2-169">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-169">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="62ea2-170">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-170">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="62ea2-171">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="62ea2-171">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="62ea2-172">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="62ea2-172">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="62ea2-173">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="62ea2-173">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="62ea2-174">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-174">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="62ea2-175">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-175">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="62ea2-176">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="62ea2-176">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="62ea2-177">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="62ea2-177">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="62ea2-178">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-178">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="62ea2-179">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-179">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="62ea2-180">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="62ea2-180">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="62ea2-181">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="62ea2-181">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="62ea2-182">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="62ea2-182">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="62ea2-183">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="62ea2-183">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="62ea2-184">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-184">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="62ea2-185">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="62ea2-185">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="62ea2-186">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="62ea2-186">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="62ea2-187">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-187">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="62ea2-188">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="62ea2-188">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="62ea2-189">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="62ea2-189">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="62ea2-190">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-190">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="62ea2-191">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-191">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="62ea2-192">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="62ea2-192">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="62ea2-193">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="62ea2-193">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="62ea2-194">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-194">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="62ea2-195">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-195">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="62ea2-196">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="62ea2-196">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="62ea2-197">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="62ea2-197">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="62ea2-198">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="62ea2-198">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="62ea2-199">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="62ea2-199">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="62ea2-200">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="62ea2-200">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="62ea2-201">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="62ea2-201">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="62ea2-202">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="62ea2-202">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="62ea2-203">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="62ea2-203">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="62ea2-204">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="62ea2-204">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="62ea2-205">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="62ea2-205">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="62ea2-206">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="62ea2-206">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="62ea2-207">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="62ea2-207">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="62ea2-208">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-208">Az.Automation</span></span>
* <span data-ttu-id="62ea2-209">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-209">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="62ea2-210">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="62ea2-210">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="62ea2-211">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="62ea2-211">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="62ea2-212">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-212">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="62ea2-213">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="62ea2-213">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="62ea2-214">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-214">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="62ea2-215">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-215">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-216">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-216">Az.Compute</span></span>
* <span data-ttu-id="62ea2-217">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-217">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="62ea2-218">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="62ea2-218">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-219">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-219">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-220">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-220">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="62ea2-221">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="62ea2-221">Az.Monitor</span></span>
* <span data-ttu-id="62ea2-222">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-222">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-223">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-223">Az.Network</span></span>
* <span data-ttu-id="62ea2-224">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-224">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="62ea2-225">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="62ea2-225">Updated cmdlet:</span></span>
        - <span data-ttu-id="62ea2-226">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="62ea2-226">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="62ea2-227">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-227">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-228">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-228">Az.Resources</span></span>
* <span data-ttu-id="62ea2-229">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-229">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-230">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-230">Az.Sql</span></span>
* <span data-ttu-id="62ea2-231">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="62ea2-231">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="62ea2-232">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-232">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="62ea2-233">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-233">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-234">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-234">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="62ea2-235">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-235">Az.CognitiveServices</span></span>
* <span data-ttu-id="62ea2-236">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-236">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="62ea2-237">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-237">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-238">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-238">Az.Compute</span></span>
* <span data-ttu-id="62ea2-239">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="62ea2-239">Proximity placement group feature.</span></span>
    - <span data-ttu-id="62ea2-240">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="62ea2-240">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="62ea2-241">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="62ea2-241">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="62ea2-242">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-242">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="62ea2-243">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-243">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="62ea2-244">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-244">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="62ea2-245">重大な変更</span><span class="sxs-lookup"><span data-stu-id="62ea2-245">Breaking changes</span></span>
    - <span data-ttu-id="62ea2-246">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="62ea2-246">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="62ea2-247">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="62ea2-247">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="62ea2-248">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="62ea2-248">Az.DeploymentManager</span></span>
* <span data-ttu-id="62ea2-249">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="62ea2-249">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="62ea2-250">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="62ea2-250">Az.Dns</span></span>
* <span data-ttu-id="62ea2-251">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="62ea2-251">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="62ea2-252">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="62ea2-252">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="62ea2-253">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-253">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="62ea2-254">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="62ea2-254">Az.FrontDoor</span></span>
* <span data-ttu-id="62ea2-255">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="62ea2-255">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="62ea2-256">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="62ea2-256">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="62ea2-257">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="62ea2-257">Az.HDInsight</span></span>
* <span data-ttu-id="62ea2-258">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-258">Removed two cmdlets:</span></span>
    - <span data-ttu-id="62ea2-259">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="62ea2-259">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="62ea2-260">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="62ea2-260">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="62ea2-261">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-261">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="62ea2-262">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-262">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="62ea2-263">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-263">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="62ea2-264">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="62ea2-264">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="62ea2-265">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="62ea2-265">Az.Monitor</span></span>
* <span data-ttu-id="62ea2-266">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="62ea2-266">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="62ea2-267">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="62ea2-267">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="62ea2-268">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="62ea2-268">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="62ea2-269">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="62ea2-269">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="62ea2-270">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="62ea2-270">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="62ea2-271">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="62ea2-271">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="62ea2-272">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="62ea2-272">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="62ea2-273">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-273">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="62ea2-274">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-274">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="62ea2-275">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-275">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="62ea2-276">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-276">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="62ea2-277">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-277">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="62ea2-278">SQR API に関する[詳細](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="62ea2-278">[More](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="62ea2-279">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-279">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-280">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-280">Az.Network</span></span>
* <span data-ttu-id="62ea2-281">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-281">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="62ea2-282">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-282">New cmdlets</span></span>
        - <span data-ttu-id="62ea2-283">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="62ea2-283">New-AzNatGateway</span></span>
        - <span data-ttu-id="62ea2-284">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="62ea2-284">Get-AzNatGateway</span></span>
        - <span data-ttu-id="62ea2-285">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="62ea2-285">Set-AzNatGateway</span></span>
        - <span data-ttu-id="62ea2-286">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="62ea2-286">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="62ea2-287">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-287">Updated cmdlets</span></span>
        - <span data-ttu-id="62ea2-288">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="62ea2-288">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="62ea2-289">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="62ea2-289">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="62ea2-290">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="62ea2-290">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="62ea2-291">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-291">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="62ea2-292">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-292">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="62ea2-293">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="62ea2-293">Az.PolicyInsights</span></span>
* <span data-ttu-id="62ea2-294">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="62ea2-294">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="62ea2-295">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-295">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="62ea2-296">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="62ea2-296">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-297">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-297">Az.RecoveryServices</span></span>
* <span data-ttu-id="62ea2-298">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="62ea2-298">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="62ea2-299">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="62ea2-299">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="62ea2-300">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="62ea2-300">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="62ea2-301">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="62ea2-301">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="62ea2-302">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="62ea2-302">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="62ea2-303">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="62ea2-303">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="62ea2-304">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="62ea2-304">Az.Relay</span></span>
* <span data-ttu-id="62ea2-305">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-305">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="62ea2-306">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="62ea2-306">Az.ServiceBus</span></span>
* <span data-ttu-id="62ea2-307">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-307">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="62ea2-308">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-308">Az.Storage</span></span>
* <span data-ttu-id="62ea2-309">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="62ea2-309">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="62ea2-310">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-310">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="62ea2-311">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-311">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="62ea2-312">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="62ea2-312">New-AzStorageAccount</span></span>
* <span data-ttu-id="62ea2-313">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="62ea2-313">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="62ea2-314">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="62ea2-314">New-AzStorageAccount</span></span>
    - <span data-ttu-id="62ea2-315">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="62ea2-315">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="62ea2-316">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="62ea2-316">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-317">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-317">Az.Websites</span></span>
* <span data-ttu-id="62ea2-318">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="62ea2-318">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="62ea2-319">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="62ea2-319">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="62ea2-320">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-320">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="62ea2-321">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="62ea2-321">Highlights since the last major release</span></span>
* <span data-ttu-id="62ea2-322">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="62ea2-322">General availability of `Az` module</span></span>
* <span data-ttu-id="62ea2-323">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="62ea2-323">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="62ea2-324">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="62ea2-324">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="62ea2-325">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-325">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="62ea2-326">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-326">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="62ea2-327">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-327">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="62ea2-328">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-328">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="62ea2-329">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-329">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-330">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-330">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="62ea2-331">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="62ea2-331">Az.Batch</span></span>
* <span data-ttu-id="62ea2-332">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-332">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="62ea2-333">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="62ea2-333">Az.Cdn</span></span>
* <span data-ttu-id="62ea2-334">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-334">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="62ea2-335">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-335">Az.CognitiveServices</span></span>
* <span data-ttu-id="62ea2-336">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-336">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-337">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-337">Az.Compute</span></span>
* <span data-ttu-id="62ea2-338">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-338">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="62ea2-339">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-339">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="62ea2-340">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-340">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="62ea2-341">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="62ea2-341">Az.DataFactory</span></span>
* <span data-ttu-id="62ea2-342">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-342">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-343">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-344">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-344">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="62ea2-345">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="62ea2-345">Az.EventGrid</span></span>
* <span data-ttu-id="62ea2-346">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-346">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="62ea2-347">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="62ea2-347">Az.EventHub</span></span>
* <span data-ttu-id="62ea2-348">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-348">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="62ea2-349">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="62ea2-349">Az.HDInsight</span></span>
* <span data-ttu-id="62ea2-350">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-350">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="62ea2-351">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="62ea2-351">Az.IotHub</span></span>
* <span data-ttu-id="62ea2-352">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-352">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="62ea2-353">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="62ea2-353">Az.KeyVault</span></span>
* <span data-ttu-id="62ea2-354">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-354">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="62ea2-355">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-355">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="62ea2-356">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="62ea2-356">Az.MachineLearning</span></span>
* <span data-ttu-id="62ea2-357">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-357">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="62ea2-358">Az.Media</span><span class="sxs-lookup"><span data-stu-id="62ea2-358">Az.Media</span></span>
* <span data-ttu-id="62ea2-359">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-359">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="62ea2-360">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="62ea2-360">Az.Monitor</span></span>
  * <span data-ttu-id="62ea2-361">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-361">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="62ea2-362">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="62ea2-362">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="62ea2-363">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="62ea2-363">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="62ea2-364">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="62ea2-364">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="62ea2-365">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="62ea2-365">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="62ea2-366">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="62ea2-366">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="62ea2-367">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-367">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-368">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-368">Az.Network</span></span>
* <span data-ttu-id="62ea2-369">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-369">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="62ea2-370">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-370">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="62ea2-371">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="62ea2-371">Az.NotificationHubs</span></span>
* <span data-ttu-id="62ea2-372">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-372">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="62ea2-373">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="62ea2-373">Az.OperationalInsights</span></span>
* <span data-ttu-id="62ea2-374">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-374">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="62ea2-375">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="62ea2-375">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="62ea2-376">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-376">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-377">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-377">Az.RecoveryServices</span></span>
* <span data-ttu-id="62ea2-378">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-378">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="62ea2-379">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-379">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="62ea2-380">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-380">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="62ea2-381">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-381">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="62ea2-382">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="62ea2-382">Az.RedisCache</span></span>
* <span data-ttu-id="62ea2-383">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-383">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-384">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-384">Az.Resources</span></span>
* <span data-ttu-id="62ea2-385">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-385">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-386">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-386">Az.Sql</span></span>
* <span data-ttu-id="62ea2-387">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="62ea2-387">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="62ea2-388">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-388">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="62ea2-389">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-389">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="62ea2-390">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-390">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="62ea2-391">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="62ea2-391">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="62ea2-392">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="62ea2-392">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="62ea2-393">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-393">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-394">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-394">Az.Websites</span></span>
* <span data-ttu-id="62ea2-395">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-395">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="62ea2-396">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-396">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="62ea2-397">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-397">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="62ea2-398">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-398">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="62ea2-399">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-399">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="62ea2-400">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="62ea2-400">Highlights since the last major release</span></span>
* <span data-ttu-id="62ea2-401">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="62ea2-401">General availability of `Az` module</span></span>
* <span data-ttu-id="62ea2-402">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="62ea2-402">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="62ea2-403">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="62ea2-403">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="62ea2-404">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-404">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="62ea2-405">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-405">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="62ea2-406">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-406">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="62ea2-407">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-407">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="62ea2-408">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-408">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-409">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-409">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="62ea2-410">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-410">Az.AnalysisServices</span></span>
* <span data-ttu-id="62ea2-411">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="62ea2-411">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="62ea2-412">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-412">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="62ea2-413">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-413">Az.Automation</span></span>
* <span data-ttu-id="62ea2-414">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-414">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="62ea2-415">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-415">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="62ea2-416">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-416">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-417">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-417">Az.Compute</span></span>
* <span data-ttu-id="62ea2-418">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-418">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="62ea2-419">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-419">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="62ea2-420">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-420">Az.ContainerInstance</span></span>
* <span data-ttu-id="62ea2-421">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-421">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="62ea2-422">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="62ea2-422">Az.DataFactory</span></span>
* <span data-ttu-id="62ea2-423">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-423">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="62ea2-424">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-424">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-425">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-425">Az.Resources</span></span>
* <span data-ttu-id="62ea2-426">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-426">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="62ea2-427">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-427">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="62ea2-428">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="62ea2-428">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="62ea2-429">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="62ea2-429">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="62ea2-430">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-430">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="62ea2-431">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="62ea2-431">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-432">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-432">Az.Sql</span></span>
* <span data-ttu-id="62ea2-433">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-433">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="62ea2-434">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-434">Az.Storage</span></span>
* <span data-ttu-id="62ea2-435">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="62ea2-435">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="62ea2-436">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="62ea2-436">New-AzStorageContext</span></span>
* <span data-ttu-id="62ea2-437">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="62ea2-437">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="62ea2-438">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="62ea2-438">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="62ea2-439">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="62ea2-439">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="62ea2-440">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="62ea2-440">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="62ea2-441">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="62ea2-441">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="62ea2-442">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="62ea2-442">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="62ea2-443">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="62ea2-443">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="62ea2-444">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="62ea2-444">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="62ea2-445">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="62ea2-445">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="62ea2-446">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="62ea2-446">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="62ea2-447">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-447">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="62ea2-448">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="62ea2-448">Highlights since the last major release</span></span>
* <span data-ttu-id="62ea2-449">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="62ea2-449">General availability of `Az` module</span></span>
* <span data-ttu-id="62ea2-450">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="62ea2-450">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="62ea2-451">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="62ea2-451">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="62ea2-452">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-452">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="62ea2-453">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-453">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="62ea2-454">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-454">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="62ea2-455">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-455">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="62ea2-456">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-456">Az.Automation</span></span>
* <span data-ttu-id="62ea2-457">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-457">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="62ea2-458">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="62ea2-458">Dynamic grouping</span></span>
    * <span data-ttu-id="62ea2-459">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="62ea2-459">Pre-Post script</span></span>
    * <span data-ttu-id="62ea2-460">再起動設定</span><span class="sxs-lookup"><span data-stu-id="62ea2-460">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-461">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-461">Az.Compute</span></span>
* <span data-ttu-id="62ea2-462">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-462">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="62ea2-463">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-463">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="62ea2-464">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="62ea2-464">Az.KeyVault</span></span>
* <span data-ttu-id="62ea2-465">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-465">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-466">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-466">Az.Network</span></span>
* <span data-ttu-id="62ea2-467">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-467">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="62ea2-468">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-468">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-469">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-469">Az.RecoveryServices</span></span>
* <span data-ttu-id="62ea2-470">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-470">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="62ea2-471">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-471">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-472">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-472">Az.Resources</span></span>
* <span data-ttu-id="62ea2-473">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-473">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="62ea2-474">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-474">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-475">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-475">Az.Sql</span></span>
* <span data-ttu-id="62ea2-476">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-476">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="62ea2-477">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-477">Az.Storage</span></span>
* <span data-ttu-id="62ea2-478">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="62ea2-478">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="62ea2-479">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="62ea2-479">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="62ea2-480">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="62ea2-480">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="62ea2-481">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="62ea2-481">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="62ea2-482">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="62ea2-482">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="62ea2-483">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="62ea2-483">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="62ea2-484">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-484">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-485">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-485">Az.Websites</span></span>
* <span data-ttu-id="62ea2-486">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-486">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="62ea2-487">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-487">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="62ea2-488">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-488">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-489">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-489">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="62ea2-490">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-490">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="62ea2-491">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-491">Az.Automation</span></span>
* <span data-ttu-id="62ea2-492">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-492">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="62ea2-493">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-493">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="62ea2-494">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="62ea2-494">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="62ea2-495">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="62ea2-495">Az.Cdn</span></span>
* <span data-ttu-id="62ea2-496">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="62ea2-496">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-497">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-497">Az.Compute</span></span>
* <span data-ttu-id="62ea2-498">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-498">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="62ea2-499">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="62ea2-499">Az.DataFactory</span></span>
* <span data-ttu-id="62ea2-500">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-500">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="62ea2-501">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="62ea2-501">Az.LogicApp</span></span>
* <span data-ttu-id="62ea2-502">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-502">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-503">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-503">Az.Network</span></span>
* <span data-ttu-id="62ea2-504">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-504">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-505">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-505">Az.RecoveryServices</span></span>
* <span data-ttu-id="62ea2-506">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-506">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="62ea2-507">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-507">SDK Update</span></span>
* <span data-ttu-id="62ea2-508">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-508">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="62ea2-509">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-509">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-510">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-510">Az.Resources</span></span>
* <span data-ttu-id="62ea2-511">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-511">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="62ea2-512">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="62ea2-512">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="62ea2-513">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-513">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="62ea2-514">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="62ea2-514">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="62ea2-515">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-515">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="62ea2-516">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="62ea2-516">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-517">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-517">Az.Sql</span></span>
* <span data-ttu-id="62ea2-518">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-518">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="62ea2-519">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-519">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="62ea2-520">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-520">Az.Storage</span></span>
* <span data-ttu-id="62ea2-521">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="62ea2-521">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="62ea2-522">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-522">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="62ea2-523">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-523">Az.AnalysisServices</span></span>
* <span data-ttu-id="62ea2-524">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="62ea2-524">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="62ea2-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-525">Az.Automation</span></span>
* <span data-ttu-id="62ea2-526">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-526">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="62ea2-527">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-527">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="62ea2-528">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-528">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="62ea2-529">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-529">Az.CognitiveServices</span></span>
* <span data-ttu-id="62ea2-530">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-530">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-531">Az.Compute</span></span>
* <span data-ttu-id="62ea2-532">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-532">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="62ea2-533">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-533">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="62ea2-534">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-534">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="62ea2-535">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="62ea2-535">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-536">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-536">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-537">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-537">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="62ea2-538">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="62ea2-538">Az.EventHub</span></span>
* <span data-ttu-id="62ea2-539">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-539">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="62ea2-540">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="62ea2-540">Az.KeyVault</span></span>
* <span data-ttu-id="62ea2-541">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-541">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="62ea2-542">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="62ea2-542">Az.LogicApp</span></span>
* <span data-ttu-id="62ea2-543">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-543">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="62ea2-544">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-544">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="62ea2-545">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-545">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="62ea2-546">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="62ea2-546">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="62ea2-547">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="62ea2-547">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="62ea2-548">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="62ea2-548">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="62ea2-549">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="62ea2-549">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="62ea2-550">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-550">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="62ea2-551">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ea2-551">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="62ea2-552">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ea2-552">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="62ea2-553">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ea2-553">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="62ea2-554">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ea2-554">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="62ea2-555">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-555">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="62ea2-556">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="62ea2-556">Az.Monitor</span></span>
* <span data-ttu-id="62ea2-557">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-557">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-558">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-558">Az.Network</span></span>
* <span data-ttu-id="62ea2-559">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-559">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="62ea2-560">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="62ea2-560">Az.OperationalInsights</span></span>
* <span data-ttu-id="62ea2-561">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-561">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="62ea2-562">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-562">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="62ea2-563">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-563">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="62ea2-564">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-564">Az.Resources</span></span>
* <span data-ttu-id="62ea2-565">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="62ea2-565">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="62ea2-566">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="62ea2-566">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="62ea2-567">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="62ea2-567">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="62ea2-568">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-568">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-569">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-569">Az.Sql</span></span>
* <span data-ttu-id="62ea2-570">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-570">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="62ea2-571">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-571">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-572">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-572">Az.Websites</span></span>
* <span data-ttu-id="62ea2-573">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-573">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="62ea2-574">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-574">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="62ea2-575">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-575">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-576">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-576">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="62ea2-577">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-577">Az.AnalysisServices</span></span>
<span data-ttu-id="62ea2-578">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="62ea2-578">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-579">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-579">Az.Compute</span></span>
* <span data-ttu-id="62ea2-580">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-580">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="62ea2-581">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-581">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="62ea2-582">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-582">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-583">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-583">Az.RecoveryServices</span></span>
<span data-ttu-id="62ea2-584">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="62ea2-584">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-585">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-585">Az.Resources</span></span>
* <span data-ttu-id="62ea2-586">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-586">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="62ea2-587">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="62ea2-587">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="62ea2-588">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-588">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="62ea2-589">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="62ea2-589">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-590">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-590">Az.Sql</span></span>
* <span data-ttu-id="62ea2-591">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-591">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="62ea2-592">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-592">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="62ea2-593">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-593">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="62ea2-594">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-594">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="62ea2-595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-595">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-596">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="62ea2-596">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="62ea2-597">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-597">Az.AnalysisServices</span></span>
* <span data-ttu-id="62ea2-598">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="62ea2-598">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-599">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-599">Az.RecoveryServices</span></span>
* <span data-ttu-id="62ea2-600">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="62ea2-600">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="62ea2-601">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-601">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="62ea2-602">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-602">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-603">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-603">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="62ea2-604">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-604">Update incorrect online help URLs</span></span>
* <span data-ttu-id="62ea2-605">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-605">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="62ea2-606">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="62ea2-606">Az.Aks</span></span>
* <span data-ttu-id="62ea2-607">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-607">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="62ea2-608">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-608">Az.Automation</span></span>
* <span data-ttu-id="62ea2-609">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-609">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="62ea2-610">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-610">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="62ea2-611">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="62ea2-611">Az.Cdn</span></span>
* <span data-ttu-id="62ea2-612">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-612">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-613">Az.Compute</span></span>
* <span data-ttu-id="62ea2-614">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-614">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="62ea2-615">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-615">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="62ea2-616">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-616">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="62ea2-617">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="62ea2-617">Az.ContainerRegistry</span></span>
* <span data-ttu-id="62ea2-618">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-618">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="62ea2-619">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="62ea2-619">Az.DataFactory</span></span>
* <span data-ttu-id="62ea2-620">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-620">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-621">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-621">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-622">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="62ea2-622">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="62ea2-623">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="62ea2-623">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="62ea2-624">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-624">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="62ea2-625">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="62ea2-625">Az.IotHub</span></span>
* <span data-ttu-id="62ea2-626">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-626">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="62ea2-627">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="62ea2-627">Az.KeyVault</span></span>
* <span data-ttu-id="62ea2-628">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-628">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-629">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-629">Az.Network</span></span>
* <span data-ttu-id="62ea2-630">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-630">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-631">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-631">Az.Resources</span></span>
* <span data-ttu-id="62ea2-632">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-632">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="62ea2-633">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-633">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="62ea2-634">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-634">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="62ea2-635">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="62ea2-635">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="62ea2-636">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="62ea2-636">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="62ea2-637">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-637">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="62ea2-638">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="62ea2-638">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="62ea2-639">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="62ea2-639">Az.ServiceFabric</span></span>
* <span data-ttu-id="62ea2-640">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="62ea2-640">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="62ea2-641">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-641">Fix some error messages.</span></span>
* <span data-ttu-id="62ea2-642">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-642">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="62ea2-643">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-643">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="62ea2-644">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="62ea2-644">Az.SignalR</span></span>
* <span data-ttu-id="62ea2-645">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-645">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-646">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-646">Az.Sql</span></span>
* <span data-ttu-id="62ea2-647">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-647">Update incorrect online help URLs</span></span>
* <span data-ttu-id="62ea2-648">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-648">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="62ea2-649">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-649">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="62ea2-650">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="62ea2-650">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="62ea2-651">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-651">Az.Storage</span></span>
* <span data-ttu-id="62ea2-652">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="62ea2-653">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="62ea2-653">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="62ea2-654">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="62ea2-654">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="62ea2-655">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="62ea2-655">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="62ea2-656">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="62ea2-656">Az.TrafficManager</span></span>
* <span data-ttu-id="62ea2-657">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-657">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-658">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-658">Az.Websites</span></span>
* <span data-ttu-id="62ea2-659">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-659">Update incorrect online help URLs</span></span>
* <span data-ttu-id="62ea2-660">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-660">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="62ea2-661">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="62ea2-661">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="62ea2-662">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-662">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="62ea2-663">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-663">Az.Accounts</span></span>
* <span data-ttu-id="62ea2-664">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="62ea2-664">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-665">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-665">Az.Compute</span></span>
* <span data-ttu-id="62ea2-666">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-666">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="62ea2-667">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="62ea2-667">Updated the description of ID in help files</span></span>
* <span data-ttu-id="62ea2-668">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-668">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-669">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-669">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-670">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-670">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="62ea2-671">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-671">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="62ea2-672">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="62ea2-672">Az.EventGrid</span></span>
* <span data-ttu-id="62ea2-673">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-673">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="62ea2-674">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="62ea2-674">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="62ea2-675">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="62ea2-675">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="62ea2-676">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="62ea2-676">Event Time-To-Live,</span></span>
        - <span data-ttu-id="62ea2-677">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="62ea2-677">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="62ea2-678">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="62ea2-678">Dead letter endpoint.</span></span>
    - <span data-ttu-id="62ea2-679">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="62ea2-679">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="62ea2-680">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="62ea2-680">Event Time-To-Live,</span></span>
        - <span data-ttu-id="62ea2-681">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="62ea2-681">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="62ea2-682">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="62ea2-682">Dead letter endpoint.</span></span>
* <span data-ttu-id="62ea2-683">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-683">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="62ea2-684">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-684">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="62ea2-685">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="62ea2-685">Az.IotHub</span></span>
* <span data-ttu-id="62ea2-686">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-686">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="62ea2-687">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="62ea2-687">Az.LogicApp</span></span>
* <span data-ttu-id="62ea2-688">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="62ea2-688">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-689">Az.Resources</span></span>
* <span data-ttu-id="62ea2-690">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-690">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="62ea2-691">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="62ea2-691">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="62ea2-692">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-692">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="62ea2-693">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-693">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="62ea2-694">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="62ea2-694">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="62ea2-695">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="62ea2-695">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="62ea2-696">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="62ea2-696">Az.SignalR</span></span>
* <span data-ttu-id="62ea2-697">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-697">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-698">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-698">Az.Sql</span></span>
* <span data-ttu-id="62ea2-699">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-699">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="62ea2-700">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-700">Az.Storage</span></span>
* <span data-ttu-id="62ea2-701">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="62ea2-701">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="62ea2-702">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="62ea2-702">New-AzStorageContext</span></span>
* <span data-ttu-id="62ea2-703">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-703">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="62ea2-704">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="62ea2-704">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-705">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-705">Az.Websites</span></span>
* <span data-ttu-id="62ea2-706">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-706">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="62ea2-707">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-707">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="62ea2-708">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-708">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="62ea2-709">全般</span><span class="sxs-lookup"><span data-stu-id="62ea2-709">General</span></span>

- <span data-ttu-id="62ea2-710">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="62ea2-710">General Availability of Az Module</span></span>
- <span data-ttu-id="62ea2-711">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="62ea2-711">Online help for each module</span></span>
- <span data-ttu-id="62ea2-712">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-712">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="62ea2-713">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-713">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="62ea2-714">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="62ea2-714">Az.Accounts</span></span>
- <span data-ttu-id="62ea2-715">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-715">Changed from Az.Profile</span></span>
- <span data-ttu-id="62ea2-716">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-716">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="62ea2-717">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="62ea2-717">Az.ApiManagement</span></span>
- <span data-ttu-id="62ea2-718">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="62ea2-718">Fixes for #7002</span></span>
- <span data-ttu-id="62ea2-719">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-719">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="62ea2-720">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="62ea2-720">Az.Batch</span></span>
- <span data-ttu-id="62ea2-721">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-721">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="62ea2-722">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-722">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="62ea2-723">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-723">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="62ea2-724">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="62ea2-724">Az.Billing</span></span>
- <span data-ttu-id="62ea2-725">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-725">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="62ea2-726">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-726">Az.CognitivServices</span></span>
- <span data-ttu-id="62ea2-727">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-727">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="62ea2-728">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-728">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="62ea2-729">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-729">Az.ContainerInstance</span></span>
- <span data-ttu-id="62ea2-730">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-730">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="62ea2-731">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="62ea2-731">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="62ea2-732">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-732">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-733">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-733">Az.DataLakeStore</span></span>
- <span data-ttu-id="62ea2-734">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-734">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="62ea2-735">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="62ea2-735">Az.Monitor</span></span>
- <span data-ttu-id="62ea2-736">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-736">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="62ea2-737">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="62ea2-737">Az.KeyVault</span></span>
- <span data-ttu-id="62ea2-738">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-738">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="62ea2-739">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="62ea2-739">Az.MachineLearning</span></span>
- <span data-ttu-id="62ea2-740">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="62ea2-740">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="62ea2-741">Az.Media</span><span class="sxs-lookup"><span data-stu-id="62ea2-741">Az.Media</span></span>
- <span data-ttu-id="62ea2-742">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-742">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="62ea2-743">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-743">Az.Network</span></span>
<span data-ttu-id="62ea2-744">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-744">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="62ea2-745">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="62ea2-745">New cmdlets added:</span></span>
        - <span data-ttu-id="62ea2-746">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="62ea2-746">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="62ea2-747">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="62ea2-747">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="62ea2-748">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="62ea2-748">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="62ea2-749">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="62ea2-749">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="62ea2-750">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="62ea2-750">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="62ea2-751">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-751">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="62ea2-752">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="62ea2-752">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="62ea2-753">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="62ea2-753">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="62ea2-754">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-754">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="62ea2-755">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="62ea2-755">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="62ea2-756">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-756">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="62ea2-757">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="62ea2-757">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="62ea2-758">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="62ea2-758">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="62ea2-759">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="62ea2-759">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="62ea2-760">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-760">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="62ea2-761">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-761">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="62ea2-762">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="62ea2-762">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="62ea2-763">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="62ea2-763">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="62ea2-764">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="62ea2-764">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="62ea2-765">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-765">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="62ea2-766">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-766">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="62ea2-767">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="62ea2-767">Az.OperationalInsights</span></span>
- <span data-ttu-id="62ea2-768">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-768">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="62ea2-769">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="62ea2-769">Az.Profile</span></span>
- <span data-ttu-id="62ea2-770">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-770">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-771">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-771">Az.RecoveryServices</span></span>
- <span data-ttu-id="62ea2-772">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-772">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="62ea2-773">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-773">Az.Resources</span></span>
- <span data-ttu-id="62ea2-774">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-774">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="62ea2-775">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="62ea2-775">Az.ServiceFabric</span></span>
- <span data-ttu-id="62ea2-776">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="62ea2-776">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="62ea2-777">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-777">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="62ea2-778">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="62ea2-778">Az.SIgnalR</span></span>
- <span data-ttu-id="62ea2-779">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="62ea2-779">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="62ea2-780">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-780">Az.Sql</span></span>
- <span data-ttu-id="62ea2-781">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-781">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="62ea2-782">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-782">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="62ea2-783">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-783">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="62ea2-784">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-784">Az.Storage</span></span>
- <span data-ttu-id="62ea2-785">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-785">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="62ea2-786">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-786">Az.Websites</span></span>
- <span data-ttu-id="62ea2-787">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="62ea2-787">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="62ea2-788">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-788">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="62ea2-789">全般</span><span class="sxs-lookup"><span data-stu-id="62ea2-789">General</span></span>

* <span data-ttu-id="62ea2-790">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="62ea2-790">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="62ea2-791">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-791">Az.Compute</span></span>

* <span data-ttu-id="62ea2-792">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-792">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-793">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-793">Az.DataLakeStore</span></span>

* <span data-ttu-id="62ea2-794">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-794">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="62ea2-795">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="62ea2-795">Az.FrontDoor</span></span>

* <span data-ttu-id="62ea2-796">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-796">Fixed some broken links</span></span>
    - <span data-ttu-id="62ea2-797">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-797">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="62ea2-798">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-798">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="62ea2-799">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-799">Az.RecoveryServices</span></span>

* <span data-ttu-id="62ea2-800">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-800">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="62ea2-801">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-801">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="62ea2-802">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-802">Az.Resources</span></span>

* <span data-ttu-id="62ea2-803">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-803">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="62ea2-804">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-804">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="62ea2-805">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-805">Az.Sql</span></span>

* <span data-ttu-id="62ea2-806">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="62ea2-806">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="62ea2-807">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-807">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="62ea2-808">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-808">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="62ea2-809">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-809">Az.Storage</span></span>

* <span data-ttu-id="62ea2-810">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-810">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="62ea2-811">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-811">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="62ea2-812">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="62ea2-812">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="62ea2-813">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="62ea2-813">Support Static Website configuration</span></span>
    - <span data-ttu-id="62ea2-814">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="62ea2-814">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="62ea2-815">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="62ea2-815">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="62ea2-816">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-816">Az.Websites</span></span>

* <span data-ttu-id="62ea2-817">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="62ea2-817">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="62ea2-818">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-818">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="62ea2-819">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="62ea2-819">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="62ea2-820">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-820">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="62ea2-821">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="62ea2-821">Az.ApiManagement</span></span>
* <span data-ttu-id="62ea2-822">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-822">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="62ea2-823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="62ea2-823">Az.Automation</span></span>
* <span data-ttu-id="62ea2-824">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="62ea2-824">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="62ea2-825">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-825">Added Update Management cmdlets</span></span>
* <span data-ttu-id="62ea2-826">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-826">Added Source Control cmdlets</span></span>
* <span data-ttu-id="62ea2-827">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-827">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="62ea2-828">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-828">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="62ea2-829">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-829">Az.Compute</span></span>
* <span data-ttu-id="62ea2-830">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-830">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="62ea2-831">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-831">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="62ea2-832">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-832">Az.ContainerInstance</span></span>
* <span data-ttu-id="62ea2-833">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-833">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="62ea2-834">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="62ea2-834">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="62ea2-835">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-835">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="62ea2-836">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-836">Az.Network</span></span>
* <span data-ttu-id="62ea2-837">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-837">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="62ea2-838">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-838">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="62ea2-839">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-839">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="62ea2-840">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-840">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="62ea2-841">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="62ea2-841">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="62ea2-842">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-842">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="62ea2-843">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-843">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="62ea2-844">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="62ea2-844">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="62ea2-845">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-845">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="62ea2-846">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-846">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="62ea2-847">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="62ea2-847">Az.Relay</span></span>
* <span data-ttu-id="62ea2-848">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="62ea2-848">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="62ea2-849">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-849">Az.Resources</span></span>
* <span data-ttu-id="62ea2-850">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-850">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="62ea2-851">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-851">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="62ea2-852">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="62ea2-852">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="62ea2-853">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="62ea2-853">Az.ServiceFabric</span></span>
* <span data-ttu-id="62ea2-854">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-854">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="62ea2-855">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-855">Az.Sql</span></span>
* <span data-ttu-id="62ea2-856">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-856">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="62ea2-857">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-857">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="62ea2-858">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-858">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="62ea2-859">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-859">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="62ea2-860">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="62ea2-860">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="62ea2-861">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="62ea2-861">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="62ea2-862">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="62ea2-862">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="62ea2-863">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="62ea2-863">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="62ea2-864">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="62ea2-864">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="62ea2-865">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="62ea2-865">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="62ea2-866">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-866">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="62ea2-867">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-867">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="62ea2-868">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="62ea2-868">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="62ea2-869">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="62ea2-869">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="62ea2-870">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="62ea2-870">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="62ea2-871">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="62ea2-871">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="62ea2-872">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-872">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="62ea2-873">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-873">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="62ea2-874">全般</span><span class="sxs-lookup"><span data-stu-id="62ea2-874">General</span></span>
* <span data-ttu-id="62ea2-875">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="62ea2-875">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="62ea2-876">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="62ea2-876">Az.Profile</span></span>
* <span data-ttu-id="62ea2-877">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-877">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="62ea2-878">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-878">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="62ea2-879">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-879">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="62ea2-880">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-880">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="62ea2-881">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-881">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="62ea2-882">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-882">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="62ea2-883">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-883">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="62ea2-884">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-884">Az.CognitiveServices</span></span>
* <span data-ttu-id="62ea2-885">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-885">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-886">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-886">Az.Compute</span></span>
* <span data-ttu-id="62ea2-887">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-887">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="62ea2-888">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="62ea2-888">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="62ea2-889">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-889">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-890">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-890">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-891">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-891">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="62ea2-892">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-892">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="62ea2-893">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="62ea2-893">Az.Insights</span></span>
* <span data-ttu-id="62ea2-894">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-894">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="62ea2-895">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="62ea2-895">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="62ea2-896">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-896">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="62ea2-897">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="62ea2-897">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-898">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-898">Az.Network</span></span>
* <span data-ttu-id="62ea2-899">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="62ea2-899">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="62ea2-900">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="62ea2-900">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="62ea2-901">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="62ea2-901">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="62ea2-902">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="62ea2-902">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="62ea2-903">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="62ea2-903">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="62ea2-904">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="62ea2-904">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="62ea2-905">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="62ea2-905">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="62ea2-906">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="62ea2-906">Az.PolicyInsights</span></span>
* <span data-ttu-id="62ea2-907">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-907">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-908">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-908">Az.Resources</span></span>
* <span data-ttu-id="62ea2-909">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-909">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="62ea2-910">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-910">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="62ea2-911">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="62ea2-911">Az.ServiceBus</span></span>
* <span data-ttu-id="62ea2-912">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-912">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="62ea2-913">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="62ea2-913">Az.ServiceFabric</span></span>
* <span data-ttu-id="62ea2-914">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-914">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="62ea2-915">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-915">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="62ea2-916">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="62ea2-916">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="62ea2-917">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="62ea2-917">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="62ea2-918">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-918">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="62ea2-919">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-919">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="62ea2-920">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="62ea2-920">Az.Profile</span></span>
* <span data-ttu-id="62ea2-921">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-921">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="62ea2-922">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-922">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-923">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-923">Az.Compute</span></span>
* <span data-ttu-id="62ea2-924">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-924">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="62ea2-925">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-925">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="62ea2-926">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="62ea2-926">Az.DataLakeStore</span></span>
* <span data-ttu-id="62ea2-927">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-927">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="62ea2-928">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-928">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="62ea2-929">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-929">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="62ea2-930">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-930">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="62ea2-931">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="62ea2-931">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-932">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-932">Az.Network</span></span>
* <span data-ttu-id="62ea2-933">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-933">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="62ea2-934">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-934">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-935">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-935">Az.Resources</span></span>
* <span data-ttu-id="62ea2-936">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-936">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="62ea2-937">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-937">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="62ea2-938">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-938">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="62ea2-939">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="62ea2-939">Azure.Storage</span></span>
* <span data-ttu-id="62ea2-940">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-940">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="62ea2-941">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="62ea2-941">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="62ea2-942">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="62ea2-942">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="62ea2-943">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-943">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="62ea2-944">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="62ea2-944">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="62ea2-945">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="62ea2-945">Az.CognitiveServices</span></span>
* <span data-ttu-id="62ea2-946">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-946">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="62ea2-947">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="62ea2-947">Az.Compute</span></span>
* <span data-ttu-id="62ea2-948">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-948">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="62ea2-949">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-949">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="62ea2-950">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-950">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="62ea2-951">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="62ea2-951">Az.DataFactoryV2</span></span>
* <span data-ttu-id="62ea2-952">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-952">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="62ea2-953">Az.Network</span><span class="sxs-lookup"><span data-stu-id="62ea2-953">Az.Network</span></span>
* <span data-ttu-id="62ea2-954">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="62ea2-954">Added NetworkProfile functionality.</span></span> <span data-ttu-id="62ea2-955">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="62ea2-955">new cmdlets added</span></span>
    - <span data-ttu-id="62ea2-956">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="62ea2-956">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="62ea2-957">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="62ea2-957">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="62ea2-958">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="62ea2-958">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="62ea2-959">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="62ea2-959">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="62ea2-960">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="62ea2-960">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="62ea2-961">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="62ea2-961">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="62ea2-962">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-962">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="62ea2-963">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-963">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="62ea2-964">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-964">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="62ea2-965">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="62ea2-965">Az.RedisCache</span></span>
* <span data-ttu-id="62ea2-966">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="62ea2-966">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="62ea2-967">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-967">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="62ea2-968">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="62ea2-968">Az.Resources</span></span>
* <span data-ttu-id="62ea2-969">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-969">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="62ea2-970">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-970">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="62ea2-971">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="62ea2-971">Az.Sql</span></span>
* <span data-ttu-id="62ea2-972">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="62ea2-972">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="62ea2-973">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="62ea2-973">Az.Websites</span></span>
* <span data-ttu-id="62ea2-974">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="62ea2-974">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="62ea2-975">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="62ea2-975">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="62ea2-976">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="62ea2-976">0.2.0 - September 2018</span></span>
 <span data-ttu-id="62ea2-977">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="62ea2-977">Initial Release</span></span>