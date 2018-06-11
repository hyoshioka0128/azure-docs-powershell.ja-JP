---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: f90c77d8c9cd78315264fb0a0a58e047aefc5041
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821872"
---
# <a name="release-notes"></a><span data-ttu-id="bb6d8-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="bb6d8-103">Release notes</span></span>

<span data-ttu-id="bb6d8-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="620---june-2018"></a><span data-ttu-id="bb6d8-105">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="bb6d8-105">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="bb6d8-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="bb6d8-106">AzureRM.Profile</span></span>
* <span data-ttu-id="bb6d8-107">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-107">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="bb6d8-108">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="bb6d8-108">AzureRM.Compute</span></span>
* <span data-ttu-id="bb6d8-109">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="bb6d8-109">VMSS VM Update feature</span></span>
    - <span data-ttu-id="bb6d8-110">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-110">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="bb6d8-111">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-111">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="bb6d8-112">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="bb6d8-112">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="bb6d8-113">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-113">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="bb6d8-114">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-114">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="bb6d8-115">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-115">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="bb6d8-116">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-116">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="bb6d8-117">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-117">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="bb6d8-118">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bb6d8-118">AzureRM.KeyVault</span></span>
* <span data-ttu-id="bb6d8-119">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-119">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="bb6d8-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="bb6d8-120">AzureRM.Network</span></span>
* <span data-ttu-id="bb6d8-121">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-121">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="bb6d8-122">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="bb6d8-122">AzureRM.Resources</span></span>
* <span data-ttu-id="bb6d8-123">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-123">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="bb6d8-124">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="bb6d8-124">AzureRM.Scheduler</span></span>
* <span data-ttu-id="bb6d8-125">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-125">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="bb6d8-126">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="bb6d8-126">AzureRM.Sql</span></span>
* <span data-ttu-id="bb6d8-127">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="bb6d8-127">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="bb6d8-128">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bb6d8-128">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="bb6d8-129">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="bb6d8-129">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="bb6d8-130">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="bb6d8-130">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="bb6d8-131">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="bb6d8-131">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="bb6d8-132">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bb6d8-132">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="bb6d8-133">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="bb6d8-133">AzureRM.Websites</span></span>
* <span data-ttu-id="bb6d8-134">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-134">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="bb6d8-135">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="bb6d8-135">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="bb6d8-136">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="bb6d8-136">AzureRM.Profile</span></span>
* <span data-ttu-id="bb6d8-137">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-137">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="bb6d8-138">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="bb6d8-138">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="bb6d8-139">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-139">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="bb6d8-140">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bb6d8-140">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="bb6d8-141">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-141">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="bb6d8-142">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-142">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="bb6d8-143">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-143">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="bb6d8-144">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-144">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="bb6d8-145">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-145">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="bb6d8-146">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-146">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="bb6d8-147">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-147">Added support for MSI identity</span></span>
* <span data-ttu-id="bb6d8-148">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-148">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="bb6d8-149">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="bb6d8-149">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="bb6d8-150">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb6d8-150">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="bb6d8-151">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="bb6d8-151">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="bb6d8-152">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="bb6d8-152">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="bb6d8-153">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="bb6d8-153">AzureRM.Batch</span></span>
* <span data-ttu-id="bb6d8-154">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-154">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="bb6d8-155">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-155">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="bb6d8-156">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="bb6d8-156">AzureRM.Consumption</span></span>
* <span data-ttu-id="bb6d8-157">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-157">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="bb6d8-158">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bb6d8-158">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="bb6d8-159">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-159">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="bb6d8-160">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-160">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="bb6d8-161">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-161">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="bb6d8-162">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="bb6d8-162">AzureRM.Network</span></span>
* <span data-ttu-id="bb6d8-163">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-163">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="bb6d8-164">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-164">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="bb6d8-165">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="bb6d8-165">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="bb6d8-166">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-166">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="bb6d8-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="bb6d8-167">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="bb6d8-168">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-168">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="bb6d8-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="bb6d8-169">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="bb6d8-170">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-170">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="bb6d8-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="bb6d8-171">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="bb6d8-172">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bb6d8-172">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="bb6d8-173">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-173">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="bb6d8-174">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="bb6d8-174">AzureRM.Sql</span></span>
* <span data-ttu-id="bb6d8-175">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-175">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="bb6d8-176">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="bb6d8-176">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="bb6d8-177">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-177">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="bb6d8-178">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-178">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="bb6d8-179">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-179">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="bb6d8-180">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bb6d8-180">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="bb6d8-181">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="bb6d8-181">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="bb6d8-182">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="bb6d8-182">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="bb6d8-183">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="bb6d8-183">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="bb6d8-184">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bb6d8-184">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="bb6d8-185">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="bb6d8-185">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="bb6d8-186">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="bb6d8-186">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>