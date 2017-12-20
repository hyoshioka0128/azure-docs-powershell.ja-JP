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
ms.openlocfilehash: cf58789ba69fd2fc157e37d0b052827b361246e5
ms.sourcegitcommit: c42c7176276ec4e1cc3360a93e6b15d32083bf9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/14/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="20171208-version-511"></a>2017.12.08 バージョン 5.1.1
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
    - 問題 https://github.com/Azure/azure-powershell/issues/4974 を修正しました
        - 監査コマンドレットに無効な AUDIT_CHANGED_GROUP 値を指定しても、エラーがスローされなくなりました。これは今後のリリースで削除される予定です。
    - 問題 https://github.com/Azure/azure-powershell/issues/5046 を修正しました
        - 監査コマンドレットの AuditAction パラメーターが無視されなくなりました
    - "Secondary" StorageKeyType を指定したときの監査コマンドレットの問題を修正しました
        - BLOB 監査の設定時に、StorageKeyType パラメーターに "Secondary" 値を指定すると、セカンダリ ストレージ アカウント キーではなくプライマリ キーが使用されました。
    - Set-AzureRmSqlServerTransparentDataEncryptionProtector からの確認メッセージの表現を変更しました
* Azure (RDFE)
    - すべての RemoteApp コマンドレットを削除しました
* Azure.Storage
    - Azure Storage Client Library 8.6.0 および Azure Storage DataMovement Library 0.6.5 にアップグレードしました

前回のリリース以降の変更点: 前回のリリース以降の変更点: https://github.com/azure/azure-powershell/compare/v5.0.1-November2017...v5.1.1-December2017

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
