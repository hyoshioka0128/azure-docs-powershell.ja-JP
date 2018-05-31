---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 5/1/2018
ms.openlocfilehash: 0b7902155c47f2e6355e9147c203867288caab81
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2018
ms.locfileid: "34461897"
---
# <a name="release-notes"></a><span data-ttu-id="848d2-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="848d2-103">Release notes</span></span>

<span data-ttu-id="848d2-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="848d2-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="610---may-2018"></a><span data-ttu-id="848d2-105">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="848d2-105">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="848d2-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="848d2-106">AzureRM.Profile</span></span>
* <span data-ttu-id="848d2-107">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-107">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="848d2-108">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="848d2-108">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="848d2-109">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="848d2-109">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="848d2-110">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="848d2-110">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="848d2-111">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-111">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="848d2-112">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-112">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="848d2-113">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-113">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="848d2-114">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="848d2-114">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="848d2-115">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-115">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="848d2-116">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-116">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="848d2-117">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-117">Added support for MSI identity</span></span>
* <span data-ttu-id="848d2-118">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="848d2-118">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="848d2-119">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="848d2-119">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="848d2-120">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="848d2-120">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="848d2-121">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="848d2-121">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="848d2-122">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="848d2-122">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="848d2-123">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="848d2-123">AzureRM.Batch</span></span>
* <span data-ttu-id="848d2-124">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="848d2-124">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="848d2-125">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="848d2-125">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="848d2-126">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="848d2-126">AzureRM.Consumption</span></span>
* <span data-ttu-id="848d2-127">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-127">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="848d2-128">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="848d2-128">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="848d2-129">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-129">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="848d2-130">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-130">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="848d2-131">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-131">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="848d2-132">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="848d2-132">AzureRM.Network</span></span>
* <span data-ttu-id="848d2-133">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-133">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="848d2-134">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-134">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="848d2-135">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="848d2-135">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="848d2-136">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-136">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="848d2-137">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="848d2-137">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="848d2-138">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-138">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="848d2-139">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="848d2-139">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="848d2-140">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-140">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="848d2-141">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="848d2-141">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="848d2-142">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="848d2-142">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="848d2-143">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="848d2-143">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="848d2-144">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="848d2-144">AzureRM.Sql</span></span>
* <span data-ttu-id="848d2-145">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="848d2-145">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="848d2-146">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="848d2-146">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="848d2-147">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="848d2-147">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="848d2-148">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="848d2-148">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="848d2-149">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="848d2-149">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="848d2-150">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="848d2-150">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="848d2-151">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="848d2-151">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="848d2-152">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="848d2-152">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="848d2-153">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="848d2-153">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="848d2-154">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="848d2-154">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="848d2-155">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="848d2-155">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="848d2-156">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="848d2-156">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>