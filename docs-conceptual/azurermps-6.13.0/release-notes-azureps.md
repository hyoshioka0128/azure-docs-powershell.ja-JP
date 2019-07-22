---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: eecd66ddf433cc2543ceeaef1519d69179f2f099
ms.sourcegitcommit: bbd3f061cac3417ce588487c1ae4e0bc52c11d6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "65534449"
---
# <a name="release-notes"></a>リリース ノート

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

---
## <a name="6130---november-2018"></a>6.13.0 - 2018 年 11 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* 最新バージョンの ClientRuntime を使用するように共通コードを更新しました。

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 型マッピングの問題に対応するために依存関係を更新しました

#### <a name="azurermautomation"></a>AzureRM.Automation
* Swagger ベースの Azure Automation コマンドレット
* Update Management コマンドレットを追加しました
* ソース管理コマンドレットを追加しました
* Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました
* DSC Register Node コマンドを修正しました

#### <a name="azurermcompute"></a>AzureRM.Compute
* SystemAssigned ID の ID の問題を修正しました
* 型マッピングの問題に対応するために依存関係を更新しました

#### <a name="azurermcontainerinstance"></a>AzureRM.ContainerInstance
* 型マッピングの問題に対応するために依存関係を更新しました

#### <a name="azurermmarketplaceordering"></a>AzureRM.MarketplaceOrdering
* marketplace コマンドレットの例の説明を更新しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました
* サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました
* Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました 
* VirtualNetwork マップのメモリ使用量に関する問題を修正しました

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* 保護されたファイル共有のポリシーの変更を修正しました
* ポリシーのタイムゾーンを大文字に変換しました

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました
* 型マッピングの問題に対応するために依存関係を更新しました

#### <a name="azurermrelay"></a>AzureRM.Relay
* New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります

#### <a name="azurermresources"></a>AzureRM.Resources
* `New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました
* -Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました
* NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* 今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました

#### <a name="azurermsql"></a>AzureRM.Sql
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

## <a name="6120---november-2018"></a>6.12.0 - 2018 年 11 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* 最新バージョンの ClientRuntime を使用するように共通コードを更新しました。
* Connect-AzureRmAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました
* Connect-AzureRmAccount の TenantId の説明を更新しました
* テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました
    - https://github.com/Azure/azure-powershell/issues/6936
* テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/7453
* MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/7462
* 接続されていない場合に "Disconnect-AzureRmAccount" でエラーがスローされる問題を修正しました
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a>AzureRM.Automation
* コマンドレット DLL ファイルの名前を Microsoft.Azure.Commands.Automation.dll に変更しました

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* Get-AzureRmCognitiveServicesAccountSkus 操作を追加しました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* Add-AzureRmVmssVMDataDisk および Remove-AzureRmVmssVMDataDisk コマンドレットを追加しました
* Get-AzureRmVMImage では AutomaticOSUpgradeProperties が表示されます
* SetAzureRmVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式では設定されません。

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* DataLake パッケージは 1.1.10 に更新されました。
* マルチスレッド操作に既定のコンカレンシーを追加しました。

#### <a name="azurerminsights"></a>AzureRM.Insights
* 問題 #7267 (自動スケーリングの領域) を修正しました
    - 新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。
* Set-AzureRMDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました
    - このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します

#### <a name="azurermnetwork"></a>AzureRM.Network
* 次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:
    - Get-AzureRmExpressRouteCircuitRouteTable
    - Get-AzureRmExpressRouteCircuitARPTable
    - Get-AzureRmExpressRouteCircuitRouteTableSummary
    - Get-AzureRMExpressRouteCrossConnectionArpTable
    - Get-AzureRMExpressRouteCrossConnectionRouteTable
    - Get-AzureRMExpressRouteCrossConnectionRouteTableSummary

#### <a name="azurermpolicyinsights"></a>AzureRM.PolicyInsights
* ポリシー修復コマンドレットを追加しました

#### <a name="azurermrecoveryservicesbackup"></a>AzureRM.RecoveryServices.Backup
* Recovery Services で Azure ファイル共有のサポートを追加しました。

#### <a name="azurermresources"></a>AzureRM.Resources
* [https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました
    - "Get-AzureRmResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。

#### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* Linux VMSS への証明書の追加を修正しました。
* "Add-AzureRmServiceFabricClusterCertificate" を修正しました
    - 新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。
    - 例外が正しく表示されます (Azure/service-fabric-issues#1054)。
* VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzureRmServiceFabricDurability" を修正しました。

## <a name="6110---october-2018"></a>6.11.0 - 2018 年 10 月
#### <a name="azurermprofile"></a>AzureRM.Profile
* CloudShell での Get-AzureRmSubscription に関する問題を修正しました。
* 最新バージョンの ClientRuntime を使用するように共通コードを更新しました。

#### <a name="azurermbackup"></a>AzureRM.Backup
* Azure Backup コマンドレットを非推奨にしました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* "New-AzureRmVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。
* ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。

#### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* 仮想ネットワーク規則のサポートを追加しました
    - Get-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。
    - Add-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。
    - Set-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。
    - Remove-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを削除します。

#### <a name="azurermnetwork"></a>AzureRM.Network
* プロトコル値をバックエンドに渡すように、Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新しました。
* ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。

#### <a name="azurermresources"></a>AzureRM.Resources
* シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzureRMRoleDefinition が理解できない例外をスローする問題を修正しました。 また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。

## <a name="6100---october-2018"></a>6.10.0 - 2018 年 10 月
#### <a name="azurestorage"></a>Azure.Storage
* コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました
    - Start-AzureStorageBlobCopy
    - Start-AzureStorageFileCopy

#### <a name="azurermcognitiveservices"></a>AzureRM.CognitiveServices
* 既存のアカウントなしでの Get-AzureRmCognitiveServicesAccountSkus がサポートされました。

#### <a name="azurermcompute"></a>AzureRM.Compute
* 必要に応じて 50 を超える結果が返されるように Get-AzureRmVM -ResourceGroupName <rg> を修正しました
* "SimpleParameterSet" の例を New-AzureRmVmss コマンドレットのヘルプに追加しました。
* Azure Disk Encryption の進行状況メッセージの誤りを修正しました

#### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF .Net SDK のバージョンを 2.3.0 に更新しました。

#### <a name="azurermnetwork"></a>AzureRM.Network
* NetworkProfile 機能を追加しました。 追加された新しいコマンドレットは次のとおりです
    - Get-AzureRMNetworkProfile
    - New-AzureRMNetworkProfile
    - Remove-AzureRMNetworkProfile
    - Set-AzureRMNetworkProfile
    - New-AzureRMContainerNicConfig
    - New-AzureRmContainerNicConfigIpConfig
* サブネット モデルでサービスの関連付けリンクを追加しました
* New-AzureRmVirtualNetworkTap、Get-AzureRmVirtualNetworkTap、Set-AzureRmVirtualNetworkTap、Remove-AzureRmVirtualNetworkTap の各コマンドレットを追加しました
* Set-AzureRmNEtworkInterfaceTapConfig、Get-AzureRmNEtworkInterfaceTapConfig、Remove-AzureRmNEtworkInterfaceTapConfig の各コマンドレットを追加しました

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* 今後、サイズ パラメーターとして任意の文字列を追加できます。 PSArgumentCompleter ポップアップで P5 を追加しました

#### <a name="azurermresources"></a>AzureRM.Resources
* 欠落していた -Mode パラメーターを Set-AzureRmPolicyDefinition に追加しました
* 配信元にユーザーが含まれる操作について Get-AzureRmProviderOperation コマンドレットのバグを修正しました

#### <a name="azurermsql"></a>AzureRM.Sql
* 一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました

#### <a name="azurermstorage"></a>AzureRM.Storage
* 特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。
    - Get-AzureRmStorageUsage

#### <a name="azurermwebsites"></a>AzureRM.Websites
* 新しいコマンドレット: Get-AzureRMWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します
* 新しいコマンドレット: New-AzureRMWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します

## <a name="690---september-2018"></a>6.9.0 - 2018 年 9 月
#### <a name="general"></a>全般
* AzureRM.SignalR が AzureRM ロールアップ モジュールに追加されました

#### <a name="azurermprofile"></a>AzureRM.Profile
* ストレージの一般的なコードに対する軽微な変更
* 完全なパラメーター型を含めるようにヘルプ ファイルを更新しました。
* ServicePrincipalCertificateWithSubscriptionId パラメーター セットの -ServicePrincipal を "任意" に変更しました 

#### <a name="azurestorage"></a>Azure.Storage
* OAuth でのストレージ コンテキストの作成がサポートされました。 
    - New-AzureStorageContext

#### <a name="azurermcdn"></a>AzureRM.Cdn
* CDN 価格 SKU に Standard_Microsoft を追加しました。 

#### <a name="azurermcompute"></a>AzureRM.Compute
* Keyvault および Storage への依存関係を一般的な依存関係に移動しました
* より多くの仮想マシンのサイズのサポートを AEM コマンドレットに追加しました
* PublicIPPrefix パラメーターを New-AzureRmVmssIpConfig に追加しました
* ResourceId パラメーターを Invoke-AzureRmVMRunCommand コマンドレットに追加しました
* Invoke-AzureRmVmssVMRunCommand コマンドレットを追加しました

#### <a name="azurermdns"></a>AzureRM.Dns
* DNS レコード作成中のエイリアス レコードのサポートを追加しました

#### <a name="azurerminsights"></a>AzureRM.Insights
* #6833 および #7102 の問題を修正しました (診断設定領域)
    - 診断設定の作成および表示/取得中の既定の名前 ("service") に関する問題
    - カテゴリでの診断設定の作成に関する問題
* メトリック時間グレイン パラメーターの非推奨メッセージを追加しました
    - Timegrains パラメーターは引き続き利用できますが (これは破壊的変更ではありません)、PT1M のみが有効であるため、バックエンドでは無視されます

#### <a name="azurermnetwork"></a>AzureRM.Network
* LoadBalancer コマンドレットへの変更
  - LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes パラメーター、EnableFloatingIp パラメーター、EnableTcpReset パラメーターを追加しました
  - LoadBalancerInboundNatRuleConfig: EnableTcpReset パラメーターを追加しました
  - LoadBalancerRuleConfig: EnableTcpReset パラメーターを追加しました
  - LoadBalancerProbeConfig: Protocol パラメーターの "HTTPS" 値のサポートを追加しました
* 新しい LoadBalancer のサブリソース OutboundRule について新しいコマンドを追加しました
  - Add-AzureRmLoadBalancerOutboundRuleConfig
  - Get-AzureRmLoadBalancerOutboundRuleConfig
  - New-AzureRmLoadBalancerOutboundRuleConfig
  - Set-AzureRmLoadBalancerOutboundRuleConfig
  - Remove-AzureRmLoadBalancerOutboundRuleConfig
* PSNetworkInterface の新しい HostedWorkloads プロパティを追加しました
* 次の機能のために新しいコマンドレットを追加しました: Azure Firewall (ARM を介して)
  - Get-AzureRmFirewall を追加しました
  - Set-AzureRmFirewall を追加しました
  - New-AzureRmFirewall を追加しました
  - Remove-AzureRmFirewall を追加しました
  - New-AzureRmFirewallApplicationRuleCollection を追加しました
  - New-AzureRmFirewallApplicationRule を追加しました
  - New-AzureRmFirewallNatRuleCollection を追加しました
  - New-AzureRmFirewallNatRule を追加しました
  - New-AzureRmFirewallNetworkRuleCollection を追加しました
  - New-AzureRmFirewallNetworkRule を追加しました
* Application Gateway での信頼されたルート証明書と自動スケーリング構成のサポートを追加しました
  - 追加された新しいコマンドレット:
      - Add-AzureRmApplicationGatewayTrustedRootCertificate
      - Get-AzureRmApplicationGatewayTrustedRootCertificate
      - New-AzureRmApplicationGatewayTrustedRootCertificate
      - Remove-AzureRmApplicationGatewayTrustedRootCertificate
      - Set-AzureRmApplicationGatewayTrustedRootCertificate
      - Get-AzureRmApplicationGatewayAutoscaleConfiguration
      - New-AzureRmApplicationGatewayAutoscaleConfiguration
      - Remove-AzureRmApplicationGatewayAutoscaleConfiguration
      - Set-AzureRmApplicationGatewayAutoscaleConfiguration
  - 省略可能なパラメーターで更新されたコマンドレット -TrustedRootCertificate
      - New-AzureRmApplicationGateway
      - Set-AzureRmApplicationGateway
      - New-AzureRmApplicationGatewayBackendHttpSetting
      - Set-AzureRmApplicationGatewayBackendHttpSetting
  - 省略可能なパラメーターで更新されたコマンドレット - AutoscaleConfiguration
      - New-AzureRmApplicationGateway
      - Set-AzureRmApplicationGateway
* インターフェイス エンドポイントのコマンドレット Get-AzureInterfaceEndpoint を追加しました
* サブネットでの複数のアドレス プレフィックスのサポートを追加しました。 更新されたコマンドレット:
  - New-AzureRmVirtualNetworkSubnetConfig
  - Set-AzureRmVirtualNetworkSubnetConfig
  - Add-AzureRmVirtualNetworkSubnetConfig
  - Get-AzureRmVirtualNetworkSubnetConfig
  - Add-AzureRmApplicationGatewayAuthenticationCertificate
  - Add-AzureRmApplicationGatewayFrontendIPConfig
  - New-AzureRmApplicationGatewayFrontendIPConfig
  - Set-AzureRmApplicationGatewayFrontendIPConfig
  - Add-AzureRmApplicationGatewayIPConfiguration
  - New-AzureRmApplicationGatewayIPConfiguration
  - Set-AzureRmApplicationGatewayIPConfiguration
  - Add-AzureRmNetworkInterfaceIpConfig
  - New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig
  - New-AzureRmVirtualNetworkGatewayIpConfig
  - Add-AzureRmVirtualNetworkGatewayIpConfig
  - Set-AzureRmLoadBalancerFrontendIpConfig
  - Add-AzureRmLoadBalancerFrontendIpConfig
  - New-AzureRmLoadBalancerFrontendIpConfig
  - New-AzureRmNetworkInterface
* サブネット委任のコマンドレットを追加しました。
  - New-AzureRmDelegation: 新しい委任を作成します。これはサブネットに追加できます
  - Remove-AzureRmDelegation: サブネットを受け取り、指定された委任の名前をそのサブネットから削除します
  - Add-AzureRmDelegation: サブネットを受け取り、指定されたサービス名を委任としてそのサブネットに追加します
  - Get-AzureRmDelegation
  - Get-AzureRmAvailableServiceDelegations

#### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* 管理対象のマネージド ディスクのサポート

#### <a name="azurermrediscache"></a>AzureRM.RedisCache
* Insights の依存関係を更新しました。

#### <a name="azurermresources"></a>AzureRM.Resources
* New-AzureRmResourceGroupDeployment を新しい RollbackAction パラメーターで更新しました
    - 新しいパラメーターを使用して OnErrorDeployment のサポートを追加しました。
* ポリシー割り当てでマネージド ID をサポートします。
* "New-AzureRmPolicyAssignment" を指定してポリシーを割り当てるとき、既定値を持つパラメーターが不要になりました
* ポリシー エイリアスを取得するための新しい Get AzureRmPolicyAlias コマンドレットを追加しました

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 問題 #7161 を修正しました

#### <a name="azurermsignalr"></a>AzureRM.SignalR
* SKU 名を Free_F1 および Standard_S1 に更新しました
* バージョン フィールドを PSSignalRResource オブジェクトに、接続文字列を PSSignalRKeys オブジェクトに追加しました。

#### <a name="azurermstorage"></a>AzureRM.Storage
* AzureRm.Storage での不変ポリシーをサポートします 
    - Remove-AzureRmStorageAccountNetworkRule
    - Get-AzureRmStorageContainer
    - Update-AzureRmStorageContainer
    - New-AzureRmStorageContainer
    - Remove-AzureRmStorageContainer
    - Add-AzureRmStorageContainerLegalHold
    - Remove-AzureRmStorageContainerLegalHold
    - Set-AzureRmStorageContainerImmutabilityPolicy
    - Get-AzureRmStorageContainerImmutabilityPolicy
    - Remove-AzureRmStorageContainerImmutabilityPolicy
    - Lock-AzureRmStorageContainerImmutabilityPolicy

#### <a name="azurermwebsites"></a>AzureRM.Websites
* 追加された 2 つの新しいコマンドレット: Get-AzureRmDeletedWebApp および Restore-AzureRmDeletedWebApp
* Windows コンテナーでの App Service プランの作成用に New-AzureRmAppServicePlan -HyperV スイッチが追加されました
* Windows コンテナー アプリを作成および管理用に、New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New パラメーター (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) が追加されました

## <a name="681---august-2018"></a>6.8.1 - 2018 年 8 月
#### <a name="general"></a>全般
* 既定のリソース グループが設定されていないという問題を修正しました。
* 共通ランタイム アセンブリを更新しました

#### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 既定のリソース グループが設定されていないという問題を修正しました。
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6603
    - Import-AzureRmApiManagementApi コマンドレットおよび *-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6879
    - CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。 4\.0.4-preview NuGet へのアップグレードによって修正しました
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6853
    - 製品を名前で検索するための Odata フィルターを修正しました
* 修正された問題 https://github.com/Azure/azure-powershell/issues/6814
    - API を名前で検索するための Odata フィルターを修正しました
* AzureMonitor ロガーのサポートを追加しました


#### <a name="azurermcompute"></a>AzureRM.Compute
* エラー出力にターゲットが見つからない問題を修正しました。
* マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました
* 既定のリソース グループが設定されていないという問題を修正しました。
* Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* コマンドレット出力の既定の表示をテーブル ビューに変更しました

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* 一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました


#### <a name="azurermresources"></a>AzureRM.Resources
* Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 修正された問題
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* 複数値ルーティング方式のサポートを追加しました
    - 複数値ルーティング用の新しい "MaxReturn" パラメーター
* サブネット ルーティング方式のサポートを追加しました
    - エンドポイントでの IP アドレス範囲 (サブネット) のサポート
* プロファイルでのカスタム ヘッダーのサポートを追加しました
* プロファイルでの予期される状態コード範囲のサポートを追加しました
* エンドポイントでのカスタム ヘッダーのサポートを追加しました

## <a name="680---august-2018"></a>6.8.0 - 2018 年 8 月
#### <a name="general"></a>全般
* 既定のリソース グループが設定されていないという問題を修正しました。

#### <a name="azurermprofile"></a>AzureRM.Profile
* Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました

#### <a name="azurermcompute"></a>AzureRM.Compute
* エラー出力にターゲットが見つからない問題を修正しました。
* マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました
* Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました

#### <a name="azurermiothub"></a>AzureRM.IotHub
* New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました

#### <a name="azurermnetwork"></a>AzureRM.Network
* 既定のモデルの表示をテーブル ビューに変更しました

#### <a name="azurermpowerbiembedded"></a>AzureRM.PowerBIEmbedded
* 一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました

#### <a name="azurermresources"></a>AzureRM.Resources
* Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。

#### <a name="azurermservicebus"></a>AzureRM.ServiceBus
* 問題の修正
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a>AzureRM.TrafficManager
* 複数値ルーティング方式のサポート
    - 複数値ルーティング用の新しい "MaxReturn" パラメーター
* サブネット ルーティング方式のサポート
    - エンドポイントでの IP アドレス範囲 (サブネット) のサポート
* プロファイルでのカスタム ヘッダーのサポート
* プロファイルでの予期される状態コード範囲のサポート
* エンドポイントでのカスタム ヘッダーのサポート

#### <a name="azurermwebsites"></a>AzureRM.Websites
* 既定のリソース グループが間違って設定されているという問題を修正しました。

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
* Set-AzureStorageShareQuota

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
* サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました  (ResouceGroupName パラメーターは省略可能になりました)。
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
* Set-AzureStorageBlobContent
* Set-AzureStorageFileContent

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
* 次の機能のために新しいコマンドを追加しました: ExpressRoute Partner API (ARM を介して)
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
* URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です
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
