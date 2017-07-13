---
title: "Azure PowerShell の変更履歴 | Microsoft Docs"
description: "Azure PowerShell の最新リリースで行われた変更の履歴です。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-resource-manager
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 5c8fa2a5a8f94cd24b66f42c237749a7b89af3b3
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-400"></a>バージョン 4.0.0

* このリリースには、重大な変更が含まれています。 変更の詳細と既存のスクリプトへの影響については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください。
* ApiManagement
  - New-AzureRmApiManagementGroup での外部グループの構成に対応しました。
* 課金
  - 新しいコマンドレット Get-AzureRmBillingPeriod
    + サブスクリプションに対する Azure の請求期間を取得するコマンドレット。
  - コマンドレット Get-AzureRmBillingInvoice を更新しました
  - 新しいプロパティ BillingPeriodNames
  - リスト ビューでの出力
* 計算
  - Premium 管理ディスクをサポートするように Set-AzureRmVMAEMExtension と Test-AzureRmVMAEMExtension の各コマンドレットが更新されました
  - IaaS VM の暗号化設定をバックアップし、障害時に復元を行います
  - ChefServiceInterval オプションの名前が ChefDaemonInterval に変更されました。 なお、以前のものは引き続き有効です。
  - 重複している DataDiskNames および NetworkInterfaceIDs の各プロパティが PS VM オブジェクトから削除されます。
  - DataDiskNames および NetworkInterfaceIDs パラメーターは、それぞれ Remove-AzureRmVMDataDisk および Remove-AzureRmVMNetworkInterface で省略可能になります。
  - Get コマンドレットがリスト オブジェクトを返すときの Get コマンドレットのパイプ処理の問題が解決されます。
  - RDFE コマンドレットと競合しているコマンドレットの名前は変更されました。 詳細については、https://github.com/Azure/azure-powershell/issues/2917 で問題を参照してください。
    + `New-AzureVMSqlServerAutoBackupConfig` の名前が `New-AzureRmVMSqlServerAutoBackupConfig` に変更されました
    + `New-AzureVMSqlServerAutoPatchingConfig` の名前が `New-AzureRmVMSqlServerAutoPatchingConfig` に変更されました
    + `New-AzureVMSqlServerKeyVaultCredentialConfig` の名前が `New-AzureRmVMSqlServerKeyVaultCredentialConfig` に変更されました
* 使用量
  - 新しいコマンドレット Get-AzureRmConsumptionUsageDetail
    + サブスクリプションの使用量の詳細を取得するコマンドレット。
* ContainerRegistry
  - Azure Container Registry の PowerShell コマンドレットが追加されました。
    + New-AzureRmContainerRegistry
    + Get-AzureRmContainerRegistry
    + Update-AzureRmContainerRegistry
    + Remove-AzureRmContainerRegistry
    + Get-AzureRmContainerRegistryCredential
    + Update-AzureRmContainerRegistryCredential
    + Test-AzureRmContainerRegistryNameAvailability
* DataLakeAnalytics
  - カタログ パッケージの取得およびリストに対応しました。
  - 深い先祖からの、次のカタログ項目の一覧表示に対応しました。
    + テーブル
    + TVF
    + 表示
    + 統計
* DataLakeStore
  - `Import-AzureRMDataLakeStoreItem` および `Export-AzureRMDataLakeStoreItem` では、パフォーマンス向上のため、トレース ログ記録が既定で無効になっています。 トレース ログ記録が必要な場合は、`-DiagnosticLogLevel` と `-DiagnosticLogPath` の各パラメーターを使用してください。
  - ADLS に小さなファイルを多数アップロードすると PowerShell がときどきクラッシュするバグを修正しました。
* EventHub
  - バグの修正:
    + Set-AzureRmEventHubNamespace コマンドレットのエラーが修正されます - "Tier" は、null にはできないため、"SkuName" にする必要があります。
    + Set-AzureRmEventHub - EventHub の更新中に発生する "オブジェクト参照がオブジェクトのインスタンスに設定されていません" というエラーが修正されます。
* 洞察
  - Add-AzureRm*AlertRule
    + 単一オブジェクト newResource、statusCode、requestId を返します。
  - Get-AzureRmAlertRule
    + 出力は、単一オブジェクトと見なされるのではなく、列挙されます。 型に変更はなく、リストのままです。
  - Remove-AzureRmAlertRule
    + statusCode は、要求によって返される状態コードに従います。以前は常に OK でした。
  - Add-AzureRmAutoscaleSetting
    + statusCode、requestId、および新しく作成または更新されたリソースを含む単一オブジェクトを返します (以前のようなリストではありません)。
    + 状態コードは、要求によって返される状態に従います。以前は常に OK でした。
  - New-AzureRmAutoscaleRule
    + パラメーター ScaleActionType が拡張され、ChangeCount、PercentChangeCount、ExactCount の各値を受け取るようになりました。
  - Remove-AzureRmAutoscaleSetting
    + 出力の statusCode は、要求によって返される statusCode に従います。 以前は常に OK でした。
  - Get-AzureRMLogProfile
    + 出力は列挙されます。 以前は単一オブジェクトと見なされていました。 出力の型は以前と同様にリストのままです。
  - Remove-AzureRmLogProfile
    + PassThru パラメーターが実装されました。
  - メトリックの API
    + SDK は MDM からメトリックを取得するようになりました。
  - Get-AzureRmMetricDefinition
    + 出力はリストのままですが、リストの構造は変更されました。
  - Get-AzureRmMetric
    + 呼び出しが変更されました。 新しい構文は次のとおりです: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]
    + 出力はリストで、要素の構造が変更されました。
* KeyVault
  - KeyVault シークレットのバックアップ/復元に対応しました。
    + キーに対して現在サポートされている機能に合わせて、シークレットをバックアップおよび復元できます。

  - キーとシークレットのバックアップ コマンドレットでは、対応するオブジェクトを入力パラメーターとして受け入れるようになりました。
    + 呼び出し元で、次のように取得操作とバックアップ操作を連結できます: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey

  - バックアップ コマンドレットが、既存のファイルを上書きする -Force スイッチに対応しました。
    + 既存のファイルを上書きしようとしてもスローされなくなり、代わりに、ユーザーは続行方法を選択しるように求められます。
* LogicApp
  - インターチェンジ制御番号のディザスター リカバリー コマンドレット用の新しいパラメーター
    + 省略可能 - 関連する制御番号を指定する -AgreementType パラメーター ("X12" または "Edifact")
* MachineLearning
  - Azure Machine Learning .Net SDK の新しいバージョンを使用するようになり、新しいコマンドレットが追加されました。
    + Add-AzureRmMlWebServiceRegionalProperty
  - ヘルプ テキストの用語を部分的に修正しています。
* ネットワーク
  - Test-AzureRmNetworkWatcherConnectivity コマンドレットが追加されました。
    + 指定されたソース VM とターゲットの接続情報を返します。
    + ソースとターゲットの間の接続を確立できない場合は、問題に関する詳細情報が返されます。
* プロファイル
  - "Send-Feedback" コマンドレットの追加: このコマンドレットを使用すると、Azure PowerShell のチームにフィードバックを送信する一連のプロンプトを開始できます。
  - 次のエイリアスは、Azure モジュールの既存のコマンドレット名と競合しているため、削除されました。
    + `Enable-AzureDataCollection` (`Enable-AzureRmDataCollection` でサポート)
    + `Disable-AzureDataCollection` (`Disable-AzureRmDataCollection` でサポート)
* リレー
  - ユーザーがすべての Azure リレー リソースを作成および管理できる Azure リレーのコマンドレットを追加します。
    + `New-AzureRmRelayNamespace`
    + `Get-AzureRmRelayNamespace`
    + `Set-AzureRmRelayNamespace`
    + `Remove-AzureRmRelayNamespace`
    + `New-AzureRmWcfRelay`
    + `Get-AzureRmWcfRelay`
    + `Set-AzureRmWcfRelay`
    + `Remove-AzureRmWcfRelay`
    + `New-AzureRmRelayHybridConnection`
    + `Get-AzureRmRelayHybridConnection`
    + `Set-AzureRmRelayHybridConnection`
    + `Remove-AzureRmRelayHybridConnection`
    + `Test-AzureRmRelayName`
    + `Get-AzureRmRelayOperation`
    + `New-AzureRmRelayKey`
    + `Get-AzureRmRelayKey`
    + `New-AzureRmRelayAuthorizationRule`
    + `Get-AzureRmRelayAuthorizationRule`
    + `Set-AzureRmRelayAuthorizationRule`
    + `Remove-AzureRmRelayAuthorizationRule`
* リソース
  - New-AzureRmResourceGroupDeployment でリソース グループをまたがるデプロイに対応しました
    + ユーザーは、さまざまなリソース グループをデプロイする際に、入れ子になったデプロイを使用できます。
* ServiceBus

  - バグの修正: ServiceBus キュー オブジェクトのプロパティ値は null に設定されていましたが、このオブジェクトが、キューを更新する Set-AzureRmServiceBusQueue コマンドレットの入力パラメーターとして使用されるようになりました。
   - 影響を受けるプロパティは、LockDuration、EntityAvailabilityStatus、DuplicateDetectionHistoryTimeWindow、MaxDeliveryCount、MessageCount です。
* ServiceFabric

  - Service Fabric のコマンドレットが追加されました。
    + Add-AzureRmServiceFabricApplicationCertificate       アプリケーション証明書として使用される証明書を追加します。
    + Add-AzureRmServiceFabricClientCertificate       クライアント認証用のクラスター設定に共通名または拇印を追加します。
    + Add-AzureRmServiceFabricClusterCertificate       既存の証明書をロールオーバーするためにクラスターにセカンダリのクラスター証明書を追加します。
    + Add-AzureRmServiceFabricNodes       クラスターに特定のノード タイプのノード/VM を追加します。
    + Add-AzureRmServiceFabricNodeType       既存のクラスターにノード タイプ/VM を追加します。
    + Get-AzureRmServiceFabricCluster       クラスター リソースの詳細を取得します。
    + New-AzureRmServiceFabricCluster は、新しい ServiceFabric クラスターを作成します。 このコマンドは、さまざまなシナリオをカバーするため、オーバーロードが多数あります。
    + overloadsemove-AzureRmServiceFabricClientCertificate       クラスターへのアクセスに使用されているクライアント証明書を削除します。
    + Remove-AzureRmServiceFabricClusterCertificate       クラスターのセキュリティに使用されているクラスター証明書を削除します。
    + Remove-AzureRmServiceFabricNodes       クラスターから特定のノード タイプのノードを削除します。
    + Remove-AzureRmServiceFabricNodeType       クラスターからノード タイプを 1 つ削除します。
    + Remove-AzureRmServiceFabricSettings       クラスターから 1 つ以上の ServiceFabric 設定を削除します。
    + Set-AzureRmServiceFabricSettings       クラスターの 1 つ以上の ServiceFabric 設定を追加または更新します。
    + Set-AzureRmServiceFabricUpgradeType       クラスターの ServiceFabric アップグレードの種類を変更します。
    + Update-AzureRmServiceFabricDurability       クラスターの持続性層を変更します。
    + Update-AzureRmServiceFabricReliability       クラスターの信頼性層を変更します。
* SQL
  - New-AzureRmSqlDatabase に -SampleName パラメーターを追加しました。
  - フェールオーバー グループのコマンドレットを更新します。
  - "Tag" パラメーターを削除します。
  - Remove-AzureRmSqlDatabaseFailoverGroup コマンドレットから "PartnerResourceGroupName" および "PartnerServerName" の各パラメーターを削除します。
  - New- および Set- のコマンドレットに 'GracePeriodWithDataLossHours' パラメーターを追加します。このパラメーターは、最終的に 'GracePeriodWithDataLossHour' に取って代わります。
  - ドキュメントが拡充および更新されました。
  - 返されるオブジェクトの書式変更と、フィールドに値が設定されないバグ (複数) の修正が行われます。
  - フェールオーバー グループ オブジェクトに 'DatabaseNames' および 'PartnerLocation' の各プロパティを追加します。
  - Switch- コマンドレットで引き起こされる、操作の完了まで待機されずに直ちに制御が戻るというバグが修正されます。
  - 大きな値の猶予期間を使用した際の整数オーバーフローのバグが修正されます。
  - 猶予期間に小さい値が指定されている場合は、最小値の 1 時間に調整されます。
  - Set-AzureRmSqlDatabaseThreatDetectionPolicy コマンドレットと Set-AzureRmSqlServerThreatDetectionPolicy コマンドレットの "ExcludedDetectionType" パラメーターの有効な値から "Usage_Anomaly" を削除します。
* Storage
  - SRP SDK が 6.3.0 にアップグレードされます。
  - New/Set-AzureRmStorageAccount: EnableHttpsTrafficOnly をサポートするように、新しいパラメーターを追加しました。
  - New/Set/Get-AzureRmStorageAccount: 返されるストレージ アカウントに新しい EnableHttpsTrafficOnly 属性が含まれます。
* Azure.Storage
  - Azure Storage クライアント ライブラリ 8.1.1 および Azure Storage データ移動ライブラリ 0.5.1 にアップグレードされます。
  - BLOB 増分コピー機能をサポートするように、新しいコマンドレットを追加しました。
