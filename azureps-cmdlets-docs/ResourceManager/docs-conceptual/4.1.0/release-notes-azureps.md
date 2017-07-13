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
# <span data-ttu-id="d0f37-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="d0f37-103">Release notes</span></span>
<a id="release-notes" class="xliff"></a>

<span data-ttu-id="d0f37-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="d0f37-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <span data-ttu-id="d0f37-105">バージョン 4.0.0</span><span class="sxs-lookup"><span data-stu-id="d0f37-105">Version 4.0.0</span></span>
<a id="version-400" class="xliff"></a>

* <span data-ttu-id="d0f37-106">このリリースには、重大な変更が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d0f37-106">This release contains breaking changes.</span></span> <span data-ttu-id="d0f37-107">変更の詳細と既存のスクリプトへの影響については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0f37-107">Please see [the migration guide](https://aka.ms/azps-migration-guide) for change details and the impact on existing scripts.</span></span>
* <span data-ttu-id="d0f37-108">ApiManagement</span><span class="sxs-lookup"><span data-stu-id="d0f37-108">ApiManagement</span></span>
  - <span data-ttu-id="d0f37-109">New-AzureRmApiManagementGroup での外部グループの構成に対応しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-109">Added support for configuring external groups in New-AzureRmApiManagementGroup.</span></span>
* <span data-ttu-id="d0f37-110">課金</span><span class="sxs-lookup"><span data-stu-id="d0f37-110">Billing</span></span>
  - <span data-ttu-id="d0f37-111">新しいコマンドレット Get-AzureRmBillingPeriod</span><span class="sxs-lookup"><span data-stu-id="d0f37-111">New Cmdlet Get-AzureRmBillingPeriod</span></span>
    + <span data-ttu-id="d0f37-112">サブスクリプションに対する Azure の請求期間を取得するコマンドレット。</span><span class="sxs-lookup"><span data-stu-id="d0f37-112">cmdlet to retrieve azure billing periods of the subscription.</span></span>
  - <span data-ttu-id="d0f37-113">コマンドレット Get-AzureRmBillingInvoice を更新しました</span><span class="sxs-lookup"><span data-stu-id="d0f37-113">Update Cmdlet Get-AzureRmBillingInvoice</span></span>
  - <span data-ttu-id="d0f37-114">新しいプロパティ BillingPeriodNames</span><span class="sxs-lookup"><span data-stu-id="d0f37-114">new property BillingPeriodNames</span></span>
  - <span data-ttu-id="d0f37-115">リスト ビューでの出力</span><span class="sxs-lookup"><span data-stu-id="d0f37-115">output in list view</span></span>
* <span data-ttu-id="d0f37-116">計算</span><span class="sxs-lookup"><span data-stu-id="d0f37-116">Compute</span></span>
  - <span data-ttu-id="d0f37-117">Premium 管理ディスクをサポートするように Set-AzureRmVMAEMExtension と Test-AzureRmVMAEMExtension の各コマンドレットが更新されました</span><span class="sxs-lookup"><span data-stu-id="d0f37-117">Updated Set-AzureRmVMAEMExtension and Test-AzureRmVMAEMExtension cmdlets to support Premium managed disks</span></span>
  - <span data-ttu-id="d0f37-118">IaaS VM の暗号化設定をバックアップし、障害時に復元を行います</span><span class="sxs-lookup"><span data-stu-id="d0f37-118">Backup encryption settings for IaaS VMs and restore on failure</span></span>
  - <span data-ttu-id="d0f37-119">ChefServiceInterval オプションの名前が ChefDaemonInterval に変更されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-119">ChefServiceInterval option is renamed to ChefDaemonInterval now.</span></span> <span data-ttu-id="d0f37-120">なお、以前のものは引き続き有効です。</span><span class="sxs-lookup"><span data-stu-id="d0f37-120">Old one will continue to work however.</span></span>
  - <span data-ttu-id="d0f37-121">重複している DataDiskNames および NetworkInterfaceIDs の各プロパティが PS VM オブジェクトから削除されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-121">Remove duplicated DataDiskNames and NetworkInterfaceIDs properties from PS VM object.</span></span>
  - <span data-ttu-id="d0f37-122">DataDiskNames および NetworkInterfaceIDs パラメーターは、それぞれ Remove-AzureRmVMDataDisk および Remove-AzureRmVMNetworkInterface で省略可能になります。</span><span class="sxs-lookup"><span data-stu-id="d0f37-122">Make DataDiskNames and NetworkInterfaceIDs parameters optional in Remove-AzureRmVMDataDisk and Remove-AzureRmVMNetworkInterface, respectively.</span></span>
  - <span data-ttu-id="d0f37-123">Get コマンドレットがリスト オブジェクトを返すときの Get コマンドレットのパイプ処理の問題が解決されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-123">Fix the piping issue of Get cmdlets when the Get cmdlets return a list object.</span></span>
  - <span data-ttu-id="d0f37-124">RDFE コマンドレットと競合しているコマンドレットの名前は変更されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-124">Cmdlets that conflicted with RDFE cmdlets have been renamed.</span></span> <span data-ttu-id="d0f37-125">詳細については、https://github.com/Azure/azure-powershell/issues/2917 で問題を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0f37-125">See issue https://github.com/Azure/azure-powershell/issues/2917 for more details</span></span>
    + <span data-ttu-id="d0f37-126">`New-AzureVMSqlServerAutoBackupConfig` の名前が `New-AzureRmVMSqlServerAutoBackupConfig` に変更されました</span><span class="sxs-lookup"><span data-stu-id="d0f37-126">`New-AzureVMSqlServerAutoBackupConfig` has been renamed to `New-AzureRmVMSqlServerAutoBackupConfig`</span></span>
    + <span data-ttu-id="d0f37-127">`New-AzureVMSqlServerAutoPatchingConfig` の名前が `New-AzureRmVMSqlServerAutoPatchingConfig` に変更されました</span><span class="sxs-lookup"><span data-stu-id="d0f37-127">`New-AzureVMSqlServerAutoPatchingConfig` has been renamed to `New-AzureRmVMSqlServerAutoPatchingConfig`</span></span>
    + <span data-ttu-id="d0f37-128">`New-AzureVMSqlServerKeyVaultCredentialConfig` の名前が `New-AzureRmVMSqlServerKeyVaultCredentialConfig` に変更されました</span><span class="sxs-lookup"><span data-stu-id="d0f37-128">`New-AzureVMSqlServerKeyVaultCredentialConfig` has been renamed to `New-AzureRmVMSqlServerKeyVaultCredentialConfig`</span></span>
* <span data-ttu-id="d0f37-129">使用量</span><span class="sxs-lookup"><span data-stu-id="d0f37-129">Consumption</span></span>
  - <span data-ttu-id="d0f37-130">新しいコマンドレット Get-AzureRmConsumptionUsageDetail</span><span class="sxs-lookup"><span data-stu-id="d0f37-130">New Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>
    + <span data-ttu-id="d0f37-131">サブスクリプションの使用量の詳細を取得するコマンドレット。</span><span class="sxs-lookup"><span data-stu-id="d0f37-131">cmdlet to retrieve usage details of the subscription.</span></span>
* <span data-ttu-id="d0f37-132">ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d0f37-132">ContainerRegistry</span></span>
  - <span data-ttu-id="d0f37-133">Azure Container Registry の PowerShell コマンドレットが追加されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-133">Add PowerShell cmdlets for Azure Container Registry</span></span>
    + <span data-ttu-id="d0f37-134">New-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d0f37-134">New-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="d0f37-135">Get-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d0f37-135">Get-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="d0f37-136">Update-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d0f37-136">Update-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="d0f37-137">Remove-AzureRmContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="d0f37-137">Remove-AzureRmContainerRegistry</span></span>
    + <span data-ttu-id="d0f37-138">Get-AzureRmContainerRegistryCredential</span><span class="sxs-lookup"><span data-stu-id="d0f37-138">Get-AzureRmContainerRegistryCredential</span></span>
    + <span data-ttu-id="d0f37-139">Update-AzureRmContainerRegistryCredential</span><span class="sxs-lookup"><span data-stu-id="d0f37-139">Update-AzureRmContainerRegistryCredential</span></span>
    + <span data-ttu-id="d0f37-140">Test-AzureRmContainerRegistryNameAvailability</span><span class="sxs-lookup"><span data-stu-id="d0f37-140">Test-AzureRmContainerRegistryNameAvailability</span></span>
* <span data-ttu-id="d0f37-141">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="d0f37-141">DataLakeAnalytics</span></span>
  - <span data-ttu-id="d0f37-142">カタログ パッケージの取得およびリストに対応しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-142">Add support for catalog package get and list</span></span>
  - <span data-ttu-id="d0f37-143">深い先祖からの、次のカタログ項目の一覧表示に対応しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-143">Add support for listing the following catalog items from deeper ancestors:</span></span>
    + <span data-ttu-id="d0f37-144">テーブル</span><span class="sxs-lookup"><span data-stu-id="d0f37-144">Table</span></span>
    + <span data-ttu-id="d0f37-145">TVF</span><span class="sxs-lookup"><span data-stu-id="d0f37-145">TVF</span></span>
    + <span data-ttu-id="d0f37-146">表示</span><span class="sxs-lookup"><span data-stu-id="d0f37-146">View</span></span>
    + <span data-ttu-id="d0f37-147">統計</span><span class="sxs-lookup"><span data-stu-id="d0f37-147">Statistics</span></span>
* <span data-ttu-id="d0f37-148">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="d0f37-148">DataLakeStore</span></span>
  - <span data-ttu-id="d0f37-149">`Import-AzureRMDataLakeStoreItem` および `Export-AzureRMDataLakeStoreItem` では、パフォーマンス向上のため、トレース ログ記録が既定で無効になっています。</span><span class="sxs-lookup"><span data-stu-id="d0f37-149">For `Import-AzureRMDataLakeStoreItem` and `Export-AzureRMDataLakeStoreItem` trace logging has been disabled by default to improve performance.</span></span> <span data-ttu-id="d0f37-150">トレース ログ記録が必要な場合は、`-DiagnosticLogLevel` と `-DiagnosticLogPath` の各パラメーターを使用してください。</span><span class="sxs-lookup"><span data-stu-id="d0f37-150">If trace logging is desired please use the `-DiagnosticLogLevel` and `-DiagnosticLogPath` parameters</span></span>
  - <span data-ttu-id="d0f37-151">ADLS に小さなファイルを多数アップロードすると PowerShell がときどきクラッシュするバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-151">Fixed a bug that would sometimes cause PowerShell to crash when uploading lots of small file to ADLS.</span></span>
* <span data-ttu-id="d0f37-152">EventHub</span><span class="sxs-lookup"><span data-stu-id="d0f37-152">EventHub</span></span>
  - <span data-ttu-id="d0f37-153">バグの修正:</span><span class="sxs-lookup"><span data-stu-id="d0f37-153">Bug fix :</span></span>
    + <span data-ttu-id="d0f37-154">Set-AzureRmEventHubNamespace コマンドレットのエラーが修正されます - "Tier" は、null にはできないため、"SkuName" にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0f37-154">Fix for Set-AzureRmEventHubNamespace cmdlet error  - 'Tier' cannot be null, where it should be 'SkuName'</span></span>
    + <span data-ttu-id="d0f37-155">Set-AzureRmEventHub - EventHub の更新中に発生する "オブジェクト参照がオブジェクトのインスタンスに設定されていません" というエラーが修正されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-155">Set-AzureRmEventHub - Fix 'Object reference not set to an instance of an object' error while updating EventHub</span></span>
* <span data-ttu-id="d0f37-156">洞察</span><span class="sxs-lookup"><span data-stu-id="d0f37-156">Insights</span></span>
  - <span data-ttu-id="d0f37-157">Add-AzureRm*AlertRule</span><span class="sxs-lookup"><span data-stu-id="d0f37-157">Add-AzureRm*AlertRule</span></span>
    + <span data-ttu-id="d0f37-158">単一オブジェクト newResource、statusCode、requestId を返します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-158">Returns a single object: newResource, statusCode, requestId</span></span>
  - <span data-ttu-id="d0f37-159">Get-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="d0f37-159">Get-AzureRmAlertRule</span></span>
    + <span data-ttu-id="d0f37-160">出力は、単一オブジェクトと見なされるのではなく、列挙されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-160">The output is now enumerated instead of considered a single object.</span></span> <span data-ttu-id="d0f37-161">型に変更はなく、リストのままです。</span><span class="sxs-lookup"><span data-stu-id="d0f37-161">Its type did not change, it is still a list.</span></span>
  - <span data-ttu-id="d0f37-162">Remove-AzureRmAlertRule</span><span class="sxs-lookup"><span data-stu-id="d0f37-162">Remove-AzureRmAlertRule</span></span>
    + <span data-ttu-id="d0f37-163">statusCode は、要求によって返される状態コードに従います。以前は常に OK でした。</span><span class="sxs-lookup"><span data-stu-id="d0f37-163">The statusCode follows the status code returned by the request, before it was Ok always.</span></span>
  - <span data-ttu-id="d0f37-164">Add-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="d0f37-164">Add-AzureRmAutoscaleSetting</span></span>
    + <span data-ttu-id="d0f37-165">statusCode、requestId、および新しく作成または更新されたリソースを含む単一オブジェクトを返します (以前のようなリストではありません)。</span><span class="sxs-lookup"><span data-stu-id="d0f37-165">Returns now a single object (not a list as before) containing statusCode, requestId, and the newly created/updated resource.</span></span>
    + <span data-ttu-id="d0f37-166">状態コードは、要求によって返される状態に従います。以前は常に OK でした。</span><span class="sxs-lookup"><span data-stu-id="d0f37-166">The status code follows the status returned by the request, before it was always Ok.</span></span>
  - <span data-ttu-id="d0f37-167">New-AzureRmAutoscaleRule</span><span class="sxs-lookup"><span data-stu-id="d0f37-167">New-AzureRmAutoscaleRule</span></span>
    + <span data-ttu-id="d0f37-168">パラメーター ScaleActionType が拡張され、ChangeCount、PercentChangeCount、ExactCount の各値を受け取るようになりました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-168">The parameter ScaleActionType has been extended, it receives the following values now: ChangeCount, PercentChangeCount, ExactCount.</span></span>
  - <span data-ttu-id="d0f37-169">Remove-AzureRmAutoscaleSetting</span><span class="sxs-lookup"><span data-stu-id="d0f37-169">Remove-AzureRmAutoscaleSetting</span></span>
    + <span data-ttu-id="d0f37-170">出力の statusCode は、要求によって返される statusCode に従います。</span><span class="sxs-lookup"><span data-stu-id="d0f37-170">The statusCode in the output follows the statusCode returned by the request.</span></span> <span data-ttu-id="d0f37-171">以前は常に OK でした。</span><span class="sxs-lookup"><span data-stu-id="d0f37-171">Before it was always Ok.</span></span>
  - <span data-ttu-id="d0f37-172">Get-AzureRMLogProfile</span><span class="sxs-lookup"><span data-stu-id="d0f37-172">Get-AzureRMLogProfile</span></span>
    + <span data-ttu-id="d0f37-173">出力は列挙されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-173">The output is now enumerated.</span></span> <span data-ttu-id="d0f37-174">以前は単一オブジェクトと見なされていました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-174">Before it was considered a single object.</span></span> <span data-ttu-id="d0f37-175">出力の型は以前と同様にリストのままです。</span><span class="sxs-lookup"><span data-stu-id="d0f37-175">The type of the output remains a list as before.</span></span>
  - <span data-ttu-id="d0f37-176">Remove-AzureRmLogProfile</span><span class="sxs-lookup"><span data-stu-id="d0f37-176">Remove-AzureRmLogProfile</span></span>
    + <span data-ttu-id="d0f37-177">PassThru パラメーターが実装されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-177">The PassThru parameter has been implemented.</span></span>
  - <span data-ttu-id="d0f37-178">メトリックの API</span><span class="sxs-lookup"><span data-stu-id="d0f37-178">Metrics API</span></span>
    + <span data-ttu-id="d0f37-179">SDK は MDM からメトリックを取得するようになりました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-179">The SDK now retrieves metrics from MDM.</span></span>
  - <span data-ttu-id="d0f37-180">Get-AzureRmMetricDefinition</span><span class="sxs-lookup"><span data-stu-id="d0f37-180">Get-AzureRmMetricDefinition</span></span>
    + <span data-ttu-id="d0f37-181">出力はリストのままですが、リストの構造は変更されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-181">The output is still a list, but the structure of the list changed.</span></span>
  - <span data-ttu-id="d0f37-182">Get-AzureRmMetric</span><span class="sxs-lookup"><span data-stu-id="d0f37-182">Get-AzureRmMetric</span></span>
    + <span data-ttu-id="d0f37-183">呼び出しが変更されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-183">The call has changed.</span></span> <span data-ttu-id="d0f37-184">新しい構文は次のとおりです: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]</span><span class="sxs-lookup"><span data-stu-id="d0f37-184">This is the new syntax: Get-AzureRmMetric ResourceId [MetricNames [TimeGrain] [AggregationType] [StartTime] [EndTime]] [DetailedOutput]</span></span>
    + <span data-ttu-id="d0f37-185">出力はリストで、要素の構造が変更されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-185">The output is a list, and the structure of its elements has changed.</span></span>
* <span data-ttu-id="d0f37-186">KeyVault</span><span class="sxs-lookup"><span data-stu-id="d0f37-186">KeyVault</span></span>
  - <span data-ttu-id="d0f37-187">KeyVault シークレットのバックアップ/復元に対応しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-187">Adding backup/restore support for KeyVault secrets</span></span>
    + <span data-ttu-id="d0f37-188">キーに対して現在サポートされている機能に合わせて、シークレットをバックアップおよび復元できます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-188">Secrets can be backed up and restored, matching the functionality currently supported for Keys</span></span>

  - <span data-ttu-id="d0f37-189">キーとシークレットのバックアップ コマンドレットでは、対応するオブジェクトを入力パラメーターとして受け入れるようになりました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-189">Backup cmdlets for Keys and Secrets now accept a corresponding object as an input parameter</span></span>
    + <span data-ttu-id="d0f37-190">呼び出し元で、次のように取得操作とバックアップ操作を連結できます: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="d0f37-190">The caller may chain retrieval and backup operations: Get-AzureKeyVaultKey -VaultName myVault -Name myKey | Backup-AzureKeyVaultKey</span></span>

  - <span data-ttu-id="d0f37-191">バックアップ コマンドレットが、既存のファイルを上書きする -Force スイッチに対応しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-191">Backup cmdlets now support a -Force switch to overwrite an existing file</span></span>
    + <span data-ttu-id="d0f37-192">既存のファイルを上書きしようとしてもスローされなくなり、代わりに、ユーザーは続行方法を選択しるように求められます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-192">Note that attempting to overwrite an existing file will no longer throw, and will instead prompt the user for a choice on how to proceed.</span></span>
* <span data-ttu-id="d0f37-193">LogicApp</span><span class="sxs-lookup"><span data-stu-id="d0f37-193">LogicApp</span></span>
  - <span data-ttu-id="d0f37-194">インターチェンジ制御番号のディザスター リカバリー コマンドレット用の新しいパラメーター</span><span class="sxs-lookup"><span data-stu-id="d0f37-194">New parameters for Interchange Control Number disaster recovery cmdlets:</span></span>
    + <span data-ttu-id="d0f37-195">省略可能 - 関連する制御番号を指定する -AgreementType パラメーター ("X12" または "Edifact")</span><span class="sxs-lookup"><span data-stu-id="d0f37-195">Optional -AgreementType parameter ("X12", or "Edifact") to specify the relevant control numbers</span></span>
* <span data-ttu-id="d0f37-196">MachineLearning</span><span class="sxs-lookup"><span data-stu-id="d0f37-196">MachineLearning</span></span>
  - <span data-ttu-id="d0f37-197">Azure Machine Learning .Net SDK の新しいバージョンを使用するようになり、新しいコマンドレットが追加されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-197">Consume new version of Azure Machine Learning .Net SDK and add a new cmdlet</span></span>
    + <span data-ttu-id="d0f37-198">Add-AzureRmMlWebServiceRegionalProperty</span><span class="sxs-lookup"><span data-stu-id="d0f37-198">Add-AzureRmMlWebServiceRegionalProperty</span></span>
  - <span data-ttu-id="d0f37-199">ヘルプ テキストの用語を部分的に修正しています。</span><span class="sxs-lookup"><span data-stu-id="d0f37-199">Minor wording fixes in help text.</span></span>
* <span data-ttu-id="d0f37-200">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="d0f37-200">Network</span></span>
  - <span data-ttu-id="d0f37-201">Test-AzureRmNetworkWatcherConnectivity コマンドレットが追加されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-201">Added Test-AzureRmNetworkWatcherConnectivity cmdlet</span></span>
    + <span data-ttu-id="d0f37-202">指定されたソース VM とターゲットの接続情報を返します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-202">Returns connectivity information for a specified source VM and a destination</span></span>
    + <span data-ttu-id="d0f37-203">ソースとターゲットの間の接続を確立できない場合は、問題に関する詳細情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-203">If connectivity between the source and destination cannot be established, the cmdlet returns details about the issue</span></span>
* <span data-ttu-id="d0f37-204">プロファイル</span><span class="sxs-lookup"><span data-stu-id="d0f37-204">Profile</span></span>
  - <span data-ttu-id="d0f37-205">"Send-Feedback" コマンドレットの追加: このコマンドレットを使用すると、Azure PowerShell のチームにフィードバックを送信する一連のプロンプトを開始できます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-205">Added \`Send-Feedback' cmdlet: allows a user to initiate a set of prompts which sends feedback to the Azure PowerShell team.</span></span>
  - <span data-ttu-id="d0f37-206">次のエイリアスは、Azure モジュールの既存のコマンドレット名と競合しているため、削除されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-206">The following aliases have been removed as they conflicted with existing cmdlet names in the Azure module:</span></span>
    + <span data-ttu-id="d0f37-207">`Enable-AzureDataCollection` (`Enable-AzureRmDataCollection` でサポート)</span><span class="sxs-lookup"><span data-stu-id="d0f37-207">`Enable-AzureDataCollection` (supported by `Enable-AzureRmDataCollection`)</span></span>
    + <span data-ttu-id="d0f37-208">`Disable-AzureDataCollection` (`Disable-AzureRmDataCollection` でサポート)</span><span class="sxs-lookup"><span data-stu-id="d0f37-208">`Disable-AzureDataCollection` (supported by `Disable-AzureRmDataCollection`)</span></span>
* <span data-ttu-id="d0f37-209">リレー</span><span class="sxs-lookup"><span data-stu-id="d0f37-209">Relay</span></span>
  - <span data-ttu-id="d0f37-210">ユーザーがすべての Azure リレー リソースを作成および管理できる Azure リレーのコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-210">Adds cmdlets for the Azure Relay which allows users to create and manage all Azure Relay resources.</span></span>
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
* <span data-ttu-id="d0f37-211">リソース</span><span class="sxs-lookup"><span data-stu-id="d0f37-211">Resources</span></span>
  - <span data-ttu-id="d0f37-212">New-AzureRmResourceGroupDeployment でリソース グループをまたがるデプロイに対応しました</span><span class="sxs-lookup"><span data-stu-id="d0f37-212">Support cross-resource-group deployments for New-AzureRmResourceGroupDeployment</span></span>
    + <span data-ttu-id="d0f37-213">ユーザーは、さまざまなリソース グループをデプロイする際に、入れ子になったデプロイを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-213">Users can now use nested deployments to deploy to different resource groups.</span></span>
* <span data-ttu-id="d0f37-214">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="d0f37-214">ServiceBus</span></span>

  - <span data-ttu-id="d0f37-215">バグの修正: ServiceBus キュー オブジェクトのプロパティ値は null に設定されていましたが、このオブジェクトが、キューを更新する Set-AzureRmServiceBusQueue コマンドレットの入力パラメーターとして使用されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-215">Bug Fix: ServiceBus Queue object property values were set to null, the object is used as input parameter in Set-AzureRmServiceBusQueue cmdlet to update Queue.</span></span>
   - <span data-ttu-id="d0f37-216">影響を受けるプロパティは、LockDuration、EntityAvailabilityStatus、DuplicateDetectionHistoryTimeWindow、MaxDeliveryCount、MessageCount です。</span><span class="sxs-lookup"><span data-stu-id="d0f37-216">Properties affected are LockDuration, EntityAvailabilityStatus, DuplicateDetectionHistoryTimeWindow, MaxDeliveryCount and MessageCount</span></span>
* <span data-ttu-id="d0f37-217">ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="d0f37-217">ServiceFabric</span></span>

  - <span data-ttu-id="d0f37-218">Service Fabric のコマンドレットが追加されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-218">Added cmdlets for service fabric</span></span>
    + <span data-ttu-id="d0f37-219">Add-AzureRmServiceFabricApplicationCertificate       アプリケーション証明書として使用される証明書を追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-219">Add-AzureRmServiceFabricApplicationCertificate       Add a certificate which will be used as application certificate</span></span>
    + <span data-ttu-id="d0f37-220">Add-AzureRmServiceFabricClientCertificate       クライアント認証用のクラスター設定に共通名または拇印を追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-220">Add-AzureRmServiceFabricClientCertificate       Add a common name or thumbprint to the cluster settings for client authentication</span></span>
    + <span data-ttu-id="d0f37-221">Add-AzureRmServiceFabricClusterCertificate       既存の証明書をロールオーバーするためにクラスターにセカンダリのクラスター証明書を追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-221">Add-AzureRmServiceFabricClusterCertificate       Add a secondary cluster certificate to the cluster for rolling over the existing certificate</span></span>
    + <span data-ttu-id="d0f37-222">Add-AzureRmServiceFabricNodes       クラスターに特定のノード タイプのノード/VM を追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-222">Add-AzureRmServiceFabricNodes       Add nodes/VMs of a specific node type to a cluster</span></span>
    + <span data-ttu-id="d0f37-223">Add-AzureRmServiceFabricNodeType       既存のクラスターにノード タイプ/VM を追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-223">Add-AzureRmServiceFabricNodeType       Add a node type/VMs to an existing cluster</span></span>
    + <span data-ttu-id="d0f37-224">Get-AzureRmServiceFabricCluster       クラスター リソースの詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-224">Get-AzureRmServiceFabricCluster       Get the details of the cluster resource</span></span>
    + <span data-ttu-id="d0f37-225">New-AzureRmServiceFabricCluster は、新しい ServiceFabric クラスターを作成します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-225">New-AzureRmServiceFabricCluster Create a new ServiceFabric cluster.</span></span> <span data-ttu-id="d0f37-226">このコマンドは、さまざまなシナリオをカバーするため、オーバーロードが多数あります。</span><span class="sxs-lookup"><span data-stu-id="d0f37-226">This command has many overloads to cover various scenarios</span></span>
    + <span data-ttu-id="d0f37-227">overloadsemove-AzureRmServiceFabricClientCertificate       クラスターへのアクセスに使用されているクライアント証明書を削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-227">Remove-AzureRmServiceFabricClientCertificate       Remove a client certificate from being used to access a cluster</span></span>
    + <span data-ttu-id="d0f37-228">Remove-AzureRmServiceFabricClusterCertificate       クラスターのセキュリティに使用されているクラスター証明書を削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-228">Remove-AzureRmServiceFabricClusterCertificate       Remove a cluster certificate from being used for cluster security</span></span>
    + <span data-ttu-id="d0f37-229">Remove-AzureRmServiceFabricNodes       クラスターから特定のノード タイプのノードを削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-229">Remove-AzureRmServiceFabricNodes       Remove nodes from a specific node type from a cluster</span></span>
    + <span data-ttu-id="d0f37-230">Remove-AzureRmServiceFabricNodeType       クラスターからノード タイプを 1 つ削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-230">Remove-AzureRmServiceFabricNodeType       Remove a node type from a cluster</span></span>
    + <span data-ttu-id="d0f37-231">Remove-AzureRmServiceFabricSettings       クラスターから 1 つ以上の ServiceFabric 設定を削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-231">Remove-AzureRmServiceFabricSettings       Remove one or more ServiceFabric settings from a cluster</span></span>
    + <span data-ttu-id="d0f37-232">Set-AzureRmServiceFabricSettings       クラスターの 1 つ以上の ServiceFabric 設定を追加または更新します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-232">Set-AzureRmServiceFabricSettings       Add or update one or more ServiceFabric settings of a cluster</span></span>
    + <span data-ttu-id="d0f37-233">Set-AzureRmServiceFabricUpgradeType       クラスターの ServiceFabric アップグレードの種類を変更します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-233">Set-AzureRmServiceFabricUpgradeType       Change the ServiceFabric upgrade type of a cluster</span></span>
    + <span data-ttu-id="d0f37-234">Update-AzureRmServiceFabricDurability       クラスターの持続性層を変更します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-234">Update-AzureRmServiceFabricDurability       Change the durability tier of a cluster</span></span>
    + <span data-ttu-id="d0f37-235">Update-AzureRmServiceFabricReliability       クラスターの信頼性層を変更します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-235">Update-AzureRmServiceFabricReliability       Change the reliability tier of a cluster</span></span>
* <span data-ttu-id="d0f37-236">SQL</span><span class="sxs-lookup"><span data-stu-id="d0f37-236">Sql</span></span>
  - <span data-ttu-id="d0f37-237">New-AzureRmSqlDatabase に -SampleName パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-237">Added -SampleName parameter to New-AzureRmSqlDatabase</span></span>
  - <span data-ttu-id="d0f37-238">フェールオーバー グループのコマンドレットを更新します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-238">Updates to Failover Group cmdlets</span></span>
  - <span data-ttu-id="d0f37-239">"Tag" パラメーターを削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-239">Remove 'Tag' parameters</span></span>
  - <span data-ttu-id="d0f37-240">Remove-AzureRmSqlDatabaseFailoverGroup コマンドレットから "PartnerResourceGroupName" および "PartnerServerName" の各パラメーターを削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-240">Remove 'PartnerResourceGroupName' and 'PartnerServerName' parameters from Remove-AzureRmSqlDatabaseFailoverGroup cmdlet</span></span>
  - <span data-ttu-id="d0f37-241">New- および Set- のコマンドレットに 'GracePeriodWithDataLossHours' パラメーターを追加します。このパラメーターは、最終的に 'GracePeriodWithDataLossHour' に取って代わります。</span><span class="sxs-lookup"><span data-stu-id="d0f37-241">Add 'GracePeriodWithDataLossHours' parameter to New- and Set- cmdlets, which shall eventually replace 'GracePeriodWithDataLossHour'</span></span>
  - <span data-ttu-id="d0f37-242">ドキュメントが拡充および更新されました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-242">Documentation has been fleshed out and updated</span></span>
  - <span data-ttu-id="d0f37-243">返されるオブジェクトの書式変更と、フィールドに値が設定されないバグ (複数) の修正が行われます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-243">Change formatting of returned objects and fix some bugs where fields were not always populated</span></span>
  - <span data-ttu-id="d0f37-244">フェールオーバー グループ オブジェクトに 'DatabaseNames' および 'PartnerLocation' の各プロパティを追加します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-244">Add 'DatabaseNames' and 'PartnerLocation' properties to Failover Group object</span></span>
  - <span data-ttu-id="d0f37-245">Switch- コマンドレットで引き起こされる、操作の完了まで待機されずに直ちに制御が戻るというバグが修正されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-245">Fix bug causing Switch- cmdlet to return immediately rather than waiting for operation to complete</span></span>
  - <span data-ttu-id="d0f37-246">大きな値の猶予期間を使用した際の整数オーバーフローのバグが修正されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-246">Fix integer overflow bug when high grace period values are used</span></span>
  - <span data-ttu-id="d0f37-247">猶予期間に小さい値が指定されている場合は、最小値の 1 時間に調整されます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-247">Adjust grace period to a minimum of 1 hour if a lower one is provided</span></span>
  - <span data-ttu-id="d0f37-248">Set-AzureRmSqlDatabaseThreatDetectionPolicy コマンドレットと Set-AzureRmSqlServerThreatDetectionPolicy コマンドレットの "ExcludedDetectionType" パラメーターの有効な値から "Usage_Anomaly" を削除します。</span><span class="sxs-lookup"><span data-stu-id="d0f37-248">Remove "Usage_Anomaly" from the accepted values for "ExcludedDetectionType" parameter of Set-AzureRmSqlDatabaseThreatDetectionPolicy cmdlet and Set-AzureRmSqlServerThreatDetectionPolicy cmdlet.</span></span>
* <span data-ttu-id="d0f37-249">Storage</span><span class="sxs-lookup"><span data-stu-id="d0f37-249">Storage</span></span>
  - <span data-ttu-id="d0f37-250">SRP SDK が 6.3.0 にアップグレードされます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-250">Upgrade SRP SDK to 6.3.0</span></span>
  - <span data-ttu-id="d0f37-251">New/Set-AzureRmStorageAccount: EnableHttpsTrafficOnly をサポートするように、新しいパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-251">New/Set-AzureRmStorageAccount:Add a new parameter to support EnableHttpsTrafficOnly</span></span>
  - <span data-ttu-id="d0f37-252">New/Set/Get-AzureRmStorageAccount: 返されるストレージ アカウントに新しい EnableHttpsTrafficOnly 属性が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-252">New/Set/Get-AzureRmStorageAccount: Returned Storage Account contains a new attribute EnableHttpsTrafficOnly</span></span>
* <span data-ttu-id="d0f37-253">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="d0f37-253">Azure.Storage</span></span>
  - <span data-ttu-id="d0f37-254">Azure Storage クライアント ライブラリ 8.1.1 および Azure Storage データ移動ライブラリ 0.5.1 にアップグレードされます。</span><span class="sxs-lookup"><span data-stu-id="d0f37-254">Upgrade to Azure Storage Client Library 8.1.1 and Azure Storage DataMovement Library 0.5.1</span></span>
  - <span data-ttu-id="d0f37-255">BLOB 増分コピー機能をサポートするように、新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="d0f37-255">Add a new cmdlet to support blob Incremental Copy feature</span></span>
