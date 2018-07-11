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
ms.openlocfilehash: 255e26aea5ea3cea866faa0d095cdf643c8ef0a8
ms.sourcegitcommit: de0e60800df1add9f3400166faacca202ef567d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/03/2018
ms.locfileid: "37406485"
---
# <a name="release-notes"></a><span data-ttu-id="bd0a3-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="bd0a3-103">Release notes</span></span>

<span data-ttu-id="bd0a3-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="640---july-2018"></a><span data-ttu-id="bd0a3-105">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="bd0a3-105">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="bd0a3-106">全般</span><span class="sxs-lookup"><span data-stu-id="bd0a3-106">General</span></span>
* <span data-ttu-id="bd0a3-107">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-107">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="bd0a3-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="bd0a3-108">AzureRM.Profile</span></span>
* <span data-ttu-id="bd0a3-109">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-109">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="bd0a3-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="bd0a3-110">AzureRM.Compute</span></span>
* <span data-ttu-id="bd0a3-111">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="bd0a3-111">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="bd0a3-112">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-112">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="bd0a3-113">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-113">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="bd0a3-114">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="bd0a3-114">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="bd0a3-115">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-115">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="bd0a3-116">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="bd0a3-116">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="bd0a3-117">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-117">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="bd0a3-118">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="bd0a3-118">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="bd0a3-119">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-119">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="bd0a3-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="bd0a3-120">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="bd0a3-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="bd0a3-121">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="bd0a3-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="bd0a3-122">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="bd0a3-123">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bd0a3-123">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="bd0a3-124">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-124">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="bd0a3-125">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-125">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="bd0a3-126">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-126">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="bd0a3-127">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-127">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="bd0a3-128">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="bd0a3-128">AzureRM.EventHub</span></span>
* <span data-ttu-id="bd0a3-129">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-129">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="bd0a3-130">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-130">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="bd0a3-131">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-131">Provided Default Parameter set.</span></span>
* <span data-ttu-id="bd0a3-132">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-132">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="bd0a3-133">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bd0a3-133">AzureRM.KeyVault</span></span>
* <span data-ttu-id="bd0a3-134">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-134">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="bd0a3-135">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="bd0a3-135">AzureRM.Network</span></span>
* <span data-ttu-id="bd0a3-136">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-136">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="bd0a3-137">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-137">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="bd0a3-138">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-138">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="bd0a3-139">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-139">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="bd0a3-140">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-140">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="bd0a3-141">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-141">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="bd0a3-142">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-142">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="bd0a3-143">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-143">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="bd0a3-144">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-144">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="bd0a3-145">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-145">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="bd0a3-146">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="bd0a3-146">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="bd0a3-147">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-147">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="bd0a3-148">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-148">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="bd0a3-149">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-149">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="bd0a3-150">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="bd0a3-150">AzureRM.Resources</span></span>
* <span data-ttu-id="bd0a3-151">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-151">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="bd0a3-152">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-152">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="bd0a3-153">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-153">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="bd0a3-154">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-154">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="bd0a3-155">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-155">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="bd0a3-156">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-156">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="bd0a3-157">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-157">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="bd0a3-158">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-158">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="bd0a3-159">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-159">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="bd0a3-160">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-160">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="bd0a3-161">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-161">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="bd0a3-162">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-162">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="bd0a3-163">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-163">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="bd0a3-164">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="bd0a3-164">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="bd0a3-165">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-165">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="bd0a3-166">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="bd0a3-166">AzureRM.Sql</span></span>
* <span data-ttu-id="bd0a3-167">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-167">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="bd0a3-168">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-168">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="bd0a3-169">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="bd0a3-169">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="bd0a3-170">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="bd0a3-170">AzureRM.Profile</span></span>
* <span data-ttu-id="bd0a3-171">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-171">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="bd0a3-172">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="bd0a3-172">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="bd0a3-173">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="bd0a3-173">Azure.Storage</span></span>
* <span data-ttu-id="bd0a3-174">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-174">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="bd0a3-175">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="bd0a3-175">AzureRM.Compute</span></span>
* <span data-ttu-id="bd0a3-176">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-176">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="bd0a3-177">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-177">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="bd0a3-178">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="bd0a3-178">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="bd0a3-179">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="bd0a3-179">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="bd0a3-180">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="bd0a3-180">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="bd0a3-181">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-181">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="bd0a3-182">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="bd0a3-182">Start-AzureRmVM</span></span>
    - <span data-ttu-id="bd0a3-183">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="bd0a3-183">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="bd0a3-184">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="bd0a3-184">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="bd0a3-185">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="bd0a3-185">Set-AzureRmVM</span></span>
    - <span data-ttu-id="bd0a3-186">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="bd0a3-186">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="bd0a3-187">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="bd0a3-187">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="bd0a3-188">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="bd0a3-188">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="bd0a3-189">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="bd0a3-189">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="bd0a3-190">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="bd0a3-190">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="bd0a3-191">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="bd0a3-191">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="bd0a3-192">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="bd0a3-192">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="bd0a3-193">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="bd0a3-193">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="bd0a3-194">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="bd0a3-194">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="bd0a3-195">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="bd0a3-195">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="bd0a3-196">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="bd0a3-196">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="bd0a3-197">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="bd0a3-197">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="bd0a3-198">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="bd0a3-198">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="bd0a3-199">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="bd0a3-199">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="bd0a3-200">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="bd0a3-200">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="bd0a3-201">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="bd0a3-201">AzureRM.EventGrid</span></span>
* <span data-ttu-id="bd0a3-202">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-202">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="bd0a3-203">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bd0a3-203">AzureRM.KeyVault</span></span>
* <span data-ttu-id="bd0a3-204">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-204">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="bd0a3-205">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="bd0a3-205">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="bd0a3-206">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="bd0a3-206">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="bd0a3-207">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="bd0a3-207">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="bd0a3-208">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-208">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="bd0a3-209">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="bd0a3-209">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="bd0a3-210">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-210">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="bd0a3-211">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-211">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="bd0a3-212">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="bd0a3-212">AzureRM.Sql</span></span>
* <span data-ttu-id="bd0a3-213">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-213">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="bd0a3-214">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="bd0a3-214">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="bd0a3-215">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-215">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="bd0a3-216">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="bd0a3-216">AzureRM.Websites</span></span>
* <span data-ttu-id="bd0a3-217">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-217">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="bd0a3-218">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-218">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="bd0a3-219">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="bd0a3-219">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="bd0a3-220">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="bd0a3-220">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="bd0a3-221">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-221">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="bd0a3-222">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="bd0a3-222">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="bd0a3-223">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="bd0a3-223">AzureRM.Profile</span></span>
* <span data-ttu-id="bd0a3-224">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-224">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="bd0a3-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="bd0a3-225">AzureRM.Compute</span></span>
* <span data-ttu-id="bd0a3-226">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="bd0a3-226">VMSS VM Update feature</span></span>
    - <span data-ttu-id="bd0a3-227">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-227">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="bd0a3-228">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-228">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="bd0a3-229">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="bd0a3-229">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="bd0a3-230">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-230">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="bd0a3-231">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-231">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="bd0a3-232">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-232">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="bd0a3-233">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-233">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="bd0a3-234">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-234">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="bd0a3-235">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="bd0a3-235">AzureRM.KeyVault</span></span>
* <span data-ttu-id="bd0a3-236">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-236">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="bd0a3-237">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="bd0a3-237">AzureRM.Network</span></span>
* <span data-ttu-id="bd0a3-238">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-238">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="bd0a3-239">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="bd0a3-239">AzureRM.Resources</span></span>
* <span data-ttu-id="bd0a3-240">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-240">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="bd0a3-241">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="bd0a3-241">AzureRM.Scheduler</span></span>
* <span data-ttu-id="bd0a3-242">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-242">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="bd0a3-243">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="bd0a3-243">AzureRM.Sql</span></span>
* <span data-ttu-id="bd0a3-244">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="bd0a3-244">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="bd0a3-245">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bd0a3-245">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="bd0a3-246">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="bd0a3-246">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="bd0a3-247">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="bd0a3-247">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="bd0a3-248">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="bd0a3-248">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="bd0a3-249">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bd0a3-249">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="bd0a3-250">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="bd0a3-250">AzureRM.Websites</span></span>
* <span data-ttu-id="bd0a3-251">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-251">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="bd0a3-252">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="bd0a3-252">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="bd0a3-253">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="bd0a3-253">AzureRM.Profile</span></span>
* <span data-ttu-id="bd0a3-254">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-254">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="bd0a3-255">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="bd0a3-255">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="bd0a3-256">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-256">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="bd0a3-257">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="bd0a3-257">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="bd0a3-258">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-258">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="bd0a3-259">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-259">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="bd0a3-260">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-260">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="bd0a3-261">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-261">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="bd0a3-262">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-262">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="bd0a3-263">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-263">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="bd0a3-264">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-264">Added support for MSI identity</span></span>
* <span data-ttu-id="bd0a3-265">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-265">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="bd0a3-266">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="bd0a3-266">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="bd0a3-267">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd0a3-267">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="bd0a3-268">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="bd0a3-268">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="bd0a3-269">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="bd0a3-269">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="bd0a3-270">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="bd0a3-270">AzureRM.Batch</span></span>
* <span data-ttu-id="bd0a3-271">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-271">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="bd0a3-272">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-272">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="bd0a3-273">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="bd0a3-273">AzureRM.Consumption</span></span>
* <span data-ttu-id="bd0a3-274">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-274">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="bd0a3-275">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="bd0a3-275">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="bd0a3-276">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-276">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="bd0a3-277">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-277">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="bd0a3-278">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-278">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="bd0a3-279">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="bd0a3-279">AzureRM.Network</span></span>
* <span data-ttu-id="bd0a3-280">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-280">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="bd0a3-281">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-281">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="bd0a3-282">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="bd0a3-282">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="bd0a3-283">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-283">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="bd0a3-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="bd0a3-284">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="bd0a3-285">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-285">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="bd0a3-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="bd0a3-286">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="bd0a3-287">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-287">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="bd0a3-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="bd0a3-288">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="bd0a3-289">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="bd0a3-289">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="bd0a3-290">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-290">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="bd0a3-291">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="bd0a3-291">AzureRM.Sql</span></span>
* <span data-ttu-id="bd0a3-292">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-292">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="bd0a3-293">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="bd0a3-293">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="bd0a3-294">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-294">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="bd0a3-295">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-295">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="bd0a3-296">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-296">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="bd0a3-297">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bd0a3-297">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="bd0a3-298">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="bd0a3-298">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="bd0a3-299">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="bd0a3-299">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="bd0a3-300">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="bd0a3-300">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="bd0a3-301">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="bd0a3-301">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="bd0a3-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="bd0a3-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="bd0a3-303">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="bd0a3-303">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>