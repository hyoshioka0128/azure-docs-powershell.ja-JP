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
ms.date: 2/20/2018
ms.openlocfilehash: 985e0fbaa2da73b398d4c574515bcbab5b1a16e0
ms.sourcegitcommit: 15bf69bf95eceb936b3a429e741add95c308826a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2018
---
# <a name="release-notes"></a><span data-ttu-id="4a207-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="4a207-103">Release notes</span></span>

<span data-ttu-id="4a207-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="4a207-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

## <a name="560---march-2018"></a><span data-ttu-id="4a207-105">5.6.0 - 2018 年 3 月</span><span class="sxs-lookup"><span data-stu-id="4a207-105">5.6.0 - March 2018</span></span>

#### <a name="general"></a><span data-ttu-id="4a207-106">全般</span><span class="sxs-lookup"><span data-stu-id="4a207-106">General</span></span>
* <span data-ttu-id="4a207-107">Cloud Shell の既定のリソース グループに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-107">Fix issue with Default Resource Group in CloudShell</span></span>
* <span data-ttu-id="4a207-108">モジュールのインポート中に不適切なスタートアップ スクリプトが実行される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-108">Fix issue where incorrect startup scripts were being executed during module import</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="4a207-109">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4a207-109">AzureRM.Profile</span></span>
* <span data-ttu-id="4a207-110">サポートされていないシナリオで MSI 認証を有効にしました</span><span class="sxs-lookup"><span data-stu-id="4a207-110">Enable MSI authentication in unsupported scenarios</span></span>
* <span data-ttu-id="4a207-111">ユーザー定義の管理対象サービス ID に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-111">Add support for user-defined Managed Service Identity</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="4a207-112">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a207-112">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4a207-113">ビルドにおけるスクリプトのクリーンアップに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-113">Fixed issue with cleaning up scripts in build</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="4a207-114">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="4a207-114">AzureRM.Cdn</span></span>
* <span data-ttu-id="4a207-115">ビルドにおけるスクリプトのクリーンアップに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-115">Fixed issue with cleaning up scripts in build</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4a207-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a207-116">AzureRM.Compute</span></span>
* <span data-ttu-id="4a207-117">'New-AzureRmVM' と 'New-AzureRmVMSS' は、データ ディスクをサポートします。</span><span class="sxs-lookup"><span data-stu-id="4a207-117">'New-AzureRmVM' and 'New-AzureRmVMSS' support data disks.</span></span>
* <span data-ttu-id="4a207-118">'New-AzureRmVM' と 'New-AzureRmVMSS' は、名前または ID でカスタム イメージをサポートします。</span><span class="sxs-lookup"><span data-stu-id="4a207-118">'New-AzureRmVM' and 'New-AzureRmVMSS' support custom image by name or by id.</span></span>
* <span data-ttu-id="4a207-119">ログ分析機能</span><span class="sxs-lookup"><span data-stu-id="4a207-119">Log analytic feature</span></span>
    - <span data-ttu-id="4a207-120">'Export-AzureRmLogAnalyticRequestRateByInterval' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-120">Added 'Export-AzureRmLogAnalyticRequestRateByInterval' cmdlet</span></span>
    - <span data-ttu-id="4a207-121">'Export-AzureRmLogAnalyticThrottledRequests' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-121">Added 'Export-AzureRmLogAnalyticThrottledRequests' cmdlet</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="4a207-122">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4a207-122">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="4a207-123">コンテナー レジストリおよび Azure File ボリューム マウントのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-123">Fix parameter sets issue for container registry and azure file volume mount</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="4a207-124">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4a207-124">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="4a207-125">次の変更を含むように ADF .Net SDK バージョン 0.6.0-preview を更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-125">Updated the ADF .Net SDK to version 0.6.0-preview containing the following changes:</span></span>
    - <span data-ttu-id="4a207-126">新しい AzureDatabricksLinkedService および DatabricksNotebookActivity を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-126">Added new AzureDatabricks LinkedService and DatabricksNotebook Activity</span></span>
    - <span data-ttu-id="4a207-127">HDInsightOnDemand LinkedService に headNodeSize プロパティと dataNodeSize プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-127">Added headNodeSize and dataNodeSize properties in HDInsightOnDemand LinkedService</span></span>
    - <span data-ttu-id="4a207-128">SalesforceMarketingCloud の LinkedService、Dataset、CopySource を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-128">Added LinkedService, Dataset, CopySource for SalesforceMarketingCloud</span></span>
    - <span data-ttu-id="4a207-129">すべてのアクティビティで SecureOutput のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-129">Added support for SecureOutput on all activities</span></span>
    - <span data-ttu-id="4a207-130">実行する同時実行アクティビティの数を制御する新しい BatchCount プロパティを ForEach アクティビティに追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-130">Added new BatchCount property on ForEach activity which control how many concurrent activities to run</span></span>
    - <span data-ttu-id="4a207-131">新しいフィルター アクティビティを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-131">Added new Filter Activity</span></span>
    - <span data-ttu-id="4a207-132">リンクされたサービス パラメーターに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-132">Added Linked Service Parameters support</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="4a207-133">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="4a207-133">AzureRM.Dns</span></span>
* <span data-ttu-id="4a207-134">プライベート DNS ゾーンのサポート (パブリック プレビュー)</span><span class="sxs-lookup"><span data-stu-id="4a207-134">Support for Private DNS Zones (Public Preview)</span></span>
    - <span data-ttu-id="4a207-135">関連付けられた仮想ネットワークのみに表示される DNS ゾーンを作成する機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-135">Adds ability to create DNS zones that are visible only to the associated virtual networks</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="4a207-136">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a207-136">AzureRM.Network</span></span>
* <span data-ttu-id="4a207-137">DNS のコマンドレットとの互換性のためにモデルの種類を更新しています。</span><span class="sxs-lookup"><span data-stu-id="4a207-137">Updating model types for compatibility with DNS cmdlets.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="4a207-138">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-138">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="4a207-139">Azure Site Recovery に対する ASR Azure の変更 (コマンドレットは現在、Enterprise から Enterprise、Enterprise から Azure、HyperV から Azure、VMware から Azure の操作をサポートしています)</span><span class="sxs-lookup"><span data-stu-id="4a207-139">Changes for ASR Azure to Azure Site Recovery (cmdlets are currently supporting operations for Enterprise to Enterprise, Enterprise to Azure, HyperV to Azure,VMware to Azure)</span></span>
    - <span data-ttu-id="4a207-140">New-AzureRmRecoveryServicesAsrProtectionContainer</span><span class="sxs-lookup"><span data-stu-id="4a207-140">New-AzureRmRecoveryServicesAsrProtectionContainer</span></span>
    - <span data-ttu-id="4a207-141">New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig</span><span class="sxs-lookup"><span data-stu-id="4a207-141">New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig</span></span>
    - <span data-ttu-id="4a207-142">Remove-AzureRmRecoveryServicesAsrProtectionContainer</span><span class="sxs-lookup"><span data-stu-id="4a207-142">Remove-AzureRmRecoveryServicesAsrProtectionContainer</span></span>
    - <span data-ttu-id="4a207-143">Update-AzureRmRecoveryServicesAsrProtectionDirection</span><span class="sxs-lookup"><span data-stu-id="4a207-143">Update-AzureRmRecoveryServicesAsrProtectionDirection</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="4a207-144">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-144">AzureRM.Storage</span></span>
* <span data-ttu-id="4a207-145">保存時の暗号化は既定で有効であり、無効にできないため、ストレージ アカウントの新規と設定の各コマンドレットのパラメーター EnableEncryptionService および DisableEncryptionService を廃止しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-145">Obsolete following parameters in new and set Storage Account cmdlets: EnableEncryptionService and DisableEncryptionService, since Encryption at Rest is enabled by default and can't be disabled.</span></span>
    - <span data-ttu-id="4a207-146">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4a207-146">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="4a207-147">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4a207-147">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4a207-148">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4a207-148">AzureRM.Websites</span></span>
* <span data-ttu-id="4a207-149">Remove-AzureRmWebAppSlot のヘルプを修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-149">Fixed the help for Remove-AzureRmWebAppSlot</span></span>

## <a name="550---march-2018"></a><span data-ttu-id="4a207-150">5.5.0 - 2018 年 3 月</span><span class="sxs-lookup"><span data-stu-id="4a207-150">5.5.0 - March 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4a207-151">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4a207-151">AzureRM.Profile</span></span>
* <span data-ttu-id="4a207-152">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-152">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="4a207-153">Newtonsoft.Json のバージョン 10.0.3 をバージョン 6.0.8 と共に読み込んでください</span><span class="sxs-lookup"><span data-stu-id="4a207-153">Load version 10.0.3 of Newtonsoft.Json side-by-side with version 6.0.8</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="4a207-154">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-154">Azure.Storage</span></span>
* <span data-ttu-id="4a207-155">論理的な削除機能のサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-155">Support Soft-Delete feature</span></span>
    - <span data-ttu-id="4a207-156">Enable-AzureStorageDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="4a207-156">Enable-AzureStorageDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="4a207-157">Disable-AzureStorageDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="4a207-157">Disable-AzureStorageDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="4a207-158">Get-AzureStorageBlob</span><span class="sxs-lookup"><span data-stu-id="4a207-158">Get-AzureStorageBlob</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="4a207-159">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a207-159">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4a207-160">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-160">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="4a207-161">ファイアウォールおよびクエリのスケールアウト機能のサポートに加え 2017-08-01 api バージョンのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-161">Add support of firewall and query scaleout feature, as well as support of 2017-08-01 api version.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="4a207-162">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="4a207-162">AzureRM.Automation</span></span>
* <span data-ttu-id="4a207-163">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-163">Fixed issue with importing aliases</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="4a207-164">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="4a207-164">AzureRM.Cdn</span></span>
* <span data-ttu-id="4a207-165">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-165">Fixed issue with importing aliases</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="4a207-166">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4a207-166">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="4a207-167">notice.txt と通知メッセージを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-167">Update notice.txt and notice message.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4a207-168">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a207-168">AzureRM.Compute</span></span>
* <span data-ttu-id="4a207-169">"New-AzureRmVMSS" では、詳細モードで接続文字列が出力されます。</span><span class="sxs-lookup"><span data-stu-id="4a207-169">'New-AzureRmVMSS' prints connection strings in verbose mode.</span></span>
* <span data-ttu-id="4a207-170">"New-AzureRmVmss" では、パブリック IP アドレス、負荷分散規則、および受信 NAT 規則がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="4a207-170">'New-AzureRmVmss' supports public IP address, load balancing rules, inbound NAT rules.</span></span>
* <span data-ttu-id="4a207-171">WriteAccelerator 機能</span><span class="sxs-lookup"><span data-stu-id="4a207-171">WriteAccelerator feature</span></span>
    - <span data-ttu-id="4a207-172">WriteAccelerator スイッチ パラメーターを次のコマンドレットを追加しました: Set-AzureRmVMOSDisk、Set-AzureRmVMDataDisk、Add-AzureRmVMDataDisk、Add-AzureRmVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="4a207-172">Added WriteAccelerator switch parameter to the following cmdlets: Set-AzureRmVMOSDisk Set-AzureRmVMDataDisk Add-AzureRmVMDataDisk Add-AzureRmVmssDataDisk</span></span>
    - <span data-ttu-id="4a207-173">OsDiskWriteAccelerator スイッチ パラメーターを Set-AzureRmVmssStorageProfile コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-173">Added OsDiskWriteAccelerator switch parameter to the following cmdlet:     Set-AzureRmVmssStorageProfile.</span></span>
    - <span data-ttu-id="4a207-174">OsDiskWriteAccelerator ブール値パラメーターを次のコマンドレットに追加しました: Update-AzureRmVM、Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="4a207-174">Added OsDiskWriteAccelerator Boolean parameter to the following cmdlets:     Update-AzureRmVM     Update-AzureRmVmss</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="4a207-175">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="4a207-175">AzureRM.DataFactories</span></span>
* <span data-ttu-id="4a207-176">一部の暗号化操作で無意味なエラーの原因になっていた、資格情報暗号化に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-176">Fix credential encryption issue that caused no meaningful error for some encryption operations</span></span>
* <span data-ttu-id="4a207-177">データ ファクトリ全体で統合ランタイムを共有できるようにしました</span><span class="sxs-lookup"><span data-stu-id="4a207-177">Enable integration runtime to be shared across data factory</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="4a207-178">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4a207-178">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="4a207-179">カスタム セットアップおよびエディション選択機能を有効にする、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "SetupScriptContainerSasUri" と "Edition" を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-179">Add parameter "SetupScriptContainerSasUri" and "Edition" for "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd to enable custom setup and edition selection functionality</span></span>
* <span data-ttu-id="4a207-180">一部の暗号化操作で重要性の低いエラーの原因になっていた、資格情報の暗号化に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-180">Fix credential encryption issue that caused no meaningful error for some encryption operations.</span></span>
* <span data-ttu-id="4a207-181">データ ファクトリ全体で統合ランタイムを共有できるようにしました</span><span class="sxs-lookup"><span data-stu-id="4a207-181">Enable integration runtime to be shared across data factory</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="4a207-182">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a207-182">AzureRM.HDInsight</span></span>
* <span data-ttu-id="4a207-183">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-183">Fixed issue with importing aliases</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="4a207-184">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4a207-184">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4a207-185">Set-AzureRmKeyVaultAccessPolicy の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-185">Fixed example for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="4a207-186">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a207-186">AzureRM.Network</span></span>
* <span data-ttu-id="4a207-187">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-187">Fixed issue with importing aliases</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="4a207-188">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-188">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="4a207-189">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-189">Fixed issue with importing aliases</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="4a207-190">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4a207-190">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="4a207-191">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-191">Fixed issue with importing aliases</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="4a207-192">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-192">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="4a207-193">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-193">Fixed issue with importing aliases</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4a207-194">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4a207-194">AzureRM.Resources</span></span>
* <span data-ttu-id="4a207-195">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-195">Fixed issue with importing aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="4a207-196">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4a207-196">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="4a207-197">キューに EnableBatchedOperations プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-197">Added EnableBatchedOperations property to Queue</span></span>
* <span data-ttu-id="4a207-198">サブスクリプションに DeadLetteringOnFilterEvaluationExceptions プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-198">Added DeadLetteringOnFilterEvaluationExceptions property to Subscriptions</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="4a207-199">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4a207-199">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="4a207-200">Service Fabric コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-200">Service Fabric cmdlet refresh</span></span>
  - <span data-ttu-id="4a207-201">ARM テンプレートを更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-201">Updated ARM templates</span></span>
  - <span data-ttu-id="4a207-202">失敗した操作がロールバックされなくなりました</span><span class="sxs-lookup"><span data-stu-id="4a207-202">Failed operations no longer rollback</span></span>
  - <span data-ttu-id="4a207-203">Add-AzureRmServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="4a207-203">Add-AzureRmServiceFabricNodeType</span></span>
    - <span data-ttu-id="4a207-204">VM は既定で管理ディスクとなります</span><span class="sxs-lookup"><span data-stu-id="4a207-204">VMs default to managed disks</span></span>
    - <span data-ttu-id="4a207-205">既存の VMSS サブネットが使用されます</span><span class="sxs-lookup"><span data-stu-id="4a207-205">Existing VMSS subnet used</span></span>
    - <span data-ttu-id="4a207-206">すべての操作はべき等です</span><span class="sxs-lookup"><span data-stu-id="4a207-206">All operations are idempotent</span></span>
  - <span data-ttu-id="4a207-207">Remove-AzureRmServiceFabricNodeType により、部分的に作成された VMSS およびクラスター ノードの種類がクリーンアップされます</span><span class="sxs-lookup"><span data-stu-id="4a207-207">Remove-AzureRmServiceFabricNodeType cleans up partially created VMSS and/or cluster node types</span></span>
  - <span data-ttu-id="4a207-208">複雑なプロパティ型について PSCluster オブジェクトの出力を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-208">Fixed output of PSCluster object for complex property types</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4a207-209">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4a207-209">AzureRM.Sql</span></span>
* <span data-ttu-id="4a207-210">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-210">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="4a207-211">Get-AzureRmSqlServer、New-AzureRmSqlServer、および Remove-AzureRmSqlServer の応答に FullyQualifiedDomainName プロパティが含まれるようになりました。</span><span class="sxs-lookup"><span data-stu-id="4a207-211">Get-AzureRmSqlServer, New-AzureRmSqlServer, and Remove-AzureRmSqlServer response now includes FullyQualifiedDomainName property.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4a207-212">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4a207-212">AzureRM.Websites</span></span>
* <span data-ttu-id="4a207-213">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-213">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="4a207-214">New-AzureRMWebApp - WebApp を簡単に作成できるようにするパラメーター セットを追加しました (ローカルの Git リポジトリをサポート)。</span><span class="sxs-lookup"><span data-stu-id="4a207-214">New-AzureRMWebApp - added parameter set for simplified WebApp creation, with local git repository support.</span></span>

## <a name="540---february-2018"></a><span data-ttu-id="4a207-215">5.4.0 - 2018 年 2 月</span><span class="sxs-lookup"><span data-stu-id="4a207-215">5.4.0 - February 2018</span></span>
#### <a name="azurermautomation"></a><span data-ttu-id="4a207-216">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="4a207-216">AzureRM.Automation</span></span>
* <span data-ttu-id="4a207-217">New-AzureRmAutomationModule の別名を Import-AzureRmAutomationModule に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-217">Added alias from New-AzureRmAutomationModule to Import-AzureRmAutomationModule</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4a207-218">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a207-218">AzureRM.Compute</span></span>
* <span data-ttu-id="4a207-219">一部の Get コマンドレットの ErrorAction に関する問題を解決しました</span><span class="sxs-lookup"><span data-stu-id="4a207-219">Fix ErrorAction issue for some of Get cmdlets.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="4a207-220">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4a207-220">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="4a207-221">Azure コンテナー インスタンス SDK 2018-02-01 を適用しました</span><span class="sxs-lookup"><span data-stu-id="4a207-221">Apply Azure Container Instance SDK 2018-02-01</span></span>
    - <span data-ttu-id="4a207-222">DNS 名ラベルのサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-222">Support DNS name label</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="4a207-223">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="4a207-223">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="4a207-224">以前動作しなかった GET コマンドレットをすべて修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-224">Fixed all of the GET cmdlets which previously weren't working.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="4a207-225">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="4a207-225">AzureRM.EventHub</span></span>
* <span data-ttu-id="4a207-226">Get-AzureRmEventHubGeoDRConfiguration ヘルプのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-226">Fix bug in Get-AzureRmEventHubGeoDRConfiguration help</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="4a207-227">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a207-227">AzureRM.Network</span></span>
* <span data-ttu-id="4a207-228">新しい接続モニターを作成するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-228">Added cmdlet to create a new connection monitor</span></span>
    - <span data-ttu-id="4a207-229">New-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="4a207-229">New-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="4a207-230">接続モニターを更新するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-230">Added cmdlet to update a connection monitor</span></span>
    - <span data-ttu-id="4a207-231">Set-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="4a207-231">Set-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="4a207-232">接続モニターまたは接続モニターのリストを取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-232">Added cmdlet to get connection monitor or connection monitor list</span></span>
    - <span data-ttu-id="4a207-233">Get-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="4a207-233">Get-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="4a207-234">接続モニターにクエリを実行するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-234">Added cmdlet to query connection monitor</span></span>
    - <span data-ttu-id="4a207-235">Get-AzureRmNetworkWatcherConnectionMonitorReport</span><span class="sxs-lookup"><span data-stu-id="4a207-235">Get-AzureRmNetworkWatcherConnectionMonitorReport</span></span>
* <span data-ttu-id="4a207-236">接続モニターを起動するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-236">Added cmdlet to start connection monitor</span></span>
    - <span data-ttu-id="4a207-237">Start-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="4a207-237">Start-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="4a207-238">接続モニターを停止するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-238">Added cmdlet to stop connection monitor</span></span>
    - <span data-ttu-id="4a207-239">Stop-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="4a207-239">Stop-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="4a207-240">接続モニターを削除するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-240">Added cmdlet to remove connection monitor</span></span>
    - <span data-ttu-id="4a207-241">Remove-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="4a207-241">Remove-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="4a207-242">Set-AzureRmApplicationGatewayBackendAddressPool のドキュメントを更新して非推奨の例を削除しました</span><span class="sxs-lookup"><span data-stu-id="4a207-242">Updated Set-AzureRmApplicationGatewayBackendAddressPool documentation to remove deprecated example</span></span>
* <span data-ttu-id="4a207-243">EnableHttp2 フラグを Application Gateway に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-243">Added EnableHttp2 flag to Application Gateway</span></span>
    - <span data-ttu-id="4a207-244">New-AzureRmApplicationGateway の更新: 省略可能なパラメーター EnableHttp2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-244">Updated New-AzureRmApplicationGateway: Added optional parameter -EnableHttp2</span></span>
* <span data-ttu-id="4a207-245">IpTag を PublicIpAddress に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-245">Add IpTags to PublicIpAddress</span></span>
    - <span data-ttu-id="4a207-246">New-AzureRmPublicIpAddress の更新: IpTag を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-246">Updated New-AzureRmPublicIpAddress: Added IpTags</span></span>
    - <span data-ttu-id="4a207-247">Iptag を追加する New-AzureRmPublicIpTag</span><span class="sxs-lookup"><span data-stu-id="4a207-247">New-AzureRmPublicIpTag to add Iptag</span></span>
* <span data-ttu-id="4a207-248">DisableBgpRoutePropagation プロパティを RouteTable および effectiveRoute に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-248">Add DisableBgpRoutePropagation property in RouteTable and effectiveRoute.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4a207-249">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4a207-249">AzureRM.Resources</span></span>
* <span data-ttu-id="4a207-250">Register-AzureRmProviderFeature: 不足している例をドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-250">Register-AzureRmProviderFeature: Added missing example in the docs</span></span>
* <span data-ttu-id="4a207-251">Register-AzureRmResourceProvider: 不足している例をドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-251">Register-AzureRmResourceProvider: Added missing example in the docs</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="4a207-252">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-252">AzureRM.Storage</span></span>
* <span data-ttu-id="4a207-253">保存時の暗号化は既定で有効であり、無効にできないため、ストレージ アカウントの新規と設定の各コマンドレットのパラメーター EnableEncryptionService および DisableEncryptionService を廃止しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-253">Obsolete following parameters in new and set Storage Account cmdlets: EnableEncryptionService and DisableEncryptionService, since Encryption at Rest is enabled by default and can't be disabled.</span></span>
    - <span data-ttu-id="4a207-254">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4a207-254">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="4a207-255">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="4a207-255">Set-AzureRmStorageAccount</span></span>


## <a name="530---february-2018"></a><span data-ttu-id="4a207-256">5.3.0 - 2018 年 2 月</span><span class="sxs-lookup"><span data-stu-id="4a207-256">5.3.0 - February 2018</span></span>
### <a name="azurermprofile"></a><span data-ttu-id="4a207-257">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4a207-257">AzureRM.Profile</span></span>
* <span data-ttu-id="4a207-258">PowerShell 3 および 4 の非推奨警告を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-258">Added deprecation warning for PowerShell 3 and 4</span></span>
* <span data-ttu-id="4a207-259">`Add-AzureRmAccount` を `Connect-AzureRmAccount` に名前変更しました。古いコマンドレット名に対して別名を追加し、他の別名 (`Login-AzAccount` および `Login-AzureRmAccount`) を新しいコマンドレット名にリダイレクトしました。</span><span class="sxs-lookup"><span data-stu-id="4a207-259">`Add-AzureRmAccount` has been renamed as `Connect-AzureRmAccount`; an alias has been added for the old cmdlet name, and other aliases (`Login-AzAccount` and `Login-AzureRmAccount`) have been redirected to the new cmdlet name.</span></span>
* <span data-ttu-id="4a207-260">`Remove-AzureRmAccount` を `Disconnect-AzureRmAccount` に名前変更しました。古いコマンドレット名に対して別名を追加し、他の別名 (`Logout-AzAccount` および `Logout-AzureRmAccount`) を新しいコマンドレット名にリダイレクトしました。</span><span class="sxs-lookup"><span data-stu-id="4a207-260">`Remove-AzureRmAccount` has been renamed as `Disconnect-AzureRmAccount`; an alias has been added for the old cmdlet name, and other aliases (`Logout-AzAccount` and `Logout-AzureRmAccount`) have been redirected to the new cmdlet name.</span></span>
* <span data-ttu-id="4a207-261">`Login-AzureRmAccount` の代わりに `Connect-AzureRmAccount` を使用するようにリソース文字列を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-261">Corrected Resource Strings to use `Connect-AzureRmAccount` instead of `Login-AzureRmAccount`</span></span>
* <span data-ttu-id="4a207-262">`Add-AzureRmEnvironment` と `Set-AzureRmEnvironment`</span><span class="sxs-lookup"><span data-stu-id="4a207-262">`Add-AzureRmEnvironment` and `Set-AzureRmEnvironment`</span></span>
  - <span data-ttu-id="4a207-263">OperationalInsights データ プレーン RP で使用するパラメーターとして `-AzureOperationalInsightsEndpoint` と `-AzureOperationalInsightsEndpointResourceId` を追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-263">Added `-AzureOperationalInsightsEndpoint` and `-AzureOperationalInsightsEndpointResourceId` as parameters for use with OperationalInsights data plane RP.</span></span>

### <a name="azurermanalysisservices"></a><span data-ttu-id="4a207-264">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a207-264">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4a207-265">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-265">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="4a207-266">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a207-266">AzureRM.Compute</span></span>
* <span data-ttu-id="4a207-267">`New-AzureRmVM` の簡素化したパラメーター セットに `-AvailabilitySetName` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-267">Added `-AvailabilitySetName` parameter to the simplified parameterset of `New-AzureRmVM`.</span></span>
* <span data-ttu-id="4a207-268">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-268">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>
* <span data-ttu-id="4a207-269">VM および VM スケール セットに対するユーザー割り当て ID のサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-269">User assigned identity support for VM and VM scale set</span></span>
    - <span data-ttu-id="4a207-270">`-IdentityType` および `-IdentityId` パラメーターを `New-AzureRmVMConfig`、`New-AzureRmVmssConfig`、`Update-AzureRmVM`、および `Update-AzureRmVmss` に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-270">`-IdentityType` and `-IdentityId` parameters are added to `New-AzureRmVMConfig`, `New-AzureRmVmssConfig`, `Update-AzureRmVM` and `Update-AzureRmVmss`</span></span>
* <span data-ttu-id="4a207-271">`-EnableIPForwarding` パラメーターを `Add-AzureRmVmssNetworkInterfaceConfig` に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-271">Added `-EnableIPForwarding` parameter to `Add-AzureRmVmssNetworkInterfaceConfig`</span></span>
* <span data-ttu-id="4a207-272">`-Priority` パラメーターを `New-AzureRmVmssConfig` に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-272">Added `-Priority` parameter to `New-AzureRmVmssConfig`</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="4a207-273">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4a207-273">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="4a207-274">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-274">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="4a207-275">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4a207-275">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="4a207-276">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-276">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>
* <span data-ttu-id="4a207-277">`Login-AzureRmAccount` を使用してログインせずにこのコマンドレットを実行した場合の `Test-AzureRmDataLakeStoreAccount` のエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-277">Corrected the error message of `Test-AzureRmDataLakeStoreAccount` when running this cmdlet without having logged in with `Login-AzureRmAccount`</span></span>

### <a name="azurermeventgrid"></a><span data-ttu-id="4a207-278">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4a207-278">AzureRM.EventGrid</span></span>
* <span data-ttu-id="4a207-279">2018-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-279">Updated to use the 2018-01-01 API version.</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="4a207-280">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="4a207-280">AzureRM.EventHub</span></span>

* <span data-ttu-id="4a207-281">Geo ディザスター リカバリー操作用に、以下の新しいコマンドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-281">Added below new commands for Geo Disaster Recovery operations.</span></span>
  - <span data-ttu-id="4a207-282">新しい別名 (ディザスター リカバリーの構成) を作成する</span><span class="sxs-lookup"><span data-stu-id="4a207-282">Creating a new Alias (Disaster Recovery configuration):</span></span>
    - `New-AzureRmEventHubGeoDRConfiguration`
  - <span data-ttu-id="4a207-283">別名 (ディザスター リカバリー構成) を取得する</span><span class="sxs-lookup"><span data-stu-id="4a207-283">Retrieve Alias (Disaster Recovery configuration) :</span></span>
    - `Get-AzureRmEventHubGeoDRConfiguration`
  - <span data-ttu-id="4a207-284">ディザスター リカバリーを無効にし、プライマリ名前空間からセカンダリ名前空間への変更の複製を停止する</span><span class="sxs-lookup"><span data-stu-id="4a207-284">Disabling the Disaster Recovery and stops replicating changes from primary to secondary namespaces</span></span>
    - `Set-AzureRmEventHubGeoDRConfigurationBreakPair`
  - <span data-ttu-id="4a207-285">ディザスター リカバリー フェールオーバーを呼び出し、セカンダリ名前空間を指すように別名を再構成する</span><span class="sxs-lookup"><span data-stu-id="4a207-285">Invoking Disaster Recovery failover and reconfigure the alias to point to the secondary namespace</span></span>
    - `Set-AzureRmEventHubGeoDRConfigurationFailOver`
  - <span data-ttu-id="4a207-286">別名 (ディザスター リカバリー構成) を削除する</span><span class="sxs-lookup"><span data-stu-id="4a207-286">Deleting an Alias(Disaster Recovery configuration)</span></span>
    - `Remove-AzureRmEventHubGeoDRConfiguration`
* <span data-ttu-id="4a207-287">名前空間名と GeoDr 構成名 (別名の可用性) のチェック用に以下のコマンドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-287">Added below new commands for checking the Namespace Name and GeoDr Configuration Name - Alias availability.</span></span>
  - <span data-ttu-id="4a207-288">名前空間名または別名 (ディザスター リカバリーの構成) の可用性のチェック</span><span class="sxs-lookup"><span data-stu-id="4a207-288">Check the Availability of Namespace name or Alias(Disaster Recovery configuration) name:</span></span>
    - `Test-AzureRmEventHubName`

### <a name="azurerminsights"></a><span data-ttu-id="4a207-289">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="4a207-289">AzureRM.Insights</span></span>
* <span data-ttu-id="4a207-290">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-290">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="4a207-291">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4a207-291">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4a207-292">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-292">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="4a207-293">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a207-293">AzureRM.Network</span></span>
* <span data-ttu-id="4a207-294">上書きの確認メッセージ "リソースを上書きしますか" を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-294">Fix overwrite message 'Are you sure you want to overwriteresource'</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="4a207-295">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-295">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="4a207-296">`Invoke-AzureRmOperationalInsightsQuery` を介した V2 API クエリ実行のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-296">Added support for V2 API querying via `Invoke-AzureRmOperationalInsightsQuery`.</span></span> <span data-ttu-id="4a207-297">新しい API の詳細については、[https://dev.loganalytics.io/](https://dev.loganalytics.io/) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a207-297">See [https://dev.loganalytics.io/](https://dev.loganalytics.io/) for more info on the new API.</span></span>

### <a name="azurermresources"></a><span data-ttu-id="4a207-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4a207-298">AzureRM.Resources</span></span>
* <span data-ttu-id="4a207-299">`Get-AzureRmADServicePrincipal`: SPN パラメーター セットと冗長であるため、既定の空のパラメーター セットから `-ServicePrincipalName` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-299">`Get-AzureRmADServicePrincipal`: Removed `-ServicePrincipalName` from the default Empty parameter set as it was redundant with the SPN parameter set</span></span>

### <a name="azurermservicebus"></a><span data-ttu-id="4a207-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4a207-300">AzureRM.ServiceBus</span></span>

* <span data-ttu-id="4a207-301">`Remove-AzureRmServiceBusRule` および `Get-AzureRmServiceBusKey` の機能修正プログラムを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-301">Added functionality fix for `Remove-AzureRmServiceBusRule` and `Get-AzureRmServiceBusKey`</span></span>
* <span data-ttu-id="4a207-302">Geo ディザスター リカバリー操作用に、以下の新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-302">Added below new commandlets for Geo Disaster Recovery operations.</span></span>
  - <span data-ttu-id="4a207-303">新しい別名 (ディザスター リカバリーの構成) を作成する</span><span class="sxs-lookup"><span data-stu-id="4a207-303">Creating a new Alias (Disaster Recovery configuration):</span></span>
    - `New-AzureRmServiceBusDRConfigurations`
  - <span data-ttu-id="4a207-304">別名 (ディザスター リカバリー構成) を取得する</span><span class="sxs-lookup"><span data-stu-id="4a207-304">Retrieve Alias (Disaster Recovery configuration) :</span></span>
    - `Get-AzureRmServiceBusDRConfigurations`
  - <span data-ttu-id="4a207-305">ディザスター リカバリーを無効にし、プライマリ名前空間からセカンダリ名前空間への変更の複製を停止する</span><span class="sxs-lookup"><span data-stu-id="4a207-305">Disabling the Disaster Recovery and stops replicating changes from primary to secondary namespaces</span></span>
    - `Set-AzureRmServiceBusDRConfigurationsBreakPairing`
  - <span data-ttu-id="4a207-306">ディザスター リカバリー フェールオーバーを呼び出し、セカンダリ名前空間を指すように別名を再構成する</span><span class="sxs-lookup"><span data-stu-id="4a207-306">Invoking Disaster Recovery failover and reconfigure the alias to point to the secondary namespace</span></span>
    - `Set-AzureRmServiceBusDRConfigurationsFailOver`
  - <span data-ttu-id="4a207-307">別名 (ディザスター リカバリー構成) を削除する</span><span class="sxs-lookup"><span data-stu-id="4a207-307">Deleting an Alias(Disaster Recovery configuration)</span></span>
    - `Remove-AzureRmServiceBusDRConfigurations`
* <span data-ttu-id="4a207-308">Geo ディザスター リカバリーをサポートするように `Test-AzureRmServiceBusName` コマンドレットを更新しました - 別名の可用性チェック操作。</span><span class="sxs-lookup"><span data-stu-id="4a207-308">Updated `Test-AzureRmServiceBusName` commandlets to support Geo Disaster Recovery - Alias name check availability operations.</span></span>
  - <span data-ttu-id="4a207-309">名前空間名または別名 (ディザスター リカバリーの構成) の可用性のチェック</span><span class="sxs-lookup"><span data-stu-id="4a207-309">Check the Availability of Namespace name or Alias(Disaster Recovery configuration) name:</span></span>
    - `Test-AzureRmServiceBusName`

### <a name="azurermusageaggregates"></a><span data-ttu-id="4a207-310">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="4a207-310">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="4a207-311">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-311">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

## <a name="520---january-2018"></a><span data-ttu-id="4a207-312">5.2.0 - 2018 年 1 月</span><span class="sxs-lookup"><span data-stu-id="4a207-312">5.2.0 - January 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="4a207-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="4a207-313">AzureRM.Profile</span></span>
* <span data-ttu-id="4a207-314">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-314">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-315">Add-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="4a207-315">Add-AzureRmAccount</span></span>
  * <span data-ttu-id="4a207-316">現在の VM/サービスの管理サービス ID の資格情報を使用して認証を行う -MSI ログインを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-316">Added -MSI login for authenticationg using the credentials of the Managed Service Identity of the current VM / Service</span></span>
  * <span data-ttu-id="4a207-317">ユーザー指定のアクセス トークンを使用してログインする場合の KeyVault 認証を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-317">Fixed KeyVault Authentication when logging in with user-provided access tokens</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="4a207-318">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-318">Azure.Storage</span></span>
* <span data-ttu-id="4a207-319">Storage サービスのプロパティを取得および設定するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-319">Add cmdlets to get and set Storage service properties</span></span>
    - <span data-ttu-id="4a207-320">Get-AzureStorageServiceProperty</span><span class="sxs-lookup"><span data-stu-id="4a207-320">Get-AzureStorageServiceProperty</span></span>
    - <span data-ttu-id="4a207-321">Update-AzureStorageServiceProperty</span><span class="sxs-lookup"><span data-stu-id="4a207-321">Update-AzureStorageServiceProperty</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="4a207-322">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a207-322">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="4a207-323">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-323">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="4a207-324">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4a207-324">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="4a207-325">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-325">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-326">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-326">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-327">New-AzureRmApiManagementProperty、Set-AzureRmApiManagementProperty、および New-AzureRmApiManagement で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-327">Obsoleted -Tags in favor of -Tag for New-AzureRmApiManagementProperty, Set-AzureRmApiManagementProperty, and New-AzureRmApiManagement</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="4a207-328">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-328">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="4a207-329">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-329">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-330">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-330">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="4a207-331">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="4a207-331">AzureRM.Automation</span></span>
* <span data-ttu-id="4a207-332">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-332">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-333">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-333">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-334">Set-AzureRmAutomationRunbook で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-334">Obsoleted -Tags in favor of -Tag for Set-AzureRmAutomationRunbook</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="4a207-335">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="4a207-335">AzureRM.Backup</span></span>
* <span data-ttu-id="4a207-336">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-336">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-337">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-337">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="4a207-338">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="4a207-338">AzureRM.Batch</span></span>
* <span data-ttu-id="4a207-339">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-339">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-340">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-340">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="4a207-341">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="4a207-341">AzureRM.Cdn</span></span>
* <span data-ttu-id="4a207-342">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-342">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-343">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-343">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-344">New-AzureRmCdnEndpoint および New-AzureRmCdnProfile で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-344">Obsoleted -Tags in favor of -Tag for New-AzureRmCdnEndpoint and New-AzureRmCdnProfile</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="4a207-345">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="4a207-345">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="4a207-346">Cognitive Services Management SDK バージョン 3.0.0 と統合しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-346">Integrate with Cognitive Services Management SDK version 3.0.0.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="4a207-347">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a207-347">AzureRM.Compute</span></span>
* <span data-ttu-id="4a207-348">簡素化したパラメーター セットを New-AzureRmVmss に追加しました。これにより、スマートな既定値を使用して、仮想マシン スケール セットおよびすべての必要なリソースを作成できます</span><span class="sxs-lookup"><span data-stu-id="4a207-348">Added simplified parameter set to New-AzureRmVmss, which creates a Virtual Machine Scale Set and all required resources using smart defaults</span></span>
* <span data-ttu-id="4a207-349">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-349">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-350">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-350">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-351">New-AzureRmVm および Update-AzureRmVm で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-351">Obsoleted -Tags in favor of -Tag for New-AzureRmVm and Update-AzureRmVm</span></span>
* <span data-ttu-id="4a207-352">ゾーンが制限に含まれる場合の Get AzureRmComputeResourceSku コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-352">Fixed Get-AzureRmComputeResourceSku cmdlet when Zone is included in restriction.</span></span>
* <span data-ttu-id="4a207-353">Azure Monitor シンクがサポートされるように、診断エージェントの構成スキーマを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-353">Updated Diagnostics Agent configuration schema for Azure Monitor sink support.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="4a207-354">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4a207-354">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="4a207-355">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-355">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-356">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-356">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="4a207-357">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="4a207-357">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="4a207-358">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-358">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-359">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-359">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="4a207-360">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="4a207-360">AzureRM.DataFactories</span></span>
* <span data-ttu-id="4a207-361">データ ストアのリンクされたサービスすべてについて、Azure Key Vault のサポートを有効にしました</span><span class="sxs-lookup"><span data-stu-id="4a207-361">Enabled Azure Key Vault support for all data store linked services</span></span>
* <span data-ttu-id="4a207-362">Azure SSIS 統合ランタイムにライセンスの種類プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-362">Added license type property for Azure SSIS integration runtime</span></span>
* <span data-ttu-id="4a207-363">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-363">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-364">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-364">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-365">New-AzureRmDataFactory で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-365">Obsoleted -Tags in favor of -Tag for New-AzureRmDataFactory</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="4a207-366">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4a207-366">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="4a207-367">データ ストアのリンクされたサービスすべてについて、Azure Key Vault のサポートを有効にしました</span><span class="sxs-lookup"><span data-stu-id="4a207-367">Enabled Azure Key Vault support for all data store linked services</span></span>
* <span data-ttu-id="4a207-368">Azure SSIS 統合ランタイムにライセンスの種類プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-368">Added license type property for Azure SSIS integration runtime</span></span>
* <span data-ttu-id="4a207-369">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-369">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-370">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-370">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-371">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドで AHUB 機能を有効にするための "LicenseType" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-371">Add parameter "LicenseType" for "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd to enable AHUB functionality</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="4a207-372">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4a207-372">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="4a207-373">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-373">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-374">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-374">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-375">New-AzureRmDataLakeAnalyticsAccount および Set-AzureRmDataLakeAnalyticsAccount で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-375">Obsoleted -Tags in favor of -Tag for New-AzureRmDataLakeAnalyticsAccount and Set-AzureRmDataLakeAnalyticsAccount</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="4a207-376">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4a207-376">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="4a207-377">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-377">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-378">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-378">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-379">New-AzureRmDataLakeStoreAccount および Set-AzureRmDataLakeStoreAccount で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-379">Obsoleted -Tags in favor of -Tag for New-AzureRmDataLakeStoreAccount and Set-AzureRmDataLakeStoreAccount</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="4a207-380">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="4a207-380">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="4a207-381">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-381">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="4a207-382">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="4a207-382">AzureRM.Dns</span></span>
* <span data-ttu-id="4a207-383">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-383">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="4a207-384">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="4a207-384">AzureRM.EventGrid</span></span>
* <span data-ttu-id="4a207-385">次の新しいコマンドレッドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-385">Added the following new cmdlet:</span></span>
  - <span data-ttu-id="4a207-386">Update-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="4a207-386">Update-AzureRmEventGridSubscription</span></span>
    - <span data-ttu-id="4a207-387">Event Grid イベント サブスクリプションのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4a207-387">Update the properties of an Event Grid event subscription.</span></span>
* <span data-ttu-id="4a207-388">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-388">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-389">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-389">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="4a207-390">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="4a207-390">AzureRM.EventHub</span></span>
* <span data-ttu-id="4a207-391">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-391">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-392">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-392">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="4a207-393">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a207-393">AzureRM.HDInsight</span></span>
* <span data-ttu-id="4a207-394">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-394">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-395">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-395">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="4a207-396">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="4a207-396">AzureRM.Insights</span></span>
* <span data-ttu-id="4a207-397">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-397">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-398">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-398">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="4a207-399">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="4a207-399">AzureRM.IotHub</span></span>
* <span data-ttu-id="4a207-400">IoTHub コマンドレットの証明書のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-400">Add Certificate support for IoTHub cmdlets</span></span>
* <span data-ttu-id="4a207-401">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-401">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-402">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-402">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="4a207-403">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4a207-403">AzureRM.KeyVault</span></span>
* <span data-ttu-id="4a207-404">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-404">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-405">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-405">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-406">実行時間が長い KeyVault コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-406">Added -AsJob support for long-running KeyVault cmdlets.</span></span> <span data-ttu-id="4a207-407">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-407">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
  * <span data-ttu-id="4a207-408">影響を受けるコマンドレット: Remove-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="4a207-408">Affected cmdlet is: Remove-AzureRmKeyVault</span></span>
* <span data-ttu-id="4a207-409">Set-AzureRmKeyVaultAccessPolicy のバグを修正しました。このバグでは AAD フィルターによって UPN が設定されるのではなく、SPN が指定の UPN に設定されていました</span><span class="sxs-lookup"><span data-stu-id="4a207-409">Fixed bug in Set-AzureRmKeyVaultAccessPolicy where the AAD filter was setting SPN to the provided UPN, rather than setting the UPN</span></span>
  - <span data-ttu-id="4a207-410">詳細については次の問題を参照してください: https://github.com/Azure/azure-powershell/issues/5201</span><span class="sxs-lookup"><span data-stu-id="4a207-410">See the following issue for more information: https://github.com/Azure/azure-powershell/issues/5201</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="4a207-411">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="4a207-411">AzureRM.LogicApp</span></span>
* <span data-ttu-id="4a207-412">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-412">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-413">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-413">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="4a207-414">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="4a207-414">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="4a207-415">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-415">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-416">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-416">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-417">Update-AzureRmMlCommitmentPlan で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-417">Obsoleted -Tags in favor of -Tag for Update-AzureRmMlCommitmentPlan</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="4a207-418">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="4a207-418">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="4a207-419">Remove-AzureRmMlOpCluster コマンドレットに IncludeAllResources パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-419">Add IncludeAllResources parameter to Remove-AzureRmMlOpCluster cmdlet</span></span>
  - <span data-ttu-id="4a207-420">このスイッチ パラメーターを使用すると、最初にクラスターで作成されたすべてのリソースが削除されます</span><span class="sxs-lookup"><span data-stu-id="4a207-420">Using this switch parameter will remove all resources that were created with the cluster originally</span></span>
* <span data-ttu-id="4a207-421">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-421">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-422">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-422">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="4a207-423">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="4a207-423">AzureRM.Media</span></span>
* <span data-ttu-id="4a207-424">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-424">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-425">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-425">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-426">Set-AzureRmMediaService および New-AzureRmMediaService で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-426">Obsoleted -Tags in favor of -Tag for Set-AzureRmMediaService and New-AzureRmMediaService</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="4a207-427">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="4a207-427">AzureRM.Network</span></span>
* <span data-ttu-id="4a207-428">実行時間が長い Network コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-428">Added -AsJob support for long-running Network cmdlets.</span></span> <span data-ttu-id="4a207-429">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-429">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
* <span data-ttu-id="4a207-430">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-430">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-431">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-431">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="4a207-432">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="4a207-432">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="4a207-433">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-433">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-434">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-434">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-435">New-AzureRmNotificationHubsNamespace および Set-AzureRmNotificationHubsNamespace で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-435">Obsoleted -Tags in favor of -Tag for New-AzureRmNotificationHubsNamespace and Set-AzureRmNotificationHubsNamespace</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="4a207-436">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-436">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="4a207-437">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-437">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-438">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-438">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-439">New-AzureRmOperationalInsightsSavedSearch、Set-AzureRmOperationalInsightsSavedSearch、New-AzureRmOperationalInsightsWorkspace、および Set-AzureRmOperationalInsightsWorkspace で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-439">Obsoleted -Tags in favor of -Tag for New-AzureRmOperationalInsightsSavedSearch, Set-AzureRmOperationalInsightsSavedSearch, New-AzureRmOperationalInsightsWorkspace, and Set-AzureRmOperationalInsightsWorkspace</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="4a207-440">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="4a207-440">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="4a207-441">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-441">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-442">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-442">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="4a207-443">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4a207-443">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="4a207-444">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-444">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-445">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-445">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="4a207-446">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4a207-446">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="4a207-447">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-447">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-448">the Restore-AzureRmRecoveryServicesBackupItem コマンドレッドに -UseOriginalStorageAccount オプションを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-448">Added -UseOriginalStorageAccount option to the Restore-AzureRmRecoveryServicesBackupItem cmdlet.</span></span>
  - <span data-ttu-id="4a207-449">このフラグを有効にすると、元のストレージ アカウントにディスクが復元されます。これにより、ユーザーは復元された VM の構成を元の VM にできる限り近いものに維持できます。</span><span class="sxs-lookup"><span data-stu-id="4a207-449">Enabling this flag results in restoring disks to their original storage accounts which allows users to maintain the configuration of restored VM as close to the original VMs as possible.</span></span>
  - <span data-ttu-id="4a207-450">これは、復元操作のパフォーマンスの向上にも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="4a207-450">It also helps in improving the performance of the restore operation.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="4a207-451">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="4a207-451">AzureRM.RedisCache</span></span>
* <span data-ttu-id="4a207-452">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-452">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-453">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-453">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-454">ファイアウォール規則のために 3 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-454">Added  3 new cmdlets for firewall rules</span></span>
* <span data-ttu-id="4a207-455">geo レプリケーションのために 3 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-455">Added  3 new cmdlets for geo replication</span></span>
* <span data-ttu-id="4a207-456">ゾーンとタグのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-456">Added support for zones and tags</span></span>
* <span data-ttu-id="4a207-457">可能な場合は、ResourceGroup を省略可能としてマークしてください。</span><span class="sxs-lookup"><span data-stu-id="4a207-457">Make ResourceGroup as optional whenever possible.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="4a207-458">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="4a207-458">AzureRM.Relay</span></span>
* <span data-ttu-id="4a207-459">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-459">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-460">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-460">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="4a207-461">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="4a207-461">AzureRM.Resources</span></span>
* <span data-ttu-id="4a207-462">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-462">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-463">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-463">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-464">実行時間が長い Resources コマンドのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-464">Added -AsJob support for long-running Resources cmdlets.</span></span> <span data-ttu-id="4a207-465">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-465">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
* <span data-ttu-id="4a207-466">名前付け規則に準拠するように Get AzureRmProviderOperation から Get-AzureRmResourceProviderAction に別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-466">Added alias from Get-AzureRmProviderOperation to Get-AzureRmResourceProviderAction to conform with naming conventions</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="4a207-467">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="4a207-467">AzureRM.Scheduler</span></span>
* <span data-ttu-id="4a207-468">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-468">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-469">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-469">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermservermanagement"></a><span data-ttu-id="4a207-470">AzureRM.ServerManagement</span><span class="sxs-lookup"><span data-stu-id="4a207-470">AzureRM.ServerManagement</span></span>
* <span data-ttu-id="4a207-471">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-471">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-472">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-472">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-473">New-AzureRmServerManagementNode および New-AzureRmServerManagementGateway で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-473">Obsoleted -Tags in favor of -Tag for New-AzureRmServerManagementNode and New-AzureRmServerManagementGateway</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="4a207-474">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4a207-474">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="4a207-475">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-475">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-476">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-476">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="4a207-477">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="4a207-477">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="4a207-478">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-478">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-479">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-479">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermsiterecovery"></a><span data-ttu-id="4a207-480">AzureRM.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-480">AzureRM.SiteRecovery</span></span>
* <span data-ttu-id="4a207-481">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-481">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-482">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-482">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="4a207-483">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4a207-483">AzureRM.Sql</span></span>
* <span data-ttu-id="4a207-484">監査コマンドのパラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-484">Update the Auditing commands parameters description</span></span>
* <span data-ttu-id="4a207-485">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-485">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-486">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-486">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-487">実行時間の長いコマンドレットに -AsJob パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-487">Added -AsJob parameter to long running cmdlets</span></span>
* <span data-ttu-id="4a207-488">Get AzureRmSqlServiceObjective の - DatabaseName パラメーターを廃止しました</span><span class="sxs-lookup"><span data-stu-id="4a207-488">Obsoleted -DatabaseName parameter from Get-AzureRmSqlServiceObjective</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="4a207-489">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-489">AzureRM.Storage</span></span>
* <span data-ttu-id="4a207-490">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-490">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-491">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-491">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-492">-EnableEncryptionService None パラメーターを指定した New-AzureRMStorageAccount コマンドレットを実行した際の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-492">Fix a null reference issue of run cmdlet New-AzureRMStorageAccount with parameter -EnableEncryptionService None</span></span>
* <span data-ttu-id="4a207-493">実行時間が長い Storage コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-493">Added -AsJob support for long-running Storage cmdlets.</span></span> <span data-ttu-id="4a207-494">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-494">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
    - <span data-ttu-id="4a207-495">影響を受けるコマンドレットは、Storage Account および Storage Account Network Rule の New-、Remove-、Add-、Update- です。</span><span class="sxs-lookup"><span data-stu-id="4a207-495">Affected cmdlets are New-, Remove-, Add-, and Update- for Storage Account and Storage Account Network Rule.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="4a207-496">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="4a207-496">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="4a207-497">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-497">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-498">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-498">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="4a207-499">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4a207-499">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="4a207-500">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-500">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-501">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-501">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="4a207-502">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="4a207-502">AzureRM.Websites</span></span>
* <span data-ttu-id="4a207-503">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-503">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="4a207-504">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-504">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="4a207-505">実行時間が長い Websites コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-505">Added -AsJob support for long-running Websites cmdlets.</span></span> <span data-ttu-id="4a207-506">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-506">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
     - <span data-ttu-id="4a207-507">影響を受けるコマンドレットは、WebApps、AppServicePlan、および Slots の New-、Remove-、Add-、Set- です</span><span class="sxs-lookup"><span data-stu-id="4a207-507">Affected cmdlets are New-, Remove-, Add-, and Set- for WebApps, AppServicePlan and Slots</span></span>

## <a name="2017128-version-511"></a><span data-ttu-id="4a207-508">2017.12.8 バージョン 5.1.1</span><span class="sxs-lookup"><span data-stu-id="4a207-508">2017.12.8 Version 5.1.1</span></span>
* <span data-ttu-id="4a207-509">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a207-509">AnalysisServices</span></span>
  - <span data-ttu-id="4a207-510">すべてのクラウドがサポートされるように、場所の検証セットを動的ルックアップに変更しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-510">Change validate set of location to dynamic lookup so that all clouds are supported.</span></span>
* <span data-ttu-id="4a207-511">Automation</span><span class="sxs-lookup"><span data-stu-id="4a207-511">Automation</span></span>
  - <span data-ttu-id="4a207-512">Import-AzureRMAutomationRunbook に更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-512">Update to Import-AzureRMAutomationRunbook</span></span>
    - <span data-ttu-id="4a207-513">Python2 Runbook がサポートされるようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-513">Support is now being provided for Python2 runbooks</span></span>
* <span data-ttu-id="4a207-514">Batch</span><span class="sxs-lookup"><span data-stu-id="4a207-514">Batch</span></span>
  - <span data-ttu-id="4a207-515">リソース グループがないアカウント操作がリソース グループの自動検出に失敗するというバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-515">Fixed a bug where account operations without a resource group failed to auto-detect the resource group</span></span>
* <span data-ttu-id="4a207-516">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="4a207-516">Compute</span></span>
  - <span data-ttu-id="4a207-517">Get-AzureRmComputeResourceSku によってゾーン情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4a207-517">Get-AzureRmComputeResourceSku shows zone information.</span></span>
  - <span data-ttu-id="4a207-518">問題 https://github.com/Azure/azure-powershell/issues/5038 を修正するために Disable-AzureRmVmssDiskEncryption を更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-518">Update Disable-AzureRmVmssDiskEncryption to fix issue https://github.com/Azure/azure-powershell/issues/5038</span></span>
  - <span data-ttu-id="4a207-519">実行時間が長い Compute コマンドレット用の -AsJob サポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-519">Added -AsJob support for long-running Compute cmdlets.</span></span> <span data-ttu-id="4a207-520">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-520">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
    - <span data-ttu-id="4a207-521">影響を受けるコマンドレット: Virtual Machines および VM Scale Sets の New-、Update-、Set-、Remove-、Start-、Restart-、Stop- コマンドレット</span><span class="sxs-lookup"><span data-stu-id="4a207-521">Affected cmdlets include: New-, Update-, Set-, Remove-, Start-, Restart-, Stop- cmdlets for Virtual Machines and Virtual Machine Scale Sets</span></span>
    - <span data-ttu-id="4a207-522">簡素化したパラメーター セットを New-AzureRmVM に追加しました。これにより、スマートな既定値を使用して、仮想マシンおよびすべての必要なリソースを作成できます</span><span class="sxs-lookup"><span data-stu-id="4a207-522">Added simplified parameter set to New-AzureRmVM, which creates a Virtual Machine and all required resources using smart defaults</span></span>
* <span data-ttu-id="4a207-523">ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="4a207-523">ContainerInstance</span></span>
  - <span data-ttu-id="4a207-524">Azure コンテナー インスタンス SDK 2017-10-01 を適用しました</span><span class="sxs-lookup"><span data-stu-id="4a207-524">Apply Azure Container Instance SDK 2017-10-01</span></span>
    - <span data-ttu-id="4a207-525">コンテナー run-to-completion のサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-525">Support container run-to-completion</span></span>
    - <span data-ttu-id="4a207-526">Azure File ボリューム マウントのサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-526">Support Azure File volume mount</span></span>
    - <span data-ttu-id="4a207-527">パブリック IP の複数ポートのオープンのサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-527">Support opening multiple ports for public IP</span></span>
* <span data-ttu-id="4a207-528">ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="4a207-528">ContainerRegistry</span></span>
  - <span data-ttu-id="4a207-529">geo レプリケーションと webhook の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="4a207-529">New cmdlets for geo-replication and webhooks</span></span>
    - <span data-ttu-id="4a207-530">Get/New/Remove-AzureRmContainerRegistryReplication</span><span class="sxs-lookup"><span data-stu-id="4a207-530">Get/New/Remove-AzureRmContainerRegistryReplication</span></span>
    - <span data-ttu-id="4a207-531">Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook</span><span class="sxs-lookup"><span data-stu-id="4a207-531">Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook</span></span>
* <span data-ttu-id="4a207-532">DataFactories</span><span class="sxs-lookup"><span data-stu-id="4a207-532">DataFactories</span></span>
    - <span data-ttu-id="4a207-533">資格情報の暗号化機能が、"リモート アクセス" 有効 (ネットワーク経由) と "リモート アクセス" 無効 (ローカル コンピューター) の両方で動作するようになりました。</span><span class="sxs-lookup"><span data-stu-id="4a207-533">Credential encryption functionality now works with both "Remote Access" enabled (Over Network) and "Remote Access" disabled (Local Machine).</span></span>
* <span data-ttu-id="4a207-534">DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="4a207-534">DataFactoryV2</span></span>
  - <span data-ttu-id="4a207-535">2 つのコマンドレットを新しく追加しました: Update-AzureRmDataFactoryV2 および Stop-AzureRmDataFactoryV2PipelineRun</span><span class="sxs-lookup"><span data-stu-id="4a207-535">Added two new cmdlets: Update-AzureRmDataFactoryV2 and Stop-AzureRmDataFactoryV2PipelineRun</span></span>
* <span data-ttu-id="4a207-536">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4a207-536">DataLakeAnalytics</span></span>
  - <span data-ttu-id="4a207-537">ScriptParameter というパラメーターを Submit-AzureRmDataLakeAnalyticsJob に追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-537">Added a parameter called ScriptParameter to Submit-AzureRmDataLakeAnalyticsJob</span></span>
    - <span data-ttu-id="4a207-538">ScriptParameter に関する詳細情報を、Submit-AzureRmDataLakeAnalyticsJob で Get-Help を使用して確認できます</span><span class="sxs-lookup"><span data-stu-id="4a207-538">Detailed information about ScriptParameter can be found using Get-Help on Submit-AzureRmDataLakeAnalyticsJob</span></span>
  - <span data-ttu-id="4a207-539">New-AzureRmDataLakeAnalyticsAccount については、パラメーター MaxDegreeOfParallelism を MaxAnalyticsUnits に変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-539">For New-AzureRmDataLakeAnalyticsAccount, changed the parameter MaxDegreeOfParallelism to MaxAnalyticsUnits</span></span>
    - <span data-ttu-id="4a207-540">パラメーター MaxAnalyticsUnits の別名を追加しました: MaxDegreeOfParallelism</span><span class="sxs-lookup"><span data-stu-id="4a207-540">Added an alias for the parameter MaxAnalyticsUnits: MaxDegreeOfParallelism</span></span>
  - <span data-ttu-id="4a207-541">New-AzureRmDataLakeAnalyticsComputePolicy については、パラメーター MaxDegreeOfParallelismPerJob を MaxAnalyticsUnitsPerJob に変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-541">For New-AzureRmDataLakeAnalyticsComputePolicy, changed the parameter MaxDegreeOfParallelismPerJob to MaxAnalyticsUnitsPerJob</span></span>
    - <span data-ttu-id="4a207-542">パラメーター MaxAnalyticsUnitsPerJob の別名を追加しました: MaxDegreeOfParallelismPerJob</span><span class="sxs-lookup"><span data-stu-id="4a207-542">Added an alias for the parameter MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob</span></span>
  - <span data-ttu-id="4a207-543">Set-AzureRmDataLakeAnalyticsAccount については、パラメーター MaxDegreeOfParallelism を MaxAnalyticsUnits に変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-543">For Set-AzureRmDataLakeAnalyticsAccount, changed the parameter MaxDegreeOfParallelism to MaxAnalyticsUnits</span></span>
    - <span data-ttu-id="4a207-544">パラメーター MaxAnalyticsUnits の別名を追加しました: MaxDegreeOfParallelism</span><span class="sxs-lookup"><span data-stu-id="4a207-544">Added an alias for the parameter MaxAnalyticsUnits: MaxDegreeOfParallelism</span></span>
  - <span data-ttu-id="4a207-545">Submit-AzureRmDataLakeAnalyticsJob については、パラメーター DegreeOfParallelism を AnalyticsUnits に変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-545">For Submit-AzureRmDataLakeAnalyticsJob, changed the parameter DegreeOfParallelism to AnalyticsUnits</span></span>
    - <span data-ttu-id="4a207-546">パラメーター AnalyticsUnits の別名を追加しました: DegreeOfParallelism</span><span class="sxs-lookup"><span data-stu-id="4a207-546">Added an alias for the parameter AnalyticsUnits: DegreeOfParallelism</span></span>
  - <span data-ttu-id="4a207-547">Update-AzureRmDataLakeAnalyticsComputePolicy については、パラメーター MaxDegreeOfParallelismPerJob を MaxAnalyticsUnitsPerJob に変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-547">For Update-AzureRmDataLakeAnalyticsComputePolicy, changed the parameter MaxDegreeOfParallelismPerJob to MaxAnalyticsUnitsPerJob</span></span>
    - <span data-ttu-id="4a207-548">パラメーター MaxAnalyticsUnitsPerJob の別名を追加しました: MaxDegreeOfParallelismPerJob</span><span class="sxs-lookup"><span data-stu-id="4a207-548">Added an alias for the parameter MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob</span></span>
* <span data-ttu-id="4a207-549">MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="4a207-549">MachineLearningCompute</span></span>
  - <span data-ttu-id="4a207-550">Set-AzureRmMlOpCluster を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-550">Add Set-AzureRmMlOpCluster</span></span>
    - <span data-ttu-id="4a207-551">クラスターのエージェント数または SSL 構成を更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-551">Update a cluster's agent count or SSL configuration</span></span>
  - <span data-ttu-id="4a207-552">オーケストレーター プロパティがオプションになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-552">Orchestrator properties are optional</span></span>
    - <span data-ttu-id="4a207-553">サービス プリンシパルが提供されていない場合、そのサービス プリンシパルはサービスによって作成されるため、オーケストレーター プロパティがオプションになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-553">The service will create a service principal if not provided, so the orchestrator properties are now optional</span></span>
* <span data-ttu-id="4a207-554">PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="4a207-554">PowerBIEmbedded</span></span>
  - <span data-ttu-id="4a207-555">Power BI Embedded 容量コマンドレットのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-555">Add support for Power BI Embedded Capacity cmdlets</span></span>
  - <span data-ttu-id="4a207-556">新しいコマンドレット Get-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a207-556">New Cmdlet Get-AzureRmPowerBIEmbeddedCapacity - Gets the details of a PowerBI Embedded Capacity.</span></span>
  - <span data-ttu-id="4a207-557">新しいコマンドレット New-AzureRmPowerBIEmbeddedCapacity - 新しい PowerBI Embedded 容量を作成します</span><span class="sxs-lookup"><span data-stu-id="4a207-557">New Cmdlet New-AzureRmPowerBIEmbeddedCapacity - Creates a new PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="4a207-558">新しいコマンドレット Remove-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを削除します</span><span class="sxs-lookup"><span data-stu-id="4a207-558">New Cmdlet Remove-AzureRmPowerBIEmbeddedCapacity - Deletes an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="4a207-559">新しいコマンドレット Resume-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを再開します</span><span class="sxs-lookup"><span data-stu-id="4a207-559">New Cmdlet Resume-AzureRmPowerBIEmbeddedCapacity - Resumes an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="4a207-560">新しいコマンドレット Suspend-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを中断します</span><span class="sxs-lookup"><span data-stu-id="4a207-560">New Cmdlet Suspend-AzureRmPowerBIEmbeddedCapacity - Suspends an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="4a207-561">新しいコマンドレット Test-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスの存在をテストします</span><span class="sxs-lookup"><span data-stu-id="4a207-561">New Cmdlet Test-AzureRmPowerBIEmbeddedCapacity - Tests the existence of an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="4a207-562">新しいコマンドレット Update-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを変更します</span><span class="sxs-lookup"><span data-stu-id="4a207-562">New Cmdlet Update-AzureRmPowerBIEmbeddedCapacity - Modifies an instance of PowerBI Embedded Capacity</span></span>
* <span data-ttu-id="4a207-563">プロファイル</span><span class="sxs-lookup"><span data-stu-id="4a207-563">Profile</span></span>
  - <span data-ttu-id="4a207-564">USGovernmentActiveDirectoryEndpoint を https://login.microsoftonline.us/ に更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-564">Updated USGovernmentActiveDirectoryEndpoint to https://login.microsoftonline.us/</span></span>
    - <span data-ttu-id="4a207-565">Azure Government エンドポイント マッピングの詳細については、https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping を参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-565">For more information about the Azure Government endpoint mappings, please see the following: https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping</span></span>
    - <span data-ttu-id="4a207-566">コマンドの -AsJob サポートを追加しました。これにより、選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます</span><span class="sxs-lookup"><span data-stu-id="4a207-566">Added -AsJob support for cmdlets, enabling selected cmdlets to execute in the background and return a job to track and control progress</span></span>
    - <span data-ttu-id="4a207-567">-AsJob パラメーターを Get-AzureRmSubscription コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-567">Added -AsJob parameter to Get-AzureRmSubscription cmdlet</span></span>
* <span data-ttu-id="4a207-568">RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4a207-568">RecoveryServices.Backup</span></span>
  - <span data-ttu-id="4a207-569">バグを修正 - Get-AzureRmRecoveryServicesBackupItem が、コンテナー名フィルターの比較で大文字と小文字を区別するようになりました。</span><span class="sxs-lookup"><span data-stu-id="4a207-569">Fixed bug - Get-AzureRmRecoveryServicesBackupItem should do case insensitive comparison for container name filter.</span></span>
  - <span data-ttu-id="4a207-570">バグを修正 - AzureVmItem に、前回のバックアップ操作が行われた時間を示すプロパティが追加されました - LastBackupTime。</span><span class="sxs-lookup"><span data-stu-id="4a207-570">Fixed bug - AzureVmItem now has a property that shows the last time a backup operation has happened - LastBackupTime.</span></span>
* <span data-ttu-id="4a207-571">リソース</span><span class="sxs-lookup"><span data-stu-id="4a207-571">Resources</span></span>
  - <span data-ttu-id="4a207-572">Get-AzureRMRoleAssignment による割り当てで、カスタム ロールの roledefiniton 名がないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-572">Fixed issue where Get-AzureRMRoleAssignment would result in a assignments without roledefiniton name for custom roles</span></span>
    - <span data-ttu-id="4a207-573">ユーザーは、ロールの種類に関係なく、Get-AzureRMRoleAssignment で、roledefinition 名を持つ割り当てを使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-573">Users can now use Get-AzureRMRoleAssignment with assignments having roledefinition names irrespective of the type of role</span></span>
  - <span data-ttu-id="4a207-574">assignablescopes に新しいスコープがある場合に、RD が見つからないというエラーを Set-AzureRMRoleRoleDefinition がスローするという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-574">Fixed issue where Set-AzureRMRoleRoleDefinition used to throw RD not found error when there was a new scope in assignablescopes</span></span>
    - <span data-ttu-id="4a207-575">ユーザーが、スコープの位置に関係なく、Set-AzureRMRoleRoleDefinition で、新しいスコープを含む割り当て可能なスコープを使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-575">Users can now use Set-AzureRMRoleRoleDefinition with assignable scopes including new scopes irrespective of the position of the scope</span></span>
  - <span data-ttu-id="4a207-576">スコープの末尾に "/" を使用できます</span><span class="sxs-lookup"><span data-stu-id="4a207-576">Allow scopes to end with "/"</span></span>
    - <span data-ttu-id="4a207-577">スコープの末尾が "/" の RoleDefinition および RoleAssignment コマンドレットをユーザーが使用できるようになりました。これにより、API および CLI との一貫性が確保されます</span><span class="sxs-lookup"><span data-stu-id="4a207-577">Users can now use RoleDefinition and RoleAssignment commandlets with scopes ending with "/" ,consistent with API and CLI</span></span>
  - <span data-ttu-id="4a207-578">ユーザーが、委任フラグを使用して RoleAssignment を作成できます</span><span class="sxs-lookup"><span data-stu-id="4a207-578">Allow users to create RoleAssignment using delegation flag</span></span>
    - <span data-ttu-id="4a207-579">ユーザーが、New-AzureRMRoleAssignment で、委任フラグ追加オプションを使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-579">Users can now use New-AzureRMRoleAssignment with an option of adding the delegation flag</span></span>
  - <span data-ttu-id="4a207-580">スコープのパラメーターを優先するように RoleAssignment get を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-580">Fix RoleAssignment get to respect the scope parameter</span></span>
  - <span data-ttu-id="4a207-581">New-AzureRmRoleAssignment コマンドレットに ServicePrincipalName の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-581">Add an alias for ServicePrincipalName in the New-AzureRmRoleAssignment Commandlet</span></span>
    - <span data-ttu-id="4a207-582">ユーザーが、New- AzureRmRoleAssignment コマンドレットを使用するときに、ServicePrincipalName ではなく ApplicationId を使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-582">Users can now use the ApplicationId instead of the ServicePrincipalName when using the New-AzureRmRoleAssignment commandlet</span></span>
* <span data-ttu-id="4a207-583">SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-583">SiteRecovery</span></span>
  - <span data-ttu-id="4a207-584">次の重大な変更のリリースに備えて、このモジュールのすべてのコマンドレットに非推奨警告を追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-584">Add deprecation warnings for all cmdlets in this module in preparation for the next breaking change release.</span></span>
    - <span data-ttu-id="4a207-585">AzureRM からコマンドレットを移行する方法の詳細については、今後の重大な変更ガイドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a207-585">Please see the upcoming breaking changes guide for more information on how to migrate your cmdlets from AzureRM.</span></span>
* <span data-ttu-id="4a207-586">SQL</span><span class="sxs-lookup"><span data-stu-id="4a207-586">Sql</span></span>
  - <span data-ttu-id="4a207-587">Set-AzureRmSqlDatabase を使用して、データベースの名前を変更する機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-587">Added ability to rename database using Set-AzureRmSqlDatabase</span></span>
  - <span data-ttu-id="4a207-588">修正された問題 https://github.com/Azure/azure-powershell/issues/4974</span><span class="sxs-lookup"><span data-stu-id="4a207-588">Fixed issue https://github.com/Azure/azure-powershell/issues/4974</span></span>
    - <span data-ttu-id="4a207-589">監査コマンドレットに無効な AUDIT_CHANGED_GROUP 値を指定しても、エラーがスローされなくなりました。これは今後のリリースで削除される予定です。</span><span class="sxs-lookup"><span data-stu-id="4a207-589">Providing invalid AUDIT_CHANGED_GROUP value for auditing cmdlets no longer throws an error and will be removed in an upcoming release.</span></span>
  - <span data-ttu-id="4a207-590">修正された問題 https://github.com/Azure/azure-powershell/issues/5046</span><span class="sxs-lookup"><span data-stu-id="4a207-590">Fixed issue https://github.com/Azure/azure-powershell/issues/5046</span></span>
    - <span data-ttu-id="4a207-591">監査コマンドレットの AuditAction パラメーターが無視されなくなりました</span><span class="sxs-lookup"><span data-stu-id="4a207-591">AuditAction parameter in auditing cmdlets is no longer being ignored</span></span>
  - <span data-ttu-id="4a207-592">"Secondary" StorageKeyType を指定したときの監査コマンドレットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-592">Fixed an issue in Auditing cmdlets when 'Secondary' StorageKeyType is provided</span></span>
    - <span data-ttu-id="4a207-593">BLOB 監査の設定時に、StorageKeyType パラメーターに "Secondary" 値を指定すると、セカンダリ ストレージ アカウント キーではなくプライマリ キーが使用されました。</span><span class="sxs-lookup"><span data-stu-id="4a207-593">When setting blob auditing, the primary storage account key was used instead of the secondary key when providing 'Secondary' value for StorageKeyType parameter.</span></span>
  - <span data-ttu-id="4a207-594">Set-AzureRmSqlServerTransparentDataEncryptionProtector からの確認メッセージの表現を変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-594">Changing the wording for confirmation message from Set-AzureRmSqlServerTransparentDataEncryptionProtector</span></span>
* <span data-ttu-id="4a207-595">Azure (RDFE)</span><span class="sxs-lookup"><span data-stu-id="4a207-595">Azure (RDFE)</span></span>
    - <span data-ttu-id="4a207-596">すべての RemoteApp コマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="4a207-596">Removed all RemoteApp Cmdles</span></span>
* <span data-ttu-id="4a207-597">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-597">Azure.Storage</span></span>
    - <span data-ttu-id="4a207-598">Azure Storage Client Library 8.6.0 および Azure Storage DataMovement Library 0.6.5 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="4a207-598">Upgrade to Azure Storage Client Library 8.6.0 and Azure Storage DataMovement Library 0.6.5</span></span>

## <a name="20171110-version-501"></a><span data-ttu-id="4a207-599">2017.11.10 バージョン 5.0.1</span><span class="sxs-lookup"><span data-stu-id="4a207-599">2017.11.10 Version 5.0.1</span></span>
* <span data-ttu-id="4a207-600">以下のモジュールで一部のコマンドレットを実行した際に失敗の原因となるアセンブリ読み込みの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-600">Fixed assembly loading issue that caused some cmdlets to fail when executing in the following modules:</span></span>
  - <span data-ttu-id="4a207-601">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4a207-601">AzureRM.ApiManagement</span></span>
  - <span data-ttu-id="4a207-602">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="4a207-602">AzureRM.Backup</span></span>
  - <span data-ttu-id="4a207-603">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="4a207-603">AzureRM.Batch</span></span>
  - <span data-ttu-id="4a207-604">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="4a207-604">AzureRM.Compute</span></span>
  - <span data-ttu-id="4a207-605">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="4a207-605">AzureRM.DataFactories</span></span>
  - <span data-ttu-id="4a207-606">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="4a207-606">AzureRM.HDInsight</span></span>
  - <span data-ttu-id="4a207-607">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="4a207-607">AzureRM.KeyVault</span></span>
  - <span data-ttu-id="4a207-608">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="4a207-608">AzureRM.RecoveryServices</span></span>
  - <span data-ttu-id="4a207-609">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4a207-609">AzureRM.RecoveryServices.Backup</span></span>
  - <span data-ttu-id="4a207-610">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-610">AzureRM.RecoveryServices.SiteRecovery</span></span>
  - <span data-ttu-id="4a207-611">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="4a207-611">AzureRM.RedisCache</span></span>
  - <span data-ttu-id="4a207-612">AzureRM.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-612">AzureRM.SiteRecovery</span></span>
  - <span data-ttu-id="4a207-613">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="4a207-613">AzureRM.Sql</span></span>
  - <span data-ttu-id="4a207-614">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-614">AzureRM.Storage</span></span>
  - <span data-ttu-id="4a207-615">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="4a207-615">AzureRM.StreamAnalytics</span></span>

## <a name="2017118---version-500"></a><span data-ttu-id="4a207-616">2017.11.8 - バージョン 5.0.0</span><span class="sxs-lookup"><span data-stu-id="4a207-616">2017.11.8 - Version 5.0.0</span></span>
* <span data-ttu-id="4a207-617">注: これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="4a207-617">NOTE: This is a breaking change release.</span></span> <span data-ttu-id="4a207-618">導入された重大な変更の完全な一覧については、移行ガイド (https://aka.ms/azps-migration-guide)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a207-618">Please see the migration guide (https://aka.ms/azps-migration-guide) for a full list of introduced breaking changes.</span></span>
* <span data-ttu-id="4a207-619">AzureRM のコマンドレットはすべて、オンライン ヘルプをサポートするようになりました</span><span class="sxs-lookup"><span data-stu-id="4a207-619">All cmdlets in AzureRM now support online help</span></span>
  - <span data-ttu-id="4a207-620">-Online パラメーターを指定して Get-Help を実行すると、既定のインターネット ブラウザーでオンライン ヘルプが表示されます</span><span class="sxs-lookup"><span data-stu-id="4a207-620">Run Get-Help with the -Online parameter to open the online help in your default Internet browser</span></span>
* <span data-ttu-id="4a207-621">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="4a207-621">AnalysisServices</span></span>
  * <span data-ttu-id="4a207-622">同期のために新しい AsAzure REST API と連携するように Synchronize-AzureAsInstance コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-622">Fixed Synchronize-AzureAsInstance command to work with new AsAzure REST API for sync</span></span>
* <span data-ttu-id="4a207-623">ApiManagement</span><span class="sxs-lookup"><span data-stu-id="4a207-623">ApiManagement</span></span>
  * <span data-ttu-id="4a207-624">ApiManagement の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-624">Please see the migration guide for breaking changes made to ApiManagement this release</span></span>
  * <span data-ttu-id="4a207-625">問題 (https://github.com/Azure/azure-powershell/issues/4510) を修正するために Get-AzureRmApiManagementUser コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-625">Updated Cmdlet Get-AzureRmApiManagementUser to fix issue https://github.com/Azure/azure-powershell/issues/4510</span></span>
  * <span data-ttu-id="4a207-626">空のパスを持つ API (https://github.com/Azure/azure-powershell/issues/4069) を作成するために、New-AzureRmApiManagementApi コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-626">Updated Cmdlet New-AzureRmApiManagementApi to create Api with Empty Path https://github.com/Azure/azure-powershell/issues/4069</span></span>
* <span data-ttu-id="4a207-627">ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-627">ApplicationInsights</span></span>
  * <span data-ttu-id="4a207-628">Application Insights のリソースを取得/作成/削除するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-628">Add commands to get/create/remove applicaiton insights resource</span></span>
    - <span data-ttu-id="4a207-629">Get-AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-629">Get-AzureRmApplicationInsights</span></span>
    - <span data-ttu-id="4a207-630">New-AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-630">New-AzureRmApplicationInsights</span></span>
    - <span data-ttu-id="4a207-631">Remove-AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="4a207-631">Remove-AzureRmApplicationInsights</span></span>
  * <span data-ttu-id="4a207-632">Application Insights のリソースの価格/日次上限を取得/更新するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-632">Add commands to get/update pricing/daily cap of applicaiton insights resource</span></span>
    - <span data-ttu-id="4a207-633">Get-AzureRmApplicationInsights -IncludeDailyCap</span><span class="sxs-lookup"><span data-stu-id="4a207-633">Get-AzureRmApplicationInsights -IncludeDailyCap</span></span>
    - <span data-ttu-id="4a207-634">Set-AzureRmApplicationInsightsPricingPlan</span><span class="sxs-lookup"><span data-stu-id="4a207-634">Set-AzureRmApplicationInsightsPricingPlan</span></span>
    - <span data-ttu-id="4a207-635">Set-AzureRmApplicationInsightsDailyCap</span><span class="sxs-lookup"><span data-stu-id="4a207-635">Set-AzureRmApplicationInsightsDailyCap</span></span>
  * <span data-ttu-id="4a207-636">Application Insights のリソースの連続エクスポートを取得/作成/更新/削除するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-636">Add commands to get/create/update/remove continuous export of applicaiton insights resource</span></span>
    - <span data-ttu-id="4a207-637">Get-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="4a207-637">Get-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="4a207-638">Set-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="4a207-638">Set-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="4a207-639">New-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="4a207-639">New-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="4a207-640">Remove-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="4a207-640">Remove-AzureRmApplicationInsightsContinuousExport</span></span>
  * <span data-ttu-id="4a207-641">Application Insights のリソースの API キーを取得/作成/削除するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-641">Add commands to get/create/remove api keys of applicaiton insights resoruce</span></span>
    - <span data-ttu-id="4a207-642">Get-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="4a207-642">Get-AzureRmApplicationInsightsApiKey</span></span>
    - <span data-ttu-id="4a207-643">New-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="4a207-643">New-AzureRmApplicationInsightsApiKey</span></span>
    - <span data-ttu-id="4a207-644">Remove-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="4a207-644">Remove-AzureRmApplicationInsightsApiKey</span></span>
* <span data-ttu-id="4a207-645">AzureBatch</span><span class="sxs-lookup"><span data-stu-id="4a207-645">AzureBatch</span></span>
  * <span data-ttu-id="4a207-646">新しいパラメーターを `New-AzureRmBatchAccount` に追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-646">Added new parameters to `New-AzureRmBatchAccount`.</span></span>
    - <span data-ttu-id="4a207-647">`PoolAllocationMode`: Batch アカウントでプールを作成するために使用する割り当てモード。</span><span class="sxs-lookup"><span data-stu-id="4a207-647">`PoolAllocationMode`: The allocation mode to use for creating pools in the Batch account.</span></span> <span data-ttu-id="4a207-648">ユーザーのサブスクリプションにプール ノードを割り当てる Batch アカウントを作成するには、これを `UserSubscription` に設定します。</span><span class="sxs-lookup"><span data-stu-id="4a207-648">To create a Batch account which allocates pool nodes in the user's subscription, set this to `UserSubscription`.</span></span>
    - <span data-ttu-id="4a207-649">`KeyVaultId`: Batch アカウントに関連付けられている Azure Key Vault のリソース ID。</span><span class="sxs-lookup"><span data-stu-id="4a207-649">`KeyVaultId`: The resource ID of the Azure key vault associated with the Batch account.</span></span>
    - <span data-ttu-id="4a207-650">`KeyVaultUrl`: Batch アカウントに関連付けられている Azure Key Vault の URL。</span><span class="sxs-lookup"><span data-stu-id="4a207-650">`KeyVaultUrl`: The URL of the Azure key vault associated with the Batch account.</span></span>
  * <span data-ttu-id="4a207-651">`New-AzureBatchTask` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-651">Updated parameters to `New-AzureBatchTask`.</span></span>
    - <span data-ttu-id="4a207-652">`RunElevated` スイッチを削除しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-652">Removed the `RunElevated` switch.</span></span> <span data-ttu-id="4a207-653">`RunElevated` の代わりに `UserIdentity` パラメーターを追加しました。以下のように `PSUserIdentity` を作成することにより同じ動作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="4a207-653">The `UserIdentity` parameter has been added to replace `RunElevated`, and the equivalent behavior can be achieved by constructing a `PSUserIdentity` as shown below:</span></span>
      - <span data-ttu-id="4a207-654">$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")</span><span class="sxs-lookup"><span data-stu-id="4a207-654">$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")</span></span>
      - <span data-ttu-id="4a207-655">$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser</span><span class="sxs-lookup"><span data-stu-id="4a207-655">$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser</span></span>
    - <span data-ttu-id="4a207-656">`AuthenticationTokenSettings` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-656">Added the `AuthenticationTokenSettings` parameter.</span></span> <span data-ttu-id="4a207-657">このパラメーターを使用すると、タスクの実行時に認証トークンを提供するようバッチ サービスに要求でき、バッチ サービスに要求を出すためにバッチ アカウント キーをタスクに渡す必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="4a207-657">This parameter allows you to request the Batch service provide an authentication token to the task when it runs, avoiding the need to pass Batch account keys to the task in order to issue requests to the Batch service.</span></span>
    - <span data-ttu-id="4a207-658">`ContainerSettings` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-658">Added the `ContainerSettings` parameter.</span></span>
      - <span data-ttu-id="4a207-659">このパラメーターを使用すると、コンテナー内部でタスクを実行するよう Batch サービスに要求できます。</span><span class="sxs-lookup"><span data-stu-id="4a207-659">This parameter allows you to request the Batch service run the task inside a container.</span></span>
    - <span data-ttu-id="4a207-660">`OutputFiles` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-660">Added the `OutputFiles` parameter.</span></span>
      - <span data-ttu-id="4a207-661">このパラメーターを使用すると、タスクの終了後に Azure Storage にファイルをアップロードするようにタスクを構成できます。</span><span class="sxs-lookup"><span data-stu-id="4a207-661">This parameter allows you to configure the task to upload files to Azure Storage after it has finished.</span></span>
  * <span data-ttu-id="4a207-662">`New-AzureBatchPool` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-662">Updated parameters to `New-AzureBatchPool`.</span></span>
    - <span data-ttu-id="4a207-663">`UserAccounts` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-663">Added the `UserAccounts` parameter.</span></span>
      - <span data-ttu-id="4a207-664">このパラメーターは、プール内の各ノードで作成されたユーザー アカウントを定義します。</span><span class="sxs-lookup"><span data-stu-id="4a207-664">This parameter defines user accounts created on each node in the pool.</span></span>
    - <span data-ttu-id="4a207-665">`TargetLowPriorityComputeNodes` を追加し、`TargetDedicated` を `TargetDedicatedComputeNodes` に名前変更しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-665">Added `TargetLowPriorityComputeNodes` and renamed `TargetDedicated` to `TargetDedicatedComputeNodes`.</span></span>
      - <span data-ttu-id="4a207-666">`TargetDedicatedComputeNodes` パラメーター用に `TargetDedicated` の別名を作成しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-666">A `TargetDedicated` alias was created for the `TargetDedicatedComputeNodes` parameter.</span></span>
    - <span data-ttu-id="4a207-667">`NetworkConfiguration` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-667">Added the `NetworkConfiguration` parameter.</span></span>
      - <span data-ttu-id="4a207-668">このパラメーターを使用すると、プールのネットワーク設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="4a207-668">This parameter allows you to configure the pools network settings.</span></span>
  * <span data-ttu-id="4a207-669">`New-AzureBatchCertificate` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-669">Updated parameters to `New-AzureBatchCertificate`.</span></span>
    - <span data-ttu-id="4a207-670">`Password` パラメーターが `SecureString` になりました。</span><span class="sxs-lookup"><span data-stu-id="4a207-670">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="4a207-671">`New-AzureBatchComputeNodeUser` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-671">Updated parameters to `New-AzureBatchComputeNodeUser`.</span></span>
    - <span data-ttu-id="4a207-672">`Password` パラメーターが `SecureString` になりました。</span><span class="sxs-lookup"><span data-stu-id="4a207-672">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="4a207-673">`Set-AzureBatchComputeNodeUser` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-673">Updated parameters to `Set-AzureBatchComputeNodeUser`.</span></span>
    - <span data-ttu-id="4a207-674">`Password` パラメーターが `SecureString` になりました。</span><span class="sxs-lookup"><span data-stu-id="4a207-674">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="4a207-675">`Get-AzureBatchNodeFile`、`Get-AzureBatchNodeFileContent`、および `Remove-AzureBatchNodeFile` で、`Name` パラメーターを `Path` に名前変更しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-675">Renamed the `Name` parameter to `Path` on `Get-AzureBatchNodeFile`, `Get-AzureBatchNodeFileContent`, and `Remove-AzureBatchNodeFile`.</span></span>
    - <span data-ttu-id="4a207-676">`Path` パラメーター用に `Name` の別名を作成しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-676">A `Name` alias was created for the `Path` parameter.</span></span>
  * <span data-ttu-id="4a207-677">オブジェクトに対する変更</span><span class="sxs-lookup"><span data-stu-id="4a207-677">Changes to objects</span></span>
    - <span data-ttu-id="4a207-678">完全なリストについては、Batch 変更ログを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-678">Please see the Batch change log for the full list</span></span>
  * <span data-ttu-id="4a207-679">Azure Active Directory ベースの認証のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-679">Added support for Azure Active Directory based authentication.</span></span>
    - <span data-ttu-id="4a207-680">Azure Active Directory 認証を使用するには、`Get-AzureRmBatchAccount` コマンドレットを使用して `BatchAccountContext` オブジェクトを取得し、この `BatchAccountContext` を Batch サービス コマンドレットの `-BatchContext` パラメーターに指定します。</span><span class="sxs-lookup"><span data-stu-id="4a207-680">To use Azure Active Directory authentication, retrieve a `BatchAccountContext` object using the `Get-AzureRmBatchAccount` cmdlet, and supply this `BatchAccountContext` to the `-BatchContext` parameter of a Batch service cmdlet.</span></span> <span data-ttu-id="4a207-681">Azure Active Directory 認証は、`PoolAllocationMode = UserSubscription` のアカウントには必須です。</span><span class="sxs-lookup"><span data-stu-id="4a207-681">Azure Active Directory authentication is mandatory for accounts with `PoolAllocationMode = UserSubscription`.</span></span>
    - <span data-ttu-id="4a207-682">既存のアカウント、または `PoolAllocationMode = BatchService` で作成された新しいアカウントの場合、`Get-AzureRmBatchAccoutKeys` コマンドレットを使用して `BatchAccountContext` オブジェクトを取得することにより、共有キー認証の使用を継続できます。</span><span class="sxs-lookup"><span data-stu-id="4a207-682">For existing accounts or for new accounts created with `PoolAllocationMode = BatchService`, you may continue to use shared key authentication by retrieving a `BatchAccountContext` object using the `Get-AzureRmBatchAccoutKeys` cmdlet.</span></span>
* <span data-ttu-id="4a207-683">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="4a207-683">Compute</span></span>
  * <span data-ttu-id="4a207-684">Azure Disk Encryption 拡張コマンド</span><span class="sxs-lookup"><span data-stu-id="4a207-684">Azure Disk Encryption Extension Commands</span></span>
    - <span data-ttu-id="4a207-685">"Set-AzureRmVmDiskEncryptionExtension" の新しいパラメーター: "-EncryptFormatAll" はデータ ディスクを暗号化フォーマットします</span><span class="sxs-lookup"><span data-stu-id="4a207-685">New Parameter for 'Set-AzureRmVmDiskEncryptionExtension': '-EncryptFormatAll' encrypt formats data disks</span></span>
    - <span data-ttu-id="4a207-686">"Set-AzureRmVmDiskEncryptionExtension" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます</span><span class="sxs-lookup"><span data-stu-id="4a207-686">New Parameters for 'Set-AzureRmVmDiskEncryptionExtension': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
    - <span data-ttu-id="4a207-687">"Disable-AzureRmVmDiskEncryption" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます</span><span class="sxs-lookup"><span data-stu-id="4a207-687">New Parameters for 'Disable-AzureRmVmDiskEncryption': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
    - <span data-ttu-id="4a207-688">"Get-AzureRmVmDiskEncryptionStatus" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます</span><span class="sxs-lookup"><span data-stu-id="4a207-688">New Parameters for 'Get-AzureRmVmDiskEncryptionStatus': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
* <span data-ttu-id="4a207-689">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4a207-689">DataLakeAnalytics</span></span>
  * <span data-ttu-id="4a207-690">DataLakeAnalytics の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-690">Please see the migration guide for breaking changes made to DataLakeAnalytics this release</span></span>
  * <span data-ttu-id="4a207-691">Get-AzureRmDataLakeAnalyticsAccount の 2 つの OutputTypes の 1 つを変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-691">Changed one of the two OutputTypes of Get-AzureRmDataLakeAnalyticsAccount</span></span>
    - <span data-ttu-id="4a207-692">List\<DataLakeAnalyticsAccount> から List\<PSDataLakeAnalyticsAccountBasic></span><span class="sxs-lookup"><span data-stu-id="4a207-692">List\<DataLakeAnalyticsAccount> to List\<PSDataLakeAnalyticsAccountBasic></span></span>
    - <span data-ttu-id="4a207-693">PSDataLakeAnalyticsAccountBasic のプロパティは DataLakeAnalyticsAccount のプロパティの厳密なサブセットです</span><span class="sxs-lookup"><span data-stu-id="4a207-693">The properties of PSDataLakeAnalyticsAccountBasic is a strict subset of the properties of DataLakeAnalyticsAccount</span></span>
    - <span data-ttu-id="4a207-694">DataLakeAnalyticsAccount にある追加プロパティはサービスによって返されません。</span><span class="sxs-lookup"><span data-stu-id="4a207-694">The additional properties that are in DataLakeAnalyticsAccount are not returned by the service.</span></span>  <span data-ttu-id="4a207-695">そのため、この変更はこれを正確に反映するためのものです。</span><span class="sxs-lookup"><span data-stu-id="4a207-695">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="4a207-696">これらの追加プロパティは引き続き PSDataLakeAnalyticsAccountBasic にありますが、これらには廃止のタグが付けられます。</span><span class="sxs-lookup"><span data-stu-id="4a207-696">These additional properties are still in PSDataLakeAnalyticsAccountBasic, but they are tagged as Obsolete.</span></span>
  * <span data-ttu-id="4a207-697">Get-AzureRmDataLakeAnalyticsJob の 2 つの OutputTypes の 1 つを変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-697">Changed one of the two OutputTypes of Get-AzureRmDataLakeAnalyticsJob</span></span>
    - <span data-ttu-id="4a207-698">List\<JobInformation> から List\<PSJobInformationBasic></span><span class="sxs-lookup"><span data-stu-id="4a207-698">List\<JobInformation> to List\<PSJobInformationBasic></span></span>
    - <span data-ttu-id="4a207-699">PSJobInformationBasic のプロパティは JobInformation のプロパティの厳密なサブセットです</span><span class="sxs-lookup"><span data-stu-id="4a207-699">The properties of PSJobInformationBasic is a strict subset of the properties of JobInformation</span></span>
    - <span data-ttu-id="4a207-700">JobInformation にある追加プロパティはサービスによって返されません。</span><span class="sxs-lookup"><span data-stu-id="4a207-700">The additional properties that are in JobInformation are not returned by the service.</span></span>  <span data-ttu-id="4a207-701">そのため、この変更はこれを正確に反映するためのものです。</span><span class="sxs-lookup"><span data-stu-id="4a207-701">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="4a207-702">これらの追加プロパティは引き続き PSJobInformationBasic にありますが、これらには廃止のタグが付けられます。</span><span class="sxs-lookup"><span data-stu-id="4a207-702">These additional properties are still in PSJobInformationBasic, but they are tagged as Obsolete.</span></span>
* <span data-ttu-id="4a207-703">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4a207-703">DataLakeStore</span></span>
  * <span data-ttu-id="4a207-704">DataLakeStore の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-704">Please see the migration guide for breaking changes made to DataLakeStore this release</span></span>
  * <span data-ttu-id="4a207-705">Get-AzureRmDataLakeStoreAccount の 2 つの OutputTypes の 1 つを変更しました</span><span class="sxs-lookup"><span data-stu-id="4a207-705">Changed one of the two OutputTypes of Get-AzureRmDataLakeStoreAccount</span></span>
    - <span data-ttu-id="4a207-706">List\<PSDataLakeStoreAccount> から List\<PSDataLakeStoreAccountBasic></span><span class="sxs-lookup"><span data-stu-id="4a207-706">List\<PSDataLakeStoreAccount> to List\<PSDataLakeStoreAccountBasic></span></span>
    - <span data-ttu-id="4a207-707">PSDataLakeStoreAccountBasic のプロパティは PSDataLakeStoreAccount のプロパティの厳密なサブセットです</span><span class="sxs-lookup"><span data-stu-id="4a207-707">The properties of PSDataLakeStoreAccountBasic is a strict subset of the properties of PSDataLakeStoreAccount</span></span>
    - <span data-ttu-id="4a207-708">PSDataLakeStoreAccount にある追加プロパティはサービスによって返されません。</span><span class="sxs-lookup"><span data-stu-id="4a207-708">The additional properties that are in PSDataLakeStoreAccount are not returned by the service.</span></span>  <span data-ttu-id="4a207-709">そのため、この変更はこれを正確に反映するためのものです。</span><span class="sxs-lookup"><span data-stu-id="4a207-709">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="4a207-710">これらの追加プロパティは引き続き PSDataLakeStoreAccountBasic にありますが、これらには廃止のタグが付けられます。</span><span class="sxs-lookup"><span data-stu-id="4a207-710">These additional properties are still in PSDataLakeStoreAccountBasic, but they are tagged as Obsolete.</span></span>
* <span data-ttu-id="4a207-711">DNS</span><span class="sxs-lookup"><span data-stu-id="4a207-711">Dns</span></span>
  * <span data-ttu-id="4a207-712">Azure DNS での CAA レコードの種類のサポート</span><span class="sxs-lookup"><span data-stu-id="4a207-712">Support for CAA record types in Azure DNS</span></span>
    - <span data-ttu-id="4a207-713">CAA レコードの種類に対するすべての操作をサポートします</span><span class="sxs-lookup"><span data-stu-id="4a207-713">Supports all operations on CAA record type</span></span>
* <span data-ttu-id="4a207-714">EventHub</span><span class="sxs-lookup"><span data-stu-id="4a207-714">EventHub</span></span>
  * <span data-ttu-id="4a207-715">EventHub の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-715">Please see the migration guide for breaking changes made to EventHub this release</span></span>
* <span data-ttu-id="4a207-716">洞察</span><span class="sxs-lookup"><span data-stu-id="4a207-716">Insights</span></span>
  * <span data-ttu-id="4a207-717">Insights の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-717">Please see the migration guide for breaking changes made to Insights this release</span></span>
* <span data-ttu-id="4a207-718">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="4a207-718">Network</span></span>
  * <span data-ttu-id="4a207-719">Network の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-719">Please see the migration guide for breaking changes made to Network this release</span></span>
  * <span data-ttu-id="4a207-720">指定された Azure リージョンで使用可能なインターネット サービス プロバイダーを一覧表示するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-720">Added cmdlet to list available internet service providers for a specified Azure region</span></span>
    - <span data-ttu-id="4a207-721">Get-AzureRmNetworkWatcherReachabilityProvidersList</span><span class="sxs-lookup"><span data-stu-id="4a207-721">Get-AzureRmNetworkWatcherReachabilityProvidersList</span></span>
  * <span data-ttu-id="4a207-722">指定された場所から Azure リージョンまでのインターネット サービス プロバイダーの相対待機時間スコアを取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-722">Added cmdlet to get the relative latency score for internet service providers from a specified location to Azure regions</span></span>
    - <span data-ttu-id="4a207-723">Get-AzureRmNetworkWatcherReachabilityReport</span><span class="sxs-lookup"><span data-stu-id="4a207-723">Get-AzureRmNetworkWatcherReachabilityReport</span></span>
* <span data-ttu-id="4a207-724">プロファイル</span><span class="sxs-lookup"><span data-stu-id="4a207-724">Profile</span></span>
  - <span data-ttu-id="4a207-725">Set-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="4a207-725">Set-AzureRmDefault</span></span>
    - <span data-ttu-id="4a207-726">このコマンドレットを使用して、既定のリソース グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="4a207-726">Use this cmdlet to set a default resource group.</span></span>  <span data-ttu-id="4a207-727">これにより、-ResourceGroup パラメーターが一部のコマンドレットで省略可能になり、リソース グループを指定しない場合に既定値が使用されます</span><span class="sxs-lookup"><span data-stu-id="4a207-727">This will make the -ResourceGroup parameter optional for some cmdlets, and will use the default when a resource group is not specified</span></span>
    - ```Set-AzureRmDefault -ResourceGroupName "ExampleResourceGroup"```
    - <span data-ttu-id="4a207-728">指定したリソース グループがサブスクリプションに存在する場合は、このリソース グループが既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4a207-728">If resource group specified exists in the subscription, this resource group will be set to default.</span></span>  <span data-ttu-id="4a207-729">それ以外の場合、リソース グループが作成され、既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="4a207-729">Otherwise, the resource group will be created and then set to default.</span></span>
  - <span data-ttu-id="4a207-730">Get-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="4a207-730">Get-AzureRmDefault</span></span>
    - <span data-ttu-id="4a207-731">このコマンドレットを使用して、現在の既定のリソース グループ (および今後はその他の既定値) を取得します。</span><span class="sxs-lookup"><span data-stu-id="4a207-731">Use this cmdlet to get the current default resource group (and other defaults in the future).</span></span>
    - ```Get-AzureRmDefault -ResourceGroup```
  - <span data-ttu-id="4a207-732">Clear-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="4a207-732">Clear-AzureRmDefault</span></span>
    - <span data-ttu-id="4a207-733">このコマンドレットを使用して、現在の既定のリソース グループを削除します</span><span class="sxs-lookup"><span data-stu-id="4a207-733">Use this cmdlet to remove the current default resource group</span></span>
    - ```Clear-AzureRmDefault -ResourceGroup```
  - <span data-ttu-id="4a207-734">Add-AzureRmEnvironment および Set-AzureRmEnvironment</span><span class="sxs-lookup"><span data-stu-id="4a207-734">Add-AzureRmEnvironment and Set-AzureRmEnvironment</span></span>
    - <span data-ttu-id="4a207-735">BatchAudience パラメーターを追加します。これにより、Batch サービスの認証トークンを取得する際に使用する Azure Batch Active Directory オーディエンスを指定できます。</span><span class="sxs-lookup"><span data-stu-id="4a207-735">Add the BatchAudience parameter, which allows you to specify the Azure Batch Active Directory audience to use when acquiring authentication tokens for the Batch service.</span></span>
* <span data-ttu-id="4a207-736">RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="4a207-736">RecoveryServices.Backup</span></span>
  * <span data-ttu-id="4a207-737">インスタント ファイル回復を実行するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-737">Added cmdlets to perform instant file recovery.</span></span>
    - <span data-ttu-id="4a207-738">Get-AzureRmRecoveryServicesBackupRPMountScript</span><span class="sxs-lookup"><span data-stu-id="4a207-738">Get-AzureRmRecoveryServicesBackupRPMountScript</span></span>
    - <span data-ttu-id="4a207-739">Disable-AzureRmRecoveryServicesBackupRPMountScript</span><span class="sxs-lookup"><span data-stu-id="4a207-739">Disable-AzureRmRecoveryServicesBackupRPMountScript</span></span>
  * <span data-ttu-id="4a207-740">RecoveryServices.Backup SDK を最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="4a207-740">Updated RecoveryServices.Backup SDK version to the latest</span></span>
  * <span data-ttu-id="4a207-741">テスト実行に必要なすべての設定がテスト自体で行われるように、Azure VM ワークロードのテストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="4a207-741">Updated tests for the Azure VM workload so that, all setups needed for test runs are done by the tests themselves.</span></span>
  * <span data-ttu-id="4a207-742">https://github.com/Azure/azure-powershell/issues/3164 を修正しました</span><span class="sxs-lookup"><span data-stu-id="4a207-742">Fixes https://github.com/Azure/azure-powershell/issues/3164</span></span>
* <span data-ttu-id="4a207-743">RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="4a207-743">RecoveryServices.SiteRecovery</span></span>
  * <span data-ttu-id="4a207-744">Azure Site Recovery に対する ASR VMware の変更 (コマンドレットは現在、Enterprise から Enterprise、Enterprise から Azure、HyperV から Azure の操作をサポートしています)</span><span class="sxs-lookup"><span data-stu-id="4a207-744">Changes for ASR VMware to Azure Site Recovery (cmdlets are currently supporting operations for Enterprise to Enterprise, Enterprise to Azure, HyperV to Azure)</span></span>
    - <span data-ttu-id="4a207-745">New-AzureRmRecoveryServicesAsrPolicy</span><span class="sxs-lookup"><span data-stu-id="4a207-745">New-AzureRmRecoveryServicesAsrPolicy</span></span>
    - <span data-ttu-id="4a207-746">New-AzureRmRecoveryServicesAsrProtectedItem</span><span class="sxs-lookup"><span data-stu-id="4a207-746">New-AzureRmRecoveryServicesAsrProtectedItem</span></span>
    - <span data-ttu-id="4a207-747">Update-AzureRmRecoveryServicesAsrPolicy</span><span class="sxs-lookup"><span data-stu-id="4a207-747">Update-AzureRmRecoveryServicesAsrPolicy</span></span>
    - <span data-ttu-id="4a207-748">Update-AzureRmRecoveryServicesAsrProtectionDirection</span><span class="sxs-lookup"><span data-stu-id="4a207-748">Update-AzureRmRecoveryServicesAsrProtectionDirection</span></span>
  * <span data-ttu-id="4a207-749">AAD ベースのコンテナーにサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-749">Added support to AAD-based vault</span></span>
  * <span data-ttu-id="4a207-750">VCenter リソースを管理するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-750">Added cmdlets to manage VCenter resources</span></span>
    - <span data-ttu-id="4a207-751">Get-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="4a207-751">Get-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="4a207-752">New-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="4a207-752">New-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="4a207-753">Remove-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="4a207-753">Remove-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="4a207-754">Update-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="4a207-754">Update-AzureRmRecoveryServicesAsrVCenter</span></span>
  * <span data-ttu-id="4a207-755">その他のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="4a207-755">Added other cmdlets</span></span>
    - <span data-ttu-id="4a207-756">Get-AzureRmRecoveryServicesAsrAlertSetting</span><span class="sxs-lookup"><span data-stu-id="4a207-756">Get-AzureRmRecoveryServicesAsrAlertSetting</span></span>
    - <span data-ttu-id="4a207-757">Get-AzureRmRecoveryServicesAsrEvent</span><span class="sxs-lookup"><span data-stu-id="4a207-757">Get-AzureRmRecoveryServicesAsrEvent</span></span>
    - <span data-ttu-id="4a207-758">New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="4a207-758">New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
    - <span data-ttu-id="4a207-759">Set-AzureRmRecoveryServicesAsrAlertSetting</span><span class="sxs-lookup"><span data-stu-id="4a207-759">Set-AzureRmRecoveryServicesAsrAlertSetting</span></span>
    - <span data-ttu-id="4a207-760">Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob</span><span class="sxs-lookup"><span data-stu-id="4a207-760">Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob</span></span>
    - <span data-ttu-id="4a207-761">Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob</span><span class="sxs-lookup"><span data-stu-id="4a207-761">Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob</span></span>
    - <span data-ttu-id="4a207-762">Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob</span><span class="sxs-lookup"><span data-stu-id="4a207-762">Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob</span></span>
    - <span data-ttu-id="4a207-763">Update-AzureRmRecoveryServicesAsrMobilityService</span><span class="sxs-lookup"><span data-stu-id="4a207-763">Update-AzureRmRecoveryServicesAsrMobilityService</span></span>
* <span data-ttu-id="4a207-764">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="4a207-764">ServiceBus</span></span>
  - <span data-ttu-id="4a207-765">ServiceBus の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="4a207-765">Please see the migration guide for breaking changes made to ServiceBus this release</span></span>
* <span data-ttu-id="4a207-766">SQL</span><span class="sxs-lookup"><span data-stu-id="4a207-766">Sql</span></span>
  * <span data-ttu-id="4a207-767">データベースに対する非同期 updateslo 操作の一覧表示およびキャンセルのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-767">Adding support for list and cancel the asynchronous updateslo operation on the database</span></span>
    - <span data-ttu-id="4a207-768">DB updateslo 操作状態を返すように既存の Get-AzureRmSqlDatabaseActivity コマンドレットを更新。</span><span class="sxs-lookup"><span data-stu-id="4a207-768">update existing cmdlet Get-AzureRmSqlDatabaseActivity to return DB updateslo operation status.</span></span>
    - <span data-ttu-id="4a207-769">データベースに対する非同期 updateslo 操作をキャンセルする新しい Stop-AzureRmSqlDatabaseActivity コマンドレットを追加。</span><span class="sxs-lookup"><span data-stu-id="4a207-769">add new cmdlet Stop-AzureRmSqlDatabaseActivity for cancel the asynchronous updateslo operation on the database.</span></span>
  * <span data-ttu-id="4a207-770">データベースとエラスティック プールのゾーン冗長性に対するサポートを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-770">Adding support for Zone Redundancy for databases and elastic pools</span></span>
    - <span data-ttu-id="4a207-771">ZoneRedundant スイッチ パラメーターを New-AzureRmSqlDatabase に追加</span><span class="sxs-lookup"><span data-stu-id="4a207-771">Adding ZoneRedundant switch parameter to New-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="4a207-772">ZoneRedundant スイッチ パラメーターを Set-AzureRmSqlDatabase に追加</span><span class="sxs-lookup"><span data-stu-id="4a207-772">Adding ZoneRedundant switch parameter to Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="4a207-773">ZoneRedundant スイッチ パラメーターを New-AzureRmSqlElasticPool に追加</span><span class="sxs-lookup"><span data-stu-id="4a207-773">Adding ZoneRedundant switch parameter to New-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="4a207-774">ZoneRedundant スイッチ パラメーターを Set-AzureRmSqlElasticPool に追加</span><span class="sxs-lookup"><span data-stu-id="4a207-774">Adding ZoneRedundant switch parameter to Set-AzureRmSqlElasticPool</span></span>
  * <span data-ttu-id="4a207-775">サーバー DNS エイリアスに対するサポートを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-775">Adding support for Server DNS Aliases</span></span>
    - <span data-ttu-id="4a207-776">サーバーとエイリアス名ごとにサーバー DNS エイリアスを取得するか、Azure SQL Server のサーバー DNS エイリアスの一覧を取得する、Get-AzureRmSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-776">Adding Get-AzureRmSqlServerDnsAlias cmdlet which gets server dns aliases by server and alias name or a list of server dns aliases for an azure Sql Server.</span></span>
    - <span data-ttu-id="4a207-777">指定の Azure SQL Server の新しいサーバー DNS エイリアスを作成する、New-AzureRmSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-777">Adding New-AzureRmSqlServerDnsAlias cmdlet which creates new server dns alias for a given Azure Sql server</span></span>
    - <span data-ttu-id="4a207-778">サーバー DNS エイリアスが指す Azure SQL Server を更新できる、Set-AzurermSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-778">Adding Set-AzurermSqlServerDnsAlias cmlet which allows updating a Azure Sql Server to which server dns alias is pointing</span></span>
    - <span data-ttu-id="4a207-779">Azure SQL Server のサーバー DNS エイリアスを削除する、Remove-AzureRmSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="4a207-779">Adding Remove-AzureRmSqlServerDnsAlias cmdlet which removes a server dns alias for a Azure Sql Server</span></span>
* <span data-ttu-id="4a207-780">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="4a207-780">Azure.Storage</span></span>
  * <span data-ttu-id="4a207-781">Azure Storage Client Library 8.5.0 および Azure Storage DataMovement Library 0.6.3 へのアップグレード</span><span class="sxs-lookup"><span data-stu-id="4a207-781">Upgrade to Azure Storage Client Library 8.5.0 and Azure Storage DataMovement Library 0.6.3</span></span>
  * <span data-ttu-id="4a207-782">ファイル共有スナップショット サポート機能を追加</span><span class="sxs-lookup"><span data-stu-id="4a207-782">Add File Share Snapshot Support Feature</span></span>
    - <span data-ttu-id="4a207-783">"SnapshotTime" パラメーターを Get-AzureStorageShare に追加</span><span class="sxs-lookup"><span data-stu-id="4a207-783">Add 'SnapshotTime' parameter to Get-AzureStorageShare</span></span>
    - <span data-ttu-id="4a207-784">"IncludeAllSnapshot" パラメーターを Remove-AzureStorageShare に追加</span><span class="sxs-lookup"><span data-stu-id="4a207-784">Add 'IncludeAllSnapshot' parameter to Remove-AzureStorageShare</span></span>
