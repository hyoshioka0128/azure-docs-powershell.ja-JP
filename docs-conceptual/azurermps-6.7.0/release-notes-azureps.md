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
ms.openlocfilehash: 2a6e20137f12ae9317c7eeed330a2433774e1ea9
ms.sourcegitcommit: 7df99dc139e93a8a4e6d5b1a27968857588d75dd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/16/2018
ms.locfileid: "40106753"
---
# <a name="release-notes"></a><span data-ttu-id="14256-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="14256-103">Release notes</span></span>

<span data-ttu-id="14256-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="14256-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="670---august-2018"></a><span data-ttu-id="14256-105">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="14256-105">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="14256-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-106">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-107">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-107">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="14256-108">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-108">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="14256-109">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-109">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="14256-110">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="14256-110">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="14256-111">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="14256-111">Azure.Storage</span></span>
* <span data-ttu-id="14256-112">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="14256-112">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="14256-113">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="14256-113">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="14256-114">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="14256-114">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="14256-115">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-115">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="14256-116">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="14256-116">Azure.AnalysisServices</span></span>
* <span data-ttu-id="14256-117">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-117">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="14256-118">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="14256-118">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="14256-119">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-119">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="14256-120">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="14256-120">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="14256-121">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-121">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="14256-122">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="14256-122">AzureRM.Automation</span></span>
* <span data-ttu-id="14256-123">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-123">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="14256-124">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="14256-124">AzureRM.Backup</span></span>
* <span data-ttu-id="14256-125">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-125">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="14256-126">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="14256-126">AzureRM.Batch</span></span>
* <span data-ttu-id="14256-127">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-127">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="14256-128">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="14256-128">AzureRM.Billing</span></span>
* <span data-ttu-id="14256-129">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-129">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="14256-130">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="14256-130">AzureRM.Cdn</span></span>
* <span data-ttu-id="14256-131">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-131">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="14256-132">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="14256-132">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="14256-133">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-133">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="14256-134">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="14256-134">AzureRM.Compute</span></span>
* <span data-ttu-id="14256-135">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-135">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="14256-136">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-136">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="14256-137">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="14256-137">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="14256-138">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-138">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="14256-139">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-139">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="14256-140">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="14256-140">AzureRM.Consumption</span></span>
* <span data-ttu-id="14256-141">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-141">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="14256-142">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="14256-142">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="14256-143">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-143">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="14256-144">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="14256-144">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="14256-145">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-145">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="14256-146">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="14256-146">AzureRM.DataFactories</span></span>
* <span data-ttu-id="14256-147">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-147">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="14256-148">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="14256-148">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="14256-149">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-149">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="14256-150">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="14256-150">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="14256-151">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-151">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="14256-152">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="14256-152">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="14256-153">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-153">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="14256-154">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-154">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="14256-155">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-155">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="14256-156">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-156">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="14256-157">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="14256-157">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="14256-158">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="14256-159">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="14256-159">AzureRM.Dns</span></span>
* <span data-ttu-id="14256-160">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="14256-161">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="14256-161">AzureRM.EventGrid</span></span>
* <span data-ttu-id="14256-162">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="14256-163">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="14256-163">AzureRM.EventHub</span></span>
* <span data-ttu-id="14256-164">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-164">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="14256-165">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="14256-165">AzureRM.HDInsight</span></span>
* <span data-ttu-id="14256-166">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-166">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="14256-167">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="14256-167">AzureRM.Insights</span></span>
* <span data-ttu-id="14256-168">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-168">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="14256-169">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="14256-169">AzureRM.IotHub</span></span>
* <span data-ttu-id="14256-170">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="14256-171">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="14256-171">AzureRM.KeyVault</span></span>
* <span data-ttu-id="14256-172">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="14256-173">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="14256-173">AzureRM.LogicApp</span></span>
* <span data-ttu-id="14256-174">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="14256-175">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="14256-175">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="14256-176">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="14256-177">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="14256-177">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="14256-178">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="14256-179">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="14256-179">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="14256-180">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="14256-181">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="14256-181">AzureRM.Media</span></span>
* <span data-ttu-id="14256-182">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-182">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="14256-183">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="14256-183">AzureRM.Network</span></span>
* <span data-ttu-id="14256-184">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-184">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="14256-185">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-185">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="14256-186">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-186">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="14256-187">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-187">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="14256-188">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-188">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="14256-189">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-189">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="14256-190">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="14256-190">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="14256-191">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="14256-191">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="14256-192">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="14256-192">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="14256-193">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="14256-194">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="14256-194">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="14256-195">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="14256-196">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="14256-196">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="14256-197">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="14256-198">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="14256-198">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="14256-199">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="14256-200">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="14256-200">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="14256-201">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="14256-202">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="14256-202">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="14256-203">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-203">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="14256-204">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="14256-204">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="14256-205">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-205">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="14256-206">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-206">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="14256-207">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-207">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="14256-208">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="14256-208">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="14256-209">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="14256-209">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="14256-210">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="14256-210">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="14256-211">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="14256-212">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="14256-212">AzureRM.RedisCache</span></span>
* <span data-ttu-id="14256-213">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="14256-214">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="14256-214">AzureRM.Relay</span></span>
* <span data-ttu-id="14256-215">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="14256-216">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="14256-216">AzureRM.Resources</span></span>
* <span data-ttu-id="14256-217">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="14256-217">Support template deployment at subscription scope.</span></span> <span data-ttu-id="14256-218">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-218">Add new Cmdlets:</span></span>
    - <span data-ttu-id="14256-219">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="14256-219">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="14256-220">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="14256-220">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="14256-221">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="14256-221">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="14256-222">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="14256-222">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="14256-223">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="14256-223">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="14256-224">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="14256-224">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="14256-225">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="14256-225">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="14256-226">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-226">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="14256-227">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-227">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="14256-228">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="14256-229">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="14256-229">AzureRM.Scheduler</span></span>
* <span data-ttu-id="14256-230">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="14256-231">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="14256-231">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="14256-232">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="14256-233">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14256-233">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="14256-234">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="14256-235">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-235">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-236">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="14256-237">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="14256-237">AzureRM.Storage</span></span>
* <span data-ttu-id="14256-238">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="14256-239">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="14256-239">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="14256-240">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="14256-241">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="14256-241">AzureRM.Tags</span></span>
* <span data-ttu-id="14256-242">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="14256-243">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="14256-243">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="14256-244">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="14256-245">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="14256-245">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="14256-246">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="14256-247">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="14256-247">AzureRM.Websites</span></span>
* <span data-ttu-id="14256-248">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="14256-249">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="14256-249">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="14256-250">全般</span><span class="sxs-lookup"><span data-stu-id="14256-250">General</span></span>
* <span data-ttu-id="14256-251">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-251">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="14256-252">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-252">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-253">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-253">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="14256-254">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-254">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="14256-255">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="14256-255">Azure.Storage</span></span>
* <span data-ttu-id="14256-256">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-256">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="14256-257">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-257">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="14256-258">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="14256-258">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="14256-259">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="14256-259">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="14256-260">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-260">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="14256-261">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="14256-261">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="14256-262">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-262">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="14256-263">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="14256-263">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="14256-264">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="14256-264">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="14256-265">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="14256-265">AzureRM.Compute</span></span>
* <span data-ttu-id="14256-266">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-266">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="14256-267">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-267">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="14256-268">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="14256-268">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="14256-269">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="14256-269">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="14256-270">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-270">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="14256-271">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-271">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="14256-272">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-272">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="14256-273">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-273">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="14256-274">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-274">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="14256-275">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-275">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="14256-276">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="14256-276">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="14256-277">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-277">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="14256-278">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="14256-278">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="14256-279">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-279">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="14256-280">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-280">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="14256-281">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="14256-281">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="14256-282">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-282">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="14256-283">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="14256-283">AzureRM.EventHub</span></span>
* <span data-ttu-id="14256-284">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-284">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="14256-285">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="14256-285">AzureRM.Insights</span></span>
* <span data-ttu-id="14256-286">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-286">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="14256-287">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="14256-287">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="14256-288">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="14256-288">AzureRM.KeyVault</span></span>
* <span data-ttu-id="14256-289">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-289">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="14256-290">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="14256-290">AzureRM.Network</span></span>
* <span data-ttu-id="14256-291">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-291">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="14256-292">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="14256-292">AzureRM.Resources</span></span>
* <span data-ttu-id="14256-293">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-293">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="14256-294">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-294">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="14256-295">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="14256-295">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="14256-296">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-296">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="14256-297">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-297">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="14256-298">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-298">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-299">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-299">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="14256-300">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="14256-300">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="14256-301">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-301">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="14256-302">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="14256-302">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="14256-303">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="14256-303">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="14256-304">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="14256-304">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="14256-305">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-305">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="14256-306">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-306">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="14256-307">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="14256-307">AzureRM.Storage</span></span>
* <span data-ttu-id="14256-308">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-308">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="14256-309">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="14256-309">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="14256-310">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="14256-310">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="14256-311">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="14256-311">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="14256-312">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="14256-312">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="14256-313">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="14256-313">AzureRM.Tags</span></span>
* <span data-ttu-id="14256-314">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="14256-314">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="14256-315">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="14256-315">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="14256-316">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-316">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-317">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-317">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="14256-318">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="14256-318">Azure.Storage</span></span>
* <span data-ttu-id="14256-319">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="14256-319">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="14256-320">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="14256-320">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="14256-321">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="14256-321">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="14256-322">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="14256-322">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="14256-323">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-323">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="14256-324">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="14256-324">AzureRM.Automation</span></span>
* <span data-ttu-id="14256-325">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-325">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="14256-326">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="14256-326">AzureRM.Compute</span></span>
* <span data-ttu-id="14256-327">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-327">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="14256-328">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-328">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="14256-329">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-329">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="14256-330">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-330">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="14256-331">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="14256-331">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="14256-332">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="14256-332">AzureRM.EventHub</span></span>
* <span data-ttu-id="14256-333">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-333">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="14256-334">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="14256-334">AzureRM.KeyVault</span></span>
* <span data-ttu-id="14256-335">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-335">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="14256-336">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="14256-336">AzureRM.LogicApp</span></span>
* <span data-ttu-id="14256-337">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-337">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="14256-338">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="14256-338">AzureRM.Network</span></span>
* <span data-ttu-id="14256-339">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="14256-339">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="14256-340">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-340">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="14256-341">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-341">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="14256-342">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-342">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="14256-343">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-343">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="14256-344">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="14256-344">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="14256-345">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="14256-345">AzureRM.Relay</span></span>
* <span data-ttu-id="14256-346">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-346">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="14256-347">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="14256-347">AzureRM.Resources</span></span>
* <span data-ttu-id="14256-348">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-348">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="14256-349">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="14256-349">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="14256-350">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-350">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="14256-351">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-351">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="14256-352">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-352">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="14256-353">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="14256-353">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="14256-354">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-354">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="14256-355">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-355">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="14256-356">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="14256-356">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="14256-357">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="14256-357">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="14256-358">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="14256-358">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="14256-359">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="14256-359">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="14256-360">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="14256-360">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="14256-361">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-361">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="14256-362">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14256-362">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="14256-363">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-363">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="14256-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-364">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-365">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-365">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="14256-366">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="14256-366">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="14256-367">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="14256-367">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="14256-368">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="14256-368">AzureRM.Websites</span></span>
* <span data-ttu-id="14256-369">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="14256-369">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="14256-370">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-370">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="14256-371">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="14256-371">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="14256-372">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="14256-372">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="14256-373">全般</span><span class="sxs-lookup"><span data-stu-id="14256-373">General</span></span>
* <span data-ttu-id="14256-374">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-374">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="14256-375">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-375">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-376">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="14256-376">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="14256-377">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="14256-377">AzureRM.Compute</span></span>
* <span data-ttu-id="14256-378">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="14256-378">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="14256-379">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="14256-379">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="14256-380">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="14256-380">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="14256-381">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="14256-381">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="14256-382">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="14256-382">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="14256-383">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="14256-383">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="14256-384">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="14256-384">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="14256-385">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="14256-385">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="14256-386">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="14256-386">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="14256-387">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="14256-387">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="14256-388">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="14256-388">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="14256-389">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="14256-389">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="14256-390">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="14256-390">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="14256-391">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="14256-391">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="14256-392">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="14256-392">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="14256-393">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-393">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="14256-394">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-394">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="14256-395">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="14256-395">AzureRM.EventHub</span></span>
* <span data-ttu-id="14256-396">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-396">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="14256-397">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-397">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="14256-398">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="14256-398">Provided Default Parameter set.</span></span>
* <span data-ttu-id="14256-399">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="14256-399">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="14256-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="14256-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="14256-401">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-401">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="14256-402">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="14256-402">AzureRM.Network</span></span>
* <span data-ttu-id="14256-403">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="14256-403">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="14256-404">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-404">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="14256-405">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-405">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="14256-406">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-406">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="14256-407">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-407">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="14256-408">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-408">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="14256-409">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-409">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="14256-410">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-410">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="14256-411">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-411">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="14256-412">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-412">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="14256-413">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="14256-413">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="14256-414">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-414">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="14256-415">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="14256-415">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="14256-416">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="14256-416">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="14256-417">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="14256-417">AzureRM.Resources</span></span>
* <span data-ttu-id="14256-418">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-418">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="14256-419">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="14256-419">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="14256-420">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="14256-420">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="14256-421">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-421">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="14256-422">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-422">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="14256-423">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-423">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="14256-424">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-424">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="14256-425">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-425">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="14256-426">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-426">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="14256-427">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-427">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="14256-428">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-428">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="14256-429">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-429">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="14256-430">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-430">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="14256-431">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="14256-431">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="14256-432">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="14256-432">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="14256-433">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-433">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-434">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="14256-434">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="14256-435">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-435">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="14256-436">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="14256-436">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="14256-437">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-437">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-438">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-438">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="14256-439">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="14256-439">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="14256-440">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="14256-440">Azure.Storage</span></span>
* <span data-ttu-id="14256-441">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-441">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="14256-442">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="14256-442">AzureRM.Compute</span></span>
* <span data-ttu-id="14256-443">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-443">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="14256-444">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-444">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="14256-445">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="14256-445">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="14256-446">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="14256-446">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="14256-447">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="14256-447">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="14256-448">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-448">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="14256-449">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="14256-449">Start-AzureRmVM</span></span>
    - <span data-ttu-id="14256-450">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="14256-450">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="14256-451">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="14256-451">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="14256-452">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="14256-452">Set-AzureRmVM</span></span>
    - <span data-ttu-id="14256-453">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="14256-453">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="14256-454">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="14256-454">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="14256-455">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="14256-455">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="14256-456">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="14256-456">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="14256-457">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="14256-457">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="14256-458">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="14256-458">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="14256-459">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="14256-459">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="14256-460">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="14256-460">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="14256-461">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="14256-461">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="14256-462">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="14256-462">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="14256-463">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="14256-463">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="14256-464">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="14256-464">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="14256-465">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="14256-465">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="14256-466">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="14256-466">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="14256-467">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="14256-467">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="14256-468">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="14256-468">AzureRM.EventGrid</span></span>
* <span data-ttu-id="14256-469">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="14256-469">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="14256-470">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="14256-470">AzureRM.KeyVault</span></span>
* <span data-ttu-id="14256-471">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-471">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="14256-472">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="14256-472">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="14256-473">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="14256-473">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="14256-474">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="14256-474">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="14256-475">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-475">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="14256-476">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="14256-476">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="14256-477">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-477">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="14256-478">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="14256-478">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="14256-479">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-479">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-480">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-480">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="14256-481">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="14256-481">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="14256-482">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-482">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="14256-483">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="14256-483">AzureRM.Websites</span></span>
* <span data-ttu-id="14256-484">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="14256-484">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="14256-485">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="14256-485">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="14256-486">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="14256-486">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="14256-487">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="14256-487">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="14256-488">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-488">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="14256-489">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="14256-489">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="14256-490">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-490">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-491">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-491">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="14256-492">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="14256-492">AzureRM.Compute</span></span>
* <span data-ttu-id="14256-493">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="14256-493">VMSS VM Update feature</span></span>
    - <span data-ttu-id="14256-494">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-494">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="14256-495">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-495">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="14256-496">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="14256-496">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="14256-497">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-497">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="14256-498">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-498">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="14256-499">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-499">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="14256-500">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-500">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="14256-501">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="14256-501">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="14256-502">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="14256-502">AzureRM.KeyVault</span></span>
* <span data-ttu-id="14256-503">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-503">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="14256-504">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="14256-504">AzureRM.Network</span></span>
* <span data-ttu-id="14256-505">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="14256-505">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="14256-506">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="14256-506">AzureRM.Resources</span></span>
* <span data-ttu-id="14256-507">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-507">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="14256-508">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="14256-508">AzureRM.Scheduler</span></span>
* <span data-ttu-id="14256-509">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="14256-509">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="14256-510">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-510">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-511">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="14256-511">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="14256-512">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="14256-512">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="14256-513">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="14256-513">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="14256-514">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="14256-514">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="14256-515">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="14256-515">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="14256-516">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="14256-516">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="14256-517">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="14256-517">AzureRM.Websites</span></span>
* <span data-ttu-id="14256-518">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="14256-518">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="14256-519">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="14256-519">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="14256-520">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="14256-520">AzureRM.Profile</span></span>
* <span data-ttu-id="14256-521">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-521">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="14256-522">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="14256-522">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="14256-523">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="14256-523">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="14256-524">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="14256-524">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="14256-525">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-525">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="14256-526">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-526">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="14256-527">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-527">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="14256-528">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="14256-528">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="14256-529">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-529">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="14256-530">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-530">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="14256-531">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-531">Added support for MSI identity</span></span>
* <span data-ttu-id="14256-532">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="14256-532">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="14256-533">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="14256-533">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="14256-534">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="14256-534">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="14256-535">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="14256-535">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="14256-536">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="14256-536">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="14256-537">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="14256-537">AzureRM.Batch</span></span>
* <span data-ttu-id="14256-538">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="14256-538">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="14256-539">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="14256-539">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="14256-540">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="14256-540">AzureRM.Consumption</span></span>
* <span data-ttu-id="14256-541">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-541">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="14256-542">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="14256-542">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="14256-543">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-543">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="14256-544">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-544">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="14256-545">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-545">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="14256-546">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="14256-546">AzureRM.Network</span></span>
* <span data-ttu-id="14256-547">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="14256-547">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="14256-548">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-548">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="14256-549">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="14256-549">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="14256-550">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-550">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="14256-551">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="14256-551">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="14256-552">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-552">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="14256-553">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="14256-553">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="14256-554">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="14256-554">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="14256-555">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="14256-555">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="14256-556">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="14256-556">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="14256-557">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="14256-557">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="14256-558">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="14256-558">AzureRM.Sql</span></span>
* <span data-ttu-id="14256-559">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="14256-559">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="14256-560">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="14256-560">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="14256-561">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="14256-561">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="14256-562">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="14256-562">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="14256-563">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="14256-563">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="14256-564">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="14256-564">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="14256-565">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="14256-565">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="14256-566">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="14256-566">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="14256-567">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="14256-567">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="14256-568">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="14256-568">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="14256-569">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="14256-569">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="14256-570">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="14256-570">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
