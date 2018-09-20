---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 08/28/2018
ms.openlocfilehash: f4f3141998be14f0b5b223aed1af283534bf061d
ms.sourcegitcommit: bc88e64c494337821274d6a66c1edad656c119c5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/20/2018
ms.locfileid: "46300835"
---
# <a name="release-notes"></a><span data-ttu-id="76abe-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="76abe-103">Release notes</span></span>

<span data-ttu-id="76abe-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="76abe-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="681---august-2018"></a><span data-ttu-id="76abe-105">6.8.1 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="76abe-105">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="76abe-106">全般</span><span class="sxs-lookup"><span data-stu-id="76abe-106">General</span></span>
* <span data-ttu-id="76abe-107">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-107">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="76abe-108">共通ランタイム アセンブリを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-108">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="76abe-109">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="76abe-109">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="76abe-110">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-110">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="76abe-111">修正された問題 https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="76abe-111">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="76abe-112">Import-AzureRmApiManagementApi コマンドレットおよび \*-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました</span><span class="sxs-lookup"><span data-stu-id="76abe-112">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="76abe-113">修正された問題 https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="76abe-113">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="76abe-114">CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="76abe-114">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="76abe-115">4.0.4-preview NuGet へのアップグレードによって修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-115">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="76abe-116">修正された問題 https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="76abe-116">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="76abe-117">製品を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-117">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="76abe-118">修正された問題 https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="76abe-118">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="76abe-119">API を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-119">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="76abe-120">AzureMonitor ロガーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-120">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="76abe-121">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-121">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-122">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-122">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="76abe-123">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-123">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="76abe-124">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-124">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="76abe-125">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-125">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-126">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-126">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-127">コマンドレット出力の既定の表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="76abe-127">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="76abe-128">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="76abe-128">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="76abe-129">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-129">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="76abe-130">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-130">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-131">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-131">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="76abe-132">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="76abe-132">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="76abe-133">修正された問題</span><span class="sxs-lookup"><span data-stu-id="76abe-133">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="76abe-134">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="76abe-134">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="76abe-135">複数値ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-135">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="76abe-136">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="76abe-136">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="76abe-137">サブネット ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-137">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="76abe-138">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-138">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="76abe-139">プロファイルでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-139">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="76abe-140">プロファイルでの予期される状態コード範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-140">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="76abe-141">エンドポイントでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-141">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="76abe-142">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="76abe-142">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="76abe-143">全般</span><span class="sxs-lookup"><span data-stu-id="76abe-143">General</span></span>
* <span data-ttu-id="76abe-144">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-144">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="76abe-145">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-145">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-146">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-146">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-147">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-147">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-148">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-148">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="76abe-149">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-149">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="76abe-150">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-150">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="76abe-151">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="76abe-151">AzureRM.IotHub</span></span>
* <span data-ttu-id="76abe-152">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-152">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-153">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-153">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-154">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="76abe-154">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="76abe-155">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="76abe-155">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="76abe-156">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-156">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="76abe-157">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-157">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-158">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-158">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="76abe-159">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="76abe-159">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="76abe-160">問題の修正</span><span class="sxs-lookup"><span data-stu-id="76abe-160">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="76abe-161">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="76abe-161">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="76abe-162">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-162">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="76abe-163">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="76abe-163">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="76abe-164">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-164">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="76abe-165">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-165">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="76abe-166">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-166">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="76abe-167">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-167">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="76abe-168">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="76abe-168">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="76abe-169">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="76abe-169">AzureRM.Websites</span></span>
* <span data-ttu-id="76abe-170">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-170">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="76abe-171">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="76abe-171">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="76abe-172">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-172">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-173">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-173">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="76abe-174">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-174">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="76abe-175">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-175">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="76abe-176">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="76abe-176">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="76abe-177">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="76abe-177">Azure.Storage</span></span>
* <span data-ttu-id="76abe-178">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="76abe-178">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="76abe-179">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="76abe-179">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="76abe-180">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="76abe-180">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="76abe-181">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-181">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="76abe-182">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="76abe-182">Azure.AnalysisServices</span></span>
* <span data-ttu-id="76abe-183">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-183">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="76abe-184">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="76abe-184">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="76abe-185">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-185">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="76abe-186">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="76abe-186">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="76abe-187">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-187">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="76abe-188">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="76abe-188">AzureRM.Automation</span></span>
* <span data-ttu-id="76abe-189">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-189">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="76abe-190">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="76abe-190">AzureRM.Backup</span></span>
* <span data-ttu-id="76abe-191">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-191">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="76abe-192">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="76abe-192">AzureRM.Batch</span></span>
* <span data-ttu-id="76abe-193">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-193">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="76abe-194">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="76abe-194">AzureRM.Billing</span></span>
* <span data-ttu-id="76abe-195">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-195">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="76abe-196">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="76abe-196">AzureRM.Cdn</span></span>
* <span data-ttu-id="76abe-197">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-197">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="76abe-198">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="76abe-198">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="76abe-199">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-199">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-200">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-200">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-201">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-201">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="76abe-202">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-202">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="76abe-203">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="76abe-203">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="76abe-204">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-204">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="76abe-205">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-205">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="76abe-206">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="76abe-206">AzureRM.Consumption</span></span>
* <span data-ttu-id="76abe-207">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-207">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="76abe-208">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="76abe-208">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="76abe-209">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-209">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="76abe-210">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="76abe-210">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="76abe-211">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-211">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="76abe-212">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="76abe-212">AzureRM.DataFactories</span></span>
* <span data-ttu-id="76abe-213">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-213">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="76abe-214">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="76abe-214">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="76abe-215">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-215">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="76abe-216">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="76abe-216">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="76abe-217">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-217">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="76abe-218">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="76abe-218">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="76abe-219">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-219">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="76abe-220">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-220">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="76abe-221">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-221">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="76abe-222">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-222">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="76abe-223">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="76abe-223">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="76abe-224">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-224">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="76abe-225">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="76abe-225">AzureRM.Dns</span></span>
* <span data-ttu-id="76abe-226">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-226">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="76abe-227">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="76abe-227">AzureRM.EventGrid</span></span>
* <span data-ttu-id="76abe-228">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-228">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="76abe-229">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="76abe-229">AzureRM.EventHub</span></span>
* <span data-ttu-id="76abe-230">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-230">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="76abe-231">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="76abe-231">AzureRM.HDInsight</span></span>
* <span data-ttu-id="76abe-232">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-232">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="76abe-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="76abe-233">AzureRM.Insights</span></span>
* <span data-ttu-id="76abe-234">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-234">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="76abe-235">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="76abe-235">AzureRM.IotHub</span></span>
* <span data-ttu-id="76abe-236">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-236">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="76abe-237">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="76abe-237">AzureRM.KeyVault</span></span>
* <span data-ttu-id="76abe-238">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-238">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="76abe-239">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="76abe-239">AzureRM.LogicApp</span></span>
* <span data-ttu-id="76abe-240">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-240">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="76abe-241">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="76abe-241">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="76abe-242">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-242">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="76abe-243">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="76abe-243">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="76abe-244">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-244">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="76abe-245">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="76abe-245">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="76abe-246">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-246">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="76abe-247">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="76abe-247">AzureRM.Media</span></span>
* <span data-ttu-id="76abe-248">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-248">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-249">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-249">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-250">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-250">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="76abe-251">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-251">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="76abe-252">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-252">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="76abe-253">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-253">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="76abe-254">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-254">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="76abe-255">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-255">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="76abe-256">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="76abe-256">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="76abe-257">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="76abe-257">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="76abe-258">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="76abe-258">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="76abe-259">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-259">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="76abe-260">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="76abe-260">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="76abe-261">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-261">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="76abe-262">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="76abe-262">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="76abe-263">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-263">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="76abe-264">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="76abe-264">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="76abe-265">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-265">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="76abe-266">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="76abe-266">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="76abe-267">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-267">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="76abe-268">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="76abe-268">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="76abe-269">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-269">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="76abe-270">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="76abe-270">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="76abe-271">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-271">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="76abe-272">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-272">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="76abe-273">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-273">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="76abe-274">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="76abe-274">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="76abe-275">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="76abe-275">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="76abe-276">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="76abe-276">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="76abe-277">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-277">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="76abe-278">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="76abe-278">AzureRM.RedisCache</span></span>
* <span data-ttu-id="76abe-279">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-279">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="76abe-280">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="76abe-280">AzureRM.Relay</span></span>
* <span data-ttu-id="76abe-281">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-281">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="76abe-282">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-282">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-283">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="76abe-283">Support template deployment at subscription scope.</span></span> <span data-ttu-id="76abe-284">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-284">Add new Cmdlets:</span></span>
    - <span data-ttu-id="76abe-285">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="76abe-285">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="76abe-286">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="76abe-286">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="76abe-287">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="76abe-287">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="76abe-288">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="76abe-288">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="76abe-289">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="76abe-289">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="76abe-290">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="76abe-290">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="76abe-291">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="76abe-291">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="76abe-292">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-292">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="76abe-293">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-293">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="76abe-294">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-294">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="76abe-295">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="76abe-295">AzureRM.Scheduler</span></span>
* <span data-ttu-id="76abe-296">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-296">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="76abe-297">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="76abe-297">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="76abe-298">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-298">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="76abe-299">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="76abe-299">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="76abe-300">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-300">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="76abe-301">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-301">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-302">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-302">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="76abe-303">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="76abe-303">AzureRM.Storage</span></span>
* <span data-ttu-id="76abe-304">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-304">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="76abe-305">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="76abe-305">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="76abe-306">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-306">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="76abe-307">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="76abe-307">AzureRM.Tags</span></span>
* <span data-ttu-id="76abe-308">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-308">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="76abe-309">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="76abe-309">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="76abe-310">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="76abe-311">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="76abe-311">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="76abe-312">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="76abe-313">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="76abe-313">AzureRM.Websites</span></span>
* <span data-ttu-id="76abe-314">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="76abe-315">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="76abe-315">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="76abe-316">全般</span><span class="sxs-lookup"><span data-stu-id="76abe-316">General</span></span>
* <span data-ttu-id="76abe-317">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-317">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="76abe-318">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-318">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-319">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-319">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="76abe-320">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-320">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="76abe-321">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="76abe-321">Azure.Storage</span></span>
* <span data-ttu-id="76abe-322">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-322">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="76abe-323">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-323">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="76abe-324">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="76abe-324">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="76abe-325">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="76abe-325">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="76abe-326">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-326">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="76abe-327">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="76abe-327">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="76abe-328">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-328">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="76abe-329">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="76abe-329">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="76abe-330">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="76abe-330">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-331">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-331">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-332">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-332">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="76abe-333">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-333">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="76abe-334">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="76abe-334">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="76abe-335">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="76abe-335">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="76abe-336">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-336">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="76abe-337">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-337">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="76abe-338">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-338">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="76abe-339">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-339">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="76abe-340">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-340">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="76abe-341">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-341">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="76abe-342">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="76abe-342">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="76abe-343">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-343">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="76abe-344">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="76abe-344">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="76abe-345">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-345">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="76abe-346">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-346">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="76abe-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="76abe-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="76abe-348">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-348">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="76abe-349">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="76abe-349">AzureRM.EventHub</span></span>
* <span data-ttu-id="76abe-350">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-350">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="76abe-351">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="76abe-351">AzureRM.Insights</span></span>
* <span data-ttu-id="76abe-352">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-352">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="76abe-353">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="76abe-353">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="76abe-354">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="76abe-354">AzureRM.KeyVault</span></span>
* <span data-ttu-id="76abe-355">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-355">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-356">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-356">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-357">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-357">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="76abe-358">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-358">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-359">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-359">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="76abe-360">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-360">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="76abe-361">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="76abe-361">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="76abe-362">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-362">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="76abe-363">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-363">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="76abe-364">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-364">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-365">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-365">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="76abe-366">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="76abe-366">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="76abe-367">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-367">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="76abe-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="76abe-368">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="76abe-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="76abe-369">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="76abe-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="76abe-370">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="76abe-371">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-371">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="76abe-372">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-372">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="76abe-373">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="76abe-373">AzureRM.Storage</span></span>
* <span data-ttu-id="76abe-374">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-374">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="76abe-375">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="76abe-375">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="76abe-376">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="76abe-376">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="76abe-377">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="76abe-377">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="76abe-378">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="76abe-378">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="76abe-379">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="76abe-379">AzureRM.Tags</span></span>
* <span data-ttu-id="76abe-380">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="76abe-380">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="76abe-381">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="76abe-381">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="76abe-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-382">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-383">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-383">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="76abe-384">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="76abe-384">Azure.Storage</span></span>
* <span data-ttu-id="76abe-385">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="76abe-385">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="76abe-386">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="76abe-386">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="76abe-387">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="76abe-387">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="76abe-388">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="76abe-388">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="76abe-389">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-389">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="76abe-390">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="76abe-390">AzureRM.Automation</span></span>
* <span data-ttu-id="76abe-391">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-391">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-392">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-392">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-393">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-393">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="76abe-394">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-394">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="76abe-395">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-395">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="76abe-396">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-396">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="76abe-397">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="76abe-397">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="76abe-398">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="76abe-398">AzureRM.EventHub</span></span>
* <span data-ttu-id="76abe-399">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-399">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="76abe-400">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="76abe-400">AzureRM.KeyVault</span></span>
* <span data-ttu-id="76abe-401">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-401">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="76abe-402">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="76abe-402">AzureRM.LogicApp</span></span>
* <span data-ttu-id="76abe-403">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-403">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-404">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-404">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-405">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="76abe-405">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="76abe-406">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-406">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="76abe-407">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-407">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="76abe-408">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-408">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="76abe-409">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-409">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="76abe-410">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="76abe-410">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="76abe-411">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="76abe-411">AzureRM.Relay</span></span>
* <span data-ttu-id="76abe-412">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-412">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="76abe-413">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-413">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-414">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-414">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="76abe-415">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="76abe-415">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="76abe-416">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-416">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="76abe-417">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-417">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="76abe-418">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-418">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="76abe-419">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="76abe-419">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="76abe-420">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-420">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="76abe-421">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-421">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="76abe-422">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="76abe-422">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="76abe-423">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="76abe-423">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="76abe-424">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="76abe-424">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="76abe-425">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="76abe-425">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="76abe-426">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="76abe-426">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="76abe-427">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-427">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="76abe-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="76abe-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="76abe-429">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-429">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="76abe-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-430">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-431">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-431">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="76abe-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="76abe-432">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="76abe-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="76abe-433">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="76abe-434">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="76abe-434">AzureRM.Websites</span></span>
* <span data-ttu-id="76abe-435">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="76abe-435">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="76abe-436">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-436">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="76abe-437">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="76abe-437">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="76abe-438">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="76abe-438">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="76abe-439">全般</span><span class="sxs-lookup"><span data-stu-id="76abe-439">General</span></span>
* <span data-ttu-id="76abe-440">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-440">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="76abe-441">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-441">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-442">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="76abe-442">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-443">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-443">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-444">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="76abe-444">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="76abe-445">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="76abe-445">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="76abe-446">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="76abe-446">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="76abe-447">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="76abe-447">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="76abe-448">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="76abe-448">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="76abe-449">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="76abe-449">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="76abe-450">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="76abe-450">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="76abe-451">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="76abe-451">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="76abe-452">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="76abe-452">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="76abe-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="76abe-453">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="76abe-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="76abe-454">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="76abe-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="76abe-455">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="76abe-456">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="76abe-456">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="76abe-457">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="76abe-457">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="76abe-458">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="76abe-458">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="76abe-459">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-459">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="76abe-460">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-460">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="76abe-461">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="76abe-461">AzureRM.EventHub</span></span>
* <span data-ttu-id="76abe-462">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-462">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="76abe-463">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-463">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="76abe-464">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="76abe-464">Provided Default Parameter set.</span></span>
* <span data-ttu-id="76abe-465">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="76abe-465">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="76abe-466">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="76abe-466">AzureRM.KeyVault</span></span>
* <span data-ttu-id="76abe-467">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-467">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-468">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-468">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-469">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="76abe-469">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="76abe-470">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-470">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="76abe-471">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-471">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="76abe-472">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-472">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="76abe-473">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-473">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="76abe-474">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-474">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="76abe-475">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-475">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="76abe-476">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-476">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="76abe-477">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-477">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="76abe-478">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-478">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="76abe-479">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="76abe-479">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="76abe-480">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-480">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="76abe-481">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="76abe-481">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="76abe-482">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="76abe-482">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="76abe-483">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-483">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-484">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-484">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="76abe-485">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="76abe-485">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="76abe-486">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="76abe-486">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="76abe-487">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-487">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="76abe-488">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-488">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="76abe-489">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-489">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="76abe-490">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-490">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="76abe-491">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-491">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="76abe-492">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-492">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="76abe-493">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-493">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="76abe-494">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-494">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="76abe-495">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-495">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="76abe-496">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-496">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="76abe-497">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="76abe-497">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="76abe-498">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="76abe-498">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="76abe-499">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-499">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-500">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="76abe-500">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="76abe-501">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-501">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="76abe-502">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="76abe-502">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="76abe-503">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-503">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-504">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-504">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="76abe-505">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="76abe-505">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="76abe-506">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="76abe-506">Azure.Storage</span></span>
* <span data-ttu-id="76abe-507">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-507">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-508">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-508">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-509">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-509">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="76abe-510">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-510">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="76abe-511">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="76abe-511">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="76abe-512">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="76abe-512">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="76abe-513">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="76abe-513">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="76abe-514">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-514">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="76abe-515">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="76abe-515">Start-AzureRmVM</span></span>
    - <span data-ttu-id="76abe-516">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="76abe-516">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="76abe-517">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="76abe-517">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="76abe-518">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="76abe-518">Set-AzureRmVM</span></span>
    - <span data-ttu-id="76abe-519">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="76abe-519">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="76abe-520">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="76abe-520">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="76abe-521">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="76abe-521">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="76abe-522">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="76abe-522">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="76abe-523">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="76abe-523">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="76abe-524">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="76abe-524">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="76abe-525">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="76abe-525">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="76abe-526">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="76abe-526">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="76abe-527">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="76abe-527">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="76abe-528">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="76abe-528">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="76abe-529">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="76abe-529">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="76abe-530">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="76abe-530">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="76abe-531">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="76abe-531">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="76abe-532">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="76abe-532">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="76abe-533">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="76abe-533">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="76abe-534">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="76abe-534">AzureRM.EventGrid</span></span>
* <span data-ttu-id="76abe-535">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="76abe-535">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="76abe-536">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="76abe-536">AzureRM.KeyVault</span></span>
* <span data-ttu-id="76abe-537">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-537">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="76abe-538">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="76abe-538">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="76abe-539">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="76abe-539">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="76abe-540">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="76abe-540">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="76abe-541">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-541">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="76abe-542">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="76abe-542">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="76abe-543">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-543">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="76abe-544">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="76abe-544">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="76abe-545">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-545">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-546">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-546">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="76abe-547">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="76abe-547">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="76abe-548">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-548">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="76abe-549">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="76abe-549">AzureRM.Websites</span></span>
* <span data-ttu-id="76abe-550">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="76abe-550">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="76abe-551">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="76abe-551">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="76abe-552">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="76abe-552">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="76abe-553">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="76abe-553">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="76abe-554">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-554">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="76abe-555">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="76abe-555">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="76abe-556">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-556">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-557">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-557">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="76abe-558">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="76abe-558">AzureRM.Compute</span></span>
* <span data-ttu-id="76abe-559">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="76abe-559">VMSS VM Update feature</span></span>
    - <span data-ttu-id="76abe-560">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-560">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="76abe-561">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-561">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="76abe-562">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="76abe-562">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="76abe-563">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-563">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="76abe-564">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-564">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="76abe-565">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-565">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="76abe-566">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-566">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="76abe-567">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="76abe-567">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="76abe-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="76abe-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="76abe-569">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-569">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="76abe-570">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-570">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-571">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="76abe-571">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="76abe-572">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="76abe-572">AzureRM.Resources</span></span>
* <span data-ttu-id="76abe-573">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-573">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="76abe-574">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="76abe-574">AzureRM.Scheduler</span></span>
* <span data-ttu-id="76abe-575">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="76abe-575">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="76abe-576">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-576">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-577">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="76abe-577">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="76abe-578">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="76abe-578">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="76abe-579">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="76abe-579">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="76abe-580">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="76abe-580">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="76abe-581">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="76abe-581">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="76abe-582">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="76abe-582">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="76abe-583">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="76abe-583">AzureRM.Websites</span></span>
* <span data-ttu-id="76abe-584">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="76abe-584">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="76abe-585">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="76abe-585">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="76abe-586">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="76abe-586">AzureRM.Profile</span></span>
* <span data-ttu-id="76abe-587">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-587">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="76abe-588">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="76abe-588">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="76abe-589">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="76abe-589">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="76abe-590">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="76abe-590">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="76abe-591">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-591">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="76abe-592">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-592">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="76abe-593">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-593">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="76abe-594">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="76abe-594">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="76abe-595">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-595">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="76abe-596">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-596">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="76abe-597">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-597">Added support for MSI identity</span></span>
* <span data-ttu-id="76abe-598">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="76abe-598">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="76abe-599">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="76abe-599">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="76abe-600">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="76abe-600">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="76abe-601">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="76abe-601">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="76abe-602">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="76abe-602">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="76abe-603">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="76abe-603">AzureRM.Batch</span></span>
* <span data-ttu-id="76abe-604">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="76abe-604">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="76abe-605">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="76abe-605">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="76abe-606">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="76abe-606">AzureRM.Consumption</span></span>
* <span data-ttu-id="76abe-607">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-607">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="76abe-608">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="76abe-608">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="76abe-609">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-609">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="76abe-610">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-610">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="76abe-611">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-611">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="76abe-612">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="76abe-612">AzureRM.Network</span></span>
* <span data-ttu-id="76abe-613">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-613">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="76abe-614">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-614">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="76abe-615">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="76abe-615">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="76abe-616">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-616">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="76abe-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="76abe-617">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="76abe-618">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-618">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="76abe-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="76abe-619">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="76abe-620">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-620">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="76abe-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="76abe-621">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="76abe-622">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="76abe-622">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="76abe-623">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="76abe-623">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="76abe-624">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="76abe-624">AzureRM.Sql</span></span>
* <span data-ttu-id="76abe-625">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="76abe-625">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="76abe-626">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="76abe-626">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="76abe-627">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="76abe-627">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="76abe-628">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="76abe-628">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="76abe-629">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="76abe-629">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="76abe-630">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="76abe-630">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="76abe-631">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="76abe-631">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="76abe-632">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="76abe-632">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="76abe-633">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="76abe-633">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="76abe-634">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="76abe-634">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="76abe-635">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="76abe-635">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="76abe-636">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="76abe-636">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
