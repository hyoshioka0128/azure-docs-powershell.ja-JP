---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: e9fa2d75c1c4e6ffaa2f7dd8e400f5b13dd4527d
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110485"
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

---
## <a name="650---july-2018"></a>6.5.0 - 2018 年 7 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* "Get-AzureRmContextAutosaveSetting" のヘルプを更新しました

#### <a name="azurestorage"></a>Azure.Storage
* 書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます
- Set-AzureStorageBlobContent
- Set-AzureStorageFileContent

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* 必須プロパティ ResourceGroupName を AS に追加しました

#### <a name="azurermautomation"></a>AzureRM.Automation
* "New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました

#### <a name="azurermcompute"></a>AzureRM.Compute
* Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました
* "Add-AzureRmVmssExtension" の例を追加しました
* "Remove-AzureRmVmssExtension" の例を追加しました
* "Set-AzureRmVMAccessExtension" のヘルプを更新しました
* New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました
* Application Gateway の次のコマンドレットを更新しました
    - New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました
    - New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました
    - Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました
* 最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました

#### <a name="azurermrelay"></a>AzureRM.Relay
* マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました

#### <a name="azurermresources"></a>AzureRM.Resources
* Roleassignment および roledefinition コマンドレットを更新しました
    - ページングの一部として実行される追加の roledefinition 呼び出しを削除しました
* Get-AzureRmRoleAssignment コマンドレットを修正しました
    - -ExpandPrincipalGroups コマンド パラメーター機能を修正しました
* "-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* コマンドレットを一覧表示するために、top および skip パラメーターを追加しました
* Standard から Premium 名前空間への移行コマンドレットを追加しました
    - Start-AzureRmServiceBusMigration
    - Get-AzureRmServiceBusMigration
    - Complete-AzureRmServiceBusMigration
    - Stop-AzureRmServiceBusMigration
    - Remove-AzureRmServiceBusMigration
* レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* "New-AzureRmServiceFabricCluster" の例を更新しました

#### <a name="azurermsql"></a>AzureRM.Sql
* ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました
    - Add-AzureRmSqlServerTransparentDataEncryptionCertificate
    - Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate

#### <a name="azurermwebsites"></a>AzureRM.Websites
* `Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます
* `Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました
* `Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます

## <a name="640---july-2018"></a>6.4.0 - 2018 年 7 月
#### <a name="general"></a>全般
* ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました

#### <a name="azurermprofile"></a>AzureRM.Profile
* Ps1Xml 属性が基本的な出力の種類に追加されました

#### <a name="azurermcompute"></a>AzureRM.Compute
* VMSS の IP タグ機能
    - "New-AzureRmVmssIpTagConfig" コマンドレットが追加されました
    - IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました
* VMSS の自動 OS ロールバック機能
    - DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました
* VMSS の OS アップグレード履歴機能
    - OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* 次のコマンドでカタログ ACL に対応するようになりました。
    - Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry
    - Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry
    - Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました
* Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました
* 再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました
* DataLake コマンドレットのテストの場所を修正しました

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* 省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました
* 新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。 既定のパラメーター セットが提供されます。
* 省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました
* ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました
    - Get-AzureRmExpressRouteCrossConnection を追加しました
    - Set-AzureRmExpressRouteCrossConnection を追加しました
    - Add-AzureRmExpressRouteCrossConnectionPeering を追加しました
    - Get-AzureRmExpressRouteCrossConnectionPeering を追加しました
    - Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました
    - Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました
    - Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました
    - Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。 このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。 このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。

#### <a name="azurermresources"></a>AzureRM.Resources
* Get-AzureRmPolicyAssignment コマンドレットを更新しました。
    - 管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました
    - 管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました
    - パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました
* Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました
    - 指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました
    - 指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました
* Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました
    - 指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました
    - 指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました
* "New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました
* "New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/6505
* "Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。

#### <a name="azurermsql"></a>AzureRM.Sql
* New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました
* 複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました

## <a name="630---june-2018"></a>6.3.0 - 2018 年 6 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* Enable-AzureRmContextAutoSave のエラー メッセージを更新しました
* 以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます

#### <a name="azurestorage"></a>Azure.Storage
* -Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* "Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました 
* Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました
    - Grant-AzureRmDiskAccess
    - Grant-AzureRmSnapshotAccess
    - Save-AzureRmVMImage
* "操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。
    - Start-AzureRmVM
    - Stop-AzureRmVM
    - Restart-AzureRmVM
    - Set-AzureRmVM
    - Remove-AzuerRmVM
    - Set-AzureRmVmss
    - Start-AzureRmVmssRollingOSUpgrade
    - Stop-AzureRmVmssRollingUpgrade
    - Start-AzureRmVmss
    - Restart-AzureRmVmss
    - Stop-AzureRmVmss
    - Remove-AzureRmVmss
    - ConvertTo-AzureRmVMManagedDisk
    - Revoke-AzureRmSnapshotAccess
    - Remove-AzureRmSnapshot
    - Revoke-AzureRmDiskAccess
    - Remove-AzureRmDisk
    - Remove-AzureRmContainerService
    - Remove-AzureRmAvailabilitySet

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* Policy Insights コマンドレットのパブリック リリース
    - API バージョン 2018-04-04 を使用します
    - Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。 このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。

#### <a name="azurermsql"></a>AzureRM.Sql
* Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました

#### <a name="azurermwebsites"></a>AzureRM.Websites
* -AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました
* 省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました

## <a name="621---june-2018"></a>6.2.1 - 2018 年 6 月
### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました

## <a name="620---june-2018"></a>6.2.0 - 2018 年 6 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました

#### <a name="azurermcompute"></a>AzureRM.Compute
* VMSS VM 更新プログラムの機能
    - "Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました
    - Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。
    - ファクトリ リポジトリの構成操作を追加しました
    - expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました
    - モデルの型をいくつか SecretBase から Object に更新しました
    - BLOB イベント トリガーを追加しました

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* 出力例に関してドキュメントを更新しました

### <a name="azurermnetwork"></a>AzureRM.Network
* Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました

#### <a name="azurermresources"></a>AzureRM.Resources
* "Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました

### <a name="azurermsql"></a>AzureRM.Sql
* 省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました
    - New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。

## <a name="610---may-2018"></a>6.1.0 - 2018 年 5 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* "Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。
* ServiceFabric Backend のサポートを追加しました。
* Application Insights Logger のサポートを追加しました。
* API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。
* プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。
* KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。
* MSI ID のサポートを追加しました。
* URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。
   - Import-AzureRmApiManagementHostnameCertificate
   - New-AzureRmApiManagementHostnameConfiguration
   - Set-AzureRmApiManagementHostnames
   - Update-AzureRmApiManagementDeployment

#### <a name="azurermbatch"></a>AzureRM.Batch
* 新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。
* 新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。

#### <a name="azurermconsumption"></a>AzureRM.Consumption
* Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。
* Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。 
* Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。 

#### <a name="azurermnetwork"></a>AzureRM.Network
* Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。
* プロトコル構成を作成するコマンドレットを追加しました。
    - New-AzureRmNetworkWatcherProtocolConfiguration
* 既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。
    - Add-AzureRmExpressRouteCircuitConnectionConfig
* 既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。
    - Remove-AzureRmExpressRouteCircuitConnectionConfig
* 回路接続を取得するコマンドレットを追加しました。
    - Get-AzureRmExpressRouteCircuitConnectionConfig

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* 生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。

#### <a name="azurermsql"></a>AzureRM.Sql
* Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。
* 新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、 Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。
* 新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。
* 更新されたコマンドレットは次のとおりです。 
    - New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase
    - New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool
    - New-AzureRmSqlDatabaseCopy
    - New-AzureRmSqlDatabaseSecondary
    - Restore-AzureRmSqlDatabase

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* "Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。