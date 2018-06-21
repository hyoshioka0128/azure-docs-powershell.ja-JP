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
# <a name="release-notes"></a><span data-ttu-id="7c29b-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="7c29b-103">Release notes</span></span>

<span data-ttu-id="7c29b-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="7c29b-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

## <a name="600---may-2018"></a><span data-ttu-id="7c29b-105">6.0.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="7c29b-105">6.0.0 - May 2018</span></span>

### <a name="general"></a><span data-ttu-id="7c29b-106">全般</span><span class="sxs-lookup"><span data-stu-id="7c29b-106">General</span></span>
* <span data-ttu-id="7c29b-107">モジュールの最小依存関係を PowerShell 5.0 に設定しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-107">Set minimum dependency of modules to PowerShell 5.0</span></span>

### <a name="azurestorage"></a><span data-ttu-id="7c29b-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="7c29b-108">Azure.Storage</span></span>
* <span data-ttu-id="7c29b-109">Storage Blob コンテナー名として以下がサポートされます</span><span class="sxs-lookup"><span data-stu-id="7c29b-109">Support  as Storage blob container name</span></span>
    - <span data-ttu-id="7c29b-110">New-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="7c29b-110">New-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="7c29b-111">Remove-AzureStorageBlobContainer</span><span class="sxs-lookup"><span data-stu-id="7c29b-111">Remove-AzureStorageBlobContainer</span></span>
    - <span data-ttu-id="7c29b-112">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7c29b-112">Set-AzureStorageBlobContent</span></span>
    - <span data-ttu-id="7c29b-113">Get-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="7c29b-113">Get-AzureStorageBlobContent</span></span>
* <span data-ttu-id="7c29b-114">一部の Storage コマンドレットのエラー出力に詳細なエラー情報が含まれていないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-114">Fix the issue that some Storage cmdlets failure output not contain detail failure information</span></span>

### <a name="azurermapimanagement"></a><span data-ttu-id="7c29b-115">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="7c29b-115">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="7c29b-116">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-116">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-117">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-117">Please refer to the migration guide for more information</span></span>

### <a name="azurermautomation"></a><span data-ttu-id="7c29b-118">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="7c29b-118">AzureRM.Automation</span></span>
* <span data-ttu-id="7c29b-119">非推奨の "Tags" エイリアスをコマンドレットから削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-119">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="7c29b-120">"Set-AzureRmAutomationRunbook"</span><span class="sxs-lookup"><span data-stu-id="7c29b-120">'Set-AzureRmAutomationRunbook'</span></span>

### <a name="azurermbatch"></a><span data-ttu-id="7c29b-121">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="7c29b-121">AzureRM.Batch</span></span>
* <span data-ttu-id="7c29b-122">New-AzureBatchPool のドキュメントを更新して、非推奨の例を削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-122">Updated New-AzureBatchPool documentation to remove deprecated example</span></span>

### <a name="azurermcdn"></a><span data-ttu-id="7c29b-123">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="7c29b-123">AzureRM.Cdn</span></span>
* <span data-ttu-id="7c29b-124">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-124">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-125">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-125">Please refer to the migration guide for more information</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="7c29b-126">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="7c29b-126">AzureRM.Compute</span></span>
* <span data-ttu-id="7c29b-127">"New-AzureRmVm" と "New-AzureRmVmss" で、パラメーターの詳細出力がサポートされます</span><span class="sxs-lookup"><span data-stu-id="7c29b-127">'New-AzureRmVm' and 'New-AzureRmVmss' support verbose output of parameters</span></span>
* <span data-ttu-id="7c29b-128">"New-AzureRmVm" と "New-AzureRmVmss" (単純なパラメーター セット) で、VM へのユーザー定義およびシステム定義の ID の割り当てがサポートされます</span><span class="sxs-lookup"><span data-stu-id="7c29b-128">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support assigning user defined and(or) system defined identities to the VM(s).</span></span>
* <span data-ttu-id="7c29b-129">VMSS の Redeploy および PerformMaintenance 機能</span><span class="sxs-lookup"><span data-stu-id="7c29b-129">VMSS Redeploy and PerformMaintenance feature</span></span>
    -  <span data-ttu-id="7c29b-130">"Set-AzureRmVmss" と "Set-AzureRmVmssVM" に、新しいスイッチ パラメーター -Redeploy と -PerformMaintenance を追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-130">Add new switch parameter -Redeploy and -PerformMaintenance to 'Set-AzureRmVmss' and 'Set-AzureRmVmssVM'</span></span>
* <span data-ttu-id="7c29b-131">"Set-AzureRmVMOperatingSystem" コマンドレットに DisableVMAgent スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-131">Add DisableVMAgent switch parameter to 'Set-AzureRmVMOperatingSystem' cmdlet</span></span>
* <span data-ttu-id="7c29b-132">"New-AzureRmVm" と "New-AzureRmVmss" (単純なパラメーター セット) で、"Win10" イメージがサポートされます</span><span class="sxs-lookup"><span data-stu-id="7c29b-132">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support a 'Win10' image.</span></span>
* <span data-ttu-id="7c29b-133">"Repair-AzureRmVmssServiceFabricUpdateDomain" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="7c29b-133">'Repair-AzureRmVmssServiceFabricUpdateDomain' cmdlet is added.</span></span>
* <span data-ttu-id="7c29b-134">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-134">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-135">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-135">Please refer to the migration guide for more details</span></span>
* <span data-ttu-id="7c29b-136">"Set-AzureRmVmDiskEncryptionExtension" で AAD パラメーターが省略可能になりました</span><span class="sxs-lookup"><span data-stu-id="7c29b-136">'Set-AzureRmVmDiskEncryptionExtension' makes AAD parameters optional</span></span>

### <a name="azurermdatafactories"></a><span data-ttu-id="7c29b-137">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="7c29b-137">AzureRM.DataFactories</span></span>
* <span data-ttu-id="7c29b-138">非推奨の "Tags" エイリアスをコマンドレットから削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-138">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="7c29b-139">New-AzureRmDataFactory</span><span class="sxs-lookup"><span data-stu-id="7c29b-139">New-AzureRmDataFactory</span></span>

### <a name="azurermdatafactoryv2"></a><span data-ttu-id="7c29b-140">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="7c29b-140">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="7c29b-141">ADF .Net SDK バージョンを、次の変更を含む 0.7.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-141">Updated the ADF .Net SDK version to 0.7.0-preview containing following changes:</span></span>
    - <span data-ttu-id="7c29b-142">ExecuteSSISPackage Activity に、実行パラメーターと接続マネージャー プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-142">Added execution parameters and connection managers property on ExecuteSSISPackage Activity</span></span>
    - <span data-ttu-id="7c29b-143">サーバー、データベース、スキーマ、ユーザー名、パスワードの代わりに完全な接続文字列を使用するように、PostgreSql、MySql のリンクされたサービスを更新しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-143">Updated PostgreSql, MySql llinked service to use full connection string instead of server, database, schema, username and password</span></span>
    - <span data-ttu-id="7c29b-144">DB2 のリンクされたサービスからスキーマを削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-144">Removed the schema from DB2 linked service</span></span>
    - <span data-ttu-id="7c29b-145">Teradata のリンクされたサービスからスキーマ プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-145">Removed schema property from Teradata linked service</span></span>
    - <span data-ttu-id="7c29b-146">Responsys の LinkedService、Dataset、CopySource を追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-146">Added LinkedService, Dataset, CopySource for Responsys</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="7c29b-147">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="7c29b-147">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="7c29b-148">非推奨の "Tags" エイリアスをコマンドレットから削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-148">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="7c29b-149">"New-AzureRmDataLakeAnalyticsAccount"</span><span class="sxs-lookup"><span data-stu-id="7c29b-149">'New-AzureRmDataLakeAnalyticsAccount'</span></span>
    - <span data-ttu-id="7c29b-150">"Set-AzureRmDataLakeAnalyticsAccount"</span><span class="sxs-lookup"><span data-stu-id="7c29b-150">'Set-AzureRmDataLakeAnalyticsAccount'</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="7c29b-151">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="7c29b-151">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="7c29b-152">Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl に、再帰的 ACL 変更の新しい機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-152">Add new feature of recursive Acl Change to Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="7c29b-153">ディレクトリのコンテンツの概要を取得する新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-153">Add new cmdlet for retrieving the content summary under a directory</span></span>
* <span data-ttu-id="7c29b-154">ディスク使用量と ACL ダンプを取得する新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-154">Add new cmdlet for retrieving the disk usage and Acl dump</span></span>
* <span data-ttu-id="7c29b-155">Set-AzureRmDataLakeStoreItemAcl bool の戻り値の型を IEnumerable<DataLakeStoreItemAce> に修正しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-155">Correct return type of Set-AzureRmDataLakeStoreItemAcl bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="7c29b-156">Set-AzureRmDataLakeStoreItemAclEntry bool の戻り値の型を IEnumerable<DataLakeStoreItemAce> に修正しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-156">Correct return type of Set-AzureRmDataLakeStoreItemAclEntry bool to IEnumerable<DataLakeStoreItemAce></span></span>
* <span data-ttu-id="7c29b-157">Export-AzureRmDataLakeStoreItem、Import-AzureRmDataLakeStoreItem、Remove-AzureRmDataLakeStoreItem の重大な変更</span><span class="sxs-lookup"><span data-stu-id="7c29b-157">Breaking changes in Export-AzureRmDataLakeStoreItem, Import-AzureRmDataLakeStoreItem, Remove-AzureRmDataLakeStoreItem</span></span>

### <a name="azurermdns"></a><span data-ttu-id="7c29b-158">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="7c29b-158">AzureRM.Dns</span></span>
* <span data-ttu-id="7c29b-159">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-159">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-160">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-160">Please refer to the migration guide for more information</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="7c29b-161">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="7c29b-161">AzureRM.EventHub</span></span>
* <span data-ttu-id="7c29b-162">例が欠落していたコマンドレットのヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-162">Updated Help for cmdlets with missing examples</span></span>

### <a name="azurerminsights"></a><span data-ttu-id="7c29b-163">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="7c29b-163">AzureRM.Insights</span></span>
* <span data-ttu-id="7c29b-164">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-164">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-165">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-165">Please refer to the migration guide for more information</span></span>

### <a name="azurermiothub"></a><span data-ttu-id="7c29b-166">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="7c29b-166">AzureRM.IotHub</span></span>
* <span data-ttu-id="7c29b-167">IotHub でタグと Basic SKU を有効にしました</span><span class="sxs-lookup"><span data-stu-id="7c29b-167">Enable tags and Basic Sku to the IotHub</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="7c29b-168">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="7c29b-168">AzureRM.KeyVault</span></span>
* <span data-ttu-id="7c29b-169">パイプ処理シナリオをサポートするための重大な変更</span><span class="sxs-lookup"><span data-stu-id="7c29b-169">Breaking changes to support piping scenarios</span></span>
* <span data-ttu-id="7c29b-170">新しいコマンドレットとして、Backup/Restore-AzureKeyVaultManagedStorageAccount、Backup/Restore-AzureKeyVaultCertificate、Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval、Undo-AzureKeyVaultManagedStorageAccountRemoval を追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-170">Added new cmdlets: Backup/Restore-AzureKeyVaultManagedStorageAccount, Backup/Restore-AzureKeyVaultCertificate, Undo-AzureKeyVaultManagedStorageSasDefinitionRemoval, and Undo-AzureKeyVaultManagedStorageAccountRemoval</span></span>

### <a name="azurermmachinelearning"></a><span data-ttu-id="7c29b-171">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="7c29b-171">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="7c29b-172">非推奨の "Tags" エイリアスをコマンドレットから削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-172">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="7c29b-173">Update-AzureRmMlCommitmentPlan</span><span class="sxs-lookup"><span data-stu-id="7c29b-173">Update-AzureRmMlCommitmentPlan</span></span>

### <a name="azurermmedia"></a><span data-ttu-id="7c29b-174">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="7c29b-174">AzureRM.Media</span></span>
* <span data-ttu-id="7c29b-175">非推奨の "Tags" エイリアスをコマンドレットから削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-175">Remove deprecated 'Tags' alias from cmdlets</span></span>
    - <span data-ttu-id="7c29b-176">"Set-AzureRmMediaService"</span><span class="sxs-lookup"><span data-stu-id="7c29b-176">'Set-AzureRmMediaService'</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="7c29b-177">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="7c29b-177">AzureRM.Network</span></span>
* <span data-ttu-id="7c29b-178">DDoS Protection プラン リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-178">Add support for DDoS protection plan resource</span></span>
* <span data-ttu-id="7c29b-179">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-179">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-180">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-180">Please refer to the migration guide for more information</span></span>

### <a name="azurermnotificationhubs"></a><span data-ttu-id="7c29b-181">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="7c29b-181">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="7c29b-182">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-182">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-183">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-183">Please refer to the migration guide for more information</span></span>

### <a name="azurermoperationalinsights"></a><span data-ttu-id="7c29b-184">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="7c29b-184">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="7c29b-185">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-185">Introduce multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-186">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-186">Please refer to the migration guide for more information</span></span>

### <a name="azurermprofile"></a><span data-ttu-id="7c29b-187">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="7c29b-187">AzureRM.Profile</span></span>
* <span data-ttu-id="7c29b-188">コンテキスト自動保存が既定で有効になります</span><span class="sxs-lookup"><span data-stu-id="7c29b-188">Enable context autosave by default</span></span>
* <span data-ttu-id="7c29b-189">米国政府の Azure 環境に、USGovernmentOperationalInsightsEndpoint プロパティと USGovernmentOperationalInsightsEndpointResourceId プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-189">Add USGovernmentOperationalInsightsEndpoint and USGovernmentOperationalInsightsEndpointResourceId properties to Azure environment for US Gov.</span></span>

### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="7c29b-190">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="7c29b-190">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="7c29b-191">SiteRecovery シナリオでの認証ヘッダーを修正しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-191">Fixed Authentication Header in SiteRecovery scenarios</span></span>

### <a name="azurermrediscache"></a><span data-ttu-id="7c29b-192">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="7c29b-192">AzureRM.RedisCache</span></span>
* <span data-ttu-id="7c29b-193">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-193">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-194">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-194">Please refer to the migration guide for more information</span></span>

### <a name="azurermresources"></a><span data-ttu-id="7c29b-195">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="7c29b-195">AzureRM.Resources</span></span>
* <span data-ttu-id="7c29b-196">Get-AzureRmRoledefinition 呼び出しから古い -AtScopeAndBelow パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-196">Remove obsolete parameter -AtScopeAndBelow from Get-AzureRmRoledefinition call</span></span>
* <span data-ttu-id="7c29b-197">Get-AzureRmRoleAssignment の結果に、削除された Users/Groups/ServicePrincipals への割り当てを含めました</span><span class="sxs-lookup"><span data-stu-id="7c29b-197">Include assignments to deleted USers/Groups/ServicePrincipals in Get-AzureRmRoleAssignment result</span></span>
* <span data-ttu-id="7c29b-198">Scope と ResourceType のタブ補完を追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-198">Add Tab completers for Scope and ResourceType</span></span>
* <span data-ttu-id="7c29b-199">ServicePrincipals を作成する便利なコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-199">Add convenience cmdlet for creating ServicePrincipals</span></span>
* <span data-ttu-id="7c29b-200">Get-AzureRmResource で Get- 機能と -Find 機能をマージしました</span><span class="sxs-lookup"><span data-stu-id="7c29b-200">Merge Get- and Find- functionality in Get-AzureRmResource</span></span>
* <span data-ttu-id="7c29b-201">次の AD コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-201">Add AD Cmdlets:</span></span>
  - <span data-ttu-id="7c29b-202">Remove-AzureRmADGroupMember</span><span class="sxs-lookup"><span data-stu-id="7c29b-202">Remove-AzureRmADGroupMember</span></span>
  - <span data-ttu-id="7c29b-203">Get-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="7c29b-203">Get-AzureRmADGroup</span></span>
  - <span data-ttu-id="7c29b-204">New-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="7c29b-204">New-AzureRmADGroup</span></span>
  - <span data-ttu-id="7c29b-205">Remove-AzureRmADGroup</span><span class="sxs-lookup"><span data-stu-id="7c29b-205">Remove-AzureRmADGroup</span></span>
  - <span data-ttu-id="7c29b-206">Remove-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="7c29b-206">Remove-AzureRmADUser</span></span>
  - <span data-ttu-id="7c29b-207">Update-AzureRmADApplication</span><span class="sxs-lookup"><span data-stu-id="7c29b-207">Update-AzureRmADApplication</span></span>
  - <span data-ttu-id="7c29b-208">Update-AzureRmADServicePrincipal</span><span class="sxs-lookup"><span data-stu-id="7c29b-208">Update-AzureRmADServicePrincipal</span></span>
  - <span data-ttu-id="7c29b-209">Update-AzureRmADUser</span><span class="sxs-lookup"><span data-stu-id="7c29b-209">Update-AzureRmADUser</span></span>

### <a name="azurermservicefabric"></a><span data-ttu-id="7c29b-210">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="7c29b-210">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="7c29b-211">既定の Linux イメージ バージョン SKU を更新しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-211">Update default Linux image version sku</span></span>
  - <span data-ttu-id="7c29b-212">NewAzureServiceFabricCluster.cs の既定値は UbuntuServer1604 SKU 更新です</span><span class="sxs-lookup"><span data-stu-id="7c29b-212">NewAzureServiceFabricCluster.cs default UbuntuServer1604 Sku update</span></span>

### <a name="azurermstorage"></a><span data-ttu-id="7c29b-213">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="7c29b-213">AzureRM.Storage</span></span>
* <span data-ttu-id="7c29b-214">複数の重大な変更を導入しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-214">Introduced multiple breaking changes</span></span>
    - <span data-ttu-id="7c29b-215">詳細については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="7c29b-215">Please refer to the migration guide for more information</span></span>

### <a name="azurermwebsites"></a><span data-ttu-id="7c29b-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="7c29b-216">AzureRM.Websites</span></span>
* <span data-ttu-id="7c29b-217">Websites SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-217">Upgrade to latest version of the Websites SDK</span></span>
* <span data-ttu-id="7c29b-218">Set-AzureRmWebApp と Set-AzureRmWebAppSlot に、-AssignIdentity プロパティと -Httpsonly プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-218">Added -AssignIdentity & -Httpsonly properties for Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
* <span data-ttu-id="7c29b-219">Get-AzureRmWebAppSnapshots と Restore-AzureRmWebAppSnapshot の 2 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="7c29b-219">Added two new cmdlets: Get-AzureRmWebAppSnapshots and Restore-AzureRmWebAppSnapshot</span></span>
