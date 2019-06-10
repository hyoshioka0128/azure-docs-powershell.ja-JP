---
ms.openlocfilehash: 911e1f7ff56feab2735f397a0128aab4aa7757c7
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498677"
---
## <a name="220---june-2019"></a>2.2.0 - 2019 年 6 月
#### <a name="azcdn"></a>Az.Cdn
* API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。

#### <a name="azcompute"></a>Az.Compute
* 操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。
    - 更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM

#### <a name="azeventhub"></a>Az.EventHub
* #9231 (Get AzEventHubNamespace がタグを返さない) を修正しました
* #9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました

#### <a name="aznetwork"></a>Az.Network
* Nat Gateway の ResourceId と InputObject を更新しました
    - ResourceId と InputObject のエイリアスを追加しました

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Get-AzPolicyEvent の null 参照の問題を修正しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました

#### <a name="azservicebus"></a>Az.ServiceBus
* #9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました
* Service Fabric のコマンドラインの文字の不足を修正しました

#### <a name="azsql"></a>Az.Sql
* Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。
* Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化
* Threat Protection の名前を Advanced Threat Protection に変更しました
* New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。

#### <a name="azwebsites"></a>Az.Websites
* Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました

## <a name="210---may-2019"></a>2.1.0 - 2019 年 5 月
#### <a name="azapimanagement"></a>Az.ApiManagement
* グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました
    - **Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します
    - **New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します
    - **New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します
    - **New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。
    - **New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します
    - **Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します
    - **Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します
* ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました
    - **Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します
    - **New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します
    - **Remove-AzApiManagementCache** - キャッシュを削除します
    - **Update-AzApiManagementCache** - キャッシュを更新します
* API スキーマの管理用に作成された新しいコマンドレット
    - **New-AzApiManagementSchema** - API の新しいスキーマを作成します
    - **Get-AzApiManagementSchema** - API で構成されたスキーマを取得します
    - **Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します
    - **Set-AzApiManagementSchema** - API で構成されたスキーマを更新します
* ユーザー トークンを生成するための新しいコマンドレットを作成しました。 
    - **New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/
* ネットワークの状態を取得する新しいコマンドレットを作成しました
    - **Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。 これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。
* ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました 
    - 新しい 'Consumption' SKU のサポートを追加しました
    - 'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました
    - 新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。 これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。
    - ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。
* 'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました
* エラー メッセージをインラインで表示するコマンドレットを更新しました 
     > PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]
* API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました
* コマンドレット **Import-AzApiManagementApi** を次のように更新しました
    - API を 'OpenApi 3.0' ドキュメント仕様からインポートする
    - 任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。
    - 任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。
* 'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました
* 'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました
* コマンドレット **New-AzApiManagementApi** を次のように更新しました 
    - 'OpenId' 承認サーバーで API を構成する。
    - 'ApiVersionSet' に API を作成する
    - 'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。
    - API スコープで 'SubscriptionRequired' を構成できるようになりました。 
* コマンドレット **Set-AzApiManagementApi** を次のように更新しました
    - 'OpenId' 承認サーバーで API を構成する。
    - 'ApiVersionSet' に API を更新する    
    - API スコープで 'SubscriptionRequired' を構成できるようになりました。 
* コマンドレット **New-AzApiManagementRevision** を次のように更新しました
    - 'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。 新しいリビジョンは親の 'ApiId' を前提としています。
    - 'ApiRevisionDescription' を入力する
    - API を複製するときに 'ServiceUrl' をオーバーライドする。
* コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました
    - 'AAD' または 'AADB2C' と 'Authority' を構成する
    - 'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する
* コマンドレット **New-AzApiManagementSubscription** を次のように更新しました
    - 'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する
    - 'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する
    - サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。
* コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました
    - 'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する
    - 'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する
    - サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。
* 'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました
    - 'New-AzApiManagementContext'
        > New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso
    - 'Get-AzApiManagementApiRelease'
        > Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId
    - 'Get-AzApiManagementApiVersionSet'
        > Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset
    - 'Get-AzApiManagementAuthorizationServer'
    - 'Get-AzApiManagementBackend'
        > Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric
    - 'Get-AzApiManagementCertificate' 
    - 'Remove-AzApiManagementApiVersionSet'
    - 'Remove-AzApiManagementSubscription'

#### <a name="azautomation"></a>Az.Automation
* JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。
    - 次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977
    - 次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600
* Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。
    * 次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347
* -Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。 これで一致するノードのみが返されるようになりました。

#### <a name="azcompute"></a>Az.Compute
* AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。
* これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました

#### <a name="azmonitor"></a>Az.Monitor
* ヘルプの例で正しくないパラメーター名を修正しました

#### <a name="aznetwork"></a>Az.Network
* 有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました
    - 更新されたコマンドレット:
        - Get-AzEffectiveRouteTable
* New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました

#### <a name="azresources"></a>Az.Resources
* 拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました

#### <a name="azsql"></a>Az.Sql
* Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました

## <a name="200---may-2019"></a>2.0.0 - 2019 年 5 月
#### <a name="azaccounts"></a>Az.Accounts
* ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Bing Search Services について、Bing の免責事項のみを表示します。
* アカウントの作成が失敗したときのエラーを改善しました。

#### <a name="azcompute"></a>Az.Compute
* 近接通信配置グループ機能。
    - 次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup
    - 新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig
* New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。
* New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。
* Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました       
* 重大な変更
    - Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。
    - Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。

#### <a name="azdeploymentmanager"></a>Az.DeploymentManager
* Azure Deployment Manager コマンドレットの最初の一般公開リリース

#### <a name="azdns"></a>Az.Dns
* DNS NameServer の自動委任
    - DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。
    - 新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Azure FrontDoor コマンドレットの最初の一般公開リリース
* WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a>Az.HDInsight
* 次の 2 つのコマンドレットを削除しました。
    - Grant-AzHDInsightHttpServicesAccess
    - Revoke-AzHDInsightHttpServicesAccess
* Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました
* 閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。
    - 閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。
    - hdinsight オペレーター ロールを持つユーザーは影響を受けません。

#### <a name="azmonitor"></a>Az.Monitor
* SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)  
    - New-AzScheduledQueryRuleAlertingAction
    - New-AzScheduledQueryRuleAznsActionGroup
    - New-AzScheduledQueryRuleLogMetricTrigger
    - New-AzScheduledQueryRuleSchedule
    - New-AzScheduledQueryRuleSource
    - New-AzScheduledQueryRuleTriggerCondition
    - New-AzScheduledQueryRule
    - Get-AzScheduledQueryRule
    - Set-AzScheduledQueryRule
    - Update-AzScheduledQueryRule
    - Remove-AzScheduledQueryRule
    - SQR API に関する[詳細](https://docs.microsoft.com/en-us/rest/api/monitor/scheduledqueryrules)情報
    - GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました

#### <a name="aznetwork"></a>Az.Network
* Nat Gateway Resource に対するサポートを追加しました
    - 新しいコマンドレット
        - New-AzNatGateway
        - Get-AzNatGateway
        - Set-AzNatGateway
        - Remove-AzNatGateway
   - 更新されたコマンドレット
        - New-AzureVirtualNetworkSubnetConfigCommand
        - Add-AzureVirtualNetworkSubnetConfigCommand
* 次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。
    - New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。
    - Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* ポリシーの評価の詳細をクエリするためのサポート。
    - Get-AzPolicyState に '-Expand' パラメーターを追加しました。 '-Expand PolicyEvaluationDetails' がサポートされます。

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Azure から Azure へのクロス サブスクリプション サイト回復のサポート。
* Azure Site Recovery に対する今後の重要な変更へのマーク付け。
* Azure Site Recovery 復旧計画のアクション終了計画の修正。
* Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。
* マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。
* その他の軽微な修正。

#### <a name="azrelay"></a>Az.Relay
* 顧客向けメッセージの入力ミスを修正しました

#### <a name="azservicebus"></a>Az.ServiceBus
* 名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました

#### <a name="azstorage"></a>Az.Storage
* ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)
* 新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。
* ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました
    - New-AzStorageAccount
* "-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)
    - New-AzStorageAccount
    - Get-AzStorageAccount
    - Set-AzStorageAccount

#### <a name="azwebsites"></a>Az.Websites
* Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります
* Get-AzWebApp*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました

## <a name="180---april-2019"></a>1.8.0 - 2019 年 4 月
### <a name="highlights-since-the-last-major-release"></a>前回のメジャー リリース以降のハイライト
* `Az` モジュールの一般提供
* `Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce
* Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/
* Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加
* Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加
* Az.Automation の Python 2 Runbook のサポートを追加
* Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット

#### <a name="azaccounts"></a>Az.Accounts
* Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新

#### <a name="azbatch"></a>Az.Batch
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azcdn"></a>Az.Cdn
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azcompute"></a>Az.Compute
* ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。
* ワイルドカードのドキュメントを修正

#### <a name="azdatafactory"></a>Az.DataFactory
* マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azeventgrid"></a>Az.EventGrid
* 作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。

#### <a name="azeventhub"></a>Az.EventHub
* 名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました 

#### <a name="azhdinsight"></a>Az.HDInsight
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="aziothub"></a>Az.IotHub
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azkeyvault"></a>Az.KeyVault
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。
* ワイルドカードのドキュメントを修正

#### <a name="azmachinelearning"></a>Az.MachineLearning
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azmedia"></a>Az.Media
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azmonitor"></a>Az.Monitor
  * GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット
      - New-AzMetricAlertRuleV2DimensionSelection
      - New-AzMetricAlertRuleV2Criteria
      - Remove-AzMetricAlertRuleV2
      - Get-AzMetricAlertRuleV2
      - Add-AzMetricAlertRuleV2
  * Monitor SDK をバージョン 0.22.0-preview に更新しました

#### <a name="aznetwork"></a>Az.Network
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。
* ワイルドカードのドキュメントを修正

#### <a name="aznotificationhubs"></a>Az.NotificationHubs
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azpowerbiembedded"></a>Az.PowerBIEmbedded
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。
* Azure VM で SQL のテーブル形式を更新しました
* AzureFileShare で場所をフェッチするよう代替の方法を追加しました
* タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました

#### <a name="azrediscache"></a>Az.RedisCache
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。

#### <a name="azresources"></a>Az.Resources
* ワイルドカードのドキュメントを修正

#### <a name="azsql"></a>Az.Sql
* Monitor SDK の依存関係が一般的なコードに置き換えられます
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。
* 複数列の分類のプロセスを強化しました。
* Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。
* リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。
* Managed Instance 作成でのタイム ゾーン パラメーターのサポート。
* ワイルドカードのドキュメントを修正

#### <a name="azwebsites"></a>Az.Websites
* 実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正
* コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。
* WebSites SDK を更新しました。
* PSAppServicePlan から AdminSiteName プロパティを削除しました。

## <a name="170---april-2019"></a>1.7.0 - 2019 年 4 月
### <a name="highlights-since-the-last-major-release"></a>前回のメジャー リリース以降のハイライト
* `Az` モジュールの一般提供
* `Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce
* Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/
* Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加
* Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加
* Az.Automation の Python 2 Runbook のサポートを追加
* Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット

#### <a name="azaccounts"></a>Az.Accounts
* AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました

#### <a name="azanalysisservices"></a>Az.AnalysisServices
* データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除
* Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました

#### <a name="azautomation"></a>Az.Automation
* New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。 IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。
* Azure Automation Update Management の動的グループのバグを修正しました

#### <a name="azcompute"></a>Az.Compute
* HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました
* 他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。 

#### <a name="azcontainerinstance"></a>Az.ContainerInstance
* 末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 3.0.2 に更新しました
* Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。

#### <a name="azresources"></a>Az.Resources
* "-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました
* "Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました
    - デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856
* スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856

#### <a name="azsql"></a>Az.Sql
* データベースのデータ分類をサポートしました。

#### <a name="azstorage"></a>Az.Storage
* -UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます
    - New-AzStorageContext
* 管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました
    - Update-AzStorageBlobServiceProperty
    - Get-AzStorageBlobServiceProperty
    - Enable-AzStorageBlobDeleteRetentionPolicy
    - Disable-AzStorageBlobDeleteRetentionPolicy
* -AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました
    - Get-AzStorageBlobContent
    - Set-AzStorageBlobContent
    - Get-AzStorageFileContent
    - Set-AzStorageFileContent

## <a name="160---march-2019"></a>1.6.0 - 2019 年 3 月
### <a name="highlights-since-the-last-major-release"></a>前回のメジャー リリース以降のハイライト
* `Az` モジュールの一般提供
* `Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce
* Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/
* Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加
* Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加
* Az.Automation の Python 2 Runbook のサポートを追加
* Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット

#### <a name="azautomation"></a>Az.Automation
* Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。
    * 動的なグループ化
    * プリ/ポスト スクリプト
    * 再起動設定

#### <a name="azcompute"></a>Az.Compute
* Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました
* Compute クライアント ライブラリを 25.0.0 に更新しました

#### <a name="azkeyvault"></a>Az.KeyVault
* KeyVault コマンドレットにワイルドカードのサポートを追加しました

#### <a name="aznetwork"></a>Az.Network
* Azure Firewall 用の脅威インテリジェンスのサポートを追加しました
* Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました
* コンテナーの登録解除用にパイプ サポートを追加しました

#### <a name="azresources"></a>Az.Resources
* Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新
* ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新

#### <a name="azsql"></a>Az.Sql
* 新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。

#### <a name="azstorage"></a>Az.Storage
* ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート
    - Set-AzStorageAccountManagementPolicy
    - Get-AzStorageAccountManagementPolicy
    - Remove-AzStorageAccountManagementPolicy
    - Add-AzStorageAccountManagementPolicyAction
    - New-AzStorageAccountManagementPolicyFilter
    - New-AzStorageAccountManagementPolicyRule

#### <a name="azwebsites"></a>Az.Websites
* 'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正 

## <a name="150---march-2019"></a>1.5.0 - 2019 年 3 月
#### <a name="azaccounts"></a>Az.Accounts
* AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました
* Connect-AzAccount の例を更新しました

#### <a name="azautomation"></a>Az.Automation
* 複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました
* Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。 現在はすべてのノードが返されるようになりました

#### <a name="azcdn"></a>Az.Cdn
* カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました

#### <a name="azcompute"></a>Az.Compute
* Get コマンドレットにワイルドカードのサポートを追加しました

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 3.0.1 に更新しました

#### <a name="azlogicapp"></a>Az.LogicApp
* ListWorkflows で結果の最初のページのみが取得される問題を修正しました

#### <a name="aznetwork"></a>Az.Network
* Network コマンドレットにワイルドカードのサポートを追加しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Azure VM での SQL Server のサポートを追加しました
* SDK の更新
* Get-ProtectableItem で VMappContainer チェックを削除しました
* Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました

#### <a name="azresources"></a>Az.Resources
* デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933
* `Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240
* `Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930

#### <a name="azsql"></a>Az.Sql
* AuditingEndpointsCommunicator を更新しました。
    - 新しい診断設定を作成する際のエッジ ケースの動作を修正しました。

#### <a name="azstorage"></a>Az.Storage
* New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました

## <a name="140---february-2019"></a>1.4.0 - 2019 年 2 月
#### <a name="azanalysisservices"></a>Az.AnalysisServices
* AddAzureASAccount コマンドレットを非推奨にしました

#### <a name="azautomation"></a>Az.Automation
* Import-AzAutomationDscNodeConfiguration のヘルプを更新しました
* Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました
* Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。

#### <a name="azcompute"></a>Az.Compute
* ID パラメーター セットに関する問題を修正しました
* Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました
* Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました
* Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* ADL で削除された項目を列挙して復元するコマンドレットを追加しました

#### <a name="azeventhub"></a>Az.EventHub
* EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました 

#### <a name="azkeyvault"></a>Az.KeyVault
* Set-AzKeyVaultSecret のタグ付けを修正しました

#### <a name="azlogicapp"></a>Az.LogicApp
* 統合アカウントに Basic SKU を追加しました
* XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました
* 統合アカウント アセンブリ用の新しいコマンドレット
    - Get-AzIntegrationAccountAssembly
    - New-AzIntegrationAccountAssembly
    - Remove-AzIntegrationAccountAssembly
    - Set-AzIntegrationAccountAssembly
* 統合アカウント バッチ構成用の新しいコマンドレット
    - Get-AzIntegrationAccountBatchConfiguration
    - New-AzIntegrationAccountBatchConfiguration
    - Remove-AzIntegrationAccountBatchConfiguration
    - Set-AzIntegrationAccountBatchConfiguration
* Logic Apps SDK をバージョン 4.1.0 に更新しました

#### <a name="azmonitor"></a>Az.Monitor
* Get-AzMetric のヘルプを更新しました

#### <a name="aznetwork"></a>Az.Network
* Add-AzApplicationGatewayCustomError のヘルプの例を更新しました

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。
    - 指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。 
    - ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。 

#### <a name="azresources"></a>Az.Resources
* 次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166
* 次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235
* 次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219
* KeyCredentials の繰り返し作成を妨げるバグを修正しました

#### <a name="azsql"></a>Az.Sql
* SQL DB のハイパースケール レベルのサポートを追加しました
* 復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました

#### <a name="azwebsites"></a>Az.Websites
* Get-AzWebAppSlotMetrics の例を修正しました

## <a name="130---february-2019"></a>1.3.0 - 2019 年 2 月
#### <a name="azaccounts"></a>Az.Accounts
* ClientRuntime を最新バージョンに更新

#### <a name="azanalysisservices"></a>Az.AnalysisServices
Az.AnalysisServices モジュールを一般公開

#### <a name="azcompute"></a>Az.Compute
* AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加
* Set-AzVMBootDiagnostics のヘルプの説明を更新
* Update-AzImage のヘルプの説明と例を更新

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
Az.RecoveryServices モジュールを一般公開

#### <a name="azresources"></a>Az.Resources
* リソース グループのタグ付けを修正 
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166
* `Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正 
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235

#### <a name="azsql"></a>Az.Sql
* Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加
* SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正
* Get-AzSqlCapability の null ref 例外を修正

## <a name="121---january-2019"></a>1.2.1 - 2019 年 1 月
#### <a name="azaccounts"></a>Az.Accounts
* 正しいバージョンの認証によるリリース

#### <a name="azanalysisservices"></a>Az.AnalysisServices
* 認証の依存関係の更新によるリリース

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* 認証の依存関係の更新によるリリース

## <a name="120---january-2019"></a>1.2.0 - 2019 年 1 月
#### <a name="azaccounts"></a>Az.Accounts
* Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加
* 誤ったオンライン ヘルプの URL を更新
* Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加

#### <a name="azaks"></a>Az.Aks
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azautomation"></a>Az.Automation
* Python 2 Runbook のサポートを追加
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azcdn"></a>Az.Cdn
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azcompute"></a>Az.Compute
* Invoke-AzVMReimage コマンドレットを追加
* TempDisk パラメーターを Set-AzVmss に追加
* New-AzVM の警告メッセージを修正

#### <a name="azcontainerregistry"></a>Az.ContainerRegistry
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 3.0.0 に更新

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* MSI を使用するときの ADLS エンドポイントの問題を解決
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462
* 誤ったオンライン ヘルプの URL を更新

#### <a name="aziothub"></a>Az.IotHub
* エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加

#### <a name="azkeyvault"></a>Az.KeyVault
* 誤ったオンライン ヘルプの URL を更新

#### <a name="aznetwork"></a>Az.Network
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azresources"></a>Az.Resources
* 'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正
* リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正
* Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正
* Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522
* Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747
* 'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932
* 一部のエラー メッセージを修正
* Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正
* 拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正

#### <a name="azsignalr"></a>Az.SignalR
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azsql"></a>Az.Sql
* 誤ったオンライン ヘルプの URL を更新
* LicenseType パラメーターの説明の使用可能な値を更新
* 更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正
* マネージド インスタンスでカスタム照合順序をサポート

#### <a name="azstorage"></a>Az.Storage
* 誤ったオンライン ヘルプの URL を更新
* Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与
    - Get/Set-AzStorageServiceLoggingProperty
    - Get/Set-AzStorageServiceMetricsProperty

#### <a name="aztrafficmanager"></a>Az.TrafficManager
* 誤ったオンライン ヘルプの URL を更新

#### <a name="azwebsites"></a>Az.Websites
* 誤ったオンライン ヘルプの URL を更新
* アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正
* SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正

## <a name="110---january-2019"></a>1.1.0 - 2019 年 1 月
#### <a name="azaccounts"></a>Az.Accounts
* "ローカル" スコープを Enable-AzureRmAlias に追加

#### <a name="azcompute"></a>Az.Compute
* 名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。
* ヘルプ ファイル内の ID の説明が更新されました
* Az.Accounts モジュールの下位互換性の問題を修正しました

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。
    - getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました

#### <a name="azeventgrid"></a>Az.EventGrid
* 2019-01-01 API バージョンを使用するように更新しました。
* 2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新
    - New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:
        - イベントの Time-To-Live
        - イベントの配信試行の最大数
        - 配信不能エンドポイント
    - Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:
        - イベントの Time-To-Live
        - イベントの配信試行の最大数
        - 配信不能エンドポイント
* New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。
* イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。

#### <a name="aziothub"></a>Az.IotHub
* IotHub SDK の最新バージョンに更新しました

#### <a name="azlogicapp"></a>Az.LogicApp
* Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます

#### <a name="azresources"></a>Az.Resources
* 'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875
* New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました
* New-AzDeployment ドキュメントのタイポを修正しました
* 'New-AzADUser' に '-MailNickname' パラメーターが必須となりました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220

#### <a name="azsignalr"></a>Az.SignalR
* Az.Accounts モジュールの下位互換性の問題を修正しました

#### <a name="azsql"></a>Az.Sql
* ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。

#### <a name="azstorage"></a>Az.Storage
* ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します
    - New-AzStorageContext
* '-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました
    - New-AzStorageBlobSASToken

#### <a name="azwebsites"></a>Az.Websites
* 'Get-AzDeletedWebApp' のバグ解析日を修正しました
* Az.Accounts モジュールの下位互換性の問題を修正しました

## <a name="100---december-2018"></a>1.0.0 - 2018 年 12 月
### <a name="general"></a>全般

- Az モジュールの一般公開
- 各モジュールのオンライン ヘルプ
- 詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください
- AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azaccounts"></a>Az.Accounts
- Az.Profile から変更しました
- プロファイルの表形式とコンテキストの種類を修正しました

### <a name="azapimanagement"></a>Az.ApiManagement
- #7002 の修正プログラム
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azbatch"></a>Az.Batch
- Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。
- `PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azbilling"></a>Az.Billing
- 課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azcognitivservices"></a>Az.CognitivServices
- New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました
- Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました

### <a name="azcontainerinstance"></a>Az.ContainerInstance
- ManagedIdentity サポートを追加しました

### <a name="azdatalakeanalytics"></a>Az.DataLakeAnalytics
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azdatalakestore"></a>Az.DataLakeStore
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azmonitor"></a>Az.Monitor
- Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azkeyvault"></a>Az.KeyVault
- 出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました

### <a name="azmachinelearning"></a>Az.MachineLearning
- Az.MachineLearningCompute モジュールのコマンドレットを組み込みました

### <a name="azmedia"></a>Az.Media
- 非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました

### <a name="aznetwork"></a>Az.Network
Application Gateway での RewriteRuleSets の構成のサポートを追加しました
    - 追加された新しいコマンドレットは次のとおりです
        - Add-AzureRmApplicationGatewayRewriteRuleSet
        - Get-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRuleSet
        - Remove-AzureRmApplicationGatewayRewriteRuleSet
        - Set-AzureRmApplicationGatewayRewriteRuleSet
        - New-AzureRmApplicationGatewayRewriteRule
        - New-AzureRmApplicationGatewayRewriteRuleActionSet
        - New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration
    - 省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット
        - New-AzureRmApplicationGateway
        - New-AzureRmApplicationGatewayRequestRoutingRule
        - Add-AzureRmApplicationGatewayRequestRoutingRule
        - New-AzureRmApplicationGatewayPathRuleConfig
        - Add-AzureRmApplicationGatewayUrlPathMapConfig
        - New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。
    - 省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット
        - Add-AzApplicationGatewaySslCertificate
        - New-AzApplicationGatewaySslCertificate
        - Set-AzApplicationGatewaySslCertificate
    - 省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azoperationalinsights"></a>Az.OperationalInsights
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azprofile"></a>Az.Profile
- モジュール名を Az.Accounts に変更しました

### <a name="azrecoveryservices"></a>Az.RecoveryServices
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azresources"></a>Az.Resources
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azservicefabric"></a>Az.ServiceFabric
- 共通名および拇印別での証明書の指定をサポートします
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azsignalr"></a>Az.SIgnalR
- SIgnalR 用の PowerShell コマンドレットの一般公開

### <a name="azsql"></a>Az.Sql
- 新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました
- SQL 監査コマンドレットのドキュメントの例を更新しました
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azstorage"></a>Az.Storage
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

### <a name="azwebsites"></a>Az.Websites
- 小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください

## <a name="070---december-2018"></a>0.7.0 - 2018 年 12 月

### <a name="general"></a>全般

* AzureRM から Az に切り替えるための軽微な変更

### <a name="azcompute"></a>Az.Compute

* `New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。

### <a name="azdatalakestore"></a>Az.DataLakeStore

* ADLS アカウントのドメインの末尾のスラッシュを修正しました

### <a name="azfrontdoor"></a>Az.FrontDoor

* 壊れたリンクを修正しました
    - New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。
    - New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。

### <a name="azrecoveryservices"></a>Az.RecoveryServices

* Azure ファイル共有の復元操作にクライアント側の検証を追加しました。
* AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。

### <a name="azresources"></a>Az.Resources

* https://github.com/Azure/azure-powershell/issues/7679 を修正しました
    - 従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。

### <a name="azsql"></a>Az.Sql

* AzureRM から Az に切り替えるための軽微な変更
* .Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました
* SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました

### <a name="azstorage"></a>Az.Storage

* New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました
* -DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました
    - Start-AzureStorageFileCopy
* 静的な Web サイトの構成のサポート
    - Enable-AzureStorageStaticWebsite
    - Disable-AzureStorageStaticWebsite

### <a name="azwebsites"></a>Az.Websites

* Set-AzureRmWebApp と Set-AzureRmWebAppSlot 
    - Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します

## <a name="061---november-2018"></a>0.6.1 - 2018 年 11 月

### <a name="azapimanagement"></a>Az.ApiManagement
* 型マッピングの問題に対応するために依存関係を更新しました

### <a name="azautomation"></a>Az.Automation
* Swagger ベースの Azure Automation コマンドレット
* Update Management コマンドレットを追加しました
* ソース管理コマンドレットを追加しました
* Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました
* DSC Register Node コマンドを修正しました

### <a name="azcompute"></a>Az.Compute
* SystemAssigned ID の ID の問題を修正しました
* 型マッピングの問題に対応するために依存関係を更新しました

### <a name="azcontainerinstance"></a>Az.ContainerInstance
* 型マッピングの問題に対応するために依存関係を更新しました

### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* marketplace コマンドレットの例の説明を更新しました

### <a name="aznetwork"></a>Az.Network
* New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました
* サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました
* Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました 
* VirtualNetwork マップのメモリ使用量に関する問題を修正しました

### <a name="azrecoveryservicesbackup"></a>Az.RecoveryServices.Backup
* 保護されたファイル共有のポリシーの変更を修正しました
* ポリシーのタイムゾーンを大文字に変換しました

### <a name="azrecoveryservicessiterecovery"></a>Az.RecoveryServices.SiteRecovery
* New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました
* 型マッピングの問題に対応するために依存関係を更新しました

### <a name="azrelay"></a>Az.Relay
* New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります

### <a name="azresources"></a>Az.Resources
* `New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました
* -Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました
* NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703

### <a name="azservicefabric"></a>Az.ServiceFabric
* 今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました

### <a name="azsql"></a>Az.Sql
* Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました
    - Get-AzureRmSqlInstance
    - New-AzureRmSqlInstance
    - Set-AzureRmSqlInstance
    - Remove-AzureRmSqlInstance
    - Get-AzureRmSqlInstanceDatabase
    - New-AzureRmSqlInstanceDatabase
    - Restore-AzureRmSqlInstanceDatabase
    - Remove-AzureRmSqlInstanceDatabase
* サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました
    - 監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました
    - レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました
    - Set-AzureRmSqlServerAuditing
    - Get-AzureRmSqlServerAuditing
    - Set-AzureRmSqlDatabaseAuditing
    - Get-AzureRmSqlDatabaseAuditing
* ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました

## <a name="050---november-2018"></a>0.5.0 - 2018 年 11 月
#### <a name="general"></a>全般
* リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります

#### <a name="azprofile"></a>Az.Profile
* 最新バージョンの ClientRuntime を使用するように共通コードを更新しました。
* Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました
* Connect-AzAccount の TenantId の説明を更新しました
* テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました
    - https://github.com/Azure/azure-powershell/issues/6936
* テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/7453
* MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/7462
* 接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* Get-AzCognitiveServicesAccountSkus 操作を追加しました

#### <a name="azcompute"></a>Az.Compute
* Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました
* Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます
* SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* DataLake パッケージは 1.1.10 に更新されました。
* マルチスレッド操作に既定のコンカレンシーを追加しました。

#### <a name="azinsights"></a>Az.Insights
* 問題 #7267 (自動スケーリングの領域) を修正しました
    - 新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。
* Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました
    - このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します

#### <a name="aznetwork"></a>Az.Network
* 次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:
    - Get-AzExpressRouteCircuitRouteTable
    - Get-AzExpressRouteCircuitARPTable
    - Get-AzExpressRouteCircuitRouteTableSummary
    - Get-AzExpressRouteCrossConnectionArpTable
    - Get-AzExpressRouteCrossConnectionRouteTable
    - Get-AzExpressRouteCrossConnectionRouteTableSummary

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* ポリシー修復コマンドレットを追加しました

#### <a name="azresources"></a>Az.Resources
* https://github.com/Azure/azure-powershell/issues/7402 を修正しました
    - "Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。

#### <a name="azservicebus"></a>Az.ServiceBus
* 移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Linux VMSS への証明書の追加を修正しました。
* "Add-AzServiceFabricClusterCertificate" を修正しました
    - 新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。
    - 例外が正しく表示されます (Azure/service-fabric-issues#1054)。
* VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。

## <a name="040---october-2018"></a>0.4.0 - 2018 年 10 月
#### <a name="azprofile"></a>Az.Profile
* CloudShell での Get-AzSubscription に関する問題を修正しました。
* 最新バージョンの ClientRuntime を使用するように共通コードを更新しました。

#### <a name="azcompute"></a>Az.Compute
* "New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。
* ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* 仮想ネットワーク規則のサポートを追加しました
    - Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。
    - Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。
    - Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。
    - Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。

#### <a name="aznetwork"></a>Az.Network
* プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。
* ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。

#### <a name="azresources"></a>Az.Resources
* シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。 また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。

## <a name="030---october-2018"></a>0.3.0 - 2018 年 10 月
#### <a name="azurestorage"></a>Azure.Storage
* コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy
* 特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。
    - Get-AzStorageUsage
    
#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* 既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。

#### <a name="azcompute"></a>Az.Compute
* 必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました
* "SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。
* Azure Disk Encryption の進行状況メッセージの誤りを修正しました

#### <a name="azdatafactoryv2"></a>Az.DataFactoryV2
* ADF .Net SDK のバージョンを 2.3.0 に更新しました。

#### <a name="aznetwork"></a>Az.Network
* NetworkProfile 機能を追加しました。 追加された新しいコマンドレットは次のとおりです
    - Get-AzNetworkProfile
    - New-AzNetworkProfile
    - Remove-AzNetworkProfile
    - Set-AzNetworkProfile
    - New-AzContainerNicConfig
    - New-AzContainerNicConfigIpConfig
* サブネット モデルでサービスの関連付けリンクを追加しました
* New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました
* Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました

#### <a name="azrediscache"></a>Az.RedisCache
* 今後、サイズ パラメーターとして任意の文字列を追加できます。 PSArgumentCompleter ポップアップで P5 を追加しました

#### <a name="azresources"></a>Az.Resources
* 欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました
* 配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました

#### <a name="azsql"></a>Az.Sql
* 一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました

#### <a name="azwebsites"></a>Az.Websites
* 新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します
* 新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します

## <a name="020---september-2018"></a>0.2.0 - 2018 年 9 月
 最初のリリース