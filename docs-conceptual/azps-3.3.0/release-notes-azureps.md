---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/15/2019
ms.openlocfilehash: fb934ed0f8bef5e2aff715debe5d406d54abf24f
ms.sourcegitcommit: 2d0c3ffaa5246f680784fa7e15b0d2536c27ff80
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/07/2020
ms.locfileid: "75718986"
---
# <a name="azure-powershell-release-notes"></a>Azure PowerShell リリース ノート

## <a name="330---january-2020"></a>3.3.0 - 2020 年 1 月
#### <a name="azaccounts"></a>Az.Accounts
* AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました

#### <a name="azcdn"></a>Az.Cdn
* New-AzCdnEndpoint コマンドレットのエラー応答の詳細が表示されます

#### <a name="azcompute"></a>Az.Compute
* OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。

#### <a name="azcontainerinstance"></a>Az.ContainerInstance
* New-AzContainerGroup の例で使用されるパラメーター名を修正しました

#### <a name="azdataboxedge"></a>Az.DataBoxEdge
* コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました
  - Edge ストレージ コンテナーを取得します
* コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました
  - 新しい Edge ストレージ コンテナーを作成します
* コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました
  - Edge ストレージ コンテナーを削除します
* コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました
  - Edge ストレージ コンテナーのデータを更新するアクションを呼び出します
* コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました
  - Edge ストレージ アカウントを取得します
* コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました
  - 新しい Edge ストレージ アカウントを作成します
* コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました
  - Edge ストレージ アカウントを削除します
* コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します
  - 共有のデータを更新するアクションを呼び出します
* コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました
  - az databoxedge ストレージ アカウント資格情報を設定します

#### <a name="azdatafactory"></a>Az.DataFactory
* Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します
* ADF .Net SDK のバージョンを 4.6.0 に更新します
* 'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。

#### <a name="azdevtestlabs"></a>Az.DevTestLabs
* Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します

#### <a name="azeventhub"></a>Az.EventHub
* 問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します

#### <a name="azhdinsight"></a>Az.HDInsight
* Invoke-AzHDInsightHiveJob.md エラーを修正します。

#### <a name="azmachinelearning"></a>Az.MachineLearning
* MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました
  - Get-AzMlOpCluster
  - Get-AzMlOpClusterKey
  - New-AzMlOpCluster
  - Remove-AzMlOpCluster
  - Set-AzMlOpCluster
  - Test-AzMlOpClusterSystemServicesUpdateAvailability
  - Update-AzMlOpClusterSystemService

#### <a name="aznetwork"></a>Az.Network
* Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Azure Site Recovery は、Azure to Azure プロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。
* Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。
* Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。
* Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。

#### <a name="azresources"></a>Az.Resources
* 'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。

#### <a name="azsql"></a>Az.Sql
* 脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。
* SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します

#### <a name="azsqlvirtualmachine"></a>Az.SqlVirtualMachine
* 新しい有効なライセンスの種類として DR を追加します

#### <a name="azstorage"></a>Az.Storage
* 将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します
    - Update-AzStorageAccountNetworkRuleSet
* パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします 
    - Get-AzureRMStorageAccount

## <a name="320---december-2019"></a>3.2.0 - 2019 年 12 月

### <a name="general"></a>全般
* すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します

#### <a name="azaccounts"></a>Az.Accounts
* Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します
* Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します

#### <a name="azbatch"></a>Az.Batch
* 問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 4.5.0 に更新します

#### <a name="azfrontdoor"></a>Az.FrontDoor
* WAF マネージド規則の除外サポートを追加しました
* SocketAddr をオートコンプリートに追加します

#### <a name="azhealthcareapis"></a>Az.HealthcareApis
* 例外処理

#### <a name="azkeyvault"></a>Az.KeyVault
* 設定されていない可能性のある値へのアクセス エラーを修正します
* 楕円曲線暗号証明書の管理
    - 証明書ポリシーの曲線を指定するためのサポートを追加しました

#### <a name="azmonitor"></a>Az.Monitor
* [診断設定を追加する] コマンドに省略可能な引数を追加しています。 存在する場合は Log Analytics へのエクスポートが固定スキーマ ( 専用、データ型) 宛でなければならないことを示す切り替え引数

#### <a name="aznetwork"></a>Az.Network
* AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。

#### <a name="azresources"></a>Az.Resources
* テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。
* ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。

#### <a name="azsql"></a>Az.Sql
* 脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました

#### <a name="azstorage"></a>Az.Storage
* OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします
    - New-AzStorageContainerSASToken
    - New-AzStorageBlobSASToken
* ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます
    - Revoke-AzStorageAccountUserDelegationKeys
* 新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。
* ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。 
    - New-AzRmStorageShare
    - Update-AzRmStorageShare
* パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します
    - Set-AzStorageShareQuota
* Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します
    - Set-AzStorageContainerAcl

## <a name="310---november-2019"></a>3.1.0 - 2019 年 11 月
### <a name="highlights-since-the-last-major-release"></a>前回のメジャー リリース以降のハイライト
* Az.DataBoxEdge 1.0.0 がリリースされました
* Az.SqlVirtualMachine 1.0.0 がリリースされました

#### <a name="azcompute"></a>Az.Compute
* VM の再適用機能
    - Set-AzVM コマンドレットに Reapply パラメーターを追加します
* VM スケール セットの AutomaticRepairs 機能:
    - 次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss
* New-AzVM でのテナント間のギャラリー イメージ サポート
* New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します
* Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します
* New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します
* New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します
* New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します
* New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します

#### <a name="azdataboxedge"></a>Az.DataBoxEdge
* コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました
    - 注文を取得します
* コマンドレット `New-AzDataBoxEdgeOrder` を追加しました
    - 新しい注文を作成します
* コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました
    - 注文を削除します
* コマンドレット `New-AzDataBoxEdgeShare` の変更
    - ローカル共有を作成するようになります
* コマンドレット `Set-AzDataBoxEdgeRole` を追加しました
    - IotRole を共有にマップできるようになりました
* コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました
    - デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します
* コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました
    - トリガーに関する情報を取得します
* コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました
    - 新しいトリガーを作成します
* コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました
    - トリガーを削除します

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 4.4.0 に更新します
* カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します

#### <a name="azeventhub"></a>Az.EventHub
* 問題 10301 を修正:SAS トークンの日付形式を修正します

#### <a name="azfrontdoor"></a>Az.FrontDoor
* Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します
* New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します
* Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します
    - New-AzFrontDoorBackendPoolsSettingObject

#### <a name="aznetwork"></a>Az.Network
* "Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。

#### <a name="azprivatedns"></a>Az.PrivateDns
* PrivateDns .net sdk をバージョン 1.0.0 に更新しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* 保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。
* 復旧計画アクション編集のための Azure Site Recovery のバグ修正。
* filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。

#### <a name="azrediscache"></a>Az.RedisCache
* "New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。 また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。
* "Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました

#### <a name="azresources"></a>Az.Resources
- ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。
- ポリシー定義作成のヘルプの例を更新しました
- サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。
- テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。
- 関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。

#### <a name="azsql"></a>Az.Sql
* データベース ReadReplicaCount のサポートを追加しました。
* ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました

## <a name="300---november-2019"></a>3.0.0 - 2019 年 11 月
### <a name="general"></a>全般
* Az.PrivateDns 1.0.0 がリリースされました

#### <a name="azaccounts"></a>Az.Accounts
* 'Resolve-Error' エイリアスの非推奨メッセージを追加します。

#### <a name="azadvisor"></a>Az.Advisor
* Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。

#### <a name="azbatch"></a>Az.Batch
* `BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。 新しい `LowPriorityCoreQuota` もあります。
  - これにより、**Get-AzBatchAccount** が影響をうけます。
* **New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。
* 新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。 これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。
  - これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。
    - `AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。
    - `StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。
* **Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。
  - アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。 (例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。
* **Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。
  - `ApplicationId` は `ApplicationName` の別名になりました。
* 新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。
* `PSApplicationPackage` の `Version` が `Name` に変更されました。
* `PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。
* `PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。
* **Set-AzBatchPoolOSVersion** を削除しました。 この操作は現在サポートされていません。
* `PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。
* `PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。
* `PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。
* **Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。 
  - **Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。
  - 新しく検証されていないイメージも返されるようになりました。 各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。
* **New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。
* トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。 これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。
* コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。 これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。
* 新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。 これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。
* 指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。
* 指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。

#### <a name="azcdn"></a>Az.Cdn
* UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。
* New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。

#### <a name="azcompute"></a>Az.Compute
* ディスク暗号化の設定機能
    - 新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet
    - DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile        
        Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk
    - DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig
* PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します
* カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します
* ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します
* 重大な変更
    - CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます
    - PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 4.3.0 に更新します

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。
* ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。
* adlsclient で要求タイムアウトごとに設定を公開します
* badoffset 復旧のための元の syncflag の受け渡しを修正します
* 応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します
* Concat のバグを修正します

#### <a name="azfrontdoor"></a>Az.FrontDoor
* モジュール全体でさまざまな入力ミスを修正しました

#### <a name="azhdinsight"></a>Az.HDInsight
* Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。
* AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。
* Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました
* 5 つのコマンドレットを削除しました。
    - Get-AzHDInsightOMS
    - Enable-AzHDInsightOMS
    - Disable-AzHDInsightOMS
    - Grant-AzHDInsightRdpServicesAccess
    - Revoke-AzHDInsightRdpServicesAccess
* 3 つのコマンドレットを追加しました。
    - Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。
    - Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。
    - Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。
* 特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。
* Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。
* コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。
* 次のコマンドレットの出力の型を変更しました:
*  - Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。
*  - Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。
*  - Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。
* いくつかのシナリオ テスト ケースを追加しました。
* 次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。

#### <a name="aziothub"></a>Az.IotHub
* 破壊的変更:
    - コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
    - コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。
    - コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
    - コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。
    - 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。
    - 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。
    - コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。
    - コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。
    - コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
    - コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。
    - コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。
    - コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。
* Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。
* Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。
* Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。
* Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。
* Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。
* Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。
* Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。
* VM の SoftDelete 機能を追加し、softdelete のテストを追加しました

#### <a name="azresources"></a>Az.Resources
* 依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します

#### <a name="aznetwork"></a>Az.Network
* 汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。
    - 更新されたコマンドレット:
        - Approve-AzPrivateEndpointConnection
        - Deny-AzPrivateEndpointConnection
        - Get-AzPrivateEndpointConnection
        - Remove-AzPrivateEndpointConnection
        - Set-AzPrivateEndpointConnection
* PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。
    - 新しいコマンドレット:
        - Get-AzPrivateLinkResource
* 機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。
    - PrivateLinkService にプロパティ EnableProxyProtocol を追加します
    - PrivateEndpointConnection にプロパティ LinkIdentifier を追加します
    - 新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。
* 'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します
* Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット
* VirtualHub の子リソース RouteTables のサポートを追加します
    - 追加された新しいコマンドレットは次のとおりです
        - Add-AzVirtualHubRoute
        - Add-AzVirtualHubRouteTable
        - Get-AzVirtualHubRouteTable
        - Remove-AzVirtualHubRouteTable
        - Set-AzVirtualHub
* VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します
    - 省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。
        - New-AzVirtualHub: パラメーター Sku を追加しました
        - Update-AzVirtualHub: パラメーター Sku を追加しました
        - New-AzVirtualWan: パラメーター VirtualWANType を追加しました
        - Update-AzVirtualWan: パラメーター VirtualWANType を追加しました
* HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します
    - 追加された新しいコマンドレットは次のとおりです
        - Update-AzureRmVirtualHubVnetConnection
    - 省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。
        - New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました
        - New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました
        - Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました
        - New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました
        - Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました
* TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します
    - 追加された新しいコマンドレットは次のとおりです
        - New-AzApplicationGatewayFirewallPolicySetting
        - New-AzApplicationGatewayFirewallPolicyExclusion
        - New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride
        - New-AzApplicationGatewayFirewallPolicyManagedRuleOverride
        - New-AzApplicationGatewayFirewallPolicyManagedRule
        - New-AzApplicationGatewayFirewallPolicyManagedRuleSet
    - 省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。
        - New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました
* CustomRule での Geo-Match 演算子のサポートを追加しました
    - FirewallCondition の演算子に GeoMatch を追加しました
* perListener および perSite ファイアウォール ポリシーのサポートを追加しました
    - 省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。
        - New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました
        - New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました
* 'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します
* Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート
* IpGroup の最上位リソース RouteTables のサポートを追加します
    - 追加された新しいコマンドレットは次のとおりです
        - New-AzIpGroup
        - Remove-AzIpGroup
        - Get-AzIpGroup
        - Set-AzIpGroup

#### <a name="azservicefabric"></a>Az.ServiceFabric
* Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。

#### <a name="azsql"></a>Az.Sql
* Managed Instance での削除されたデータベースの復元のサポートを追加しました。
* 古い監査コマンドレットをコードから非推奨にしました。
* 非推奨の別名を削除しました。
* Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)
* Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)
* Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します
* 非推奨の脆弱性評価の設定コマンドレットの別名を削除します
* 高度な脅威検出の設定コマンドレットを非推奨にします 
* データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。

#### <a name="azstorage"></a>Az.Storage
* Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします
    -  New-AzStorageAccount
    -  Set-AzStorageAccount
* ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します
    -  Get-AzStorageFileHandle
    -  Close-AzStorageFileHandle
    
## <a name="280---october-2019"></a>2.8.0 - 2019 年 10 月
### <a name="general"></a>全般
* Az. HealthcareApis 1.0.0 リリース

#### <a name="azaccounts"></a>Az.Accounts
* 生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。

#### <a name="azapimanagement"></a>Az.ApiManagement
* **Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました
    - 次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068

#### <a name="azautomation"></a>Az.Automation
* Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。 

#### <a name="azbatch"></a>Az.Batch
* **Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。

#### <a name="azcompute"></a>Az.Compute
* New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します
* Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します
* Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。 
* Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。
* ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。
* ADF .Net SDK のバージョンを 4.2.0 に更新します

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します

#### <a name="azhealthcareapis"></a>Az.HealthcareApis
* PowerShell のバージョンを1.0.0 に更新しました
* SDK のバージョンを1.0.2 に更新しました
* 新しい SDK バージョンを参照するようにテストを更新します
* 出力構造を入れ子からフラット化に更新しました。

#### <a name="aziothub"></a>Az.IotHub
* 新しいルーティング ソースの追加:DigitalTwinChangeEvents
* 軽微なバグの修正:Get-AzIothub が subscriptionId を返さない 

#### <a name="azmonitor"></a>Az.Monitor
* アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver
* 受信側で有効になっている共通のアラート スキーマを使用します。 これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません
* Webhook で Azure Active Directory 認証をサポートするようになりました。

#### <a name="aznetwork"></a>Az.Network
* サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。
* Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました
    - 追加された新しいコマンドレットは次のとおりです
        - New-AzureRmTrafficSelectorPolicy
    - 省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection
* ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します
    - 更新されたコマンドレット:
        - Add-AzNetworkSecurityRuleConfig
        - New-AzNetworkSecurityRuleConfig
        - Set-AzNetworkSecurityRuleConfig
* Cortex コマンドレットでの例外処理を改善します
* VirtualNetworkGateways の新しい世代と SKU
  - VirtualNetworkGateways の新しい世代を導入します。
  - VirtualNetworkGateways の新しい高スループット SKU を導入します。

#### <a name="azrediscache"></a>Az.RedisCache
* '-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました

#### <a name="azsql"></a>Az.Sql
* Managed Instance に Active Directory 管理者を設定するためのサポートを追加します

#### <a name="azstorage"></a>Az.Storage
* Storage クライアント ライブラリを 11.1.0 にアップグレードします
* 管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する
    -  Get-AzRmStorageContainer
* サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する
    -  Get-AzStorageAccount

#### <a name="azstoragesync"></a>Az.StorageSync
* Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。

#### <a name="azwebsites"></a>Az.Websites
* Set-AzWebApp でアプリの ASP の更新が失敗していました

## <a name="270---september-2019"></a>2.7.0 - 2019 年 9 月
#### <a name="azapimanagement"></a>Az.ApiManagement
* 'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました
* リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。 代わりに 'Set-AzApiManagement' を使用してください。

#### <a name="azautomation"></a>Az.Automation
* 'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました
* Register-AzAutomationDSCNode に OS 制限の説明を追加しました
* AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。

#### <a name="azcompute"></a>Az.Compute
* UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します
* Incremental パラメーターを New-AzSnapshotConfig に追加します
* 低優先度の仮想マシン機能を追加します。
    - MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。
    - MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。
* サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。
* Get-AzRemoteDesktopFile の null 例外を修正します。
* VHD Seek メソッドの終了相対位置を修正します。
* New-AzVM と Update-AzVM の UltraSSD の問題を修正します。

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します
* ADF .Net SDK のバージョンを 4.1.3 に更新しました

#### <a name="azhdinsight"></a>Az.HDInsight
* 破壊的変更についてお知らせします

#### <a name="aziothub"></a>Az.IotHub
* geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。
* IotHub のメッセージ詳細化を管理するためのサポートを追加します。 新たに追加されたコマンドレットは次のとおりです。
    - Add-AzIotHubMessageEnrichment
    - Get-AzIotHubMessageEnrichment
    - Remove-AzIotHubMessageEnrichment
    - Set-AzIotHubMessageEnrichment

#### <a name="azmonitor"></a>Az.Monitor
* 最新の Monitor SDK (0.24.1-preview) を指しています
   - Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。 これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。
   - **ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。 この変更に対応するために、シナリオ テストが更新されました。
   - クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。 現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。 **注**: これは、アラート チームによって検証する必要がある一時的な変更です。
   - クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。 この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。
   - クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。 この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。
* メトリック アラート V2 の動的しきい値条件のサポート
    - New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました
    - Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました
* スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化
 - コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。
 - ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました
 - 省略可能なパラメーター 'ActionGroup' の例を追加しました
 - ヘルプ ファイルを全体的に改善しました
* 'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します

#### <a name="aznetwork"></a>Az.Network
* 'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します 
* 'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します
* 'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました
* クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました
* クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました
* セキュリティ規則モデルの不適切なマッピングを修正しました
* プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました
    - PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました
    - PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました
    - 新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました
* Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました
* Virtual WAN でのマルチリンクのサポート
    - 新しいコマンドレット
        - New-AzVpnSiteLink
        - New-AzVpnSiteLinkConnection
    - 更新されたコマンドレット:
        - New-VpnSite
        - Update-VpnSite
        - New-VpnConnection
        - Update-VpnConnection
* AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました
* VM ポリシーと元のストレージ アカウントの復元のテストを追加しました

#### <a name="azresources"></a>Az.Resources
* New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました
* アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。
    - New-AzServiceFabricApplication
    - New-AzServiceFabricApplicationType
    - New-AzServiceFabricApplicationTypeVersion
    - New-AzServiceFabricService
    - Update-AzServiceFabricApplication
    - Get-AzServiceFabricApplication
    - Get-AzServiceFabricApplicationType
    - Get-AzServiceFabricApplicationTypeVersion
    - Get-AzServiceFabricService
    - Remove-AzServiceFabricApplication
    - Remove-AzServiceFabricApplicationType
    - Remove-AzServiceFabricApplicationTypeVersion
    - Remove-AzServiceFabricServic
* Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。

#### <a name="azsignalr"></a>Az.SignalR
* Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します

#### <a name="azsql"></a>Az.Sql
* 'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します
* エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。
* Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します
* 監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。
* 複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。

#### <a name="azstorage"></a>Az.Storage
* 'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました
* Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします
    -  Set-AzStorageFileContent
    -  Get-AzStorageFileContent
* コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。
    -  Set-AzStorageBlobContent
* 管理プレーン API を使用した Azure ファイル共有の管理をサポートします
    -  New-AzRmStorageShare
    -  Get-AzRmStorageShare
    -  Update-AzRmStorageShare
    -  Remove-AzRmStorageShare

#### <a name="azwebsites"></a>Az.Websites
* アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します
* Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します
* 'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します

## <a name="260---august-2019"></a>2.6.0 - 2019 年 8 月
#### <a name="general"></a>全般
* 多数のモジュールでさまざまな入力ミスを修正しました

#### <a name="azaccounts"></a>Az.Accounts
* Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)

#### <a name="azaks"></a>Az.Aks
* "Get-AzAks" の出力に関する問題を修正しました
    * 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847

#### <a name="azapimanagement"></a>Az.ApiManagement
* 次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351
    - .NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。
* **Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。
  https://github.com/Azure/azure-powershell/issues/9482
* **New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752
* モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました

#### <a name="azbatch"></a>Az.Batch
* ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました

#### <a name="azcdn"></a>Az.Cdn
* CDN モジュール変換ヘルパーの入力ミスを修正しました

#### <a name="azcompute"></a>Az.Compute
* New-AzVMConfig コマンドレットに VmssId を追加しました
* New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました
* VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました
* Host と HostGroup の機能を追加しました
    - 新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost
    - HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました
* "Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました
* "Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました

#### <a name="azdatafactory"></a>Az.DataFactory
* "New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました
* ADF .Net SDK のバージョンを 4.1.2 に更新しました
* "Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました
* トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました

#### <a name="azdatalakestore"></a>Az.DataLakeStore
* 任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。

#### <a name="azeventhub"></a>Az.EventHub
* 問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス
* 問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています
* Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました
* 問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません

#### <a name="azmarketplaceordering"></a>Az.MarketplaceOrdering
* "Azure" がすべて小文字であるドキュメントの入力ミスを修正しました

#### <a name="azmonitor"></a>Az.Monitor
* ヘルプ ドキュメントで正しくないパラメーター名を修正しました

#### <a name="aznetwork"></a>Az.Network
* New-AzPrivateLinkServiceIpConfig を更新しました
    - "PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。
    - 現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。
* SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました
* 適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました 
* Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。
* AzNetworkServiceTag の Location パラメーターの説明を更新しました

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* "New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました
    - 例を追加しました
    - "-Name" パラメーターの説明を更新しました
* New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました
* New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* "Get-AzRecoveryServicesBackupJobDetail.md" を更新しました

#### <a name="azresources"></a>Az.Resources
* Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました
    - 変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました
    - "condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます
* サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました

#### <a name="azservicebus"></a>Az.ServiceBus
* 問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス
* 問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません
* キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました 

#### <a name="azservicefabric"></a>Az.ServiceFabric
* ノード タイプの追加のコマンドレットのバグを修正しました。
    - リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。 問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681
    - virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。 問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407
    - Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました

#### <a name="azsql"></a>Az.Sql
* 古い監査コマンドレットのドキュメントを更新しました。

#### <a name="azstorage"></a>Az.Storage
* コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました
* BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします
    -  Set-AzStorageBlobContent
    -  Start-AzStorageBlobCopy
* BLOB のコピーでリハイドレート優先度をサポートします
    -  Start-AzStorageBlobCopy

#### <a name="azwebsites"></a>Az.Websites
* Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました

## <a name="250---july-2019"></a>2.5.0 - 2019 年 7 月
#### <a name="azaccounts"></a>Az.Accounts
* 最新バージョンの ClientRuntime を使用するように共通コードを更新しました。

#### <a name="azapplicationinsights"></a>Az.ApplicationInsights
* 「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました 

#### <a name="azautomation"></a>Az.Automation
* リソース文字列の入力ミスを修正しました 

#### <a name="azcognitiveservices"></a>Az.CognitiveServices
* NetworkRuleSet のサポートを追加しました。

#### <a name="azcompute"></a>Az.Compute
* VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。

#### <a name="azcontainerregistry"></a>Az.ContainerRegistry
* Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました
    - 詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633

#### <a name="azdatafactory"></a>Az.DataFactory
* ADF .Net SDK のバージョンを 4.1.0 に更新しました
* 「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました

#### <a name="azeventhub"></a>Az.EventHub
* SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken
* authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました

#### <a name="azkeyvault"></a>Az.KeyVault
* 証明書ポリシーの KeySize を指定するためのサポートを追加しました

#### <a name="azlogicapp"></a>Az.LogicApp
* Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました
    - フィルター処理用に新しい MapType パラメーターを追加しました

#### <a name="azmanagedservices"></a>Az.ManagedServices
* API バージョン 2019-06-01 (GA) のサポートを追加しました

#### <a name="aznetwork"></a>Az.Network
* プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました
    - 新しいコマンドレット
        - Set-AzPrivateEndpoint
        - Set-AzPrivateLinkService
        - Approve-AzPrivateEndpointConnection
        - Deny-AzPrivateEndpointConnection
        - Get-AzPrivateEndpointConnection
        - Remove-AzPrivateEndpointConnection
        - Test-AzPrivateLinkServiceVisibility
        - Get-AzAutoApprovedPrivateLinkService
* 次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ
    - New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました
        - このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。
        - このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。
* AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました
* ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました
    - 更新されたコマンドレット
        - Add-AzNetworkSecurityRuleConfig
        - New-AzNetworkSecurityRuleConfig
        - Set-AzNetworkSecurityRuleConfig
* ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました
* LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました
    - 更新されたコマンドレット:
        - New-AzLoadBalancerFrontendIpConfig
        - Add-AzLoadBalancerFrontendIpConfig
        - Set-AzLoadBalancerFrontendIpConfig
* プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新
    - New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。 このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* 保存された検索条件の既定のバージョンを 1 に更新しました。 
* カスタム ログの null 正規表現の扱いを修正しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* "Get-AzRecoveryServicesBackupJob.md" を更新しました
* "Get-AzRecoveryServicesBackupContainer.md" を更新しました
* "Get-AzRecoveryServicesVault.md" を更新しました
* "Wait-AzRecoveryServicesBackupJob.md" を更新しました
* "Set-AzRecoveryServicesVaultContext.md" を更新しました
* "Get-AzRecoveryServicesBackupItem.md" を更新しました
* "Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました
* "Restore-AzRecoveryServicesBackupItem.md" を更新しました
* Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました
* "Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました

#### <a name="azresources"></a>Az.Resources
- 「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました
- 新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました

#### <a name="azservicebus"></a>Az.ServiceBus
* SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken
* authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました

#### <a name="azsql"></a>Az.Sql
* Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました
* メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました
* 警告メッセージの軽微な入力ミスを修正しました。

#### <a name="azstorage"></a>Az.Storage
* 正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました

#### <a name="azstoragesync"></a>Az.StorageSync
* Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。
* TierFilesOlderThanDays に従うように問題 9551 を修正しました

#### <a name="azwebsites"></a>Az.Websites
* Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました
* Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました
* New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました

## <a name="240---july-2019"></a>2.4.0 - 2019 年 7 月
#### <a name="azaccounts"></a>Az.Accounts
* プロファイル コマンドレットのサポートの追加
* 生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加
* Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正

#### <a name="azadvisor"></a>Az.Advisor
* Az.Advisor の GA リリース
* このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました

#### <a name="azapimanagement"></a>Az.ApiManagement
* 次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671
    - **Get-AzApiManagementSubscription**
        - ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました
        - スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました
* [https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正
    - **Import-AzApiManagementApi**
        - Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました

#### <a name="azautomation"></a>Az.Automation
* 文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。

#### <a name="azcompute"></a>Az.Compute
* New-AzImageConfig への HyperVGeneration パラメーターの追加

#### <a name="azdatafactory"></a>Az.DataFactory
* アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新

#### <a name="azeventgrid"></a>Az.EventGrid
* 'New-AzEventGridSubscription' ドキュメントのタイポを修正

#### <a name="aziothub"></a>Az.IotHub
* 承認ポリシー キーの再生成のサポートを追加

#### <a name="aznetwork"></a>Az.Network
* パブリック ip タグに 'RoutingPreference' を追加しました
* 'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました

#### <a name="azpolicyinsights"></a>Az.PolicyInsights
* Get-AzPolicyState の null 参照の問題を修正しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました

#### <a name="azrecoveryservices"></a>Az.RecoveryServices
* IaaSVMs の get-policy コマンドを修正しました

#### <a name="azresources"></a>Az.Resources
    - Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました
    - Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました
    - Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました
    - ポリシー コマンドレットの少数のドキュメントと例を更新しました

#### <a name="azservicebus"></a>Az.ServiceBus
* 問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題

#### <a name="azsql"></a>Az.Sql
* プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました
* 新しいコマンドレットによる Azure SQL Server\Database 監査をサポート
    - Set-AzSqlServerAudit
    - Get-AzSqlServerAudit
    - Remove-AzSqlServerAudit
    - Set-AzSqlDatabaseAudit
    - Get-AzSqlDatabaseAudit
    - Remove-AzSqlDatabaseAudit
* 脆弱性評価の設定から電子メールの制限を削除しました

#### <a name="azstorage"></a>Az.Storage
* 2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。
    -  Enable-AzStorageStaticWebsite
* 例を追加して Get AzStorageBlobContent のヘルプを更新しました
* StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示
* Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート
    -  New-AzStorageAccount
    -  Set-AzStorageAccount
* ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート
    - Get-AzStorageFileHandle
    - Close-AzStorageFileHandle

#### <a name="azstoragesync"></a>Az.StorageSync
* このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました

## <a name="232---june-2019"></a>2.3.2 - 2019 年 6 月
#### <a name="azaccounts"></a>Az.Accounts
* 関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました
    - 詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983
* AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました
  - Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic
  - Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest

#### <a name="azcompute"></a>Az.Compute
* 単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。
* "New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました

#### <a name="azdns"></a>Az.Dns
* "Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。

#### <a name="azeventgrid"></a>Az.EventGrid
* 2019-06-01 API バージョンを使用するように更新しました。
* 新しいコマンドレット:
    - New-AzureRmEventGridDomain
        - 新しい Azure Event Grid ドメインを作成します。
    - Get-AzureRmEventGridDomain
        - Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。
    - Remove-AzureRmEventGridDomain
        - Azure Event Grid ドメインを削除します。
    - New-AzureRmEventGridDomainKey
        - Azure Event Grid ドメインの共有アクセス キーを再生成します。
    - Get-AzureRmEventGridDomainKey
        - Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。
    - New-AzureRmEventGridDomainTopic:
        - 新しい Azure Event Grid ドメイン トピックを作成します。
    - Get-AzureRmEventGridDomainTopic
        - Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。 
    - Remove-AzureRmEventGridDomainTopic:
        - 既存の Azure Event Grid ドメイン トピックを削除します。
* 更新されたコマンドレット:
    - New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:
        - 新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。
        - 新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。
        - 既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。
        - 以下を指定するための新しい省略可能なパラメーターを追加:
            - イベント サブスクリプションの有効期限の日付
            - 高度なフィルター パラメーター
        - 宛先として servicebusqueue の新しい列挙型を追加しました。
        - -IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました 
    - Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:
        - 結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。
    - Remove-AzureRmEventGridSubscription
        - Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。
        - Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。

#### <a name="azfrontdoor"></a>Az.FrontDoor
* New-AzFrontDoorWafMatchConditionObject
    - 変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました
* New-AzFrontDoorWafManagedRuleObject
    - 新しいオート コンプリート値を追加しました

#### <a name="aznetwork"></a>Az.Network
* 仮想ネットワーク ゲートウェイ リソースのサポートを追加しました
    - 新しいコマンドレット
        - Get-AzVirtualNetworkGatewayVpnClientConnectionHealth
* AvailablePrivateEndpointType を追加しました
    - 新しいコマンドレット 
        - Get-AzAvailablePrivateEndpointType
* PrivatePrivateLinkService を追加しました
    - 新しいコマンドレット 
        - Get-AzPrivateLinkService 
        - New-AzPrivateLinkService
        - Remove-AzPrivateLinkService
        - New-AzPrivateLinkServiceIpConfig
        - Set-AzPrivateEndpointConnection
* PrivateEndpoint を追加しました
    - 新しいコマンドレット
        - Get-AzPrivateEndpoint
        - New-AzPrivateEndpoint
        - Remove-AzPrivateEndpoint
        - New-AzPrivateLinkServiceConnection
* 次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ
    - New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。
    - Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。
* ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。
* ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。
* ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました
* TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました
* 書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。
* NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました
* すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました
* ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました
* AzureFirewall および NatGateway の Availability Zones のサポートを追加しました
* Get-AzNetworkServiceTag コマンドレットを追加しました
* Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました
    - New-AzFirewall コマンドレットを更新:
        - 1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました
        - 仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました
        - ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)
        - パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました 
* 次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。 
    - New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。
    - Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。
    - Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。

#### <a name="azoperationalinsights"></a>Az.OperationalInsights
* "New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました

#### <a name="azresources"></a>Az.Resources
* 追加の [テンプレートのエクスポート] オプションがサポートされました
    - Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました
    - Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました
    - エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました

#### <a name="azservicefabric"></a>Az.ServiceFabric
* 場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました

#### <a name="azsql"></a>Az.Sql
* Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました
* Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました
* Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました
   - Add-AzSqlInstanceKeyVaultKey
   - Get-AzSqlInstanceKeyVaultKey
   - Remove-AzSqlInstanceKeyVaultKey
   - Get-AzSqlInstanceTransparentDataEncryptionProtector
   - Set-AzSqlInstanceTransparentDataEncryptionProtector

#### <a name="azstorage"></a>Az.Storage
* ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました
    - New-AzStorageAccount
* BLOB 不変コマンドレットの説明を明確化しました
    -  Remove-AzRmStorageContainerImmutabilityPolicy

#### <a name="azwebsites"></a>Az.Websites
* クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました
* Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました

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
    - SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報
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
* Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/
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
* Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/
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
* Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/
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

* [https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました
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
* [https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました
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
