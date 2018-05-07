---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 2/20/2018
ms.openlocfilehash: 2e80d314991539cb630a0f2a96048bb2e70a05b6
ms.sourcegitcommit: 5f0013981fcea1d689649b9a2b2ffe84ae842e56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2018
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

---

# <a name="azure-powershell-570"></a>Azure PowerShell 5.7.0

Azure PowerShell 5.7.0 インストーラー: [リンク](https://github.com/Azure/azure-powershell/releases/download/v5.7.0-April2018/azure-powershell.5.7.0.msi)

ARM コマンドレット用のギャラリー モジュール: [リンク](https://www.powershellgallery.com/packages/AzureRM/5.7.0)

PowerShell ギャラリーから `AzureRM` をインストールするには、次のコマンドを実行します。

```powershell
Install-Module -Name AzureRM -Repository PSGallery -Force
```

以前のバージョンの `AzureRM` から更新するには、次のコマンドを実行します。

```powershell
Update-Module -Name AzureRM
```

## <a name="changes-since-last-release"></a>前回のリリース以降の変更点

#### <a name="general"></a>全般
* Azure ClientRuntime の最新バージョンに更新しました

#### <a name="azurestorage"></a>Azure.Storage
* FIPS ポリシーが有効になっているコンピューターで BLOB のアップロード コマンドレットとファイルのアップロード コマンドレットが失敗するという問題を修正
    - Set-AzureStorageBlobContent
    - Set-AzureStorageFileContent

#### <a name="azurermbilling"></a>AzureRM.Billing
* 新しいコマンドレット Get-AzureRmEnrollmentAccount
  - 登録アカウントを取得するためのコマンドレット

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Cognitive Services Management SDK バージョン 4.0.0 との統合。
* Get-AzureRmCognitiveServicesAccountUsage 操作の追加。

#### <a name="azurermcompute"></a>AzureRM.Compute
* `Get-AzureRmVmssDiskEncryptionStatus` によるデータ ディスク レベルでの暗号化状態のサポート
* `Get-AzureRmVmssVmDiskEncryptionStatus` によるデータ ディスク レベルでの暗号化状態のサポート
* ゾーン回復性の更新
* "New-AzureRmVm" および "New-AzureRmVmss" (シンプルなパラメーター セット) による可用性ゾーンのサポート。

#### <a name="azurermcontainerregistry"></a>AzureRM.ContainerRegistry
* Commands.Resources.Rest および ARM/Storage SDK への依存の分離。

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* デバッグ機能の追加
* ADLS データプレーン SDK のバージョンを 1.1.2 に更新
* Export-AzureRmDataLakeStoreItem - パラメーター PerFileThreadCount、ConcurrentFileCount が非推奨になり、パラメーター Concurrency が導入されました
* Import-AzureRMDataLakeStoreItem - パラメーター PerFileThreadCount、ConcurrentFileCount が非推奨になり、パラメーター Concurrency が導入されました
* Get-AzureRMDataLakeStoreItemContent - 4 MB を超えるコンテンツのテール動作を修正しました
* Set-AzureRMDataLakeStoreItemExpiry - 相対的な有効期限を設定するための新しいパラメーター セット SetRelativeExpiry を導入しました
* Remove-AzureRmDataLakeStoreItem - パラメーター Clean が非推奨になりました。

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* New-AzureRmEventHubGeoDRConfiguration の AlternameName を修正しました

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* コマンドレットを更新して、パイプ処理シナリオを追加しました
* 今後の重大な変更リリースを対象とした非推奨メッセージの追加

#### <a name="azurermnetwork"></a>AzureRM.Network
* Network コマンドレットでのエラー メッセージの修正

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* customproperties をサポートするように Rules の CorrelationFilter に "properties" を追加しました
* New-AzureRmServiceBusGeoDRConfiguration ヘルプを更新し、Rules コマンドレットの出力を修正しました
* New-AzureRmServiceBusQueue および New-AzureRmServiceBusSubscription コマンドレットの auto-forward プロパティを修正しました

#### <a name="azurermsql"></a>AzureRM.Sql
* エラスティック プールで非同期操作のキャンセルをサポートする新しいコマンドレット "Stop-AzureRmSqlElasticPoolActivity" の追加
* コマンドレット Get-AzureRmSqlDatabaseActivity および Get-AzureRmSqlElasticPoolActivity の応答を詳細情報が反映されるように更新

前回のリリース以降の変更点: https://github.com/Azure/azure-powershell/compare/v5.6.0-March2018...v5.7.0-April2018

## <a name="560---march-2018"></a>5.6.0 - 2018 年 3 月

#### <a name="general"></a>全般
* Cloud Shell の既定のリソース グループに関する問題を修正しました
* モジュールのインポート中に不適切なスタートアップ スクリプトが実行される問題を修正しました

#### <a name="azurermprofile"></a>AzureRM.Profile
* サポートされていないシナリオで MSI 認証を有効にしました
* ユーザー定義の管理対象サービス ID に対応するようになりました

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* ビルドにおけるスクリプトのクリーンアップに関する問題を修正しました

#### <a name="azurermcdn"></a>AzureRM.Cdn
* ビルドにおけるスクリプトのクリーンアップに関する問題を修正しました

#### <a name="azurermcompute"></a>AzureRM.Compute
* 'New-AzureRmVM' と 'New-AzureRmVMSS' は、データ ディスクをサポートします。
* 'New-AzureRmVM' と 'New-AzureRmVMSS' は、名前または ID でカスタム イメージをサポートします。
* ログ分析機能
    - 'Export-AzureRmLogAnalyticRequestRateByInterval' コマンドレットを追加しました
    - 'Export-AzureRmLogAnalyticThrottledRequests' コマンドレットを追加しました

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* コンテナー レジストリおよび Azure File ボリューム マウントのパラメーター セットの問題を修正しました

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* 次の変更を含むように ADF .Net SDK バージョン 0.6.0-preview を更新しました
    - 新しい AzureDatabricksLinkedService および DatabricksNotebookActivity を追加しました
    - HDInsightOnDemand LinkedService に headNodeSize プロパティと dataNodeSize プロパティを追加しました
    - SalesforceMarketingCloud の LinkedService、Dataset、CopySource を追加しました
    - すべてのアクティビティで SecureOutput のサポートを追加しました
    - 実行する同時実行アクティビティの数を制御する新しい BatchCount プロパティを ForEach アクティビティに追加しました
    - 新しいフィルター アクティビティを追加しました
    - リンクされたサービス パラメーターに対応するようになりました

#### <a name="azurermdns"></a>AzureRM.Dns
* プライベート DNS ゾーンのサポート (パブリック プレビュー)
    - 関連付けられた仮想ネットワークのみに表示される DNS ゾーンを作成する機能を追加しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* DNS のコマンドレットとの互換性のためにモデルの種類を更新しています。

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Azure Site Recovery に対する ASR Azure の変更 (コマンドレットは現在、Enterprise から Enterprise、Enterprise から Azure、HyperV から Azure、VMware から Azure の操作をサポートしています)
    - New-AzureRmRecoveryServicesAsrProtectionContainer
    - New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig
    - Remove-AzureRmRecoveryServicesAsrProtectionContainer
    - Update-AzureRmRecoveryServicesAsrProtectionDirection

#### <a name="azurermstorage"></a>AzureRM.Storage
* 保存時の暗号化は既定で有効であり、無効にできないため、ストレージ アカウントの新規と設定の各コマンドレットのパラメーター EnableEncryptionService および DisableEncryptionService を廃止しました。
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Remove-AzureRmWebAppSlot のヘルプを修正しました

## <a name="550---march-2018"></a>5.5.0 - 2018 年 3 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* 別名のインポートに関する問題を修正しました
* Newtonsoft.Json のバージョン 10.0.3 をバージョン 6.0.8 と共に読み込んでください

#### <a name="azurestorage"></a>Azure.Storage
* 論理的な削除機能のサポート
    - Enable-AzureStorageDeleteRetentionPolicy
    - Disable-AzureStorageDeleteRetentionPolicy
    - Get-AzureStorageBlob

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* 別名のインポートに関する問題を修正しました
* ファイアウォールおよびクエリのスケールアウト機能のサポートに加え 2017-08-01 api バージョンのサポートを追加しました。

#### <a name="azurermautomation"></a>AzureRM.Automation
* 別名のインポートに関する問題を修正しました

#### <a name="azurermcdn"></a>AzureRM.Cdn
* 別名のインポートに関する問題を修正しました

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* notice.txt と通知メッセージを更新しました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* "New-AzureRmVMSS" では、詳細モードで接続文字列が出力されます。
* "New-AzureRmVmss" では、パブリック IP アドレス、負荷分散規則、および受信 NAT 規則がサポートされます。
* WriteAccelerator 機能
    - WriteAccelerator スイッチ パラメーターを次のコマンドレットを追加しました: Set-AzureRmVMOSDisk、Set-AzureRmVMDataDisk、Add-AzureRmVMDataDisk、Add-AzureRmVmssDataDisk
    - OsDiskWriteAccelerator スイッチ パラメーターを Set-AzureRmVmssStorageProfile コマンドレットに追加しました。
    - OsDiskWriteAccelerator ブール値パラメーターを次のコマンドレットに追加しました: Update-AzureRmVM、Update-AzureRmVmss

#### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* 一部の暗号化操作で無意味なエラーの原因になっていた、資格情報暗号化に関する問題を修正しました
* データ ファクトリ全体で統合ランタイムを共有できるようにしました

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* カスタム セットアップおよびエディション選択機能を有効にする、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "SetupScriptContainerSasUri" と "Edition" を追加しました
* 一部の暗号化操作で重要性の低いエラーの原因になっていた、資格情報の暗号化に関する問題を修正しました。
* データ ファクトリ全体で統合ランタイムを共有できるようにしました

#### <a name="azurermhdinsight"></a>AzureRM.HDInsight
* 別名のインポートに関する問題を修正しました

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Set-AzureRmKeyVaultAccessPolicy の例を修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* 別名のインポートに関する問題を修正しました

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* 別名のインポートに関する問題を修正しました

#### <a name="azurermrecoveryservices"></a>AzureRM.RecoveryServices
* 別名のインポートに関する問題を修正しました

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* 別名のインポートに関する問題を修正しました

#### <a name="azurermresources"></a>AzureRM.Resources
* 別名のインポートに関する問題を修正しました

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* キューに EnableBatchedOperations プロパティを追加しました
* サブスクリプションに DeadLetteringOnFilterEvaluationExceptions プロパティを追加しました

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Service Fabric コマンドレットを更新しました
  - ARM テンプレートを更新しました
  - 失敗した操作がロールバックされなくなりました
  - Add-AzureRmServiceFabricNodeType
    - VM は既定で管理ディスクとなります
    - 既存の VMSS サブネットが使用されます
    - すべての操作はべき等です
  - Remove-AzureRmServiceFabricNodeType により、部分的に作成された VMSS およびクラスター ノードの種類がクリーンアップされます
  - 複雑なプロパティ型について PSCluster オブジェクトの出力を修正しました

#### <a name="azurermsql"></a>AzureRM.Sql
* 別名のインポートに関する問題を修正しました
* Get-AzureRmSqlServer、New-AzureRmSqlServer、および Remove-AzureRmSqlServer の応答に FullyQualifiedDomainName プロパティが含まれるようになりました。

#### <a name="azurermwebsites"></a>AzureRM.Websites
* 別名のインポートに関する問題を修正しました
* New-AzureRMWebApp - WebApp を簡単に作成できるようにするパラメーター セットを追加しました (ローカルの Git リポジトリをサポート)。

## <a name="540---february-2018"></a>5.4.0 - 2018 年 2 月
#### <a name="azurermautomation"></a>AzureRM.Automation
* New-AzureRmAutomationModule の別名を Import-AzureRmAutomationModule に追加しました

#### <a name="azurermcompute"></a>AzureRM.Compute
* 一部の Get コマンドレットの ErrorAction に関する問題を解決しました

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Azure コンテナー インスタンス SDK 2018-02-01 を適用しました
    - DNS 名ラベルのサポート

#### <a name="azurermdevtestlabs"></a>AzureRM.DevTestLabs
* 以前動作しなかった GET コマンドレットをすべて修正しました

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Get-AzureRmEventHubGeoDRConfiguration ヘルプのバグを修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* 新しい接続モニターを作成するコマンドレットを追加しました
    - New-AzureRmNetworkWatcherConnectionMonitor
* 接続モニターを更新するコマンドレットを追加しました
    - Set-AzureRmNetworkWatcherConnectionMonitor
* 接続モニターまたは接続モニターのリストを取得するコマンドレットを追加しました
    - Get-AzureRmNetworkWatcherConnectionMonitor
* 接続モニターにクエリを実行するコマンドレットを追加しました
    - Get-AzureRmNetworkWatcherConnectionMonitorReport
* 接続モニターを起動するコマンドレットを追加しました
    - Start-AzureRmNetworkWatcherConnectionMonitor
* 接続モニターを停止するコマンドレットを追加しました
    - Stop-AzureRmNetworkWatcherConnectionMonitor
* 接続モニターを削除するコマンドレットを追加しました
    - Remove-AzureRmNetworkWatcherConnectionMonitor
* Set-AzureRmApplicationGatewayBackendAddressPool のドキュメントを更新して非推奨の例を削除しました
* EnableHttp2 フラグを Application Gateway に追加しました
    - New-AzureRmApplicationGateway の更新: 省略可能なパラメーター EnableHttp2 を追加しました
* IpTag を PublicIpAddress に追加しました
    - New-AzureRmPublicIpAddress の更新: IpTag を追加しました
    - Iptag を追加する New-AzureRmPublicIpTag
* DisableBgpRoutePropagation プロパティを RouteTable および effectiveRoute に追加しました

#### <a name="azurermresources"></a>AzureRM.Resources
* Register-AzureRmProviderFeature: 不足している例をドキュメントに追加しました
* Register-AzureRmResourceProvider: 不足している例をドキュメントに追加しました

#### <a name="azurermstorage"></a>AzureRM.Storage
* 保存時の暗号化は既定で有効であり、無効にできないため、ストレージ アカウントの新規と設定の各コマンドレットのパラメーター EnableEncryptionService および DisableEncryptionService を廃止しました。
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount


## <a name="530---february-2018"></a>5.3.0 - 2018 年 2 月
### <a name="azurermprofile"></a>AzureRM.Profile
* PowerShell 3 および 4 の非推奨警告を追加しました
* `Add-AzureRmAccount` を `Connect-AzureRmAccount` に名前変更しました。古いコマンドレット名に対して別名を追加し、他の別名 (`Login-AzAccount` および `Login-AzureRmAccount`) を新しいコマンドレット名にリダイレクトしました。
* `Remove-AzureRmAccount` を `Disconnect-AzureRmAccount` に名前変更しました。古いコマンドレット名に対して別名を追加し、他の別名 (`Logout-AzAccount` および `Logout-AzureRmAccount`) を新しいコマンドレット名にリダイレクトしました。
* `Login-AzureRmAccount` の代わりに `Connect-AzureRmAccount` を使用するようにリソース文字列を修正しました
* `Add-AzureRmEnvironment` と `Set-AzureRmEnvironment`
  - OperationalInsights データ プレーン RP で使用するパラメーターとして `-AzureOperationalInsightsEndpoint` と `-AzureOperationalInsightsEndpointResourceId` を追加しました。

### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました

### <a name="azurermcompute"></a>AzureRM.Compute
* `New-AzureRmVM` の簡素化したパラメーター セットに `-AvailabilitySetName` パラメーターを追加しました。
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました
* VM および VM スケール セットに対するユーザー割り当て ID のサポート
    - `-IdentityType` および `-IdentityId` パラメーターを `New-AzureRmVMConfig`、`New-AzureRmVmssConfig`、`Update-AzureRmVM`、および `Update-AzureRmVmss` に追加しました
* `-EnableIPForwarding` パラメーターを `Add-AzureRmVmssNetworkInterfaceConfig` に追加しました
* `-Priority` パラメーターを `New-AzureRmVmssConfig` に追加しました

### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました

### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました
* `Login-AzureRmAccount` を使用してログインせずにこのコマンドレットを実行した場合の `Test-AzureRmDataLakeStoreAccount` のエラー メッセージを修正しました

### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* 2018-01-01 API バージョンを使用するように更新しました。

### <a name="azurermeventhub"></a>AzureRM.EventHub

* Geo ディザスター リカバリー操作用に、以下の新しいコマンドを追加しました。
  - 新しい別名 (ディザスター リカバリーの構成) を作成する
    - `New-AzureRmEventHubGeoDRConfiguration`
  - 別名 (ディザスター リカバリー構成) を取得する
    - `Get-AzureRmEventHubGeoDRConfiguration`
  - ディザスター リカバリーを無効にし、プライマリ名前空間からセカンダリ名前空間への変更の複製を停止する
    - `Set-AzureRmEventHubGeoDRConfigurationBreakPair`
  - ディザスター リカバリー フェールオーバーを呼び出し、セカンダリ名前空間を指すように別名を再構成する
    - `Set-AzureRmEventHubGeoDRConfigurationFailOver`
  - 別名 (ディザスター リカバリー構成) を削除する
    - `Remove-AzureRmEventHubGeoDRConfiguration`
* 名前空間名と GeoDr 構成名 (別名の可用性) のチェック用に以下のコマンドを追加しました。
  - 名前空間名または別名 (ディザスター リカバリーの構成) の可用性のチェック
    - `Test-AzureRmEventHubName`

### <a name="azurerminsights"></a>AzureRM.Insights
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました

### <a name="azurermnetwork"></a>AzureRM.Network
* 上書きの確認メッセージ "リソースを上書きしますか" を修正しました

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* `Invoke-AzureRmOperationalInsightsQuery` を介した V2 API クエリ実行のサポートを追加しました。 新しい API の詳細については、[https://dev.loganalytics.io/](https://dev.loganalytics.io/) を参照してください。

### <a name="azurermresources"></a>AzureRM.Resources
* `Get-AzureRmADServicePrincipal`: SPN パラメーター セットと冗長であるため、既定の空のパラメーター セットから `-ServicePrincipalName` を削除しました。

### <a name="azurermservicebus"></a>AzureRM.ServiceBus

* `Remove-AzureRmServiceBusRule` および `Get-AzureRmServiceBusKey` の機能修正プログラムを追加しました
* Geo ディザスター リカバリー操作用に、以下の新しいコマンドレットを追加しました。
  - 新しい別名 (ディザスター リカバリーの構成) を作成する
    - `New-AzureRmServiceBusDRConfigurations`
  - 別名 (ディザスター リカバリー構成) を取得する
    - `Get-AzureRmServiceBusDRConfigurations`
  - ディザスター リカバリーを無効にし、プライマリ名前空間からセカンダリ名前空間への変更の複製を停止する
    - `Set-AzureRmServiceBusDRConfigurationsBreakPairing`
  - ディザスター リカバリー フェールオーバーを呼び出し、セカンダリ名前空間を指すように別名を再構成する
    - `Set-AzureRmServiceBusDRConfigurationsFailOver`
  - 別名 (ディザスター リカバリー構成) を削除する
    - `Remove-AzureRmServiceBusDRConfigurations`
* Geo ディザスター リカバリーをサポートするように `Test-AzureRmServiceBusName` コマンドレットを更新しました - 別名の可用性チェック操作。
  - 名前空間名または別名 (ディザスター リカバリーの構成) の可用性のチェック
    - `Test-AzureRmServiceBusName`

### <a name="azurermusageaggregates"></a>AzureRM.UsageAggregates
* `Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました

## <a name="520---january-2018"></a>5.2.0 - 2018 年 1 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* Add-AzureRmAccount
  * 現在の VM/サービスの管理サービス ID の資格情報を使用して認証を行う -MSI ログインを追加しました
  * ユーザー指定のアクセス トークンを使用してログインする場合の KeyVault 認証を修正しました

#### <a name="azurestorage"></a>Azure.Storage
* Storage サービスのプロパティを取得および設定するコマンドレットを追加しました
    - Get-AzureStorageServiceProperty
    - Update-AzureStorageServiceProperty

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmApiManagementProperty、Set-AzureRmApiManagementProperty、および New-AzureRmApiManagement で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermapplicationinsights"></a>AzureRM.ApplicationInsights
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermautomation"></a>AzureRM.Automation
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* Set-AzureRmAutomationRunbook で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermbackup"></a>AzureRM.Backup
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermbatch"></a>AzureRM.Batch
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermcdn"></a>AzureRM.Cdn
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmCdnEndpoint および New-AzureRmCdnProfile で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Cognitive Services Management SDK バージョン 3.0.0 と統合しました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* 簡素化したパラメーター セットを New-AzureRmVmss に追加しました。これにより、スマートな既定値を使用して、仮想マシン スケール セットおよびすべての必要なリソースを作成できます
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmVm および Update-AzureRmVm で -Tag が優先されるように -Tags を廃止しました
* ゾーンが制限に含まれる場合の Get AzureRmComputeResourceSku コマンドレットを修正しました。
* Azure Monitor シンクがサポートされるように、診断エージェントの構成スキーマを更新しました。

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermcontainerregistry"></a>AzureRM.ContainerRegistry
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* データ ストアのリンクされたサービスすべてについて、Azure Key Vault のサポートを有効にしました
* Azure SSIS 統合ランタイムにライセンスの種類プロパティを追加しました
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmDataFactory で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* データ ストアのリンクされたサービスすべてについて、Azure Key Vault のサポートを有効にしました
* Azure SSIS 統合ランタイムにライセンスの種類プロパティを追加しました
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* "Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドで AHUB 機能を有効にするための "LicenseType" パラメーターを追加しました

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmDataLakeAnalyticsAccount および Set-AzureRmDataLakeAnalyticsAccount で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmDataLakeStoreAccount および Set-AzureRmDataLakeStoreAccount で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermdevtestlabs"></a>AzureRM.DevTestLabs
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermdns"></a>AzureRM.Dns
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* 次の新しいコマンドレッドを追加しました。
  - Update-AzureRmEventGridSubscription
    - Event Grid イベント サブスクリプションのプロパティを更新します。
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermhdinsight"></a>AzureRM.HDInsight
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurerminsights"></a>AzureRM.Insights
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermiothub"></a>AzureRM.IotHub
* IoTHub コマンドレットの証明書のサポートを追加しました
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* 実行時間が長い KeyVault コマンドレットのために -AsJob のサポートを追加しました。 選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。
  * 影響を受けるコマンドレット: Remove-AzureRmKeyVault
* Set-AzureRmKeyVaultAccessPolicy のバグを修正しました。このバグでは AAD フィルターによって UPN が設定されるのではなく、SPN が指定の UPN に設定されていました
  - 詳細については次の問題を参照してください: https://github.com/Azure/azure-powershell/issues/5201

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* Update-AzureRmMlCommitmentPlan で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermmachinelearningcompute"></a>AzureRM.MachineLearningCompute
* Remove-AzureRmMlOpCluster コマンドレットに IncludeAllResources パラメーターを追加しました
  - このスイッチ パラメーターを使用すると、最初にクラスターで作成されたすべてのリソースが削除されます
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermmedia"></a>AzureRM.Media
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* Set-AzureRmMediaService および New-AzureRmMediaService で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* 実行時間が長い Network コマンドレットのために -AsJob のサポートを追加しました。 選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmNotificationHubsNamespace および Set-AzureRmNotificationHubsNamespace で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmOperationalInsightsSavedSearch、Set-AzureRmOperationalInsightsSavedSearch、New-AzureRmOperationalInsightsWorkspace、および Set-AzureRmOperationalInsightsWorkspace で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermrecoveryservices"></a>AzureRM.RecoveryServices
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* the Restore-AzureRmRecoveryServicesBackupItem コマンドレッドに -UseOriginalStorageAccount オプションを追加しました。
  - このフラグを有効にすると、元のストレージ アカウントにディスクが復元されます。これにより、ユーザーは復元された VM の構成を元の VM にできる限り近いものに維持できます。
  - これは、復元操作のパフォーマンスの向上にも役立ちます。

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* ファイアウォール規則のために 3 つの新しいコマンドレットを追加しました
* geo レプリケーションのために 3 つの新しいコマンドレットを追加しました
* ゾーンとタグのサポートを追加しました
* 可能な場合は、ResourceGroup を省略可能としてマークしてください。

#### <a name="azurermrelay"></a>AzureRM.Relay
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermresources"></a>AzureRM.Resources
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* 実行時間が長い Resources コマンドのために -AsJob のサポートを追加しました。 選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。
* 名前付け規則に準拠するように Get AzureRmProviderOperation から Get-AzureRmResourceProviderAction に別名を追加しました

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermservermanagement"></a>AzureRM.ServerManagement
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* New-AzureRmServerManagementNode および New-AzureRmServerManagementGateway で -Tag が優先されるように -Tags を廃止しました

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermsiterecovery"></a>AzureRM.SiteRecovery
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermsql"></a>AzureRM.Sql
* 監査コマンドのパラメーターの説明を更新しました
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* 実行時間の長いコマンドレットに -AsJob パラメーターを追加しました
* Get AzureRmSqlServiceObjective の - DatabaseName パラメーターを廃止しました

#### <a name="azurermstorage"></a>AzureRM.Storage
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* -EnableEncryptionService None パラメーターを指定した New-AzureRMStorageAccount コマンドレットを実行した際の null 参照の問題を修正しました
* 実行時間が長い Storage コマンドレットのために -AsJob のサポートを追加しました。 選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。
    - 影響を受けるコマンドレットは、Storage Account および Storage Account Network Rule の New-、Remove-、Add-、Update- です。

#### <a name="azurermstreamanalytics"></a>AzureRM.StreamAnalytics
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました

#### <a name="azurermwebsites"></a>AzureRM.Websites
* 有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました
* 現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました
* 実行時間が長い Websites コマンドレットのために -AsJob のサポートを追加しました。 選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。
     - 影響を受けるコマンドレットは、WebApps、AppServicePlan、および Slots の New-、Remove-、Add-、Set- です

## <a name="2017128-version-511"></a>2017.12.8 バージョン 5.1.1
* AnalysisServices
  - すべてのクラウドがサポートされるように、場所の検証セットを動的ルックアップに変更しました。
* Automation
  - Import-AzureRMAutomationRunbook に更新しました
    - Python2 Runbook がサポートされるようになりました
* Batch
  - リソース グループがないアカウント操作がリソース グループの自動検出に失敗するというバグを修正しました
* コンピューティング
  - Get-AzureRmComputeResourceSku によってゾーン情報が表示されます。
  - 問題 https://github.com/Azure/azure-powershell/issues/5038 を修正するために Disable-AzureRmVmssDiskEncryption を更新しました
  - 実行時間が長い Compute コマンドレット用の -AsJob サポートを追加しました。 選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。
    - 影響を受けるコマンドレット: Virtual Machines および VM Scale Sets の New-、Update-、Set-、Remove-、Start-、Restart-、Stop- コマンドレット
    - 簡素化したパラメーター セットを New-AzureRmVM に追加しました。これにより、スマートな既定値を使用して、仮想マシンおよびすべての必要なリソースを作成できます
* ContainerInstance
  - Azure コンテナー インスタンス SDK 2017-10-01 を適用しました
    - コンテナー run-to-completion のサポート
    - Azure File ボリューム マウントのサポート
    - パブリック IP の複数ポートのオープンのサポート
* ContainerRegistry
  - geo レプリケーションと webhook の新しいコマンドレット
    - Get/New/Remove-AzureRmContainerRegistryReplication
    - Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook
* DataFactories
    - 資格情報の暗号化機能が、"リモート アクセス" 有効 (ネットワーク経由) と "リモート アクセス" 無効 (ローカル コンピューター) の両方で動作するようになりました。
* DataFactoryV2
  - 2 つのコマンドレットを新しく追加しました: Update-AzureRmDataFactoryV2 および Stop-AzureRmDataFactoryV2PipelineRun
* DataLakeAnalytics
  - ScriptParameter というパラメーターを Submit-AzureRmDataLakeAnalyticsJob に追加しました
    - ScriptParameter に関する詳細情報を、Submit-AzureRmDataLakeAnalyticsJob で Get-Help を使用して確認できます
  - New-AzureRmDataLakeAnalyticsAccount については、パラメーター MaxDegreeOfParallelism を MaxAnalyticsUnits に変更しました
    - パラメーター MaxAnalyticsUnits の別名を追加しました: MaxDegreeOfParallelism
  - New-AzureRmDataLakeAnalyticsComputePolicy については、パラメーター MaxDegreeOfParallelismPerJob を MaxAnalyticsUnitsPerJob に変更しました
    - パラメーター MaxAnalyticsUnitsPerJob の別名を追加しました: MaxDegreeOfParallelismPerJob
  - Set-AzureRmDataLakeAnalyticsAccount については、パラメーター MaxDegreeOfParallelism を MaxAnalyticsUnits に変更しました
    - パラメーター MaxAnalyticsUnits の別名を追加しました: MaxDegreeOfParallelism
  - Submit-AzureRmDataLakeAnalyticsJob については、パラメーター DegreeOfParallelism を AnalyticsUnits に変更しました
    - パラメーター AnalyticsUnits の別名を追加しました: DegreeOfParallelism
  - Update-AzureRmDataLakeAnalyticsComputePolicy については、パラメーター MaxDegreeOfParallelismPerJob を MaxAnalyticsUnitsPerJob に変更しました
    - パラメーター MaxAnalyticsUnitsPerJob の別名を追加しました: MaxDegreeOfParallelismPerJob
* MachineLearningCompute
  - Set-AzureRmMlOpCluster を追加しました
    - クラスターのエージェント数または SSL 構成を更新しました
  - オーケストレーター プロパティがオプションになりました
    - サービス プリンシパルが提供されていない場合、そのサービス プリンシパルはサービスによって作成されるため、オーケストレーター プロパティがオプションになりました
* PowerBIEmbedded
  - Power BI Embedded 容量コマンドレットのサポートを追加しました
  - 新しいコマンドレット Get-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量の詳細を取得します。
  - 新しいコマンドレット New-AzureRmPowerBIEmbeddedCapacity - 新しい PowerBI Embedded 容量を作成します
  - 新しいコマンドレット Remove-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを削除します
  - 新しいコマンドレット Resume-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを再開します
  - 新しいコマンドレット Suspend-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを中断します
  - 新しいコマンドレット Test-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスの存在をテストします
  - 新しいコマンドレット Update-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを変更します
* プロファイル
  - USGovernmentActiveDirectoryEndpoint を https://login.microsoftonline.us/ に更新しました
    - Azure Government エンドポイント マッピングの詳細については、https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping を参照してください
    - コマンドの -AsJob サポートを追加しました。これにより、選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます
    - -AsJob パラメーターを Get-AzureRmSubscription コマンドレットに追加しました
* RecoveryServices.Backup
  - バグを修正 - Get-AzureRmRecoveryServicesBackupItem が、コンテナー名フィルターの比較で大文字と小文字を区別するようになりました。
  - バグを修正 - AzureVmItem に、前回のバックアップ操作が行われた時間を示すプロパティが追加されました - LastBackupTime。
* リソース
  - Get-AzureRMRoleAssignment による割り当てで、カスタム ロールの roledefiniton 名がないという問題を修正しました
    - ユーザーは、ロールの種類に関係なく、Get-AzureRMRoleAssignment で、roledefinition 名を持つ割り当てを使用できるようになりました
  - assignablescopes に新しいスコープがある場合に、RD が見つからないというエラーを Set-AzureRMRoleRoleDefinition がスローするという問題を修正しました
    - ユーザーが、スコープの位置に関係なく、Set-AzureRMRoleRoleDefinition で、新しいスコープを含む割り当て可能なスコープを使用できるようになりました
  - スコープの末尾に "/" を使用できます
    - スコープの末尾が "/" の RoleDefinition および RoleAssignment コマンドレットをユーザーが使用できるようになりました。これにより、API および CLI との一貫性が確保されます
  - ユーザーが、委任フラグを使用して RoleAssignment を作成できます
    - ユーザーが、New-AzureRMRoleAssignment で、委任フラグ追加オプションを使用できるようになりました
  - スコープのパラメーターを優先するように RoleAssignment get を修正しました
  - New-AzureRmRoleAssignment コマンドレットに ServicePrincipalName の別名を追加しました
    - ユーザーが、New- AzureRmRoleAssignment コマンドレットを使用するときに、ServicePrincipalName ではなく ApplicationId を使用できるようになりました
* SiteRecovery
  - 次の重大な変更のリリースに備えて、このモジュールのすべてのコマンドレットに非推奨警告を追加しました。
    - AzureRM からコマンドレットを移行する方法の詳細については、今後の重大な変更ガイドを参照してください。
* SQL
  - Set-AzureRmSqlDatabase を使用して、データベースの名前を変更する機能を追加しました
  - 修正された問題 https://github.com/Azure/azure-powershell/issues/4974
    - 監査コマンドレットに無効な AUDIT_CHANGED_GROUP 値を指定しても、エラーがスローされなくなりました。これは今後のリリースで削除される予定です。
  - 修正された問題 https://github.com/Azure/azure-powershell/issues/5046
    - 監査コマンドレットの AuditAction パラメーターが無視されなくなりました
  - "Secondary" StorageKeyType を指定したときの監査コマンドレットの問題を修正しました
    - BLOB 監査の設定時に、StorageKeyType パラメーターに "Secondary" 値を指定すると、セカンダリ ストレージ アカウント キーではなくプライマリ キーが使用されました。
  - Set-AzureRmSqlServerTransparentDataEncryptionProtector からの確認メッセージの表現を変更しました
* Azure (RDFE)
    - すべての RemoteApp コマンドレットを削除しました
* Azure.Storage
    - Azure Storage Client Library 8.6.0 および Azure Storage DataMovement Library 0.6.5 にアップグレードしました

## <a name="20171110-version-501"></a>2017.11.10 バージョン 5.0.1
* 以下のモジュールで一部のコマンドレットを実行した際に失敗の原因となるアセンブリ読み込みの問題を修正しました
  - AzureRM.ApiManagement
  - AzureRM.Backup
  - AzureRM.Batch
  - AzureRM.Compute
  - AzureRM.DataFactories
  - AzureRM.HDInsight
  - AzureRM.KeyVault
  - AzureRM.RecoveryServices
  - AzureRM.RecoveryServices.Backup
  - AzureRM.RecoveryServices.SiteRecovery
  - AzureRM.RedisCache
  - AzureRM.SiteRecovery
  - AzureRM.Sql
  - AzureRM.Storage
  - AzureRM.StreamAnalytics

## <a name="2017118---version-500"></a>2017.11.8 - バージョン 5.0.0
* 注: これは重大な変更のリリースです。 導入された重大な変更の完全な一覧については、移行ガイド (https://aka.ms/azps-migration-guide)) を参照してください。
* AzureRM のコマンドレットはすべて、オンライン ヘルプをサポートするようになりました
  - -Online パラメーターを指定して Get-Help を実行すると、既定のインターネット ブラウザーでオンライン ヘルプが表示されます
* AnalysisServices
  * 同期のために新しい AsAzure REST API と連携するように Synchronize-AzureAsInstance コマンドを修正しました
* ApiManagement
  * ApiManagement の、このリリースでの重大な変更については、移行ガイドを参照してください
  * 問題 (https://github.com/Azure/azure-powershell/issues/4510) を修正するために Get-AzureRmApiManagementUser コマンドレットを更新しました
  * 空のパスを持つ API (https://github.com/Azure/azure-powershell/issues/4069) を作成するために、New-AzureRmApiManagementApi コマンドレットを更新しました
* ApplicationInsights
  * Application Insights のリソースを取得/作成/削除するコマンドを追加
    - Get-AzureRmApplicationInsights
    - New-AzureRmApplicationInsights
    - Remove-AzureRmApplicationInsights
  * Application Insights のリソースの価格/日次上限を取得/更新するコマンドを追加
    - Get-AzureRmApplicationInsights -IncludeDailyCap
    - Set-AzureRmApplicationInsightsPricingPlan
    - Set-AzureRmApplicationInsightsDailyCap
  * Application Insights のリソースの連続エクスポートを取得/作成/更新/削除するコマンドを追加
    - Get-AzureRmApplicationInsightsContinuousExport
    - Set-AzureRmApplicationInsightsContinuousExport
    - New-AzureRmApplicationInsightsContinuousExport
    - Remove-AzureRmApplicationInsightsContinuousExport
  * Application Insights のリソースの API キーを取得/作成/削除するコマンドを追加
    - Get-AzureRmApplicationInsightsApiKey
    - New-AzureRmApplicationInsightsApiKey
    - Remove-AzureRmApplicationInsightsApiKey
* AzureBatch
  * 新しいパラメーターを `New-AzureRmBatchAccount` に追加しました。
    - `PoolAllocationMode`: Batch アカウントでプールを作成するために使用する割り当てモード。 ユーザーのサブスクリプションにプール ノードを割り当てる Batch アカウントを作成するには、これを `UserSubscription` に設定します。
    - `KeyVaultId`: Batch アカウントに関連付けられている Azure Key Vault のリソース ID。
    - `KeyVaultUrl`: Batch アカウントに関連付けられている Azure Key Vault の URL。
  * `New-AzureBatchTask` のパラメーターを更新しました。
    - `RunElevated` スイッチを削除しました。 `RunElevated` の代わりに `UserIdentity` パラメーターを追加しました。以下のように `PSUserIdentity` を作成することにより同じ動作を行うことができます。
      - $autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")
      - $userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser
    - `AuthenticationTokenSettings` パラメーターを追加しました。 このパラメーターを使用すると、タスクの実行時に認証トークンを提供するようバッチ サービスに要求でき、バッチ サービスに要求を出すためにバッチ アカウント キーをタスクに渡す必要がなくなります。
    - `ContainerSettings` パラメーターを追加しました。
      - このパラメーターを使用すると、コンテナー内部でタスクを実行するよう Batch サービスに要求できます。
    - `OutputFiles` パラメーターを追加しました。
      - このパラメーターを使用すると、タスクの終了後に Azure Storage にファイルをアップロードするようにタスクを構成できます。
  * `New-AzureBatchPool` のパラメーターを更新しました。
    - `UserAccounts` パラメーターを追加しました。
      - このパラメーターは、プール内の各ノードで作成されたユーザー アカウントを定義します。
    - `TargetLowPriorityComputeNodes` を追加し、`TargetDedicated` を `TargetDedicatedComputeNodes` に名前変更しました。
      - `TargetDedicatedComputeNodes` パラメーター用に `TargetDedicated` の別名を作成しました。
    - `NetworkConfiguration` パラメーターを追加しました。
      - このパラメーターを使用すると、プールのネットワーク設定を構成できます。
  * `New-AzureBatchCertificate` のパラメーターを更新しました。
    - `Password` パラメーターが `SecureString` になりました。
  * `New-AzureBatchComputeNodeUser` のパラメーターを更新しました。
    - `Password` パラメーターが `SecureString` になりました。
  * `Set-AzureBatchComputeNodeUser` のパラメーターを更新しました。
    - `Password` パラメーターが `SecureString` になりました。
  * `Get-AzureBatchNodeFile`、`Get-AzureBatchNodeFileContent`、および `Remove-AzureBatchNodeFile` で、`Name` パラメーターを `Path` に名前変更しました。
    - `Path` パラメーター用に `Name` の別名を作成しました。
  * オブジェクトに対する変更
    - 完全なリストについては、Batch 変更ログを参照してください
  * Azure Active Directory ベースの認証のサポートを追加しました。
    - Azure Active Directory 認証を使用するには、`Get-AzureRmBatchAccount` コマンドレットを使用して `BatchAccountContext` オブジェクトを取得し、この `BatchAccountContext` を Batch サービス コマンドレットの `-BatchContext` パラメーターに指定します。 Azure Active Directory 認証は、`PoolAllocationMode = UserSubscription` のアカウントには必須です。
    - 既存のアカウント、または `PoolAllocationMode = BatchService` で作成された新しいアカウントの場合、`Get-AzureRmBatchAccoutKeys` コマンドレットを使用して `BatchAccountContext` オブジェクトを取得することにより、共有キー認証の使用を継続できます。
* コンピューティング
  * Azure Disk Encryption 拡張コマンド
    - "Set-AzureRmVmDiskEncryptionExtension" の新しいパラメーター: "-EncryptFormatAll" はデータ ディスクを暗号化フォーマットします
    - "Set-AzureRmVmDiskEncryptionExtension" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます
    - "Disable-AzureRmVmDiskEncryption" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます
    - "Get-AzureRmVmDiskEncryptionStatus" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます
* DataLakeAnalytics
  * DataLakeAnalytics の、このリリースでの重大な変更については、移行ガイドを参照してください
  * Get-AzureRmDataLakeAnalyticsAccount の 2 つの OutputTypes の 1 つを変更しました
    - List\<DataLakeAnalyticsAccount> から List\<PSDataLakeAnalyticsAccountBasic>
    - PSDataLakeAnalyticsAccountBasic のプロパティは DataLakeAnalyticsAccount のプロパティの厳密なサブセットです
    - DataLakeAnalyticsAccount にある追加プロパティはサービスによって返されません。  そのため、この変更はこれを正確に反映するためのものです。 これらの追加プロパティは引き続き PSDataLakeAnalyticsAccountBasic にありますが、これらには廃止のタグが付けられます。
  * Get-AzureRmDataLakeAnalyticsJob の 2 つの OutputTypes の 1 つを変更しました
    - List\<JobInformation> から List\<PSJobInformationBasic>
    - PSJobInformationBasic のプロパティは JobInformation のプロパティの厳密なサブセットです
    - JobInformation にある追加プロパティはサービスによって返されません。  そのため、この変更はこれを正確に反映するためのものです。 これらの追加プロパティは引き続き PSJobInformationBasic にありますが、これらには廃止のタグが付けられます。
* DataLakeStore
  * DataLakeStore の、このリリースでの重大な変更については、移行ガイドを参照してください
  * Get-AzureRmDataLakeStoreAccount の 2 つの OutputTypes の 1 つを変更しました
    - List\<PSDataLakeStoreAccount> から List\<PSDataLakeStoreAccountBasic>
    - PSDataLakeStoreAccountBasic のプロパティは PSDataLakeStoreAccount のプロパティの厳密なサブセットです
    - PSDataLakeStoreAccount にある追加プロパティはサービスによって返されません。  そのため、この変更はこれを正確に反映するためのものです。 これらの追加プロパティは引き続き PSDataLakeStoreAccountBasic にありますが、これらには廃止のタグが付けられます。
* DNS
  * Azure DNS での CAA レコードの種類のサポート
    - CAA レコードの種類に対するすべての操作をサポートします
* EventHub
  * EventHub の、このリリースでの重大な変更については、移行ガイドを参照してください
* 洞察
  * Insights の、このリリースでの重大な変更については、移行ガイドを参照してください
* ネットワーク
  * Network の、このリリースでの重大な変更については、移行ガイドを参照してください
  * 指定された Azure リージョンで使用可能なインターネット サービス プロバイダーを一覧表示するコマンドレットを追加しました
    - Get-AzureRmNetworkWatcherReachabilityProvidersList
  * 指定された場所から Azure リージョンまでのインターネット サービス プロバイダーの相対待機時間スコアを取得するコマンドレットを追加しました
    - Get-AzureRmNetworkWatcherReachabilityReport
* プロファイル
  - Set-AzureRmDefault
    - このコマンドレットを使用して、既定のリソース グループを設定します。  これにより、-ResourceGroup パラメーターが一部のコマンドレットで省略可能になり、リソース グループを指定しない場合に既定値が使用されます
    - ```Set-AzureRmDefault -ResourceGroupName "ExampleResourceGroup"```
    - 指定したリソース グループがサブスクリプションに存在する場合は、このリソース グループが既定値に設定されます。  それ以外の場合、リソース グループが作成され、既定値に設定されます。
  - Get-AzureRmDefault
    - このコマンドレットを使用して、現在の既定のリソース グループ (および今後はその他の既定値) を取得します。
    - ```Get-AzureRmDefault -ResourceGroup```
  - Clear-AzureRmDefault
    - このコマンドレットを使用して、現在の既定のリソース グループを削除します
    - ```Clear-AzureRmDefault -ResourceGroup```
  - Add-AzureRmEnvironment および Set-AzureRmEnvironment
    - BatchAudience パラメーターを追加します。これにより、Batch サービスの認証トークンを取得する際に使用する Azure Batch Active Directory オーディエンスを指定できます。
* RecoveryServices.Backup
  * インスタント ファイル回復を実行するコマンドレットを追加しました。
    - Get-AzureRmRecoveryServicesBackupRPMountScript
    - Disable-AzureRmRecoveryServicesBackupRPMountScript
  * RecoveryServices.Backup SDK を最新バージョンに更新しました
  * テスト実行に必要なすべての設定がテスト自体で行われるように、Azure VM ワークロードのテストを更新しました。
  * https://github.com/Azure/azure-powershell/issues/3164 を修正しました
* RecoveryServices.SiteRecovery
  * Azure Site Recovery に対する ASR VMware の変更 (コマンドレットは現在、Enterprise から Enterprise、Enterprise から Azure、HyperV から Azure の操作をサポートしています)
    - New-AzureRmRecoveryServicesAsrPolicy
    - New-AzureRmRecoveryServicesAsrProtectedItem
    - Update-AzureRmRecoveryServicesAsrPolicy
    - Update-AzureRmRecoveryServicesAsrProtectionDirection
  * AAD ベースのコンテナーにサポートを追加しました
  * VCenter リソースを管理するコマンドレットを追加しました
    - Get-AzureRmRecoveryServicesAsrVCenter
    - New-AzureRmRecoveryServicesAsrVCenter
    - Remove-AzureRmRecoveryServicesAsrVCenter
    - Update-AzureRmRecoveryServicesAsrVCenter
  * その他のコマンドレットを追加しました
    - Get-AzureRmRecoveryServicesAsrAlertSetting
    - Get-AzureRmRecoveryServicesAsrEvent
    - New-AzureRmRecoveryServicesAsrProtectableItem
    - Set-AzureRmRecoveryServicesAsrAlertSetting
    - Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob
    - Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob
    - Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob
    - Update-AzureRmRecoveryServicesAsrMobilityService
* ServiceBus
  - ServiceBus の、このリリースでの重大な変更については、移行ガイドを参照してください
* SQL
  * データベースに対する非同期 updateslo 操作の一覧表示およびキャンセルのサポートを追加
    - DB updateslo 操作状態を返すように既存の Get-AzureRmSqlDatabaseActivity コマンドレットを更新。
    - データベースに対する非同期 updateslo 操作をキャンセルする新しい Stop-AzureRmSqlDatabaseActivity コマンドレットを追加。
  * データベースとエラスティック プールのゾーン冗長性に対するサポートを追加
    - ZoneRedundant スイッチ パラメーターを New-AzureRmSqlDatabase に追加
    - ZoneRedundant スイッチ パラメーターを Set-AzureRmSqlDatabase に追加
    - ZoneRedundant スイッチ パラメーターを New-AzureRmSqlElasticPool に追加
    - ZoneRedundant スイッチ パラメーターを Set-AzureRmSqlElasticPool に追加
  * サーバー DNS エイリアスに対するサポートを追加
    - サーバーとエイリアス名ごとにサーバー DNS エイリアスを取得するか、Azure SQL Server のサーバー DNS エイリアスの一覧を取得する、Get-AzureRmSqlServerDnsAlias コマンドレットを追加
    - 指定の Azure SQL Server の新しいサーバー DNS エイリアスを作成する、New-AzureRmSqlServerDnsAlias コマンドレットを追加
    - サーバー DNS エイリアスが指す Azure SQL Server を更新できる、Set-AzurermSqlServerDnsAlias コマンドレットを追加
    - Azure SQL Server のサーバー DNS エイリアスを削除する、Remove-AzureRmSqlServerDnsAlias コマンドレットを追加
* Azure.Storage
  * Azure Storage Client Library 8.5.0 および Azure Storage DataMovement Library 0.6.3 へのアップグレード
  * ファイル共有スナップショット サポート機能を追加
    - "SnapshotTime" パラメーターを Get-AzureStorageShare に追加
    - "IncludeAllSnapshot" パラメーターを Remove-AzureStorageShare に追加
