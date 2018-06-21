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
ms.date: 5/1/2018
ms.openlocfilehash: 8515a267e80e5d1f7bb97557efa72b9e86b7b45d
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/08/2018
ms.locfileid: "33912005"
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

---

## <a name="600---may-2018"></a>6.0.0 - 2018 年 5 月

### <a name="general"></a>全般
* モジュールの最小依存関係を PowerShell 5.0 に設定しました

### <a name="azurestorage"></a>Azure.Storage
* Storage Blob コンテナー名として以下がサポートされます
    - New-AzureStorageBlobContainer
    - Remove-AzureStorageBlobContainer
    - Set-AzureStorageBlobContent
    - Get-AzureStorageBlobContent
* 一部の Storage コマンドレットのエラー出力に詳細なエラー情報が含まれていないという問題を修正しました

### <a name="azurermapimanagement"></a>AzureRM.ApiManagement
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermautomation"></a>AzureRM.Automation
* 非推奨の "Tags" エイリアスをコマンドレットから削除しました
    - "Set-AzureRmAutomationRunbook"

### <a name="azurermbatch"></a>AzureRM.Batch
* New-AzureBatchPool のドキュメントを更新して、非推奨の例を削除しました

### <a name="azurermcdn"></a>AzureRM.Cdn
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermcompute"></a>AzureRM.Compute
* "New-AzureRmVm" と "New-AzureRmVmss" で、パラメーターの詳細出力がサポートされます
* "New-AzureRmVm" と "New-AzureRmVmss" (単純なパラメーター セット) で、VM へのユーザー定義およびシステム定義の ID の割り当てがサポートされます
* VMSS の Redeploy および PerformMaintenance 機能
    -  "Set-AzureRmVmss" と "Set-AzureRmVmssVM" に、新しいスイッチ パラメーター -Redeploy と -PerformMaintenance を追加しました
* "Set-AzureRmVMOperatingSystem" コマンドレットに DisableVMAgent スイッチ パラメーターを追加しました
* "New-AzureRmVm" と "New-AzureRmVmss" (単純なパラメーター セット) で、"Win10" イメージがサポートされます
* "Repair-AzureRmVmssServiceFabricUpdateDomain" コマンドレットが追加されました
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください
* "Set-AzureRmVmDiskEncryptionExtension" で AAD パラメーターが省略可能になりました

### <a name="azurermdatafactories"></a>AzureRM.DataFactories
* 非推奨の "Tags" エイリアスをコマンドレットから削除しました
    - New-AzureRmDataFactory

### <a name="azurermdatafactoryv2"></a>AzureRM.DataFactoryV2
* ADF .Net SDK バージョンを、次の変更を含む 0.7.0-preview に更新しました
    - ExecuteSSISPackage Activity に、実行パラメーターと接続マネージャー プロパティを追加しました
    - サーバー、データベース、スキーマ、ユーザー名、パスワードの代わりに完全な接続文字列を使用するように、PostgreSql、MySql のリンクされたサービスを更新しました
    - DB2 のリンクされたサービスからスキーマを削除しました
    - Teradata のリンクされたサービスからスキーマ プロパティを削除しました
    - Responsys の LinkedService、Dataset、CopySource を追加しました

### <a name="azurermdatalakeanalytics"></a>AzureRM.DataLakeAnalytics
* 非推奨の "Tags" エイリアスをコマンドレットから削除しました
    - "New-AzureRmDataLakeAnalyticsAccount"
    - "Set-AzureRmDataLakeAnalyticsAccount"

### <a name="azurermdatalakestore"></a>AzureRM.DataLakeStore
* Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl に、再帰的 ACL 変更の新しい機能を追加しました
* ディレクトリのコンテンツの概要を取得する新しいコマンドレットを追加しました
* ディスク使用量と ACL ダンプを取得する新しいコマンドレットを追加しました
* Set-AzureRmDataLakeStoreItemAcl bool の戻り値の型を IEnumerable<DataLakeStoreItemAce> に修正しました
* Set-AzureRmDataLakeStoreItemAclEntry bool の戻り値の型を IEnumerable<DataLakeStoreItemAce> に修正しました
* Export-AzureRmDataLakeStoreItem、Import-AzureRmDataLakeStoreItem、Remove-AzureRmDataLakeStoreItem の重大な変更

### <a name="azurermdns"></a>AzureRM.Dns
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermeventhub"></a>AzureRM.EventHub
* 例が欠落していたコマンドレットのヘルプを更新しました

### <a name="azurerminsights"></a>AzureRM.Insights
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermiothub"></a>AzureRM.IotHub
* IotHub でタグと Basic SKU を有効にしました

### <a name="azurermkeyvault"></a>AzureRM.KeyVault
* パイプ処理シナリオをサポートするための重大な変更
* 新しいコマンドレットとして、Backup/Restore-AzureKeyVaultManagedStorageAccount、Backup/Restore-AzureKeyVaultCertificate、Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval、Undo-AzureKeyVaultManagedStorageAccountRemoval を追加しました

### <a name="azurermmachinelearning"></a>AzureRM.MachineLearning
* 非推奨の "Tags" エイリアスをコマンドレットから削除しました
    - Update-AzureRmMlCommitmentPlan

### <a name="azurermmedia"></a>AzureRM.Media
* 非推奨の "Tags" エイリアスをコマンドレットから削除しました
    - "Set-AzureRmMediaService"

### <a name="azurermnetwork"></a>AzureRM.Network
* DDoS Protection プラン リソースのサポートを追加しました
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermnotificationhubs"></a>AzureRM.NotificationHubs
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermoperationalinsights"></a>AzureRM.OperationalInsights
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermprofile"></a>AzureRM.Profile
* コンテキスト自動保存が既定で有効になります
* 米国政府の Azure 環境に、USGovernmentOperationalInsightsEndpoint プロパティと USGovernmentOperationalInsightsEndpointResourceId プロパティを追加しました

### <a name="azurermrecoveryservicessiterecovery"></a>AzureRM.RecoveryServices.SiteRecovery
* SiteRecovery シナリオでの認証ヘッダーを修正しました

### <a name="azurermrediscache"></a>AzureRM.RedisCache
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermresources"></a>AzureRM.Resources
* Get-AzureRmRoledefinition 呼び出しから古い -AtScopeAndBelow パラメーターを削除しました
* Get-AzureRmRoleAssignment の結果に、削除された Users/Groups/ServicePrincipals への割り当てを含めました
* Scope と ResourceType のタブ補完を追加しました
* ServicePrincipals を作成する便利なコマンドレットを追加しました
* Get-AzureRmResource で Get- 機能と -Find 機能をマージしました
* 次の AD コマンドレットを追加しました
  - Remove-AzureRmADGroupMember
  - Get-AzureRmADGroup
  - New-AzureRmADGroup
  - Remove-AzureRmADGroup
  - Remove-AzureRmADUser
  - Update-AzureRmADApplication
  - Update-AzureRmADServicePrincipal
  - Update-AzureRmADUser

### <a name="azurermservicefabric"></a>AzureRM.ServiceFabric
* 既定の Linux イメージ バージョン SKU を更新しました
  - NewAzureServiceFabricCluster.cs の既定値は UbuntuServer1604 SKU 更新です

### <a name="azurermstorage"></a>AzureRM.Storage
* 複数の重大な変更を導入しました
    - 詳細については、移行ガイドを参照してください

### <a name="azurermwebsites"></a>AzureRM.Websites
* Websites SDK の最新バージョンに更新しました
* Set-AzureRmWebApp と Set-AzureRmWebAppSlot に、-AssignIdentity プロパティと -Httpsonly プロパティを追加しました
* Get-AzureRmWebAppSnapshots と Restore-AzureRmWebAppSnapshot の 2 つの新しいコマンドレットを追加しました
