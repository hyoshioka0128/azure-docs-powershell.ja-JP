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
ms.openlocfilehash: e9fa2d75c1c4e6ffaa2f7dd8e400f5b13dd4527d
ms.sourcegitcommit: 8b882d1c27d9e323447ff85f56d11bbf5e244d7f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/18/2018
ms.locfileid: "39110485"
---
# <a name="release-notes"></a><span data-ttu-id="fa33a-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="fa33a-103">Release notes</span></span>

<span data-ttu-id="fa33a-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="fa33a-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="650---july-2018"></a><span data-ttu-id="fa33a-105">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="fa33a-105">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fa33a-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fa33a-106">AzureRM.Profile</span></span>
* <span data-ttu-id="fa33a-107">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-107">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="fa33a-108">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fa33a-108">Azure.Storage</span></span>
* <span data-ttu-id="fa33a-109">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="fa33a-109">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="fa33a-110">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="fa33a-110">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="fa33a-111">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="fa33a-111">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="fa33a-112">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="fa33a-112">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="fa33a-113">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-113">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="fa33a-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="fa33a-114">AzureRM.Automation</span></span>
* <span data-ttu-id="fa33a-115">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-115">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fa33a-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fa33a-116">AzureRM.Compute</span></span>
* <span data-ttu-id="fa33a-117">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-117">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="fa33a-118">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-118">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="fa33a-119">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-119">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="fa33a-120">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-120">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="fa33a-121">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-121">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="fa33a-122">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="fa33a-122">AzureRM.EventHub</span></span>
* <span data-ttu-id="fa33a-123">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-123">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fa33a-124">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa33a-124">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fa33a-125">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-125">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="fa33a-126">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="fa33a-126">AzureRM.LogicApp</span></span>
* <span data-ttu-id="fa33a-127">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-127">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fa33a-128">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fa33a-128">AzureRM.Network</span></span>
* <span data-ttu-id="fa33a-129">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="fa33a-129">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="fa33a-130">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-130">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="fa33a-131">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-131">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="fa33a-132">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-132">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="fa33a-133">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-133">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="fa33a-134">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-134">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="fa33a-135">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="fa33a-135">AzureRM.Relay</span></span>
* <span data-ttu-id="fa33a-136">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-136">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fa33a-137">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fa33a-137">AzureRM.Resources</span></span>
* <span data-ttu-id="fa33a-138">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-138">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="fa33a-139">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-139">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="fa33a-140">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-140">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="fa33a-141">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-141">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="fa33a-142">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-142">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="fa33a-143">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fa33a-143">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fa33a-144">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-144">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="fa33a-145">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-145">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="fa33a-146">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fa33a-146">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fa33a-147">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fa33a-147">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fa33a-148">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fa33a-148">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fa33a-149">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fa33a-149">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="fa33a-150">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="fa33a-150">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="fa33a-151">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-151">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="fa33a-152">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fa33a-152">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="fa33a-153">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-153">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fa33a-154">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fa33a-154">AzureRM.Sql</span></span>
* <span data-ttu-id="fa33a-155">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-155">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="fa33a-156">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="fa33a-156">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="fa33a-157">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="fa33a-157">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fa33a-158">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fa33a-158">AzureRM.Websites</span></span>
* <span data-ttu-id="fa33a-159">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="fa33a-159">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="fa33a-160">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-160">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="fa33a-161">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="fa33a-161">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="fa33a-162">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="fa33a-162">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="fa33a-163">全般</span><span class="sxs-lookup"><span data-stu-id="fa33a-163">General</span></span>
* <span data-ttu-id="fa33a-164">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-164">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="fa33a-165">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fa33a-165">AzureRM.Profile</span></span>
* <span data-ttu-id="fa33a-166">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-166">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fa33a-167">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fa33a-167">AzureRM.Compute</span></span>
* <span data-ttu-id="fa33a-168">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="fa33a-168">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="fa33a-169">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-169">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="fa33a-170">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-170">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="fa33a-171">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="fa33a-171">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="fa33a-172">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-172">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="fa33a-173">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="fa33a-173">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="fa33a-174">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-174">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="fa33a-175">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="fa33a-175">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="fa33a-176">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-176">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="fa33a-177">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="fa33a-177">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="fa33a-178">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="fa33a-178">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="fa33a-179">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="fa33a-179">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fa33a-180">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fa33a-180">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fa33a-181">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="fa33a-181">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="fa33a-182">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="fa33a-182">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="fa33a-183">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-183">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="fa33a-184">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-184">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="fa33a-185">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="fa33a-185">AzureRM.EventHub</span></span>
* <span data-ttu-id="fa33a-186">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-186">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="fa33a-187">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-187">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="fa33a-188">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="fa33a-188">Provided Default Parameter set.</span></span>
* <span data-ttu-id="fa33a-189">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="fa33a-189">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fa33a-190">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa33a-190">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fa33a-191">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-191">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="fa33a-192">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fa33a-192">AzureRM.Network</span></span>
* <span data-ttu-id="fa33a-193">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-193">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="fa33a-194">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-194">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="fa33a-195">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-195">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="fa33a-196">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-196">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="fa33a-197">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-197">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="fa33a-198">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-198">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="fa33a-199">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-199">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="fa33a-200">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-200">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="fa33a-201">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-201">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="fa33a-202">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-202">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="fa33a-203">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="fa33a-203">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="fa33a-204">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-204">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="fa33a-205">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="fa33a-205">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="fa33a-206">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="fa33a-206">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fa33a-207">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fa33a-207">AzureRM.Resources</span></span>
* <span data-ttu-id="fa33a-208">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-208">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="fa33a-209">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="fa33a-209">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="fa33a-210">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="fa33a-210">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="fa33a-211">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-211">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="fa33a-212">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-212">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="fa33a-213">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-213">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="fa33a-214">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-214">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="fa33a-215">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-215">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="fa33a-216">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-216">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="fa33a-217">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-217">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="fa33a-218">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-218">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="fa33a-219">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-219">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="fa33a-220">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-220">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="fa33a-221">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="fa33a-221">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="fa33a-222">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="fa33a-222">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fa33a-223">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fa33a-223">AzureRM.Sql</span></span>
* <span data-ttu-id="fa33a-224">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-224">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="fa33a-225">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-225">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="fa33a-226">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="fa33a-226">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fa33a-227">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fa33a-227">AzureRM.Profile</span></span>
* <span data-ttu-id="fa33a-228">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-228">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="fa33a-229">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="fa33a-229">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="fa33a-230">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="fa33a-230">Azure.Storage</span></span>
* <span data-ttu-id="fa33a-231">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-231">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fa33a-232">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fa33a-232">AzureRM.Compute</span></span>
* <span data-ttu-id="fa33a-233">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-233">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="fa33a-234">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-234">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="fa33a-235">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="fa33a-235">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="fa33a-236">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="fa33a-236">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="fa33a-237">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="fa33a-237">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="fa33a-238">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-238">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="fa33a-239">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fa33a-239">Start-AzureRmVM</span></span>
    - <span data-ttu-id="fa33a-240">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fa33a-240">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="fa33a-241">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fa33a-241">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="fa33a-242">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="fa33a-242">Set-AzureRmVM</span></span>
    - <span data-ttu-id="fa33a-243">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="fa33a-243">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="fa33a-244">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fa33a-244">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="fa33a-245">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="fa33a-245">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="fa33a-246">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="fa33a-246">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="fa33a-247">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fa33a-247">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="fa33a-248">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fa33a-248">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="fa33a-249">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fa33a-249">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="fa33a-250">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="fa33a-250">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="fa33a-251">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="fa33a-251">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="fa33a-252">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="fa33a-252">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="fa33a-253">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="fa33a-253">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="fa33a-254">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="fa33a-254">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="fa33a-255">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="fa33a-255">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="fa33a-256">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="fa33a-256">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="fa33a-257">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="fa33a-257">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="fa33a-258">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="fa33a-258">AzureRM.EventGrid</span></span>
* <span data-ttu-id="fa33a-259">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-259">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="fa33a-260">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa33a-260">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fa33a-261">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-261">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="fa33a-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="fa33a-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="fa33a-263">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="fa33a-263">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="fa33a-264">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="fa33a-264">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="fa33a-265">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-265">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="fa33a-266">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="fa33a-266">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="fa33a-267">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-267">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="fa33a-268">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="fa33a-268">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fa33a-269">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fa33a-269">AzureRM.Sql</span></span>
* <span data-ttu-id="fa33a-270">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-270">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fa33a-271">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fa33a-271">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fa33a-272">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-272">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fa33a-273">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fa33a-273">AzureRM.Websites</span></span>
* <span data-ttu-id="fa33a-274">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-274">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="fa33a-275">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="fa33a-275">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="fa33a-276">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="fa33a-276">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="fa33a-277">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="fa33a-277">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="fa33a-278">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-278">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="fa33a-279">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="fa33a-279">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fa33a-280">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fa33a-280">AzureRM.Profile</span></span>
* <span data-ttu-id="fa33a-281">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-281">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="fa33a-282">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="fa33a-282">AzureRM.Compute</span></span>
* <span data-ttu-id="fa33a-283">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="fa33a-283">VMSS VM Update feature</span></span>
    - <span data-ttu-id="fa33a-284">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-284">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="fa33a-285">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-285">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="fa33a-286">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="fa33a-286">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="fa33a-287">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-287">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="fa33a-288">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-288">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="fa33a-289">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-289">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="fa33a-290">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-290">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="fa33a-291">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-291">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="fa33a-292">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="fa33a-292">AzureRM.KeyVault</span></span>
* <span data-ttu-id="fa33a-293">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-293">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="fa33a-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fa33a-294">AzureRM.Network</span></span>
* <span data-ttu-id="fa33a-295">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="fa33a-295">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="fa33a-296">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="fa33a-296">AzureRM.Resources</span></span>
* <span data-ttu-id="fa33a-297">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-297">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="fa33a-298">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="fa33a-298">AzureRM.Scheduler</span></span>
* <span data-ttu-id="fa33a-299">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-299">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="fa33a-300">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fa33a-300">AzureRM.Sql</span></span>
* <span data-ttu-id="fa33a-301">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="fa33a-301">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="fa33a-302">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fa33a-302">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="fa33a-303">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="fa33a-303">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="fa33a-304">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="fa33a-304">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="fa33a-305">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="fa33a-305">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="fa33a-306">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fa33a-306">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="fa33a-307">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="fa33a-307">AzureRM.Websites</span></span>
* <span data-ttu-id="fa33a-308">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-308">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="fa33a-309">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="fa33a-309">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="fa33a-310">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="fa33a-310">AzureRM.Profile</span></span>
* <span data-ttu-id="fa33a-311">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-311">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="fa33a-312">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="fa33a-312">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="fa33a-313">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="fa33a-313">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="fa33a-314">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="fa33a-314">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="fa33a-315">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-315">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="fa33a-316">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-316">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="fa33a-317">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-317">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="fa33a-318">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-318">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="fa33a-319">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-319">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="fa33a-320">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-320">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="fa33a-321">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-321">Added support for MSI identity</span></span>
* <span data-ttu-id="fa33a-322">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="fa33a-322">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="fa33a-323">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="fa33a-323">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="fa33a-324">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa33a-324">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="fa33a-325">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="fa33a-325">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="fa33a-326">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="fa33a-326">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="fa33a-327">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="fa33a-327">AzureRM.Batch</span></span>
* <span data-ttu-id="fa33a-328">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-328">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="fa33a-329">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-329">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="fa33a-330">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="fa33a-330">AzureRM.Consumption</span></span>
* <span data-ttu-id="fa33a-331">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-331">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="fa33a-332">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="fa33a-332">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="fa33a-333">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-333">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="fa33a-334">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-334">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="fa33a-335">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-335">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="fa33a-336">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="fa33a-336">AzureRM.Network</span></span>
* <span data-ttu-id="fa33a-337">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-337">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="fa33a-338">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-338">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="fa33a-339">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="fa33a-339">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="fa33a-340">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-340">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="fa33a-341">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="fa33a-341">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="fa33a-342">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-342">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="fa33a-343">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="fa33a-343">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="fa33a-344">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-344">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="fa33a-345">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="fa33a-345">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="fa33a-346">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="fa33a-346">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="fa33a-347">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="fa33a-347">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="fa33a-348">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="fa33a-348">AzureRM.Sql</span></span>
* <span data-ttu-id="fa33a-349">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-349">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="fa33a-350">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="fa33a-350">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="fa33a-351">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-351">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="fa33a-352">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="fa33a-352">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="fa33a-353">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="fa33a-353">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="fa33a-354">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fa33a-354">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="fa33a-355">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="fa33a-355">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="fa33a-356">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="fa33a-356">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="fa33a-357">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="fa33a-357">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="fa33a-358">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="fa33a-358">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="fa33a-359">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="fa33a-359">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="fa33a-360">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="fa33a-360">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>