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
ms.date: 11/14/2017
ms.openlocfilehash: ab35cbc4ec1a0bd4e7ee40e1864bd7941f5bca87
ms.sourcegitcommit: 79dd3700b5cb4cb90b268778b482082052160093
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/14/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

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
* 注: これは重大な変更のリリースです。 導入された重大な変更の完全な一覧については、移行ガイド (https://aka.ms/azps-migration-guide) を参照してください。
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
    * https://github.com/Azure/azure-powershell/issues/3164 を修正
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