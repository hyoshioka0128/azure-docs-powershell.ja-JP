Azure PowerShell 4.3.1 インストーラー: [リンク](https://github.com/Azure/azure-powershell/releases/download/v4.3.1-August2017/azure-powershell.4.3.1.msi)

ARM コマンドレット用のギャラリー モジュール: [リンク](https://www.powershellgallery.com/packages/AzureRM/4.3.1)

Service Management (RDFE) のレガシ コマンドレット用のギャラリー モジュール: [リンク](https://www.powershellgallery.com/packages/Azure/4.3.1)

## <a name="changes-in-431"></a>4.3.1 の変更点

- 特定のアセンブリが署名されていないことで、モジュールのインポート時に `could not load file or assembly` エラーが発生する問題を修正しました。

## <a name="changes-in-430"></a>4.3.0 の変更点

* AnalysisServices
    * Set-AzureRmAnalysisServciesServer のバグを修正
        - 管理者が指定されなかった場合、管理者は削除されます。
    * New-AzureRmAnalysisServicesServer と Set-AzureRmAnalysisServicesServer で BackupBlobContainerUri を追加
        - Azure Analysis Services サーバーのバックアップ/復元のためのバックアップ BLOB コンテナーの設定/無効化が可能になります。
    * New-AzureRmAnalysisServicesServer と Set-AzureRmAnalysisServicesServer で SKU ルックアップを更新
        - ハードコードされた SKU を動的ルックアップに変更しました。
    * Add-AzureAnalysisServicesAccount でサービス プリンシパルを使ったログインをサポート
* Automation
    * 100 を超えるレコードを取得するよう AutomationDSC* コマンドレットを変更
    * いくつかの Automation コマンドレット (Get-AzureRmAutomationVariable、Get-AzureRmAutomationJob など) を呼び出した後に詳細ストリームが動作しなくなる問題を解決しました。
    * StartAzureAutomationDscCompilationJob と ImportAzureAutomationDscNodeConfiguration に NodeConfiguration Build のバージョン管理のサポートを追加しました。
    * 既存の問題のバグ修正 - エイリアスの問題 #3775 について、runOn エイリアスと HybridWorkers のサポートを修正。
* コンピューティング
    * Set-AzureRmVMAEMExtension: 新しい Premium ディスク サイズのサポートを追加
    * Set-AzureRmVMAEMExtension: M シリーズのサポートを追加
    * Add-AzureRmVmssExtension に ForceUpdateTag パラメーターを追加
    * New-AzureRmVmssIpConfig に Primary パラメーターを追加
    * Add-AzureRmVmssNetworkInterfaceConfig に EnableAcceleratedNetworking パラメーターを追加
    * Set-AzureRmVmss に InstanceId を追加
    * Get-AzureRmVM -Status 出力に MaintenanceRedeployStatus を公開
    * Get-AzureRmComputeResourceSku の表形式に制限と機能を公開
* DataLakeStore
    * 次の問題を修正: https://github.com/Azure/azure-powershell/issues/4323
* EventHub
    * NamespaceAttributes に ResourceGroup プロパティを追加
        - 'ResourceGroup' は、名前空間があるリソース グループの名前を取得
    * 新しいパラメーターとパラメーター エイリアスでコマンドレットを更新
        - AuthorizationRule の操作を行うための Namespace と EventHub のパラメーター セットでコマンドレットを更新しました。
        - New-AzureRmEventHubAuthorizationRule
            + 既存の NameSpace または EventHub に新しい AuthorizationRule を追加します。
        - Get-AzureRmEventHubAuthorizationRule
            + 既存の NameSpace または EventHub の AuthorizationRule または AuthorizationRule のリストを取得します。
        - Set-AzureRmEventHubAuthorizationRule
            + EventHub NameSpace の既存の AuthorizationRule のプロパティを更新します。
        - Remove-AzureRmEventHubAuthorizationRule
            + 既存の NameSpace または EventHub の既存の AuthorizationRule を削除します。
        - New-AzureRmEventHubKey
            + 既存の NameSpace または EventHub の AuthorizationRule の新しいプライマリ/セカンダリ キーを生成します。
        - Get-AzureRmEventHubKey
            + 既存の NameSpace または EventHub の AuthorizationRule のプライマリ/セカンダリ キーを取得します。
* ネットワーク
    * New-AzureRmExpressRouteCircuitPeeringConfig: IPv6 サポートを追加しました。 新しい省略可能なパラメーターを追加しました。
        - PeerAddressType
    * Set-AzureRmExpressRouteCircuitPeeringConfig: IPv6 サポートを追加しました。 新しい省略可能なパラメーターを追加しました。
        - PeerAddressType
    * Remove-AzureRmExpressRouteCircuitPeeringConfig: IPv6 サポートを追加しました。 新しい省略可能なパラメーターを追加しました。
        - PeerAddressType
    * パラメーター -ProbeEnabled を非推奨としてマークしました。
        - Add-AzureRmApplicationGatewayBackendHttpSettings
        - New-AzureRmApplicationGatewayBackendHttpSettings
        - Set-AzureRmApplicationGatewayBackendHttpSettings
* プロファイル
    * データの収集は既定で有効になっています。 ユーザー エクスペリエンス向上のため、マイクロソフトによって利用状況データが収集されます。 データは匿名として扱われ、コマンド ライン引数の値は含まれません。
        - この機能を無効にするには、Disable-AzureRmDataCollection コマンドレットを使用します。
        - この機能を有効にするには、Enable-AzureRmDataCollection コマンドレットを使用します。
* リソース
    * ARM に要求を送信する前に、次の roledefinition コマンドレットと roleassignment コマンドレットに対するスコープの検証サポートを追加
        - Get-AzureRMRoleAssignment
        - New-AzureRMRoleAssignment
        - Remove-AzureRMRoleAssignment
        - Get-AzureRMRoleDefinition
        - New-AzureRMRoleDefinition
        - Remove-AzureRMRoleDefinition
        - Set-AzureRMRoleDefinition
* ServiceBus
    * NameSpace、Queue、Topic の AuthorizationRules の新しいコマンドレットを追加しました。 パラメーター セットに基づいて、承認規則の操作が実行されます。
     - New-AzureRmServiceBusAuthorizationRule
       - 既存の ServiceBus NameSpace/Queue/Topic に新しい AuthorizationRule を追加します。
     - Get-AzureRmServiceBusAuthorizationRule
       - 既存の ServiceBus NameSpace/Queue/Topic の AuthorizationRule または AuthorizationRules のリストを取得します。
     - Set-AzureRmServiceBusAuthorizationRule
       - ServiceBus NameSpace/Queue/Topic の既存の AuthorizationRule のプロパティを更新します。
     - New-AzureRmServiceBusKey
       - 既存の ServiceBus NameSpace/Queue/Topic の AuthorizationRule の新しいプライマリ/セカンダリ キーを生成します。
     - Get-AzureRmServiceBusKey
       - 既存の ServiceBus NameSpace/Queue/Topic の AuthorizationRule のプライマリ/セカンダリ キーを取得します。
     - Remove-AzureRmServiceBusNamespaceAuthorizationRule
       - ServiceBus NameSpace/Queue/Topic の既存の AuthorizationRule を削除します。
    * NamespceAttributes にリソース グループのプロパティを追加しました。
* SQL
    * 暗号化の保護の種類が AzureKeyVault に設定されている場合に警告を表示して確認を要求するよう、Set-AzureRmSqlServerTransparentDataEncryptionProtector を更新
    * 監査設定に対する新しい更新コマンドレットを追加
        - Azure SQL データベースの監査設定を取得する Get-AzureRmSqlDatabaseAuditing コマンドレットを追加
        - Azure SQL サーバーの監査設定を取得する Get-AzureRmSqlServerAuditing コマンドレットを追加
        - Azure SQL データベースの監査設定を変更する Set-AzureRmSqlDatabaseAuditing コマンドレットを追加
        - Azure SQL サーバーの監査設定を変更する Set-AzureRmSqlServerAuditing コマンドレットを追加
    * 既存の監査ポリシー コマンドレットを非推奨化
        - Get-AzureRmSqlDatabaseAuditingPolicy を非推奨化
        - Get-AzureRmSqlServerAuditingPolicy を非推奨化
        - Set-AzureRmSqlDatabaseAuditingPolicy を非推奨化
        - Set-AzureRmSqlServerAuditingPolicy を非推奨化
        - Use-AzureRmSqlServerAuditingPolicy を非推奨化
        - Remove-AzureRmSqlDatabaseAuditing を非推奨化
        - Remove-AzureRmSqlServerAuditing を非推奨化
    * Update-AzureRmSqlSyncGroup のスキーマ ファイルの解析で大文字と小文字が区別されなくなりました。
* Storage
    * リソース モード ストレージ アカウント コマンドレットに NeworkRule のサポートを追加
        - New-AzureRmStorageAccount
        - Set-AzureRmStorageAccount
        - Get-AzureRmStorageAccountNetworkRuleSet
        - Update-AzureRmStorageAccountNetworkRuleSet
        - Add-AzureRmStorageAccountNetworkRule
        - Remove-AzureRmStorageAccountNetworkRule

[前回のリリース以降の変更点](https://github.com/Azure/azure-powershell/compare/v4.2.1-July2017...v4.3.1-August2017)を見る
