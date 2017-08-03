---
title: "Azure PowerShell の変更履歴 | Microsoft Docs"
description: "Azure PowerShell の最新リリースで行われた変更の履歴です。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 07/26/2017
ms.openlocfilehash: cc2fe75f498f9043e5a4b632c144877af0143173
ms.sourcegitcommit: 20bcef86db4e4869125bb63085fcffd009c19280
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="20170717---version-421"></a>2017.07.17 - バージョン 4.2.1
* コンピューティング
    - VM ディスクおよび VM ディスク スナップショットの作成および更新コマンドレットに関する問題が修正されます (リンク)[https://github.com/azure/azure-powershell/issues/4309]
      - New-AzureRmDisk
      - New-AzureRmSnapshot
      - Update-AzureRmDisk
      - Update-AzureRmSnapshot
* プロファイル
    - RDFE の非対話型ユーザー認証に関する問題が修正されます (リンク)[https://github.com/Azure/azure-powershell/issues/4299]
* サービス管理
    - 非対話型ユーザー認証に関する問題が修正されます (リンク)[https://github.com/Azure/azure-powershell/issues/4299]

## <a name="2017711---version-420"></a>2017.7.11 - バージョン 4.2.0
* AnalysisServices
    * 新しいデータ プレーン API が追加されます。
        - AS サーバー ログ、Export-AzureAnalysisServicesInstanceLog をフェッチする API を導入しました。
* Automation
    * New-AzureRmAutomationSchedule の週ごとおよび月ごとのスケジュールの TimeZone 値を適切に設定
        - この問題について詳しくは、https://github.com/Azure/azure-powershell/issues/3043 をご覧ください。
* AzureBatch
    - 新しい Get-AzureBatchJobPreparationAndReleaseTaskStatus コマンドレットを追加しました。
    - バイト範囲の開始と終了を Get-AzureBatchNodeFileContent パラメーターに追加しました。
* CognitiveServices
    * Cognitive Services Management SDK バージョン 1.0.0 と統合します。
    * アカウント名の長さチェックのバグを修正します。
* コンピューティング
    * イメージ ディスクでのストレージ アカウントの種類のサポート:
        - 'StorageAccountType' パラメーターが Set-AzureRmImageOsDisk および Add-AzureRmImageDataDisk に追加されました
    * Vmss Ip 構成での PrivateIP および PublicIP 機能:
        - 'PrivateIPAddressVersion'、'PublicIPAddressConfigurationName'、'PublicIPAddressConfigurationIdleTimeoutInMinutes'、および 'DnsSetting' 名が New-AzureRmVmssIpConfig に追加されました
        - IPv4 または IPv6 を指定するための 'PrivateIPAddressVersion' パラメーターが New-AzureRmVmssIpConfig に追加されました
    * パフォーマンス メンテナンス機能:
        - 'PerformMaintenance' スイッチ パラメーターが Restart-AzureRmVM に追加されました。
        - Get-AzureRmVM - 状態に、特定の VM のパフォーマンス メンテナンスの情報が示されます
    * 仮想マシン ID 機能:
        - 'IdentityType' パラメーターが New-AzureRmVMConfig および UpdateAzureRmVM に追加されました
        - Get-AzureRmVM に特定の VM の ID 情報が表示されます
    * Vmss ID 機能:
        - 'IdentityType' パラメーターが New-AzureRmVmssConfig に追加されました
        - Get-AzureRmVmss に特定の Vmss の ID 情報が表示されます
    * Vmss ブート診断機能:
        - Vmss オブジェクトのブート診断を設定するための新しいコマンドレット: Set-AzureRmVmssBootDiagnostics
        - 'BootDiagnostic' パラメーターが New-AzureRmVmssConfig に追加されました
    * Vmss LicenseType 機能:
        - 'LicenseType' パラメーターが New-AzureRmVmssConfig に追加されました
    * RecoveryPolicyMode サポート:
        - 'RecoveryPolicyMode' パラメーターが New-AzureRmVmssConfig に追加されました
    * Compute Resource SKU 機能:
        - 新しいコマンドレット 'Get-AzureRmComputeResourceSku' により、すべてのコンピューティング リソース SKU が表示されます
* DataFactories
    * New-AzureRmDataFactoryGatewayKey が非推奨になりました
    * New-AzureRmDataFactoryGatewayAuthKey および Get-AzureRmDataFactoryGatewayAuthKey の追加によりゲートウェイ認証キー機能を導入します
* DataLakeAnalytics
    * 次のコマンドによるコンピューティング ポリシー CRUD に対応しました。
        - New-AzureRMDataLakeAnalyticsComputePolicy
        - Get-AzureRMDataLakeAnalyticsComputePolicy
        - Remove-AzureRMDataLakeAnalyticsComputePolicy
        - Update-AzureRMDataLakeAnalyticsComputePolicy
    * 繰り返し発生するジョブとジョブ パイプラインをサポートするジョブ リレーションシップ メタデータに対応しました。 次のコマンドを更新または追加しました。
        - Submit-AzureRMDataLakeAnalyticsJob
        - Get-AzureRMDataLakeAnalyticsJob
        - Get-AzureRMDataLakeAnalyticsJobRecurrence
        - Get-AzureRMDataLakeAnalyticsJobPipeline
    * Azure Resource 対象ユーザーではなく、正しい Data Lake 固有の対象ユーザーを使用するようにジョブおよびカタログ API のトークン対象ユーザーを更新しました。
* DataLakeStore
    * Set-AzureRMDataLakeStoreAccount コマンドレットでユーザー管理型 KeyVault キーの交換のサポートを追加しました。
    * ユーザー管理型 KeyVault が追加されたとき、またはキーが交換されたときに `enableKeyVault` 呼び出しを自動的にトリガーするよう QOL (生活の質) の更新を追加しました。
    * Azure Resource 対象ユーザーではなく、正しい Data Lake 固有の対象ユーザーを使用するようにジョブおよびカタログ API のトークン対象ユーザーを更新しました。
    * 次のコマンドレットを使用して作成または追加されるファイルのサイズを制限するバグを修正しました。
        - New-AzureRmDataLakeStoreItem
        - Add-AzureRmDataLakeStoreItemContent
* DNS
    * Get-AzureRmDnsZone のパイプ処理シナリオでのバグを修正します。
        - 詳しくは、https://github.com/Azure/azure-powershell/issues/4203 をご覧ください。
* HDInsight
    * Operations Management Suite (OMS) の有効化/無効化のサポートを追加しました。
    * 新しいコマンドレット
        - Enable-AzureRmHDInsightOperationsManagementSuite
        - Disable-AzureRmHDInsightOperationsManagementSuite
        - Get-AzureRmHDInsightOperationsManagementSuite
    * Spark カスタム構成を Add-AzureRmHDInsightConfigValues に設定する新しいパラメーターを追加します。
        - Spark 1.6 向けのパラメーター SparkDefaults と SparkThriftConf
        - Spark 2.0 向けのパラメーター Spark2Defaults と Spark2ThriftConf
* 洞察
    * 問題 #4215 (変更要求) により、Get-AzureRmLog コマンドレットの時間枠の 15 日間という制限が削除されます。 また、単体テスト名がわずかに変更されます。
    * 問題 #3957: Get-AzureRmLog の問題が修正されました。
        - 問題 #1: バックエンドが、継続トークンによって次ページにリンクされ、200 レコードごとのページでレコードを返す。 それ以上のレコードがあるはずのところ、コマンドレットで 200 レコードしか返されませんでした。 これは、MaxEvents に設定した値に関係なく発生していました (その値が 200 未満である場合を除く)。
        - 問題 #2: ドキュメントにこのコマンドレットに関する正しくないデータが含まれていた (既定の時間枠が 1 時間など)。
        - #1 の修正: コマンドレットは、MaxEvents またはセットの末尾に到達するまで、バックエンドによって返された継続トークンに続くようになりました。<br>MaxEvents の既定値は 1000 で、その最大値は 100000 です。 MaxEvents の 1 未満の値はすべて無視され、代わりに既定値が使用されます。 これらの値と動作は以前と同じですが、これらを正確に文書化しました。<br>MaxEvents の別名、MaxRecords が追加されました。コマンドレットの名前はイベントを示さなくなり、ログのみを示すようになりました。
        - #2 の修正: ドキュメント内の情報が正確かつより詳細になりました (新しい別名、正確な時間枠、正確な既定値、最小値、および最大値)。
* KeyVault
    * -UserPrincipalName が Set-AzureRMKeyVaultAccessPolicy および Remove-AzureRMKeyVaultAccessPolicy コマンドレットに指定されているときにディレクトリ クエリからメール アドレスを削除します。
      - いずれのコマンドレットも -EmailAddress パラメーターを指定するようになりました。このパラメーターは、メール アドレスのクエリ実行時に -UserPrincipalName パラメーターの代わりに使用できます。  ディレクトリに一致するメール アドレスが複数ある場合、コマンドレットは失敗します。
* ネットワーク
    * New-AzureRmIpsecPolicy: SALifeTimeSeconds および SADataSizeKilobytes は必須のパラメーターではなくなりました。
        - SALifeTimeSeconds の既定値は 27000 秒です。
        - SADataSizeKilobytes の既定値は 102400000 KB です。
    * ssl ポリシーを使用し、Application Gateway のすべての ssl オプション api を一覧表示するカスタム暗号スイートの構成のサポートを追加しました。
        - 省略可能なパラメーター -PolicyType、-PolicyName、-MinProtocolVersion、-Ciphersuite を追加しました。
            - Add-AzureRmApplicationGatewaySslPolicy
            - New-AzureRmApplicationGatewaySslPolicy
            - Set-AzureRmApplicationGatewaySslPolicy
        - Get-AzureRmApplicationGatewayAvailableSslOptions (別名: List-AzureRmApplicationGatewayAvailableSslOptions) を追加しました。
        - Get-AzureRmApplicationGatewaySslPredefinedPolicy (別名: List-AzureRmApplicationGatewaySslPredefinedPolicy) を追加しました。
    * Application Gateway でのリダイレクト サポートを追加しました。
        - Add-AzureRmApplicationGatewayRedirectConfiguration を追加しました。
        - Get-AzureRmApplicationGatewayRedirectConfiguration を追加しました。
        - New-AzureRmApplicationGatewayRedirectConfiguration を追加しました。
        - Remove-AzureRmApplicationGatewayRedirectConfiguration を追加しました。
        - Set-AzureRmApplicationGatewayRedirectConfiguration を追加しました。
        - 省略可能なパラメーター、-RedirectConfiguration を追加しました。
            - Add-AzureRmApplicationGatewayRequestRoutingRule
            - New-AzureRmApplicationGatewayRequestRoutingRule
            - Set-AzureRmApplicationGatewayRequestRoutingRule
        - 省略可能なパラメーター、-DefaultRedirectConfiguration を追加しました。
            - Add-AzureRmApplicationGatewayUrlPathMapConfig
            - New-AzureRmApplicationGatewayUrlPathMapConfig
            - Set-AzureRmApplicationGatewayUrlPathMapConfig
        - 省略可能なパラメーター、-RedirectConfiguration を追加しました。
            - Add-AzureRmApplicationGatewayPathRuleConfig
            - New-AzureRmApplicationGatewayPathRuleConfig
            - Set-AzureRmApplicationGatewayPathRuleConfig
        - 省略可能なパラメーター、-RedirectConfigurations を追加しました。
            - New-AzureRmApplicationGateway
            - Set-AzureRmApplicationGateway
    * Application Gateway での Azure Websites のサポートを追加しました。
        - New-AzureRmApplicationGatewayProbeHealthResponseMatch を追加しました。
        - 省略可能なパラメーター、-PickHostNameFromBackendHttpSettings、-MinServers、-Match を追加しました。
            - Add-AzureRmApplicationGatewayProbeConfig
            - New-AzureRmApplicationGatewayProbeConfig
            - Set-AzureRmApplicationGatewayProbeConfig
        - 省略可能なパラメーター、-PickHostNameFromBackendAddress、-AffinityCookieName、-ProbeEnabled、-Path を追加しました。
            - Add-AzureRmApplicationGatewayBackendHttpSettings
            - New-AzureRmApplicationGatewayBackendHttpSettings
            - Set-AzureRmApplicationGatewayBackendHttpSettings
    * VM スケール セットを使用して作成される publicipaddress リソースを取得するように Get-AzureRmPublicIPaddress を更新します。
    * 仮想ネットワークの現在の使用量を取得するコマンドレットを追加しました。
        - Get-AzureRmVirtualNetworkUsageList
* プロファイル
    * Import-AzureRmContext または Save-AzureRmContext 使用時のエラーを修正しました。
        - この問題について詳しくは、https://github.com/Azure/azure-powershell/issues/3954 をご覧ください。
* RecoveryServices.SiteRecovery
    * Azure Site Recovery 操作用の新しいモジュールを導入します。
        - すべてのコマンドレットが AzureRmRecoveryServicesAsr* で始まります。
* SQL
    * データ同期 PowerShell コマンドレットを AzureRM.Sql に追加します。
    * サーバーの作成時にタイムアウトを回避する新しい REST API バージョンを使用するように AzureRmSqlServer コマンドレットを更新しました。
    * サーバーの旧バージョン (2.0) がなくなったため、サーバーのアップグレード コマンドレットは非推奨になりました。
    * 新しい省略可能なスイッチ パラメーター AssignIdentity を New-AzureRmSqlServer および Set-AzureRmSqlServer コマンドレットに追加して、SQL サーバー リソース用のリソース ID のプロビジョニングに対応します。
    * パラメーター ResourceGroupName が Get-AzureRmSqlServer で省略できるようになりました。
        - 詳しくは、https://github.com/Azure/azure-powershell/issues/635 をご覧ください。
* ServiceManagement   ExpressRoute の場合:
    * New-AzureBgpPeering コマンドレットに次の新しいオプションが追加されました。
        - PeerAddressType: "IPv4" または "IPv6" の値を指定して、対応するアドレス ファミリの種類の BGP ピアリングを作成できます。
    * Set-AzureBgpPeering コマンドレットに次の新しいオプションが追加されました。
        - PeerAddressType: "IPv4" または "IPv6" の値を指定して、対応するアドレス ファミリの種類の BGP ピアリングを更新できます。
    * Remove-AzureBgpPeering コマンドレットに次の新しいオプションが追加されました。
        - PeerAddressType: "IPv4"、"IPv6"、または "すべて" の値を指定して、対応するアドレス ファミリの種類またはこれらすべての BGP ピアリングを削除できます。

## <a name="20170607---version-410"></a>2017.06.07 - バージョン 4.1.0
* AnalysisServices
    * 新しい SKU が追加されました: B1、B2、S0
    * スケールアップ/スケールダウンのサポートが追加されました。
* CognitiveServices
    * Cognitive Services リソースの作成時のライセンス契約の詳細表示が更新されます。
* コンピューティング
    * 複数の管理ディスクを使用した仮想マシン用の Test-AzureRmVMAEMExtension が修正されます。
    * Set-AzureRmVMAEMExtension を更新しました。Premium 管理ディスクのキャッシュ情報が追加されます。
    * Add-AzureRmVhd: vhd のサイズ制限が 4TB に増えます。
    * Stop-AzureRmVM: STayProvisioned パラメーターのドキュメントをわかりやすくします。
    * New-AzureRmDiskUpdateConfig
      * パラメーター CreateOption、StorageAccountId、ImageReference、SourceUri、SourceResourceId は非推奨になりました。
    * Set-AzureRmDiskUpdateImageReference: コマンドレットが非推奨になりました。
    * New-AzureRmSnapshotUpdateConfig
      * パラメーター CreateOption、StorageAccountId、ImageReference、SourceUri、SourceResourceId は非推奨になりました。
    * Set-AzureRmSnapshotUpdateImageReference: コマンドレットが非推奨になりました。
* DataLakeStore
    * Enable-AzureRmDataLakeStoreKeyVault (Enable-AdlStoreKeyVault)
      * DataLake ストア用に KeyVault 管理型暗号化を有効にします。
* DevTestLabs
    * 現在の、または更新された DevTest Labs API バージョンを操作するようにコマンドレットを更新します。
* IotHub
    * IoTHub コマンドレットのルーティングのサポートを追加します。
* KeyVault
  * KeyVault 管理ストレージ アカウント キーをサポートする新しいコマンドレット
    * Get-AzureKeyVaultManagedStorageAccount
    * Add-AzureKeyVaultManagedStorageAccount
    * Remove-AzureKeyVaultManagedStorageAccount
    * Update-AzureKeyVaultManagedStorageAccount
    * Update-AzureKeyVaultManagedStorageAccountKey
    * Get-AzureKeyVaultManagedStorageSasDefinition
    * Set-AzureKeyVaultManagedStorageSasDefinition
    * Remove-AzureKeyVaultManagedStorageSasDefinition
* ネットワーク
    * Get-AzureRmNetworkUsage: ネットワークの使用量と容量の詳細を表示する新しいコマンドレット
    * VirtualNetworkGateways 用の新しい GatewaySku オプションを追加しました。
        * VpnGw1、VpnGw2、VpnGw3 は Vpn ゲートウェイ用に追加された新しい SKU です。
    * Set-AzureRmNetworkWatcherConfigFlowLog
      * ヘルプの例を修正しました。
* NotificationHubs
    * 新しい API 用の NotificationHubs コマンドレットの透過的な更新
* プロファイル
    * Resolve-AzureRmError
      * サーバー要求/応答データを含む、コマンドレットによってスローされるエラーと例外の詳細を表示する新しいコマンドレット
    * Send-Feedback
      * ログインなしのフィードバックの送信を有効にしました。
    * Get-AzureRmSubscription
      * CSP サブスクリプションの取得のバグを修正します。
* リソース
    * roleassignments の数が 1000 を超えた場合に Get-AzureRMRoleAssignment が正しくない要求になる問題を修正しました。
        * 返される roleassignments の数が 1000 を超えた場合でも Get-AzureRMRoleAssignment を使用できるようになりました。
* SQL
    * Restore-AzureRmSqlDatabase: ドキュメントの例を更新しました。
* Storage
    * リソース モード ストレージ アカウント コマンドレットに AssignIdentity 設定のサポートを追加します。
        * New-AzureRmStorageAccount
        * Set-AzureRmStorageAccount
    * リソース モード ストレージ アカウント コマンドレットに顧客キーのサポートを追加します。
        * Set-AzureRmStorageAccount
        * New-AzureRmStorageAccountEncryptionKeySource
* TrafficManager

    * 新しいモニター設定 'MonitorIntervalInSeconds'、'MonitorTimeoutInSeconds'、'MonitorToleratedNumberOfFailures'
    * 新しいモニター プロトコル 'TCP'
* サービス管理
    * Add-AzureVhd: vhd のサイズ制限が 4TB に増えます。
    * New-AzureBGPPeering: LegacyMode に対応しました。
* Azure.Storage
    * ワイルドカード文字を許可し、種類 StorageContext を更新するパラメーターのヘルプを更新します。

## <a name="20170523---version-402"></a>2017.05.23 - バージョン 4.0.2
* プロファイル
    * Add-AzureRmAccount
      * AzureRM.profile の 2.x バージョンとの下位互換性のために `-EnvironmentName` パラメーター エイリアスを追加しました。

## <a name="20170512---version-401"></a>2017.05.12 - バージョン 4.0.1
 * オフライン シナリオの New-AzureStorageContext に関する問題を修正しました: https://github.com/Azure/azure-powershell/issues/3939

## <a name="20170510---version-400"></a>2017.05.10 - バージョン 4.0.0


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
