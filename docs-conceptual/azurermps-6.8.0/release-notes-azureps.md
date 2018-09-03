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
ms.openlocfilehash: 6043d17df1b5e91521bad31e65372c10ee6a5c6a
ms.sourcegitcommit: 9cb98f055a0525c2061f65149965d5e7c3e03ddc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/30/2018
ms.locfileid: "43117381"
---
# <a name="release-notes"></a><span data-ttu-id="96473-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="96473-103">Release notes</span></span>

<span data-ttu-id="96473-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="96473-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="680---august-2018"></a><span data-ttu-id="96473-105">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="96473-105">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="96473-106">全般</span><span class="sxs-lookup"><span data-stu-id="96473-106">General</span></span>
* <span data-ttu-id="96473-107">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-107">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="96473-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-108">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-109">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-109">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-110">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-110">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-111">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-111">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="96473-112">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-112">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="96473-113">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-113">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="96473-114">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="96473-114">AzureRM.IotHub</span></span>
* <span data-ttu-id="96473-115">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-115">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="96473-116">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-116">AzureRM.Network</span></span>
* <span data-ttu-id="96473-117">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="96473-117">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="96473-118">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="96473-118">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="96473-119">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-119">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="96473-120">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="96473-120">AzureRM.Resources</span></span>
* <span data-ttu-id="96473-121">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-121">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="96473-122">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96473-122">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="96473-123">問題の修正</span><span class="sxs-lookup"><span data-stu-id="96473-123">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="96473-124">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="96473-124">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="96473-125">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="96473-125">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="96473-126">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="96473-126">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="96473-127">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="96473-127">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="96473-128">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="96473-128">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="96473-129">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="96473-129">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="96473-130">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="96473-130">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="96473-131">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="96473-131">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="96473-132">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="96473-132">AzureRM.Websites</span></span>
* <span data-ttu-id="96473-133">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-133">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="96473-134">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="96473-134">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="96473-135">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-135">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-136">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-136">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="96473-137">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-137">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="96473-138">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-138">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="96473-139">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="96473-139">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="96473-140">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="96473-140">Azure.Storage</span></span>
* <span data-ttu-id="96473-141">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="96473-141">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="96473-142">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="96473-142">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="96473-143">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96473-143">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="96473-144">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-144">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="96473-145">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96473-145">Azure.AnalysisServices</span></span>
* <span data-ttu-id="96473-146">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-146">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="96473-147">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="96473-147">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="96473-148">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-148">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="96473-149">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="96473-149">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="96473-150">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-150">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="96473-151">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="96473-151">AzureRM.Automation</span></span>
* <span data-ttu-id="96473-152">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-152">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="96473-153">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="96473-153">AzureRM.Backup</span></span>
* <span data-ttu-id="96473-154">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-154">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="96473-155">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="96473-155">AzureRM.Batch</span></span>
* <span data-ttu-id="96473-156">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-156">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="96473-157">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="96473-157">AzureRM.Billing</span></span>
* <span data-ttu-id="96473-158">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-158">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="96473-159">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="96473-159">AzureRM.Cdn</span></span>
* <span data-ttu-id="96473-160">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-160">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="96473-161">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="96473-161">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="96473-162">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-162">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-163">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-163">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-164">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-164">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="96473-165">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-165">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="96473-166">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="96473-166">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="96473-167">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-167">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="96473-168">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-168">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="96473-169">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="96473-169">AzureRM.Consumption</span></span>
* <span data-ttu-id="96473-170">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-170">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="96473-171">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="96473-171">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="96473-172">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-172">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="96473-173">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="96473-173">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="96473-174">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-174">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="96473-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="96473-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="96473-176">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-176">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="96473-177">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="96473-177">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="96473-178">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-178">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="96473-179">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="96473-179">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="96473-180">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-180">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="96473-181">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96473-181">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="96473-182">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-182">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="96473-183">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-183">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="96473-184">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-184">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="96473-185">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-185">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="96473-186">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="96473-186">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="96473-187">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="96473-188">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="96473-188">AzureRM.Dns</span></span>
* <span data-ttu-id="96473-189">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="96473-190">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="96473-190">AzureRM.EventGrid</span></span>
* <span data-ttu-id="96473-191">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="96473-192">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="96473-192">AzureRM.EventHub</span></span>
* <span data-ttu-id="96473-193">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="96473-194">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="96473-194">AzureRM.HDInsight</span></span>
* <span data-ttu-id="96473-195">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="96473-196">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="96473-196">AzureRM.Insights</span></span>
* <span data-ttu-id="96473-197">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="96473-198">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="96473-198">AzureRM.IotHub</span></span>
* <span data-ttu-id="96473-199">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="96473-200">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96473-200">AzureRM.KeyVault</span></span>
* <span data-ttu-id="96473-201">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-201">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="96473-202">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="96473-202">AzureRM.LogicApp</span></span>
* <span data-ttu-id="96473-203">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-203">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="96473-204">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="96473-204">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="96473-205">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-205">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="96473-206">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="96473-206">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="96473-207">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="96473-208">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="96473-208">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="96473-209">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="96473-210">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="96473-210">AzureRM.Media</span></span>
* <span data-ttu-id="96473-211">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="96473-212">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-212">AzureRM.Network</span></span>
* <span data-ttu-id="96473-213">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-213">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="96473-214">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-214">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="96473-215">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-215">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="96473-216">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-216">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="96473-217">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-217">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="96473-218">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-218">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="96473-219">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="96473-219">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="96473-220">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="96473-220">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="96473-221">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="96473-221">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="96473-222">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-222">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="96473-223">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="96473-223">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="96473-224">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="96473-225">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="96473-225">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="96473-226">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="96473-227">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="96473-227">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="96473-228">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="96473-229">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="96473-229">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="96473-230">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="96473-231">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="96473-231">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="96473-232">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-232">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="96473-233">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="96473-233">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="96473-234">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-234">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="96473-235">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-235">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="96473-236">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-236">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="96473-237">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="96473-237">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="96473-238">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="96473-238">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="96473-239">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="96473-239">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="96473-240">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="96473-241">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="96473-241">AzureRM.RedisCache</span></span>
* <span data-ttu-id="96473-242">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="96473-243">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="96473-243">AzureRM.Relay</span></span>
* <span data-ttu-id="96473-244">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="96473-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="96473-245">AzureRM.Resources</span></span>
* <span data-ttu-id="96473-246">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="96473-246">Support template deployment at subscription scope.</span></span> <span data-ttu-id="96473-247">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-247">Add new Cmdlets:</span></span>
    - <span data-ttu-id="96473-248">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="96473-248">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="96473-249">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="96473-249">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="96473-250">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="96473-250">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="96473-251">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="96473-251">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="96473-252">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="96473-252">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="96473-253">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="96473-253">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="96473-254">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="96473-254">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="96473-255">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-255">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="96473-256">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-256">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="96473-257">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-257">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="96473-258">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="96473-258">AzureRM.Scheduler</span></span>
* <span data-ttu-id="96473-259">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="96473-260">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96473-260">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="96473-261">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="96473-262">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96473-262">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="96473-263">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="96473-264">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-264">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-265">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="96473-266">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="96473-266">AzureRM.Storage</span></span>
* <span data-ttu-id="96473-267">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="96473-268">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="96473-268">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="96473-269">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-269">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="96473-270">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="96473-270">AzureRM.Tags</span></span>
* <span data-ttu-id="96473-271">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-271">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="96473-272">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="96473-272">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="96473-273">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-273">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="96473-274">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="96473-274">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="96473-275">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-275">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="96473-276">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="96473-276">AzureRM.Websites</span></span>
* <span data-ttu-id="96473-277">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="96473-278">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="96473-278">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="96473-279">全般</span><span class="sxs-lookup"><span data-stu-id="96473-279">General</span></span>
* <span data-ttu-id="96473-280">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-280">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="96473-281">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-281">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-282">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-282">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="96473-283">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-283">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="96473-284">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="96473-284">Azure.Storage</span></span>
* <span data-ttu-id="96473-285">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-285">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="96473-286">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-286">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="96473-287">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="96473-287">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="96473-288">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="96473-288">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="96473-289">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-289">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="96473-290">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="96473-290">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="96473-291">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-291">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="96473-292">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="96473-292">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="96473-293">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="96473-293">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-294">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-294">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-295">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-295">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="96473-296">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-296">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="96473-297">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="96473-297">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="96473-298">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="96473-298">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="96473-299">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-299">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="96473-300">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-300">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="96473-301">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-301">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="96473-302">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-302">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="96473-303">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-303">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="96473-304">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-304">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="96473-305">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="96473-305">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="96473-306">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-306">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="96473-307">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="96473-307">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="96473-308">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-308">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="96473-309">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-309">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="96473-310">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96473-310">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="96473-311">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-311">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="96473-312">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="96473-312">AzureRM.EventHub</span></span>
* <span data-ttu-id="96473-313">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-313">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="96473-314">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="96473-314">AzureRM.Insights</span></span>
* <span data-ttu-id="96473-315">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-315">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="96473-316">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="96473-316">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="96473-317">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96473-317">AzureRM.KeyVault</span></span>
* <span data-ttu-id="96473-318">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-318">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="96473-319">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-319">AzureRM.Network</span></span>
* <span data-ttu-id="96473-320">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-320">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="96473-321">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="96473-321">AzureRM.Resources</span></span>
* <span data-ttu-id="96473-322">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-322">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="96473-323">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-323">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="96473-324">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96473-324">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="96473-325">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-325">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="96473-326">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-326">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="96473-327">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-327">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-328">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-328">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="96473-329">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="96473-329">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="96473-330">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-330">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="96473-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="96473-331">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="96473-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="96473-332">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="96473-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="96473-333">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="96473-334">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-334">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="96473-335">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-335">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="96473-336">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="96473-336">AzureRM.Storage</span></span>
* <span data-ttu-id="96473-337">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-337">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="96473-338">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="96473-338">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="96473-339">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96473-339">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="96473-340">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96473-340">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="96473-341">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="96473-341">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="96473-342">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="96473-342">AzureRM.Tags</span></span>
* <span data-ttu-id="96473-343">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="96473-343">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="96473-344">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="96473-344">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="96473-345">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-345">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-346">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-346">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="96473-347">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="96473-347">Azure.Storage</span></span>
* <span data-ttu-id="96473-348">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="96473-348">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="96473-349">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="96473-349">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="96473-350">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="96473-350">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="96473-351">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96473-351">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="96473-352">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-352">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="96473-353">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="96473-353">AzureRM.Automation</span></span>
* <span data-ttu-id="96473-354">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-354">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-355">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-355">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-356">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-356">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="96473-357">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-357">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="96473-358">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-358">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="96473-359">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-359">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="96473-360">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="96473-360">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="96473-361">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="96473-361">AzureRM.EventHub</span></span>
* <span data-ttu-id="96473-362">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-362">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="96473-363">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96473-363">AzureRM.KeyVault</span></span>
* <span data-ttu-id="96473-364">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-364">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="96473-365">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="96473-365">AzureRM.LogicApp</span></span>
* <span data-ttu-id="96473-366">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-366">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="96473-367">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-367">AzureRM.Network</span></span>
* <span data-ttu-id="96473-368">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="96473-368">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="96473-369">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-369">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="96473-370">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-370">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="96473-371">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-371">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="96473-372">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-372">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="96473-373">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="96473-373">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="96473-374">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="96473-374">AzureRM.Relay</span></span>
* <span data-ttu-id="96473-375">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-375">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="96473-376">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="96473-376">AzureRM.Resources</span></span>
* <span data-ttu-id="96473-377">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-377">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="96473-378">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="96473-378">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="96473-379">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-379">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="96473-380">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-380">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="96473-381">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-381">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="96473-382">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96473-382">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="96473-383">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-383">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="96473-384">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-384">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="96473-385">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="96473-385">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="96473-386">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="96473-386">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="96473-387">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="96473-387">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="96473-388">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="96473-388">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="96473-389">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="96473-389">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="96473-390">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-390">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="96473-391">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96473-391">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="96473-392">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-392">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="96473-393">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-393">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-394">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-394">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="96473-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="96473-395">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="96473-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="96473-396">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="96473-397">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="96473-397">AzureRM.Websites</span></span>
* <span data-ttu-id="96473-398">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="96473-398">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="96473-399">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-399">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="96473-400">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="96473-400">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="96473-401">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="96473-401">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="96473-402">全般</span><span class="sxs-lookup"><span data-stu-id="96473-402">General</span></span>
* <span data-ttu-id="96473-403">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-403">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="96473-404">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-404">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-405">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="96473-405">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-406">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-406">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-407">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="96473-407">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="96473-408">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="96473-408">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="96473-409">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="96473-409">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="96473-410">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="96473-410">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="96473-411">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="96473-411">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="96473-412">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="96473-412">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="96473-413">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="96473-413">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="96473-414">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="96473-414">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="96473-415">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="96473-415">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="96473-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="96473-416">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="96473-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="96473-417">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="96473-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="96473-418">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="96473-419">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96473-419">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="96473-420">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="96473-420">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="96473-421">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="96473-421">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="96473-422">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-422">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="96473-423">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-423">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="96473-424">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="96473-424">AzureRM.EventHub</span></span>
* <span data-ttu-id="96473-425">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-425">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="96473-426">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-426">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="96473-427">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="96473-427">Provided Default Parameter set.</span></span>
* <span data-ttu-id="96473-428">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="96473-428">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="96473-429">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96473-429">AzureRM.KeyVault</span></span>
* <span data-ttu-id="96473-430">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-430">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="96473-431">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-431">AzureRM.Network</span></span>
* <span data-ttu-id="96473-432">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="96473-432">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="96473-433">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-433">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="96473-434">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-434">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="96473-435">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-435">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="96473-436">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-436">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="96473-437">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-437">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="96473-438">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-438">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="96473-439">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-439">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="96473-440">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-440">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="96473-441">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-441">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="96473-442">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="96473-442">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="96473-443">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-443">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="96473-444">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="96473-444">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="96473-445">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="96473-445">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="96473-446">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="96473-446">AzureRM.Resources</span></span>
* <span data-ttu-id="96473-447">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-447">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="96473-448">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="96473-448">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="96473-449">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="96473-449">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="96473-450">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-450">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="96473-451">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-451">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="96473-452">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-452">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="96473-453">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-453">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="96473-454">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-454">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="96473-455">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-455">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="96473-456">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-456">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="96473-457">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-457">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="96473-458">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-458">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="96473-459">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-459">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="96473-460">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="96473-460">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="96473-461">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="96473-461">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="96473-462">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-462">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-463">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="96473-463">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="96473-464">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-464">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="96473-465">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="96473-465">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="96473-466">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-466">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-467">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-467">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="96473-468">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="96473-468">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="96473-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="96473-469">Azure.Storage</span></span>
* <span data-ttu-id="96473-470">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-470">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-471">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-471">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-472">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-472">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="96473-473">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-473">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="96473-474">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="96473-474">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="96473-475">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="96473-475">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="96473-476">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="96473-476">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="96473-477">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-477">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="96473-478">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="96473-478">Start-AzureRmVM</span></span>
    - <span data-ttu-id="96473-479">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="96473-479">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="96473-480">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="96473-480">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="96473-481">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="96473-481">Set-AzureRmVM</span></span>
    - <span data-ttu-id="96473-482">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="96473-482">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="96473-483">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="96473-483">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="96473-484">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="96473-484">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="96473-485">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="96473-485">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="96473-486">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="96473-486">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="96473-487">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="96473-487">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="96473-488">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="96473-488">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="96473-489">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="96473-489">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="96473-490">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="96473-490">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="96473-491">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="96473-491">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="96473-492">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="96473-492">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="96473-493">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="96473-493">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="96473-494">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="96473-494">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="96473-495">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="96473-495">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="96473-496">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="96473-496">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="96473-497">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="96473-497">AzureRM.EventGrid</span></span>
* <span data-ttu-id="96473-498">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="96473-498">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="96473-499">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96473-499">AzureRM.KeyVault</span></span>
* <span data-ttu-id="96473-500">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-500">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="96473-501">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="96473-501">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="96473-502">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="96473-502">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="96473-503">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="96473-503">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="96473-504">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-504">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="96473-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="96473-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="96473-506">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-506">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="96473-507">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="96473-507">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="96473-508">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-508">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-509">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-509">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="96473-510">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="96473-510">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="96473-511">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-511">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="96473-512">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="96473-512">AzureRM.Websites</span></span>
* <span data-ttu-id="96473-513">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="96473-513">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="96473-514">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="96473-514">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="96473-515">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="96473-515">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="96473-516">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="96473-516">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="96473-517">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-517">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="96473-518">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="96473-518">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="96473-519">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-519">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-520">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-520">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="96473-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="96473-521">AzureRM.Compute</span></span>
* <span data-ttu-id="96473-522">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="96473-522">VMSS VM Update feature</span></span>
    - <span data-ttu-id="96473-523">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-523">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="96473-524">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-524">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="96473-525">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="96473-525">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="96473-526">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-526">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="96473-527">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-527">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="96473-528">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-528">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="96473-529">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-529">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="96473-530">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="96473-530">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="96473-531">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="96473-531">AzureRM.KeyVault</span></span>
* <span data-ttu-id="96473-532">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-532">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="96473-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-533">AzureRM.Network</span></span>
* <span data-ttu-id="96473-534">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="96473-534">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="96473-535">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="96473-535">AzureRM.Resources</span></span>
* <span data-ttu-id="96473-536">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-536">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="96473-537">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="96473-537">AzureRM.Scheduler</span></span>
* <span data-ttu-id="96473-538">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="96473-538">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="96473-539">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-539">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-540">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="96473-540">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="96473-541">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="96473-541">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="96473-542">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="96473-542">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="96473-543">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="96473-543">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="96473-544">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="96473-544">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="96473-545">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="96473-545">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="96473-546">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="96473-546">AzureRM.Websites</span></span>
* <span data-ttu-id="96473-547">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="96473-547">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="96473-548">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="96473-548">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="96473-549">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="96473-549">AzureRM.Profile</span></span>
* <span data-ttu-id="96473-550">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-550">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="96473-551">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="96473-551">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="96473-552">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="96473-552">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="96473-553">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="96473-553">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="96473-554">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-554">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="96473-555">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-555">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="96473-556">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-556">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="96473-557">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="96473-557">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="96473-558">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-558">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="96473-559">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-559">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="96473-560">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-560">Added support for MSI identity</span></span>
* <span data-ttu-id="96473-561">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="96473-561">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="96473-562">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="96473-562">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="96473-563">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="96473-563">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="96473-564">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="96473-564">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="96473-565">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="96473-565">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="96473-566">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="96473-566">AzureRM.Batch</span></span>
* <span data-ttu-id="96473-567">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="96473-567">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="96473-568">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="96473-568">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="96473-569">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="96473-569">AzureRM.Consumption</span></span>
* <span data-ttu-id="96473-570">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-570">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="96473-571">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="96473-571">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="96473-572">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-572">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="96473-573">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-573">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="96473-574">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-574">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="96473-575">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="96473-575">AzureRM.Network</span></span>
* <span data-ttu-id="96473-576">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="96473-576">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="96473-577">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-577">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="96473-578">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="96473-578">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="96473-579">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-579">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="96473-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="96473-580">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="96473-581">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-581">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="96473-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="96473-582">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="96473-583">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="96473-583">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="96473-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="96473-584">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="96473-585">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="96473-585">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="96473-586">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="96473-586">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="96473-587">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="96473-587">AzureRM.Sql</span></span>
* <span data-ttu-id="96473-588">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="96473-588">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="96473-589">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="96473-589">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="96473-590">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="96473-590">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="96473-591">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="96473-591">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="96473-592">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="96473-592">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="96473-593">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="96473-593">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="96473-594">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="96473-594">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="96473-595">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="96473-595">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="96473-596">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="96473-596">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="96473-597">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="96473-597">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="96473-598">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="96473-598">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="96473-599">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="96473-599">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
