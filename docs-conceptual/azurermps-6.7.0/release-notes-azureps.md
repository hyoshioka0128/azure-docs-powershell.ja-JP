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
ms.openlocfilehash: 2a6e20137f12ae9317c7eeed330a2433774e1ea9
ms.sourcegitcommit: f648ac92fafb16cc0e9ca6bc85d00fa327baf396
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/28/2018
ms.locfileid: "43018533"
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

---
## <a name="670---august-2018"></a>6.7.0 - 2018 年 8 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* Azure ClientRuntime の最新バージョンに更新しました。
* コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました
    - https://github.com/Azure/azure-powershell/issues/6489
* コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました
* "Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a>Azure.Storage
* Azure ファイル共有のクォータについて 5 TB の制限を削除しました
- Set-AzureStorageShareQuota

#### <a name="azurermanalysisservices"></a>AzureRM.AnalysisServices
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azureanalysisservices"></a>Azure.AnalysisServices
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermapplicationinsights"></a>AzureRM.ApplicationInsights
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermautomation"></a>AzureRM.Automation
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermbackup"></a>AzureRM.Backup
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermbatch"></a>AzureRM.Batch
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermbilling"></a>AzureRM.Billing
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermcdn"></a>AzureRM.Cdn
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* Azure ClientRuntime の最新バージョンに更新しました。
* EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました
* 場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。
* Save-AzureRmVMImage のパラメーターの説明を修正しました
* 単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました

#### <a name="azurermconsumption"></a>AzureRM.Consumption
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermcontainerregistry"></a>AzureRM.ContainerRegistry
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました
* Set-AzureRmDataLakeStoreItemAcl の例を更新しました
* Azure ClientRuntime の最新バージョンに更新しました。
* Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました

#### <a name="azurermdevtestlabs"></a>AzureRM.DevTestLabs
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermdns"></a>AzureRM.Dns
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermeventgrid"></a>AzureRM.EventGrid
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermhdinsight"></a>AzureRM.HDInsight
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurerminsights"></a>AzureRM.Insights
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermiothub"></a>AzureRM.IotHub
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermlogicapp"></a>AzureRM.LogicApp
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermmachinelearningcompute"></a>AzureRM.MachineLearningCompute
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermmarketplaceordering"></a>AzureRM.MarketplaceOrdering
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermmedia"></a>AzureRM.Media
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermnetwork"></a>AzureRM.Network
* Set-AzureRmLocalNetworkGateway の例を追加しました
* Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました
* Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました
* Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました
* Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました
* Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました
* 最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました
* 存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました

#### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermrecoveryservices"></a>AzureRM.RecoveryServices
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。 指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。
* Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。
* Azure ClientRuntime の最新バージョンに更新しました。
* TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。 マネージド ディスクの復元先となるリソース グループ。 マネージド ディスクを含む VM のバックアップに適用されます。

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermrelay"></a>AzureRM.Relay
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermresources"></a>AzureRM.Resources
* サブスクリプション スコープでテンプレートのデプロイをサポートします。 新しいコマンドレットを追加しました。
    - New-AzureRmDeployment
    - Get-AzureRmDeployment
    - Test-AzureRmDeployment
    - Remove-AzureRmDeployment
    - Stop-AzureRmDeployment
    - Save-AzureRmDeploymentTemplate
    - Get-AzureRmDeploymentOperation
* コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/5705
* New-AzureRmResourceGroupDeployment の例を修正しました
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermscheduler"></a>AzureRM.Scheduler
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermsql"></a>AzureRM.Sql
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermstorage"></a>AzureRM.Storage
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermstreamanalytics"></a>AzureRM.StreamAnalytics
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermtags"></a>AzureRM.Tags
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermusageaggregates"></a>AzureRM.UsageAggregates
* Azure ClientRuntime の最新バージョンに更新しました。

#### <a name="azurermwebsites"></a>AzureRM.Websites
* Azure ClientRuntime の最新バージョンに更新しました。

## <a name="660---july-2018"></a>6.6.0 - 2018 年 7 月
#### <a name="general"></a>全般
* 完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。

#### <a name="azurermprofile"></a>AzureRM.Profile
* リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。
* Common.Storage に ps1xml の種類を追加しました

#### <a name="azurestorage"></a>Azure.Storage
* DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました
* Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6370
    - PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6515
    - エンコードの種類でオーバーロードされないように File.Save のバグを修正しました
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6560
    - Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました

#### <a name="azurermcompute"></a>AzureRM.Compute
* New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。
* Invoke-AzureRmVMRunCommand コマンドレットを修正しました
* サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました   (ResouceGroupName パラメーターは省略可能になりました)。
* 条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。
* ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。
* New-AzureRmDisk の例を更新しました
* "New-AzureRmVM" の例を追加しました
* Set-AzureRmVMOSDisk の説明を更新しました
* スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。 

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF .NET SDK のバージョンを 1.1.0 に更新しました。
* データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。
     - 新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。
     - 新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました

#### <a name="azurermeventhub"></a>AzureRM.EventHub
* 削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました

#### <a name="azurerminsights"></a>AzureRM.Insights
* ヘルプ ファイルの OutputType のフォーマットを修正しました
* Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します

#### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。

#### <a name="azurermresources"></a>AzureRM.Resources
* "Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/6765
* "Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました
* いくつかの問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a>AzureRM.Sql
* 次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。
    - Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy
* 次のコマンドレットで脆弱性評価のサポートを追加しました。
    - Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings
    - Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline
    - Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan
* Remove-AzureRmSqlServerFirewallRule の例を修正しました
* Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました

#### <a name="azurermstorage"></a>AzureRM.Storage
* Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました
* StorageAccount コマンドレットの出力をテーブル ビューで表示します
    - Get-AzureRmStorageAccount
    - New-AzureRmStorageAccount
    - Set-AzureRmStorageAccount

#### <a name="azurermtags"></a>AzureRM.Tags
* Tag コマンドレットのヘルプから間違ったステートメントを削除しました
    - https://github.com/Azure/azure-powershell/issues/3878

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
