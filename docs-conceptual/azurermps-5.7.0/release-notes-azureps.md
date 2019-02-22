---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 2/20/2018
ms.openlocfilehash: 1a9d38cd60ba596c085e5ee9f8d815e238362b1f
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153844"
---
# <a name="release-notes"></a><span data-ttu-id="8e20c-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="8e20c-103">Release notes</span></span>

<span data-ttu-id="8e20c-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="8e20c-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---

# <a name="azure-powershell-570"></a><span data-ttu-id="8e20c-105">Azure PowerShell 5.7.0</span><span class="sxs-lookup"><span data-stu-id="8e20c-105">Azure PowerShell 5.7.0</span></span>

<span data-ttu-id="8e20c-106">Azure PowerShell 5.7.0 インストーラー: [リンク](https://github.com/Azure/azure-powershell/releases/download/v5.7.0-April2018/azure-powershell.5.7.0.msi)</span><span class="sxs-lookup"><span data-stu-id="8e20c-106">Azure PowerShell 5.7.0 Installer: [link](https://github.com/Azure/azure-powershell/releases/download/v5.7.0-April2018/azure-powershell.5.7.0.msi)</span></span>

<span data-ttu-id="8e20c-107">ARM コマンドレット用のギャラリー モジュール: [リンク](https://www.powershellgallery.com/packages/AzureRM/5.7.0)</span><span class="sxs-lookup"><span data-stu-id="8e20c-107">Gallery Module for ARM Cmdlets: [link](https://www.powershellgallery.com/packages/AzureRM/5.7.0)</span></span>

<span data-ttu-id="8e20c-108">PowerShell ギャラリーから `AzureRM` をインストールするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-108">To install `AzureRM` from the PowerShell Gallery, run the following command:</span></span>

```powershell-interactive
Install-Module -Name AzureRM -Repository PSGallery -Force
```

<span data-ttu-id="8e20c-109">以前のバージョンの `AzureRM` から更新するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-109">To update from an older version of `AzureRM`, run the following command:</span></span>

```powershell-interactive
Update-Module -Name AzureRM
```

## <a name="changes-since-last-release"></a><span data-ttu-id="8e20c-110">前回のリリース以降の変更点</span><span class="sxs-lookup"><span data-stu-id="8e20c-110">Changes Since Last Release</span></span>

#### <a name="general"></a><span data-ttu-id="8e20c-111">全般</span><span class="sxs-lookup"><span data-stu-id="8e20c-111">General</span></span>
* <span data-ttu-id="8e20c-112">Azure ClientRuntime の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-112">Updated to the latest version of the Azure ClientRuntime</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="8e20c-113">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-113">Azure.Storage</span></span>
* <span data-ttu-id="8e20c-114">FIPS ポリシーが有効になっているコンピューターで BLOB のアップロード コマンドレットとファイルのアップロード コマンドレットが失敗するという問題を修正</span><span class="sxs-lookup"><span data-stu-id="8e20c-114">Fix the issue that upload Blob and upload File cmdlets fail on FIPS policy enabled machines</span></span>
    - <span data-ttu-id="8e20c-115">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8e20c-115">Set-AzureStorageBlobContent</span></span>
    - <span data-ttu-id="8e20c-116">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8e20c-116">Set-AzureStorageFileContent</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="8e20c-117">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="8e20c-117">AzureRM.Billing</span></span>
* <span data-ttu-id="8e20c-118">新しいコマンドレット Get-AzureRmEnrollmentAccount</span><span class="sxs-lookup"><span data-stu-id="8e20c-118">New Cmdlet Get-AzureRmEnrollmentAccount</span></span>
  - <span data-ttu-id="8e20c-119">登録アカウントを取得するためのコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8e20c-119">cmdlet to retrieve enrollment accounts</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="8e20c-120">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-120">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="8e20c-121">Cognitive Services Management SDK バージョン 4.0.0 との統合。</span><span class="sxs-lookup"><span data-stu-id="8e20c-121">Integrate with Cognitive Services Management SDK version 4.0.0.</span></span>
* <span data-ttu-id="8e20c-122">Get-AzureRmCognitiveServicesAccountUsage 操作の追加。</span><span class="sxs-lookup"><span data-stu-id="8e20c-122">Add Get-AzureRmCognitiveServicesAccountUsage operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="8e20c-123">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-123">AzureRM.Compute</span></span>
* <span data-ttu-id="8e20c-124">`Get-AzureRmVmssDiskEncryptionStatus` によるデータ ディスク レベルでの暗号化状態のサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-124">`Get-AzureRmVmssDiskEncryptionStatus` supports encryption status at data disk level</span></span>
* <span data-ttu-id="8e20c-125">`Get-AzureRmVmssVmDiskEncryptionStatus` によるデータ ディスク レベルでの暗号化状態のサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-125">`Get-AzureRmVmssVmDiskEncryptionStatus` supports encryption status at data disk level</span></span>
* <span data-ttu-id="8e20c-126">ゾーン回復性の更新</span><span class="sxs-lookup"><span data-stu-id="8e20c-126">Update for Zone Resilient</span></span>
* <span data-ttu-id="8e20c-127">"New-AzureRmVm" および "New-AzureRmVmss" (シンプルなパラメーター セット) による可用性ゾーンのサポート。</span><span class="sxs-lookup"><span data-stu-id="8e20c-127">'New-AzureRmVm' and 'New-AzureRmVmss' (simple parameter set) support availability zones.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="8e20c-128">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8e20c-128">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="8e20c-129">Commands.Resources.Rest および ARM/Storage SDK への依存の分離。</span><span class="sxs-lookup"><span data-stu-id="8e20c-129">Decouple reliance on Commands.Resources.Rest and ARM/Storage SDKs.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="8e20c-130">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8e20c-130">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="8e20c-131">デバッグ機能の追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-131">Add debug functionality</span></span>
* <span data-ttu-id="8e20c-132">ADLS データプレーン SDK のバージョンを 1.1.2 に更新</span><span class="sxs-lookup"><span data-stu-id="8e20c-132">Update the version of the ADLS dataplane SDK to 1.1.2</span></span>
* <span data-ttu-id="8e20c-133">Export-AzureRmDataLakeStoreItem - パラメーター PerFileThreadCount、ConcurrentFileCount が非推奨になり、パラメーター Concurrency が導入されました</span><span class="sxs-lookup"><span data-stu-id="8e20c-133">Export-AzureRmDataLakeStoreItem - Deprecated parameters PerFileThreadCount, ConcurrentFileCount and introduced parameter Concurrency</span></span>
* <span data-ttu-id="8e20c-134">Import-AzureRMDataLakeStoreItem - パラメーター PerFileThreadCount、ConcurrentFileCount が非推奨になり、パラメーター Concurrency が導入されました</span><span class="sxs-lookup"><span data-stu-id="8e20c-134">Import-AzureRMDataLakeStoreItem - Deprecated parametersPerFileThreadCount, ConcurrentFileCount and introduced parameter Concurrency</span></span>
* <span data-ttu-id="8e20c-135">Get-AzureRMDataLakeStoreItemContent - 4 MB を超えるコンテンツのテール動作を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-135">Get-AzureRMDataLakeStoreItemContent - Fixed the tail behavior for contents greater than 4MB</span></span>
* <span data-ttu-id="8e20c-136">Set-AzureRMDataLakeStoreItemExpiry - 相対的な有効期限を設定するための新しいパラメーター セット SetRelativeExpiry を導入しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-136">Set-AzureRMDataLakeStoreItemExpiry - Introduced new parameter set SetRelativeExpiry for setting relative expiration time</span></span>
* <span data-ttu-id="8e20c-137">Remove-AzureRmDataLakeStoreItem - パラメーター Clean が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-137">Remove-AzureRmDataLakeStoreItem - Deprecated parameter Clean.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="8e20c-138">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="8e20c-138">AzureRM.EventHub</span></span>
* <span data-ttu-id="8e20c-139">New-AzureRmEventHubGeoDRConfiguration の AlternameName を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-139">Fixed AlternameName in New-AzureRmEventHubGeoDRConfiguration</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="8e20c-140">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8e20c-140">AzureRM.KeyVault</span></span>
* <span data-ttu-id="8e20c-141">コマンドレットを更新して、パイプ処理シナリオを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-141">Updated cmdlets to include piping scenarios</span></span>
* <span data-ttu-id="8e20c-142">今後の重大な変更リリースを対象とした非推奨メッセージの追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-142">Add deprecation messages for upcoming breaking change release</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="8e20c-143">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8e20c-143">AzureRM.Network</span></span>
* <span data-ttu-id="8e20c-144">Network コマンドレットでのエラー メッセージの修正</span><span class="sxs-lookup"><span data-stu-id="8e20c-144">Fix error message with Network cmdlets</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="8e20c-145">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8e20c-145">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="8e20c-146">customproperties をサポートするように Rules の CorrelationFilter に "properties" を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-146">Added 'properties' in CorrelationFilter of Rules to support customproperties</span></span>
* <span data-ttu-id="8e20c-147">New-AzureRmServiceBusGeoDRConfiguration ヘルプを更新し、Rules コマンドレットの出力を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-147">updated New-AzureRmServiceBusGeoDRConfiguration help and fixed Rules cmdlet output</span></span>
* <span data-ttu-id="8e20c-148">New-AzureRmServiceBusQueue および New-AzureRmServiceBusSubscription コマンドレットの auto-forward プロパティを修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-148">Fixed auto-forward properties in New-AzureRmServiceBusQueue and New-AzureRmServiceBusSubscription cmdlet</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="8e20c-149">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="8e20c-149">AzureRM.Sql</span></span>
* <span data-ttu-id="8e20c-150">エラスティック プールで非同期操作のキャンセルをサポートする新しいコマンドレット "Stop-AzureRmSqlElasticPoolActivity" の追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-150">Add new cmdlet 'Stop-AzureRmSqlElasticPoolActivity' to support canceling the asynchronous operations on elastic pool</span></span>
* <span data-ttu-id="8e20c-151">コマンドレット Get-AzureRmSqlDatabaseActivity および Get-AzureRmSqlElasticPoolActivity の応答を詳細情報が反映されるように更新</span><span class="sxs-lookup"><span data-stu-id="8e20c-151">Update the response for cmdlets Get-AzureRmSqlDatabaseActivity and Get-AzureRmSqlElasticPoolActivity to reflect more information in the response</span></span>

<span data-ttu-id="8e20c-152">前回のリリース以降の変更点: https://github.com/Azure/azure-powershell/compare/v5.6.0-March2018...v5.7.0-April2018</span><span class="sxs-lookup"><span data-stu-id="8e20c-152">Changes since last release: https://github.com/Azure/azure-powershell/compare/v5.6.0-March2018...v5.7.0-April2018</span></span>

## <a name="560---march-2018"></a><span data-ttu-id="8e20c-153">5.6.0 - 2018 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8e20c-153">5.6.0 - March 2018</span></span>

#### <a name="general"></a><span data-ttu-id="8e20c-154">全般</span><span class="sxs-lookup"><span data-stu-id="8e20c-154">General</span></span>
* <span data-ttu-id="8e20c-155">Cloud Shell の既定のリソース グループに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-155">Fix issue with Default Resource Group in CloudShell</span></span>
* <span data-ttu-id="8e20c-156">モジュールのインポート中に不適切なスタートアップ スクリプトが実行される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-156">Fix issue where incorrect startup scripts were being executed during module import</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="8e20c-157">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="8e20c-157">AzureRM.Profile</span></span>
* <span data-ttu-id="8e20c-158">サポートされていないシナリオで MSI 認証を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8e20c-158">Enable MSI authentication in unsupported scenarios</span></span>
* <span data-ttu-id="8e20c-159">ユーザー定義の管理対象サービス ID に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-159">Add support for user-defined Managed Service Identity</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="8e20c-160">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-160">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="8e20c-161">ビルドにおけるスクリプトのクリーンアップに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-161">Fixed issue with cleaning up scripts in build</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="8e20c-162">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="8e20c-162">AzureRM.Cdn</span></span>
* <span data-ttu-id="8e20c-163">ビルドにおけるスクリプトのクリーンアップに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-163">Fixed issue with cleaning up scripts in build</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="8e20c-164">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-164">AzureRM.Compute</span></span>
* <span data-ttu-id="8e20c-165">'New-AzureRmVM' と 'New-AzureRmVMSS' は、データ ディスクをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8e20c-165">'New-AzureRmVM' and 'New-AzureRmVMSS' support data disks.</span></span>
* <span data-ttu-id="8e20c-166">'New-AzureRmVM' と 'New-AzureRmVMSS' は、名前または ID でカスタム イメージをサポートします。</span><span class="sxs-lookup"><span data-stu-id="8e20c-166">'New-AzureRmVM' and 'New-AzureRmVMSS' support custom image by name or by id.</span></span>
* <span data-ttu-id="8e20c-167">ログ分析機能</span><span class="sxs-lookup"><span data-stu-id="8e20c-167">Log analytic feature</span></span>
    - <span data-ttu-id="8e20c-168">'Export-AzureRmLogAnalyticRequestRateByInterval' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-168">Added 'Export-AzureRmLogAnalyticRequestRateByInterval' cmdlet</span></span>
    - <span data-ttu-id="8e20c-169">'Export-AzureRmLogAnalyticThrottledRequests' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-169">Added 'Export-AzureRmLogAnalyticThrottledRequests' cmdlet</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="8e20c-170">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8e20c-170">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="8e20c-171">コンテナー レジストリおよび Azure File ボリューム マウントのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-171">Fix parameter sets issue for container registry and azure file volume mount</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="8e20c-172">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8e20c-172">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="8e20c-173">次の変更を含むように ADF .Net SDK バージョン 0.6.0-preview を更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-173">Updated the ADF .Net SDK to version 0.6.0-preview containing the following changes:</span></span>
    - <span data-ttu-id="8e20c-174">新しい AzureDatabricksLinkedService および DatabricksNotebookActivity を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-174">Added new AzureDatabricks LinkedService and DatabricksNotebook Activity</span></span>
    - <span data-ttu-id="8e20c-175">HDInsightOnDemand LinkedService に headNodeSize プロパティと dataNodeSize プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-175">Added headNodeSize and dataNodeSize properties in HDInsightOnDemand LinkedService</span></span>
    - <span data-ttu-id="8e20c-176">SalesforceMarketingCloud の LinkedService、Dataset、CopySource を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-176">Added LinkedService, Dataset, CopySource for SalesforceMarketingCloud</span></span>
    - <span data-ttu-id="8e20c-177">すべてのアクティビティで SecureOutput のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-177">Added support for SecureOutput on all activities</span></span>
    - <span data-ttu-id="8e20c-178">実行する同時実行アクティビティの数を制御する新しい BatchCount プロパティを ForEach アクティビティに追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-178">Added new BatchCount property on ForEach activity which control how many concurrent activities to run</span></span>
    - <span data-ttu-id="8e20c-179">新しいフィルター アクティビティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-179">Added new Filter Activity</span></span>
    - <span data-ttu-id="8e20c-180">リンクされたサービス パラメーターに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-180">Added Linked Service Parameters support</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="8e20c-181">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="8e20c-181">AzureRM.Dns</span></span>
* <span data-ttu-id="8e20c-182">プライベート DNS ゾーンのサポート (パブリック プレビュー)</span><span class="sxs-lookup"><span data-stu-id="8e20c-182">Support for Private DNS Zones (Public Preview)</span></span>
    - <span data-ttu-id="8e20c-183">関連付けられた仮想ネットワークのみに表示される DNS ゾーンを作成する機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-183">Adds ability to create DNS zones that are visible only to the associated virtual networks</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="8e20c-184">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8e20c-184">AzureRM.Network</span></span>
* <span data-ttu-id="8e20c-185">DNS のコマンドレットとの互換性のためにモデルの種類を更新しています。</span><span class="sxs-lookup"><span data-stu-id="8e20c-185">Updating model types for compatibility with DNS cmdlets.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="8e20c-186">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-186">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8e20c-187">Azure Site Recovery に対する ASR Azure の変更 (コマンドレットは現在、Enterprise から Enterprise、Enterprise から Azure、HyperV から Azure、VMware から Azure の操作をサポートしています)</span><span class="sxs-lookup"><span data-stu-id="8e20c-187">Changes for ASR Azure to Azure Site Recovery (cmdlets are currently supporting operations for Enterprise to Enterprise, Enterprise to Azure, HyperV to Azure,VMware to Azure)</span></span>
    - <span data-ttu-id="8e20c-188">New-AzureRmRecoveryServicesAsrProtectionContainer</span><span class="sxs-lookup"><span data-stu-id="8e20c-188">New-AzureRmRecoveryServicesAsrProtectionContainer</span></span>
    - <span data-ttu-id="8e20c-189">New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig</span><span class="sxs-lookup"><span data-stu-id="8e20c-189">New-AzureRmRecoveryServicesAsrAzureToAzureDiskReplicationConfig</span></span>
    - <span data-ttu-id="8e20c-190">Remove-AzureRmRecoveryServicesAsrProtectionContainer</span><span class="sxs-lookup"><span data-stu-id="8e20c-190">Remove-AzureRmRecoveryServicesAsrProtectionContainer</span></span>
    - <span data-ttu-id="8e20c-191">Update-AzureRmRecoveryServicesAsrProtectionDirection</span><span class="sxs-lookup"><span data-stu-id="8e20c-191">Update-AzureRmRecoveryServicesAsrProtectionDirection</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="8e20c-192">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-192">AzureRM.Storage</span></span>
* <span data-ttu-id="8e20c-193">ストレージ アカウントの新規と設定の各コマンドレットについて、次のパラメーターを廃止しました。EnableEncryptionService および DisableEncryptionService (保存時の暗号化は既定で有効であり、無効にできないため)</span><span class="sxs-lookup"><span data-stu-id="8e20c-193">Obsolete following parameters in new and set Storage Account cmdlets: EnableEncryptionService and DisableEncryptionService, since Encryption at Rest is enabled by default and can't be disabled.</span></span>
    - <span data-ttu-id="8e20c-194">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8e20c-194">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="8e20c-195">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8e20c-195">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="8e20c-196">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="8e20c-196">AzureRM.Websites</span></span>
* <span data-ttu-id="8e20c-197">Remove-AzureRmWebAppSlot のヘルプを修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-197">Fixed the help for Remove-AzureRmWebAppSlot</span></span>

## <a name="550---march-2018"></a><span data-ttu-id="8e20c-198">5.5.0 - 2018 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8e20c-198">5.5.0 - March 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="8e20c-199">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="8e20c-199">AzureRM.Profile</span></span>
* <span data-ttu-id="8e20c-200">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-200">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="8e20c-201">Newtonsoft.Json のバージョン 10.0.3 をバージョン 6.0.8 と共に読み込んでください</span><span class="sxs-lookup"><span data-stu-id="8e20c-201">Load version 10.0.3 of Newtonsoft.Json side-by-side with version 6.0.8</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="8e20c-202">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-202">Azure.Storage</span></span>
* <span data-ttu-id="8e20c-203">論理的な削除機能のサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-203">Support Soft-Delete feature</span></span>
    - <span data-ttu-id="8e20c-204">Enable-AzureStorageDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8e20c-204">Enable-AzureStorageDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8e20c-205">Disable-AzureStorageDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8e20c-205">Disable-AzureStorageDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8e20c-206">Get-AzureStorageBlob</span><span class="sxs-lookup"><span data-stu-id="8e20c-206">Get-AzureStorageBlob</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="8e20c-207">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-207">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="8e20c-208">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-208">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="8e20c-209">ファイアウォールおよびクエリのスケールアウト機能のサポートに加え 2017-08-01 api バージョンのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-209">Add support of firewall and query scaleout feature, as well as support of 2017-08-01 api version.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="8e20c-210">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="8e20c-210">AzureRM.Automation</span></span>
* <span data-ttu-id="8e20c-211">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-211">Fixed issue with importing aliases</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="8e20c-212">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="8e20c-212">AzureRM.Cdn</span></span>
* <span data-ttu-id="8e20c-213">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-213">Fixed issue with importing aliases</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="8e20c-214">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-214">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="8e20c-215">notice.txt と通知メッセージを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-215">Update notice.txt and notice message.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="8e20c-216">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-216">AzureRM.Compute</span></span>
* <span data-ttu-id="8e20c-217">"New-AzureRmVMSS" では、詳細モードで接続文字列が出力されます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-217">'New-AzureRmVMSS' prints connection strings in verbose mode.</span></span>
* <span data-ttu-id="8e20c-218">"New-AzureRmVmss" では、パブリック IP アドレス、負荷分散規則、および受信 NAT 規則がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-218">'New-AzureRmVmss' supports public IP address, load balancing rules, inbound NAT rules.</span></span>
* <span data-ttu-id="8e20c-219">WriteAccelerator 機能</span><span class="sxs-lookup"><span data-stu-id="8e20c-219">WriteAccelerator feature</span></span>
    - <span data-ttu-id="8e20c-220">WriteAccelerator スイッチ パラメーターを次のコマンドレットを追加しました: Set-AzureRmVMOSDisk、Set-AzureRmVMDataDisk、Add-AzureRmVMDataDisk、Add-AzureRmVmssDataDisk</span><span class="sxs-lookup"><span data-stu-id="8e20c-220">Added WriteAccelerator switch parameter to the following cmdlets: Set-AzureRmVMOSDisk Set-AzureRmVMDataDisk Add-AzureRmVMDataDisk Add-AzureRmVmssDataDisk</span></span>
    - <span data-ttu-id="8e20c-221">OsDiskWriteAccelerator スイッチ パラメーターを次のコマンドレットを追加しました:    Set-AzureRmVmssStorageProfile。</span><span class="sxs-lookup"><span data-stu-id="8e20c-221">Added OsDiskWriteAccelerator switch parameter to the following cmdlet:     Set-AzureRmVmssStorageProfile.</span></span>
    - <span data-ttu-id="8e20c-222">OsDiskWriteAccelerator ブール値パラメーターを次のコマンドレットを追加しました:    Update-AzureRmVM     Update-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="8e20c-222">Added OsDiskWriteAccelerator Boolean parameter to the following cmdlets:     Update-AzureRmVM     Update-AzureRmVmss</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="8e20c-223">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="8e20c-223">AzureRM.DataFactories</span></span>
* <span data-ttu-id="8e20c-224">一部の暗号化操作で無意味なエラーの原因になっていた、資格情報暗号化に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-224">Fix credential encryption issue that caused no meaningful error for some encryption operations</span></span>
* <span data-ttu-id="8e20c-225">データ ファクトリ全体で統合ランタイムを共有できるようにしました</span><span class="sxs-lookup"><span data-stu-id="8e20c-225">Enable integration runtime to be shared across data factory</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="8e20c-226">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8e20c-226">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="8e20c-227">カスタム セットアップおよびエディション選択機能を有効にする、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "SetupScriptContainerSasUri" と "Edition" を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-227">Add parameter "SetupScriptContainerSasUri" and "Edition" for "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd to enable custom setup and edition selection functionality</span></span>
* <span data-ttu-id="8e20c-228">一部の暗号化操作で重要性の低いエラーの原因になっていた、資格情報の暗号化に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-228">Fix credential encryption issue that caused no meaningful error for some encryption operations.</span></span>
* <span data-ttu-id="8e20c-229">データ ファクトリ全体で統合ランタイムを共有できるようにしました</span><span class="sxs-lookup"><span data-stu-id="8e20c-229">Enable integration runtime to be shared across data factory</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="8e20c-230">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8e20c-230">AzureRM.HDInsight</span></span>
* <span data-ttu-id="8e20c-231">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-231">Fixed issue with importing aliases</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="8e20c-232">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8e20c-232">AzureRM.KeyVault</span></span>
* <span data-ttu-id="8e20c-233">Set-AzureRmKeyVaultAccessPolicy の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-233">Fixed example for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="8e20c-234">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8e20c-234">AzureRM.Network</span></span>
* <span data-ttu-id="8e20c-235">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-235">Fixed issue with importing aliases</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="8e20c-236">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-236">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="8e20c-237">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-237">Fixed issue with importing aliases</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="8e20c-238">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-238">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="8e20c-239">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-239">Fixed issue with importing aliases</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="8e20c-240">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-240">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8e20c-241">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-241">Fixed issue with importing aliases</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="8e20c-242">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="8e20c-242">AzureRM.Resources</span></span>
* <span data-ttu-id="8e20c-243">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-243">Fixed issue with importing aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="8e20c-244">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8e20c-244">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="8e20c-245">キューに EnableBatchedOperations プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-245">Added EnableBatchedOperations property to Queue</span></span>
* <span data-ttu-id="8e20c-246">サブスクリプションに DeadLetteringOnFilterEvaluationExceptions プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-246">Added DeadLetteringOnFilterEvaluationExceptions property to Subscriptions</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="8e20c-247">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8e20c-247">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="8e20c-248">Service Fabric コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-248">Service Fabric cmdlet refresh</span></span>
  - <span data-ttu-id="8e20c-249">ARM テンプレートを更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-249">Updated ARM templates</span></span>
  - <span data-ttu-id="8e20c-250">失敗した操作がロールバックされなくなりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-250">Failed operations no longer rollback</span></span>
  - <span data-ttu-id="8e20c-251">Add-AzureRmServiceFabricNodeType</span><span class="sxs-lookup"><span data-stu-id="8e20c-251">Add-AzureRmServiceFabricNodeType</span></span>
    - <span data-ttu-id="8e20c-252">VM は既定でマネージド ディスクとなります</span><span class="sxs-lookup"><span data-stu-id="8e20c-252">VMs default to managed disks</span></span>
    - <span data-ttu-id="8e20c-253">既存の VMSS サブネットが使用されます</span><span class="sxs-lookup"><span data-stu-id="8e20c-253">Existing VMSS subnet used</span></span>
    - <span data-ttu-id="8e20c-254">すべての操作はべき等です</span><span class="sxs-lookup"><span data-stu-id="8e20c-254">All operations are idempotent</span></span>
  - <span data-ttu-id="8e20c-255">Remove-AzureRmServiceFabricNodeType により、部分的に作成された VMSS およびクラスター ノードの種類がクリーンアップされます</span><span class="sxs-lookup"><span data-stu-id="8e20c-255">Remove-AzureRmServiceFabricNodeType cleans up partially created VMSS and/or cluster node types</span></span>
  - <span data-ttu-id="8e20c-256">複雑なプロパティ型について PSCluster オブジェクトの出力を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-256">Fixed output of PSCluster object for complex property types</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="8e20c-257">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="8e20c-257">AzureRM.Sql</span></span>
* <span data-ttu-id="8e20c-258">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-258">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="8e20c-259">Get-AzureRmSqlServer、New-AzureRmSqlServer、および Remove-AzureRmSqlServer の応答に FullyQualifiedDomainName プロパティが含まれるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-259">Get-AzureRmSqlServer, New-AzureRmSqlServer, and Remove-AzureRmSqlServer response now includes FullyQualifiedDomainName property.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="8e20c-260">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="8e20c-260">AzureRM.Websites</span></span>
* <span data-ttu-id="8e20c-261">別名のインポートに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-261">Fixed issue with importing aliases</span></span>
* <span data-ttu-id="8e20c-262">New-AzureRMWebApp - WebApp を簡単に作成できるようにするパラメーター セットを追加しました (ローカルの Git リポジトリをサポート)。</span><span class="sxs-lookup"><span data-stu-id="8e20c-262">New-AzureRMWebApp - added parameter set for simplified WebApp creation, with local git repository support.</span></span>

## <a name="540---february-2018"></a><span data-ttu-id="8e20c-263">5.4.0 - 2018 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8e20c-263">5.4.0 - February 2018</span></span>
#### <a name="azurermautomation"></a><span data-ttu-id="8e20c-264">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="8e20c-264">AzureRM.Automation</span></span>
* <span data-ttu-id="8e20c-265">New-AzureRmAutomationModule の別名を Import-AzureRmAutomationModule に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-265">Added alias from New-AzureRmAutomationModule to Import-AzureRmAutomationModule</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="8e20c-266">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-266">AzureRM.Compute</span></span>
* <span data-ttu-id="8e20c-267">一部の Get コマンドレットの ErrorAction に関する問題を解決しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-267">Fix ErrorAction issue for some of Get cmdlets.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="8e20c-268">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8e20c-268">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="8e20c-269">Azure コンテナー インスタンス SDK 2018-02-01 を適用しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-269">Apply Azure Container Instance SDK 2018-02-01</span></span>
    - <span data-ttu-id="8e20c-270">DNS 名ラベルのサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-270">Support DNS name label</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="8e20c-271">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="8e20c-271">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="8e20c-272">以前動作しなかった GET コマンドレットをすべて修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-272">Fixed all of the GET cmdlets which previously weren't working.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="8e20c-273">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="8e20c-273">AzureRM.EventHub</span></span>
* <span data-ttu-id="8e20c-274">Get-AzureRmEventHubGeoDRConfiguration ヘルプのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-274">Fix bug in Get-AzureRmEventHubGeoDRConfiguration help</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="8e20c-275">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8e20c-275">AzureRM.Network</span></span>
* <span data-ttu-id="8e20c-276">新しい接続モニターを作成するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-276">Added cmdlet to create a new connection monitor</span></span>
    - <span data-ttu-id="8e20c-277">New-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="8e20c-277">New-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="8e20c-278">接続モニターを更新するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-278">Added cmdlet to update a connection monitor</span></span>
    - <span data-ttu-id="8e20c-279">Set-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="8e20c-279">Set-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="8e20c-280">接続モニターまたは接続モニターのリストを取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-280">Added cmdlet to get connection monitor or connection monitor list</span></span>
    - <span data-ttu-id="8e20c-281">Get-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="8e20c-281">Get-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="8e20c-282">接続モニターにクエリを実行するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-282">Added cmdlet to query connection monitor</span></span>
    - <span data-ttu-id="8e20c-283">Get-AzureRmNetworkWatcherConnectionMonitorReport</span><span class="sxs-lookup"><span data-stu-id="8e20c-283">Get-AzureRmNetworkWatcherConnectionMonitorReport</span></span>
* <span data-ttu-id="8e20c-284">接続モニターを起動するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-284">Added cmdlet to start connection monitor</span></span>
    - <span data-ttu-id="8e20c-285">Start-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="8e20c-285">Start-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="8e20c-286">接続モニターを停止するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-286">Added cmdlet to stop connection monitor</span></span>
    - <span data-ttu-id="8e20c-287">Stop-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="8e20c-287">Stop-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="8e20c-288">接続モニターを削除するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-288">Added cmdlet to remove connection monitor</span></span>
    - <span data-ttu-id="8e20c-289">Remove-AzureRmNetworkWatcherConnectionMonitor</span><span class="sxs-lookup"><span data-stu-id="8e20c-289">Remove-AzureRmNetworkWatcherConnectionMonitor</span></span>
* <span data-ttu-id="8e20c-290">Set-AzureRmApplicationGatewayBackendAddressPool のドキュメントを更新して非推奨の例を削除しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-290">Updated Set-AzureRmApplicationGatewayBackendAddressPool documentation to remove deprecated example</span></span>
* <span data-ttu-id="8e20c-291">EnableHttp2 フラグを Application Gateway に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-291">Added EnableHttp2 flag to Application Gateway</span></span>
    - <span data-ttu-id="8e20c-292">New-AzureRmApplicationGateway の更新: 省略可能なパラメーター -EnableHttp2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-292">Updated New-AzureRmApplicationGateway: Added optional parameter -EnableHttp2</span></span>
* <span data-ttu-id="8e20c-293">IpTag を PublicIpAddress に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-293">Add IpTags to PublicIpAddress</span></span>
    - <span data-ttu-id="8e20c-294">New-AzureRmPublicIpAddress の更新: IpTag を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-294">Updated New-AzureRmPublicIpAddress: Added IpTags</span></span>
    - <span data-ttu-id="8e20c-295">Iptag を追加する New-AzureRmPublicIpTag</span><span class="sxs-lookup"><span data-stu-id="8e20c-295">New-AzureRmPublicIpTag to add Iptag</span></span>
* <span data-ttu-id="8e20c-296">DisableBgpRoutePropagation プロパティを RouteTable および effectiveRoute に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-296">Add DisableBgpRoutePropagation property in RouteTable and effectiveRoute.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="8e20c-297">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="8e20c-297">AzureRM.Resources</span></span>
* <span data-ttu-id="8e20c-298">Register-AzureRmProviderFeature: 不足している例をドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-298">Register-AzureRmProviderFeature: Added missing example in the docs</span></span>
* <span data-ttu-id="8e20c-299">Register-AzureRmResourceProvider: 不足している例をドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-299">Register-AzureRmResourceProvider: Added missing example in the docs</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="8e20c-300">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-300">AzureRM.Storage</span></span>
* <span data-ttu-id="8e20c-301">ストレージ アカウントの新規と設定の各コマンドレットについて、次のパラメーターを廃止しました。EnableEncryptionService および DisableEncryptionService (保存時の暗号化は既定で有効であり、無効にできないため)</span><span class="sxs-lookup"><span data-stu-id="8e20c-301">Obsolete following parameters in new and set Storage Account cmdlets: EnableEncryptionService and DisableEncryptionService, since Encryption at Rest is enabled by default and can't be disabled.</span></span>
    - <span data-ttu-id="8e20c-302">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8e20c-302">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="8e20c-303">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8e20c-303">Set-AzureRmStorageAccount</span></span>


## <a name="530---february-2018"></a><span data-ttu-id="8e20c-304">5.3.0 - 2018 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8e20c-304">5.3.0 - February 2018</span></span>
### <a name="azurermprofile"></a><span data-ttu-id="8e20c-305">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="8e20c-305">AzureRM.Profile</span></span>
* <span data-ttu-id="8e20c-306">PowerShell 3 および 4 の非推奨警告を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-306">Added deprecation warning for PowerShell 3 and 4</span></span>
* <span data-ttu-id="8e20c-307">`Add-AzureRmAccount` を `Connect-AzureRmAccount` に名前変更しました。古いコマンドレット名に対して別名を追加し、他の別名 (`Login-AzAccount` および `Login-AzureRmAccount`) を新しいコマンドレット名にリダイレクトしました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-307">`Add-AzureRmAccount` has been renamed as `Connect-AzureRmAccount`; an alias has been added for the old cmdlet name, and other aliases (`Login-AzAccount` and `Login-AzureRmAccount`) have been redirected to the new cmdlet name.</span></span>
* <span data-ttu-id="8e20c-308">`Remove-AzureRmAccount` を `Disconnect-AzureRmAccount` に名前変更しました。古いコマンドレット名に対して別名を追加し、他の別名 (`Logout-AzAccount` および `Logout-AzureRmAccount`) を新しいコマンドレット名にリダイレクトしました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-308">`Remove-AzureRmAccount` has been renamed as `Disconnect-AzureRmAccount`; an alias has been added for the old cmdlet name, and other aliases (`Logout-AzAccount` and `Logout-AzureRmAccount`) have been redirected to the new cmdlet name.</span></span>
* <span data-ttu-id="8e20c-309">`Login-AzureRmAccount` の代わりに `Connect-AzureRmAccount` を使用するようにリソース文字列を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-309">Corrected Resource Strings to use `Connect-AzureRmAccount` instead of `Login-AzureRmAccount`</span></span>
* <span data-ttu-id="8e20c-310">`Add-AzureRmEnvironment` と `Set-AzureRmEnvironment`</span><span class="sxs-lookup"><span data-stu-id="8e20c-310">`Add-AzureRmEnvironment` and `Set-AzureRmEnvironment`</span></span>
  - <span data-ttu-id="8e20c-311">OperationalInsights データ プレーン RP で使用するパラメーターとして `-AzureOperationalInsightsEndpoint` と `-AzureOperationalInsightsEndpointResourceId` を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-311">Added `-AzureOperationalInsightsEndpoint` and `-AzureOperationalInsightsEndpointResourceId` as parameters for use with OperationalInsights data plane RP.</span></span>

### <a name="azurermanalysisservices"></a><span data-ttu-id="8e20c-312">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-312">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="8e20c-313">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-313">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermcompute"></a><span data-ttu-id="8e20c-314">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-314">AzureRM.Compute</span></span>
* <span data-ttu-id="8e20c-315">`New-AzureRmVM` の簡素化したパラメーター セットに `-AvailabilitySetName` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-315">Added `-AvailabilitySetName` parameter to the simplified parameterset of `New-AzureRmVM`.</span></span>
* <span data-ttu-id="8e20c-316">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-316">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>
* <span data-ttu-id="8e20c-317">VM および VM スケール セットに対するユーザー割り当て ID のサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-317">User assigned identity support for VM and VM scale set</span></span>
    - <span data-ttu-id="8e20c-318">`-IdentityType` および `-IdentityId` パラメーターを `New-AzureRmVMConfig`、`New-AzureRmVmssConfig`、`Update-AzureRmVM`、および `Update-AzureRmVmss` に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-318">`-IdentityType` and `-IdentityId` parameters are added to `New-AzureRmVMConfig`, `New-AzureRmVmssConfig`, `Update-AzureRmVM` and `Update-AzureRmVmss`</span></span>
* <span data-ttu-id="8e20c-319">`-EnableIPForwarding` パラメーターを `Add-AzureRmVmssNetworkInterfaceConfig` に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-319">Added `-EnableIPForwarding` parameter to `Add-AzureRmVmssNetworkInterfaceConfig`</span></span>
* <span data-ttu-id="8e20c-320">`-Priority` パラメーターを `New-AzureRmVmssConfig` に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-320">Added `-Priority` parameter to `New-AzureRmVmssConfig`</span></span>

### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="8e20c-321">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8e20c-321">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="8e20c-322">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-322">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermdatalakestore"></a><span data-ttu-id="8e20c-323">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8e20c-323">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="8e20c-324">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-324">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>
* <span data-ttu-id="8e20c-325">`Login-AzureRmAccount` を使用してログインせずにこのコマンドレットを実行した場合の `Test-AzureRmDataLakeStoreAccount` のエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-325">Corrected the error message of `Test-AzureRmDataLakeStoreAccount` when running this cmdlet without having logged in with `Login-AzureRmAccount`</span></span>

### <a name="azurermeventgrid"></a><span data-ttu-id="8e20c-326">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8e20c-326">AzureRM.EventGrid</span></span>
* <span data-ttu-id="8e20c-327">2018-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-327">Updated to use the 2018-01-01 API version.</span></span>

### <a name="azurermeventhub"></a><span data-ttu-id="8e20c-328">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="8e20c-328">AzureRM.EventHub</span></span>

* <span data-ttu-id="8e20c-329">Geo ディザスター リカバリー操作用に、以下の新しいコマンドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-329">Added below new commands for Geo Disaster Recovery operations.</span></span>
  - <span data-ttu-id="8e20c-330">新しい別名 (ディザスター リカバリーの構成) を作成する</span><span class="sxs-lookup"><span data-stu-id="8e20c-330">Creating a new Alias (Disaster Recovery configuration):</span></span>
    - `New-AzureRmEventHubGeoDRConfiguration`
  - <span data-ttu-id="8e20c-331">別名 (ディザスター リカバリー構成) を取得する</span><span class="sxs-lookup"><span data-stu-id="8e20c-331">Retrieve Alias (Disaster Recovery configuration) :</span></span>
    - `Get-AzureRmEventHubGeoDRConfiguration`
  - <span data-ttu-id="8e20c-332">ディザスター リカバリーを無効にし、プライマリ名前空間からセカンダリ名前空間への変更の複製を停止する</span><span class="sxs-lookup"><span data-stu-id="8e20c-332">Disabling the Disaster Recovery and stops replicating changes from primary to secondary namespaces</span></span>
    - `Set-AzureRmEventHubGeoDRConfigurationBreakPair`
  - <span data-ttu-id="8e20c-333">ディザスター リカバリー フェールオーバーを呼び出し、セカンダリ名前空間を指すように別名を再構成する</span><span class="sxs-lookup"><span data-stu-id="8e20c-333">Invoking Disaster Recovery failover and reconfigure the alias to point to the secondary namespace</span></span>
    - `Set-AzureRmEventHubGeoDRConfigurationFailOver`
  - <span data-ttu-id="8e20c-334">別名 (ディザスター リカバリー構成) を削除する</span><span class="sxs-lookup"><span data-stu-id="8e20c-334">Deleting an Alias(Disaster Recovery configuration)</span></span>
    - `Remove-AzureRmEventHubGeoDRConfiguration`
* <span data-ttu-id="8e20c-335">名前空間名と GeoDr 構成名 (別名の可用性) のチェック用に以下のコマンドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-335">Added below new commands for checking the Namespace Name and GeoDr Configuration Name - Alias availability.</span></span>
  - <span data-ttu-id="8e20c-336">名前空間名または別名 (ディザスター リカバリーの構成) の可用性のチェック</span><span class="sxs-lookup"><span data-stu-id="8e20c-336">Check the Availability of Namespace name or Alias(Disaster Recovery configuration) name:</span></span>
    - `Test-AzureRmEventHubName`

### <a name="azurerminsights"></a><span data-ttu-id="8e20c-337">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="8e20c-337">AzureRM.Insights</span></span>
* <span data-ttu-id="8e20c-338">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-338">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="8e20c-339">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8e20c-339">AzureRM.KeyVault</span></span>
* <span data-ttu-id="8e20c-340">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-340">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="8e20c-341">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8e20c-341">AzureRM.Network</span></span>
* <span data-ttu-id="8e20c-342">上書きの確認メッセージ "リソースを上書きしますか" を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-342">Fix overwrite message 'Are you sure you want to overwriteresource'</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="8e20c-343">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-343">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="8e20c-344">`Invoke-AzureRmOperationalInsightsQuery` を介した V2 API クエリ実行のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-344">Added support for V2 API querying via `Invoke-AzureRmOperationalInsightsQuery`.</span></span> <span data-ttu-id="8e20c-345">新しい API の詳細については、[https://dev.loganalytics.io/](https://dev.loganalytics.io/) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e20c-345">See [https://dev.loganalytics.io/](https://dev.loganalytics.io/) for more info on the new API.</span></span>

### <a name="azurermresources"></a><span data-ttu-id="8e20c-346">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="8e20c-346">AzureRM.Resources</span></span>
* <span data-ttu-id="8e20c-347">`Get-AzureRmADServicePrincipal`:SPN パラメーター セットと冗長であるため、既定の空のパラメーター セットから `-ServicePrincipalName` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-347">`Get-AzureRmADServicePrincipal`: Removed `-ServicePrincipalName` from the default Empty parameter set as it was redundant with the SPN parameter set</span></span>

### <a name="azurermservicebus"></a><span data-ttu-id="8e20c-348">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8e20c-348">AzureRM.ServiceBus</span></span>

* <span data-ttu-id="8e20c-349">`Remove-AzureRmServiceBusRule` および `Get-AzureRmServiceBusKey` の機能修正プログラムを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-349">Added functionality fix for `Remove-AzureRmServiceBusRule` and `Get-AzureRmServiceBusKey`</span></span>
* <span data-ttu-id="8e20c-350">Geo ディザスター リカバリー操作用に、以下の新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-350">Added below new commandlets for Geo Disaster Recovery operations.</span></span>
  - <span data-ttu-id="8e20c-351">新しい別名 (ディザスター リカバリーの構成) を作成する</span><span class="sxs-lookup"><span data-stu-id="8e20c-351">Creating a new Alias (Disaster Recovery configuration):</span></span>
    - `New-AzureRmServiceBusDRConfigurations`
  - <span data-ttu-id="8e20c-352">別名 (ディザスター リカバリー構成) を取得する</span><span class="sxs-lookup"><span data-stu-id="8e20c-352">Retrieve Alias (Disaster Recovery configuration) :</span></span>
    - `Get-AzureRmServiceBusDRConfigurations`
  - <span data-ttu-id="8e20c-353">ディザスター リカバリーを無効にし、プライマリ名前空間からセカンダリ名前空間への変更の複製を停止する</span><span class="sxs-lookup"><span data-stu-id="8e20c-353">Disabling the Disaster Recovery and stops replicating changes from primary to secondary namespaces</span></span>
    - `Set-AzureRmServiceBusDRConfigurationsBreakPairing`
  - <span data-ttu-id="8e20c-354">ディザスター リカバリー フェールオーバーを呼び出し、セカンダリ名前空間を指すように別名を再構成する</span><span class="sxs-lookup"><span data-stu-id="8e20c-354">Invoking Disaster Recovery failover and reconfigure the alias to point to the secondary namespace</span></span>
    - `Set-AzureRmServiceBusDRConfigurationsFailOver`
  - <span data-ttu-id="8e20c-355">別名 (ディザスター リカバリー構成) を削除する</span><span class="sxs-lookup"><span data-stu-id="8e20c-355">Deleting an Alias(Disaster Recovery configuration)</span></span>
    - `Remove-AzureRmServiceBusDRConfigurations`
* <span data-ttu-id="8e20c-356">Geo ディザスター リカバリーをサポートするように `Test-AzureRmServiceBusName` コマンドレットを更新しました - 別名の可用性チェック操作。</span><span class="sxs-lookup"><span data-stu-id="8e20c-356">Updated `Test-AzureRmServiceBusName` commandlets to support Geo Disaster Recovery - Alias name check availability operations.</span></span>
  - <span data-ttu-id="8e20c-357">名前空間名または別名 (ディザスター リカバリーの構成) の可用性のチェック</span><span class="sxs-lookup"><span data-stu-id="8e20c-357">Check the Availability of Namespace name or Alias(Disaster Recovery configuration) name:</span></span>
    - `Test-AzureRmServiceBusName`

### <a name="azurermusageaggregates"></a><span data-ttu-id="8e20c-358">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="8e20c-358">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="8e20c-359">`Connect-AzureRmAccount` を使用するように `Login-AzureRmAccount` の使用方法を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-359">Corrected usage of `Login-AzureRmAccount` to use `Connect-AzureRmAccount`</span></span>

## <a name="520---january-2018"></a><span data-ttu-id="8e20c-360">5.2.0 - 2018 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8e20c-360">5.2.0 - January 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="8e20c-361">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="8e20c-361">AzureRM.Profile</span></span>
* <span data-ttu-id="8e20c-362">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-362">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-363">Add-AzureRmAccount</span><span class="sxs-lookup"><span data-stu-id="8e20c-363">Add-AzureRmAccount</span></span>
  * <span data-ttu-id="8e20c-364">現在の VM/サービスの管理サービス ID の資格情報を使用して認証を行う -MSI ログインを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-364">Added -MSI login for authenticationg using the credentials of the Managed Service Identity of the current VM / Service</span></span>
  * <span data-ttu-id="8e20c-365">ユーザー指定のアクセス トークンを使用してログインする場合の KeyVault 認証を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-365">Fixed KeyVault Authentication when logging in with user-provided access tokens</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="8e20c-366">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-366">Azure.Storage</span></span>
* <span data-ttu-id="8e20c-367">Storage サービスのプロパティを取得および設定するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-367">Add cmdlets to get and set Storage service properties</span></span>
    - <span data-ttu-id="8e20c-368">Get-AzureStorageServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8e20c-368">Get-AzureStorageServiceProperty</span></span>
    - <span data-ttu-id="8e20c-369">Update-AzureStorageServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8e20c-369">Update-AzureStorageServiceProperty</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="8e20c-370">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-370">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="8e20c-371">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-371">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="8e20c-372">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8e20c-372">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="8e20c-373">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-373">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-374">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-374">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-375">New-AzureRmApiManagementProperty、Set-AzureRmApiManagementProperty、および New-AzureRmApiManagement で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-375">Obsoleted -Tags in favor of -Tag for New-AzureRmApiManagementProperty, Set-AzureRmApiManagementProperty, and New-AzureRmApiManagement</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="8e20c-376">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-376">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="8e20c-377">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-377">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-378">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-378">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="8e20c-379">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="8e20c-379">AzureRM.Automation</span></span>
* <span data-ttu-id="8e20c-380">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-380">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-381">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-381">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-382">Set-AzureRmAutomationRunbook で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-382">Obsoleted -Tags in favor of -Tag for Set-AzureRmAutomationRunbook</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="8e20c-383">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="8e20c-383">AzureRM.Backup</span></span>
* <span data-ttu-id="8e20c-384">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-384">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-385">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-385">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="8e20c-386">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="8e20c-386">AzureRM.Batch</span></span>
* <span data-ttu-id="8e20c-387">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-387">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-388">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-388">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="8e20c-389">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="8e20c-389">AzureRM.Cdn</span></span>
* <span data-ttu-id="8e20c-390">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-390">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-391">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-391">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-392">New-AzureRmCdnEndpoint および New-AzureRmCdnProfile で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-392">Obsoleted -Tags in favor of -Tag for New-AzureRmCdnEndpoint and New-AzureRmCdnProfile</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="8e20c-393">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-393">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="8e20c-394">Cognitive Services Management SDK バージョン 3.0.0 と統合しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-394">Integrate with Cognitive Services Management SDK version 3.0.0.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="8e20c-395">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-395">AzureRM.Compute</span></span>
* <span data-ttu-id="8e20c-396">簡素化したパラメーター セットを New-AzureRmVmss に追加しました。これにより、スマートな既定値を使用して、仮想マシン スケール セットおよびすべての必要なリソースを作成できます</span><span class="sxs-lookup"><span data-stu-id="8e20c-396">Added simplified parameter set to New-AzureRmVmss, which creates a Virtual Machine Scale Set and all required resources using smart defaults</span></span>
* <span data-ttu-id="8e20c-397">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-397">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-398">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-398">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-399">New-AzureRmVm および Update-AzureRmVm で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-399">Obsoleted -Tags in favor of -Tag for New-AzureRmVm and Update-AzureRmVm</span></span>
* <span data-ttu-id="8e20c-400">ゾーンが制限に含まれる場合の Get AzureRmComputeResourceSku コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-400">Fixed Get-AzureRmComputeResourceSku cmdlet when Zone is included in restriction.</span></span>
* <span data-ttu-id="8e20c-401">Azure Monitor シンクがサポートされるように、診断エージェントの構成スキーマを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-401">Updated Diagnostics Agent configuration schema for Azure Monitor sink support.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="8e20c-402">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8e20c-402">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="8e20c-403">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-403">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-404">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-404">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="8e20c-405">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8e20c-405">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="8e20c-406">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-406">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-407">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-407">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="8e20c-408">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="8e20c-408">AzureRM.DataFactories</span></span>
* <span data-ttu-id="8e20c-409">データ ストアのリンクされたサービスすべてについて、Azure Key Vault のサポートを有効にしました</span><span class="sxs-lookup"><span data-stu-id="8e20c-409">Enabled Azure Key Vault support for all data store linked services</span></span>
* <span data-ttu-id="8e20c-410">Azure SSIS 統合ランタイムにライセンスの種類プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-410">Added license type property for Azure SSIS integration runtime</span></span>
* <span data-ttu-id="8e20c-411">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-411">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-412">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-412">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-413">New-AzureRmDataFactory で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-413">Obsoleted -Tags in favor of -Tag for New-AzureRmDataFactory</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="8e20c-414">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8e20c-414">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="8e20c-415">データ ストアのリンクされたサービスすべてについて、Azure Key Vault のサポートを有効にしました</span><span class="sxs-lookup"><span data-stu-id="8e20c-415">Enabled Azure Key Vault support for all data store linked services</span></span>
* <span data-ttu-id="8e20c-416">Azure SSIS 統合ランタイムにライセンスの種類プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-416">Added license type property for Azure SSIS integration runtime</span></span>
* <span data-ttu-id="8e20c-417">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-417">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-418">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-418">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-419">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドで AHUB 機能を有効にするための "LicenseType" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-419">Add parameter "LicenseType" for "Set-AzureRmDataFactoryV2IntegrationRuntime" cmd to enable AHUB functionality</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="8e20c-420">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8e20c-420">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="8e20c-421">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-421">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-422">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-422">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-423">New-AzureRmDataLakeAnalyticsAccount および Set-AzureRmDataLakeAnalyticsAccount で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-423">Obsoleted -Tags in favor of -Tag for New-AzureRmDataLakeAnalyticsAccount and Set-AzureRmDataLakeAnalyticsAccount</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="8e20c-424">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8e20c-424">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="8e20c-425">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-425">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-426">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-426">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-427">New-AzureRmDataLakeStoreAccount および Set-AzureRmDataLakeStoreAccount で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-427">Obsoleted -Tags in favor of -Tag for New-AzureRmDataLakeStoreAccount and Set-AzureRmDataLakeStoreAccount</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="8e20c-428">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="8e20c-428">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="8e20c-429">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-429">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="8e20c-430">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="8e20c-430">AzureRM.Dns</span></span>
* <span data-ttu-id="8e20c-431">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-431">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="8e20c-432">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8e20c-432">AzureRM.EventGrid</span></span>
* <span data-ttu-id="8e20c-433">次の新しいコマンドレッドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-433">Added the following new cmdlet:</span></span>
  - <span data-ttu-id="8e20c-434">Update-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8e20c-434">Update-AzureRmEventGridSubscription</span></span>
    - <span data-ttu-id="8e20c-435">Event Grid イベント サブスクリプションのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-435">Update the properties of an Event Grid event subscription.</span></span>
* <span data-ttu-id="8e20c-436">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-436">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-437">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-437">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="8e20c-438">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="8e20c-438">AzureRM.EventHub</span></span>
* <span data-ttu-id="8e20c-439">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-439">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-440">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-440">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="8e20c-441">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8e20c-441">AzureRM.HDInsight</span></span>
* <span data-ttu-id="8e20c-442">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-442">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-443">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-443">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="8e20c-444">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="8e20c-444">AzureRM.Insights</span></span>
* <span data-ttu-id="8e20c-445">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-445">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-446">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-446">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="8e20c-447">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="8e20c-447">AzureRM.IotHub</span></span>
* <span data-ttu-id="8e20c-448">IoTHub コマンドレットの証明書のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-448">Add Certificate support for IoTHub cmdlets</span></span>
* <span data-ttu-id="8e20c-449">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-449">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-450">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-450">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="8e20c-451">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8e20c-451">AzureRM.KeyVault</span></span>
* <span data-ttu-id="8e20c-452">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-452">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-453">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-453">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-454">実行時間が長い KeyVault コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-454">Added -AsJob support for long-running KeyVault cmdlets.</span></span> <span data-ttu-id="8e20c-455">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-455">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
  * <span data-ttu-id="8e20c-456">影響を受けるコマンドレット: Remove-AzureRmKeyVault</span><span class="sxs-lookup"><span data-stu-id="8e20c-456">Affected cmdlet is: Remove-AzureRmKeyVault</span></span>
* <span data-ttu-id="8e20c-457">Set-AzureRmKeyVaultAccessPolicy のバグを修正しました。このバグでは AAD フィルターによって UPN が設定されるのではなく、SPN が指定の UPN に設定されていました</span><span class="sxs-lookup"><span data-stu-id="8e20c-457">Fixed bug in Set-AzureRmKeyVaultAccessPolicy where the AAD filter was setting SPN to the provided UPN, rather than setting the UPN</span></span>
  - <span data-ttu-id="8e20c-458">詳細については次の問題を参照してください: https://github.com/Azure/azure-powershell/issues/5201</span><span class="sxs-lookup"><span data-stu-id="8e20c-458">See the following issue for more information: https://github.com/Azure/azure-powershell/issues/5201</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="8e20c-459">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8e20c-459">AzureRM.LogicApp</span></span>
* <span data-ttu-id="8e20c-460">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-460">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-461">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-461">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="8e20c-462">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8e20c-462">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="8e20c-463">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-463">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-464">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-464">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-465">Update-AzureRmMlCommitmentPlan で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-465">Obsoleted -Tags in favor of -Tag for Update-AzureRmMlCommitmentPlan</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="8e20c-466">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="8e20c-466">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="8e20c-467">Remove-AzureRmMlOpCluster コマンドレットに IncludeAllResources パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-467">Add IncludeAllResources parameter to Remove-AzureRmMlOpCluster cmdlet</span></span>
  - <span data-ttu-id="8e20c-468">このスイッチ パラメーターを使用すると、最初にクラスターで作成されたすべてのリソースが削除されます</span><span class="sxs-lookup"><span data-stu-id="8e20c-468">Using this switch parameter will remove all resources that were created with the cluster originally</span></span>
* <span data-ttu-id="8e20c-469">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-469">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-470">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-470">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="8e20c-471">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="8e20c-471">AzureRM.Media</span></span>
* <span data-ttu-id="8e20c-472">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-472">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-473">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-473">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-474">Set-AzureRmMediaService および New-AzureRmMediaService で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-474">Obsoleted -Tags in favor of -Tag for Set-AzureRmMediaService and New-AzureRmMediaService</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="8e20c-475">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="8e20c-475">AzureRM.Network</span></span>
* <span data-ttu-id="8e20c-476">実行時間が長い Network コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-476">Added -AsJob support for long-running Network cmdlets.</span></span> <span data-ttu-id="8e20c-477">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-477">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
* <span data-ttu-id="8e20c-478">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-478">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-479">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-479">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="8e20c-480">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8e20c-480">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="8e20c-481">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-481">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-482">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-482">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-483">New-AzureRmNotificationHubsNamespace および Set-AzureRmNotificationHubsNamespace で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-483">Obsoleted -Tags in favor of -Tag for New-AzureRmNotificationHubsNamespace and Set-AzureRmNotificationHubsNamespace</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="8e20c-484">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-484">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="8e20c-485">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-485">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-486">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-486">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-487">New-AzureRmOperationalInsightsSavedSearch、Set-AzureRmOperationalInsightsSavedSearch、New-AzureRmOperationalInsightsWorkspace、および Set-AzureRmOperationalInsightsWorkspace で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-487">Obsoleted -Tags in favor of -Tag for New-AzureRmOperationalInsightsSavedSearch, Set-AzureRmOperationalInsightsSavedSearch, New-AzureRmOperationalInsightsWorkspace, and Set-AzureRmOperationalInsightsWorkspace</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="8e20c-488">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8e20c-488">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="8e20c-489">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-489">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-490">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-490">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="8e20c-491">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-491">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="8e20c-492">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-492">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-493">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-493">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="8e20c-494">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8e20c-494">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8e20c-495">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-495">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-496">the Restore-AzureRmRecoveryServicesBackupItem コマンドレッドに -UseOriginalStorageAccount オプションを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-496">Added -UseOriginalStorageAccount option to the Restore-AzureRmRecoveryServicesBackupItem cmdlet.</span></span>
  - <span data-ttu-id="8e20c-497">このフラグを有効にすると、元のストレージ アカウントにディスクが復元されます。これにより、ユーザーは復元された VM の構成を元の VM にできる限り近いものに維持できます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-497">Enabling this flag results in restoring disks to their original storage accounts which allows users to maintain the configuration of restored VM as close to the original VMs as possible.</span></span>
  - <span data-ttu-id="8e20c-498">これは、復元操作のパフォーマンスの向上にも役立ちます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-498">It also helps in improving the performance of the restore operation.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="8e20c-499">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8e20c-499">AzureRM.RedisCache</span></span>
* <span data-ttu-id="8e20c-500">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-500">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-501">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-501">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-502">ファイアウォール規則のために 3 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-502">Added  3 new cmdlets for firewall rules</span></span>
* <span data-ttu-id="8e20c-503">geo レプリケーションのために 3 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-503">Added  3 new cmdlets for geo replication</span></span>
* <span data-ttu-id="8e20c-504">ゾーンとタグのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-504">Added support for zones and tags</span></span>
* <span data-ttu-id="8e20c-505">可能な場合は、ResourceGroup を省略可能としてマークしてください。</span><span class="sxs-lookup"><span data-stu-id="8e20c-505">Make ResourceGroup as optional whenever possible.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="8e20c-506">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="8e20c-506">AzureRM.Relay</span></span>
* <span data-ttu-id="8e20c-507">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-507">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-508">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-508">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="8e20c-509">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="8e20c-509">AzureRM.Resources</span></span>
* <span data-ttu-id="8e20c-510">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-510">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-511">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-511">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-512">実行時間が長い Resources コマンドのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-512">Added -AsJob support for long-running Resources cmdlets.</span></span> <span data-ttu-id="8e20c-513">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-513">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
* <span data-ttu-id="8e20c-514">名前付け規則に準拠するように Get AzureRmProviderOperation から Get-AzureRmResourceProviderAction に別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-514">Added alias from Get-AzureRmProviderOperation to Get-AzureRmResourceProviderAction to conform with naming conventions</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="8e20c-515">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="8e20c-515">AzureRM.Scheduler</span></span>
* <span data-ttu-id="8e20c-516">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-516">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-517">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-517">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermservermanagement"></a><span data-ttu-id="8e20c-518">AzureRM.ServerManagement</span><span class="sxs-lookup"><span data-stu-id="8e20c-518">AzureRM.ServerManagement</span></span>
* <span data-ttu-id="8e20c-519">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-519">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-520">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-520">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-521">New-AzureRmServerManagementNode および New-AzureRmServerManagementGateway で -Tag が優先されるように -Tags を廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-521">Obsoleted -Tags in favor of -Tag for New-AzureRmServerManagementNode and New-AzureRmServerManagementGateway</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="8e20c-522">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8e20c-522">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="8e20c-523">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-523">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-524">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-524">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="8e20c-525">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8e20c-525">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="8e20c-526">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-526">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-527">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-527">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermsiterecovery"></a><span data-ttu-id="8e20c-528">AzureRM.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-528">AzureRM.SiteRecovery</span></span>
* <span data-ttu-id="8e20c-529">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-529">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-530">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-530">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="8e20c-531">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="8e20c-531">AzureRM.Sql</span></span>
* <span data-ttu-id="8e20c-532">監査コマンドのパラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-532">Update the Auditing commands parameters description</span></span>
* <span data-ttu-id="8e20c-533">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-533">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-534">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-534">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-535">実行時間の長いコマンドレットに -AsJob パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-535">Added -AsJob parameter to long running cmdlets</span></span>
* <span data-ttu-id="8e20c-536">Get AzureRmSqlServiceObjective の - DatabaseName パラメーターを廃止しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-536">Obsoleted -DatabaseName parameter from Get-AzureRmSqlServiceObjective</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="8e20c-537">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-537">AzureRM.Storage</span></span>
* <span data-ttu-id="8e20c-538">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-538">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-539">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-539">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-540">-EnableEncryptionService None パラメーターを指定した New-AzureRMStorageAccount コマンドレットを実行した際の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-540">Fix a null reference issue of run cmdlet New-AzureRMStorageAccount with parameter -EnableEncryptionService None</span></span>
* <span data-ttu-id="8e20c-541">実行時間が長い Storage コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-541">Added -AsJob support for long-running Storage cmdlets.</span></span> <span data-ttu-id="8e20c-542">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-542">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
    - <span data-ttu-id="8e20c-543">影響を受けるコマンドレットは、Storage Account および Storage Account Network Rule の New-、Remove-、Add-、Update- です。</span><span class="sxs-lookup"><span data-stu-id="8e20c-543">Affected cmdlets are New-, Remove-, Add-, and Update- for Storage Account and Storage Account Network Rule.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="8e20c-544">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="8e20c-544">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="8e20c-545">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-545">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-546">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-546">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="8e20c-547">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8e20c-547">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="8e20c-548">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-548">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-549">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-549">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="8e20c-550">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="8e20c-550">AzureRM.Websites</span></span>
* <span data-ttu-id="8e20c-551">有効な場所を介したタブ補完が可能になるように、-Location パラメーターに Location Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-551">Added Location Completer to -Location parameters allowing tab completion through valid Locations</span></span>
* <span data-ttu-id="8e20c-552">現在のサブスクリプションのリソース グループを介したタブ補完が可能になるように、ResourceGroup パラメーターに ResourceGroup Completer を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-552">Added ResourceGroup Completer to -ResourceGroup parameters allowing tab completion through resource groups in current subscription</span></span>
* <span data-ttu-id="8e20c-553">実行時間が長い Websites コマンドレットのために -AsJob のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-553">Added -AsJob support for long-running Websites cmdlets.</span></span> <span data-ttu-id="8e20c-554">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-554">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
     - <span data-ttu-id="8e20c-555">影響を受けるコマンドレットは、WebApps、AppServicePlan、および Slots の New-、Remove-、Add-、Set- です</span><span class="sxs-lookup"><span data-stu-id="8e20c-555">Affected cmdlets are New-, Remove-, Add-, and Set- for WebApps, AppServicePlan and Slots</span></span>

## <a name="2017128-version-511"></a><span data-ttu-id="8e20c-556">2017.12.8 バージョン 5.1.1</span><span class="sxs-lookup"><span data-stu-id="8e20c-556">2017.12.8 Version 5.1.1</span></span>
* <span data-ttu-id="8e20c-557">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-557">AnalysisServices</span></span>
  - <span data-ttu-id="8e20c-558">すべてのクラウドがサポートされるように、場所の検証セットを動的ルックアップに変更しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-558">Change validate set of location to dynamic lookup so that all clouds are supported.</span></span>
* <span data-ttu-id="8e20c-559">Automation</span><span class="sxs-lookup"><span data-stu-id="8e20c-559">Automation</span></span>
  - <span data-ttu-id="8e20c-560">Import-AzureRMAutomationRunbook に更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-560">Update to Import-AzureRMAutomationRunbook</span></span>
    - <span data-ttu-id="8e20c-561">Python2 Runbook がサポートされるようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-561">Support is now being provided for Python2 runbooks</span></span>
* <span data-ttu-id="8e20c-562">Batch</span><span class="sxs-lookup"><span data-stu-id="8e20c-562">Batch</span></span>
  - <span data-ttu-id="8e20c-563">リソース グループがないアカウント操作がリソース グループの自動検出に失敗するというバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-563">Fixed a bug where account operations without a resource group failed to auto-detect the resource group</span></span>
* <span data-ttu-id="8e20c-564">Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-564">Compute</span></span>
  - <span data-ttu-id="8e20c-565">Get-AzureRmComputeResourceSku によってゾーン情報が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-565">Get-AzureRmComputeResourceSku shows zone information.</span></span>
  - <span data-ttu-id="8e20c-566">問題 https://github.com/Azure/azure-powershell/issues/5038 を修正するために Disable-AzureRmVmssDiskEncryption を更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-566">Update Disable-AzureRmVmssDiskEncryption to fix issue https://github.com/Azure/azure-powershell/issues/5038</span></span>
  - <span data-ttu-id="8e20c-567">実行時間が長い Compute コマンドレット用の -AsJob サポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-567">Added -AsJob support for long-running Compute cmdlets.</span></span> <span data-ttu-id="8e20c-568">選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-568">Allows selected cmdlets to run in the background and return a job to track and control progress.</span></span>
    - <span data-ttu-id="8e20c-569">影響を受けるコマンドレット: Virtual Machines および VM Scale Sets の New-、Update-、Set-、Remove-、Start-、Restart-、Stop- コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8e20c-569">Affected cmdlets include: New-, Update-, Set-, Remove-, Start-, Restart-, Stop- cmdlets for Virtual Machines and Virtual Machine Scale Sets</span></span>
    - <span data-ttu-id="8e20c-570">簡素化したパラメーター セットを New-AzureRmVM に追加しました。これにより、スマートな既定値を使用して、仮想マシンおよびすべての必要なリソースを作成できます</span><span class="sxs-lookup"><span data-stu-id="8e20c-570">Added simplified parameter set to New-AzureRmVM, which creates a Virtual Machine and all required resources using smart defaults</span></span>
* <span data-ttu-id="8e20c-571">ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8e20c-571">ContainerInstance</span></span>
  - <span data-ttu-id="8e20c-572">Azure コンテナー インスタンス SDK 2017-10-01 を適用しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-572">Apply Azure Container Instance SDK 2017-10-01</span></span>
    - <span data-ttu-id="8e20c-573">コンテナー run-to-completion のサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-573">Support container run-to-completion</span></span>
    - <span data-ttu-id="8e20c-574">Azure File ボリューム マウントのサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-574">Support Azure File volume mount</span></span>
    - <span data-ttu-id="8e20c-575">パブリック IP の複数ポートのオープンのサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-575">Support opening multiple ports for public IP</span></span>
* <span data-ttu-id="8e20c-576">ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8e20c-576">ContainerRegistry</span></span>
  - <span data-ttu-id="8e20c-577">geo レプリケーションと webhook の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8e20c-577">New cmdlets for geo-replication and webhooks</span></span>
    - <span data-ttu-id="8e20c-578">Get/New/Remove-AzureRmContainerRegistryReplication</span><span class="sxs-lookup"><span data-stu-id="8e20c-578">Get/New/Remove-AzureRmContainerRegistryReplication</span></span>
    - <span data-ttu-id="8e20c-579">Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook</span><span class="sxs-lookup"><span data-stu-id="8e20c-579">Get/New/Remove/Test/Update-AzureRmContainerRegistryWebhook</span></span>
* <span data-ttu-id="8e20c-580">DataFactories</span><span class="sxs-lookup"><span data-stu-id="8e20c-580">DataFactories</span></span>
    - <span data-ttu-id="8e20c-581">資格情報の暗号化機能が、"リモート アクセス" 有効 (ネットワーク経由) と "リモート アクセス" 無効 (ローカル コンピューター) の両方で動作するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-581">Credential encryption functionality now works with both "Remote Access" enabled (Over Network) and "Remote Access" disabled (Local Machine).</span></span>
* <span data-ttu-id="8e20c-582">DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8e20c-582">DataFactoryV2</span></span>
  - <span data-ttu-id="8e20c-583">追加された 2 つの新しいコマンドレット: Update-AzureRmDataFactoryV2 および Stop-AzureRmDataFactoryV2PipelineRun</span><span class="sxs-lookup"><span data-stu-id="8e20c-583">Added two new cmdlets: Update-AzureRmDataFactoryV2 and Stop-AzureRmDataFactoryV2PipelineRun</span></span>
* <span data-ttu-id="8e20c-584">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8e20c-584">DataLakeAnalytics</span></span>
  - <span data-ttu-id="8e20c-585">ScriptParameter というパラメーターを Submit-AzureRmDataLakeAnalyticsJob に追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-585">Added a parameter called ScriptParameter to Submit-AzureRmDataLakeAnalyticsJob</span></span>
    - <span data-ttu-id="8e20c-586">ScriptParameter に関する詳細情報を、Submit-AzureRmDataLakeAnalyticsJob で Get-Help を使用して確認できます</span><span class="sxs-lookup"><span data-stu-id="8e20c-586">Detailed information about ScriptParameter can be found using Get-Help on Submit-AzureRmDataLakeAnalyticsJob</span></span>
  - <span data-ttu-id="8e20c-587">New-AzureRmDataLakeAnalyticsAccount については、パラメーター MaxDegreeOfParallelism を MaxAnalyticsUnits に変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-587">For New-AzureRmDataLakeAnalyticsAccount, changed the parameter MaxDegreeOfParallelism to MaxAnalyticsUnits</span></span>
    - <span data-ttu-id="8e20c-588">パラメーター MaxAnalyticsUnits の別名を追加しました: MaxDegreeOfParallelism</span><span class="sxs-lookup"><span data-stu-id="8e20c-588">Added an alias for the parameter MaxAnalyticsUnits: MaxDegreeOfParallelism</span></span>
  - <span data-ttu-id="8e20c-589">New-AzureRmDataLakeAnalyticsComputePolicy については、パラメーター MaxDegreeOfParallelismPerJob を MaxAnalyticsUnitsPerJob に変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-589">For New-AzureRmDataLakeAnalyticsComputePolicy, changed the parameter MaxDegreeOfParallelismPerJob to MaxAnalyticsUnitsPerJob</span></span>
    - <span data-ttu-id="8e20c-590">パラメーター MaxAnalyticsUnitsPerJob の別名を追加しました: MaxDegreeOfParallelismPerJob</span><span class="sxs-lookup"><span data-stu-id="8e20c-590">Added an alias for the parameter MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob</span></span>
  - <span data-ttu-id="8e20c-591">Set-AzureRmDataLakeAnalyticsAccount については、パラメーター MaxDegreeOfParallelism を MaxAnalyticsUnits に変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-591">For Set-AzureRmDataLakeAnalyticsAccount, changed the parameter MaxDegreeOfParallelism to MaxAnalyticsUnits</span></span>
    - <span data-ttu-id="8e20c-592">パラメーター MaxAnalyticsUnits の別名を追加しました: MaxDegreeOfParallelism</span><span class="sxs-lookup"><span data-stu-id="8e20c-592">Added an alias for the parameter MaxAnalyticsUnits: MaxDegreeOfParallelism</span></span>
  - <span data-ttu-id="8e20c-593">Submit-AzureRmDataLakeAnalyticsJob については、パラメーター DegreeOfParallelism を AnalyticsUnits に変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-593">For Submit-AzureRmDataLakeAnalyticsJob, changed the parameter DegreeOfParallelism to AnalyticsUnits</span></span>
    - <span data-ttu-id="8e20c-594">パラメーター AnalyticsUnits の別名を追加しました: DegreeOfParallelism</span><span class="sxs-lookup"><span data-stu-id="8e20c-594">Added an alias for the parameter AnalyticsUnits: DegreeOfParallelism</span></span>
  - <span data-ttu-id="8e20c-595">Update-AzureRmDataLakeAnalyticsComputePolicy については、パラメーター MaxDegreeOfParallelismPerJob を MaxAnalyticsUnitsPerJob に変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-595">For Update-AzureRmDataLakeAnalyticsComputePolicy, changed the parameter MaxDegreeOfParallelismPerJob to MaxAnalyticsUnitsPerJob</span></span>
    - <span data-ttu-id="8e20c-596">パラメーター MaxAnalyticsUnitsPerJob の別名を追加しました: MaxDegreeOfParallelismPerJob</span><span class="sxs-lookup"><span data-stu-id="8e20c-596">Added an alias for the parameter MaxAnalyticsUnitsPerJob: MaxDegreeOfParallelismPerJob</span></span>
* <span data-ttu-id="8e20c-597">MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="8e20c-597">MachineLearningCompute</span></span>
  - <span data-ttu-id="8e20c-598">Set-AzureRmMlOpCluster を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-598">Add Set-AzureRmMlOpCluster</span></span>
    - <span data-ttu-id="8e20c-599">クラスターのエージェント数または SSL 構成を更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-599">Update a cluster's agent count or SSL configuration</span></span>
  - <span data-ttu-id="8e20c-600">オーケストレーター プロパティがオプションになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-600">Orchestrator properties are optional</span></span>
    - <span data-ttu-id="8e20c-601">サービス プリンシパルが提供されていない場合、そのサービス プリンシパルはサービスによって作成されるため、オーケストレーター プロパティがオプションになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-601">The service will create a service principal if not provided, so the orchestrator properties are now optional</span></span>
* <span data-ttu-id="8e20c-602">PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8e20c-602">PowerBIEmbedded</span></span>
  - <span data-ttu-id="8e20c-603">Power BI Embedded 容量コマンドレットのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-603">Add support for Power BI Embedded Capacity cmdlets</span></span>
  - <span data-ttu-id="8e20c-604">新しいコマンドレット Get-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量の詳細を取得します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-604">New Cmdlet Get-AzureRmPowerBIEmbeddedCapacity - Gets the details of a PowerBI Embedded Capacity.</span></span>
  - <span data-ttu-id="8e20c-605">新しいコマンドレット New-AzureRmPowerBIEmbeddedCapacity - 新しい PowerBI Embedded 容量を作成します</span><span class="sxs-lookup"><span data-stu-id="8e20c-605">New Cmdlet New-AzureRmPowerBIEmbeddedCapacity - Creates a new PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="8e20c-606">新しいコマンドレット Remove-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを削除します</span><span class="sxs-lookup"><span data-stu-id="8e20c-606">New Cmdlet Remove-AzureRmPowerBIEmbeddedCapacity - Deletes an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="8e20c-607">新しいコマンドレット Resume-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを再開します</span><span class="sxs-lookup"><span data-stu-id="8e20c-607">New Cmdlet Resume-AzureRmPowerBIEmbeddedCapacity - Resumes an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="8e20c-608">新しいコマンドレット Suspend-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを中断します</span><span class="sxs-lookup"><span data-stu-id="8e20c-608">New Cmdlet Suspend-AzureRmPowerBIEmbeddedCapacity - Suspends an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="8e20c-609">新しいコマンドレット Test-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスの存在をテストします</span><span class="sxs-lookup"><span data-stu-id="8e20c-609">New Cmdlet Test-AzureRmPowerBIEmbeddedCapacity - Tests the existence of an instance of PowerBI Embedded Capacity</span></span>
  - <span data-ttu-id="8e20c-610">新しいコマンドレット Update-AzureRmPowerBIEmbeddedCapacity - PowerBI Embedded 容量のインスタンスを変更します</span><span class="sxs-lookup"><span data-stu-id="8e20c-610">New Cmdlet Update-AzureRmPowerBIEmbeddedCapacity - Modifies an instance of PowerBI Embedded Capacity</span></span>
* <span data-ttu-id="8e20c-611">プロファイル</span><span class="sxs-lookup"><span data-stu-id="8e20c-611">Profile</span></span>
  - <span data-ttu-id="8e20c-612">USGovernmentActiveDirectoryEndpoint を https://login.microsoftonline.us/ に更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-612">Updated USGovernmentActiveDirectoryEndpoint to https://login.microsoftonline.us/</span></span>
    - <span data-ttu-id="8e20c-613">Azure Government エンドポイント マッピングの詳細については、 https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping を参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-613">For more information about the Azure Government endpoint mappings, please see the following: https://docs.microsoft.com/en-us/azure/azure-government/documentation-government-developer-guide#endpoint-mapping</span></span>
    - <span data-ttu-id="8e20c-614">コマンドの -AsJob サポートを追加しました。これにより、選択したコマンドレットをバック グラウンドで実行し、進行状況を追跡および制御するジョブを返すことができます</span><span class="sxs-lookup"><span data-stu-id="8e20c-614">Added -AsJob support for cmdlets, enabling selected cmdlets to execute in the background and return a job to track and control progress</span></span>
    - <span data-ttu-id="8e20c-615">-AsJob パラメーターを Get-AzureRmSubscription コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-615">Added -AsJob parameter to Get-AzureRmSubscription cmdlet</span></span>
* <span data-ttu-id="8e20c-616">RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8e20c-616">RecoveryServices.Backup</span></span>
  - <span data-ttu-id="8e20c-617">バグを修正 - Get-AzureRmRecoveryServicesBackupItem が、コンテナー名フィルターの比較で大文字と小文字を区別するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-617">Fixed bug - Get-AzureRmRecoveryServicesBackupItem should do case insensitive comparison for container name filter.</span></span>
  - <span data-ttu-id="8e20c-618">バグを修正 - AzureVmItem に、前回のバックアップ操作が行われた時間を示すプロパティが追加されました - LastBackupTime。</span><span class="sxs-lookup"><span data-stu-id="8e20c-618">Fixed bug - AzureVmItem now has a property that shows the last time a backup operation has happened - LastBackupTime.</span></span>
* <span data-ttu-id="8e20c-619">リソース</span><span class="sxs-lookup"><span data-stu-id="8e20c-619">Resources</span></span>
  - <span data-ttu-id="8e20c-620">Get-AzureRMRoleAssignment による割り当てで、カスタム ロールの roledefiniton 名がないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-620">Fixed issue where Get-AzureRMRoleAssignment would result in a assignments without roledefiniton name for custom roles</span></span>
    - <span data-ttu-id="8e20c-621">ユーザーは、ロールの種類に関係なく、Get-AzureRMRoleAssignment で、roledefinition 名を持つ割り当てを使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-621">Users can now use Get-AzureRMRoleAssignment with assignments having roledefinition names irrespective of the type of role</span></span>
  - <span data-ttu-id="8e20c-622">assignablescopes に新しいスコープがある場合に、RD が見つからないというエラーを Set-AzureRMRoleRoleDefinition がスローするという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-622">Fixed issue where Set-AzureRMRoleRoleDefinition used to throw RD not found error when there was a new scope in assignablescopes</span></span>
    - <span data-ttu-id="8e20c-623">ユーザーが、スコープの位置に関係なく、Set-AzureRMRoleRoleDefinition で、新しいスコープを含む割り当て可能なスコープを使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-623">Users can now use Set-AzureRMRoleRoleDefinition with assignable scopes including new scopes irrespective of the position of the scope</span></span>
  - <span data-ttu-id="8e20c-624">スコープの末尾に "/" を使用できます</span><span class="sxs-lookup"><span data-stu-id="8e20c-624">Allow scopes to end with "/"</span></span>
    - <span data-ttu-id="8e20c-625">スコープの末尾が "/" の RoleDefinition および RoleAssignment コマンドレットをユーザーが使用できるようになりました。これにより、API および CLI との一貫性が確保されます</span><span class="sxs-lookup"><span data-stu-id="8e20c-625">Users can now use RoleDefinition and RoleAssignment commandlets with scopes ending with "/" ,consistent with API and CLI</span></span>
  - <span data-ttu-id="8e20c-626">ユーザーが、委任フラグを使用して RoleAssignment を作成できます</span><span class="sxs-lookup"><span data-stu-id="8e20c-626">Allow users to create RoleAssignment using delegation flag</span></span>
    - <span data-ttu-id="8e20c-627">ユーザーが、New-AzureRMRoleAssignment で、委任フラグ追加オプションを使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-627">Users can now use New-AzureRMRoleAssignment with an option of adding the delegation flag</span></span>
  - <span data-ttu-id="8e20c-628">スコープのパラメーターを優先するように RoleAssignment get を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-628">Fix RoleAssignment get to respect the scope parameter</span></span>
  - <span data-ttu-id="8e20c-629">New-AzureRmRoleAssignment コマンドレットに ServicePrincipalName の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-629">Add an alias for ServicePrincipalName in the New-AzureRmRoleAssignment Commandlet</span></span>
    - <span data-ttu-id="8e20c-630">ユーザーが、New- AzureRmRoleAssignment コマンドレットを使用するときに、ServicePrincipalName ではなく ApplicationId を使用できるようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-630">Users can now use the ApplicationId instead of the ServicePrincipalName when using the New-AzureRmRoleAssignment commandlet</span></span>
* <span data-ttu-id="8e20c-631">SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-631">SiteRecovery</span></span>
  - <span data-ttu-id="8e20c-632">次の重大な変更のリリースに備えて、このモジュールのすべてのコマンドレットに非推奨警告を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-632">Add deprecation warnings for all cmdlets in this module in preparation for the next breaking change release.</span></span>
    - <span data-ttu-id="8e20c-633">AzureRM からコマンドレットを移行する方法の詳細については、今後の重大な変更ガイドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e20c-633">Please see the upcoming breaking changes guide for more information on how to migrate your cmdlets from AzureRM.</span></span>
* <span data-ttu-id="8e20c-634">SQL</span><span class="sxs-lookup"><span data-stu-id="8e20c-634">Sql</span></span>
  - <span data-ttu-id="8e20c-635">Set-AzureRmSqlDatabase を使用して、データベースの名前を変更する機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-635">Added ability to rename database using Set-AzureRmSqlDatabase</span></span>
  - <span data-ttu-id="8e20c-636">修正された問題 https://github.com/Azure/azure-powershell/issues/4974</span><span class="sxs-lookup"><span data-stu-id="8e20c-636">Fixed issue https://github.com/Azure/azure-powershell/issues/4974</span></span>
    - <span data-ttu-id="8e20c-637">監査コマンドレットに無効な AUDIT_CHANGED_GROUP 値を指定しても、エラーがスローされなくなりました。これは今後のリリースで削除される予定です。</span><span class="sxs-lookup"><span data-stu-id="8e20c-637">Providing invalid AUDIT_CHANGED_GROUP value for auditing cmdlets no longer throws an error and will be removed in an upcoming release.</span></span>
  - <span data-ttu-id="8e20c-638">修正された問題 https://github.com/Azure/azure-powershell/issues/5046</span><span class="sxs-lookup"><span data-stu-id="8e20c-638">Fixed issue https://github.com/Azure/azure-powershell/issues/5046</span></span>
    - <span data-ttu-id="8e20c-639">監査コマンドレットの AuditAction パラメーターが無視されなくなりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-639">AuditAction parameter in auditing cmdlets is no longer being ignored</span></span>
  - <span data-ttu-id="8e20c-640">"Secondary" StorageKeyType を指定したときの監査コマンドレットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-640">Fixed an issue in Auditing cmdlets when 'Secondary' StorageKeyType is provided</span></span>
    - <span data-ttu-id="8e20c-641">BLOB 監査の設定時に、StorageKeyType パラメーターに "Secondary" 値を指定すると、セカンダリ ストレージ アカウント キーではなくプライマリ キーが使用されました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-641">When setting blob auditing, the primary storage account key was used instead of the secondary key when providing 'Secondary' value for StorageKeyType parameter.</span></span>
  - <span data-ttu-id="8e20c-642">Set-AzureRmSqlServerTransparentDataEncryptionProtector からの確認メッセージの表現を変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-642">Changing the wording for confirmation message from Set-AzureRmSqlServerTransparentDataEncryptionProtector</span></span>
* <span data-ttu-id="8e20c-643">Azure (RDFE)</span><span class="sxs-lookup"><span data-stu-id="8e20c-643">Azure (RDFE)</span></span>
    - <span data-ttu-id="8e20c-644">すべての RemoteApp コマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-644">Removed all RemoteApp Cmdles</span></span>
* <span data-ttu-id="8e20c-645">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-645">Azure.Storage</span></span>
    - <span data-ttu-id="8e20c-646">Azure Storage Client Library 8.6.0 および Azure Storage DataMovement Library 0.6.5 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="8e20c-646">Upgrade to Azure Storage Client Library 8.6.0 and Azure Storage DataMovement Library 0.6.5</span></span>

## <a name="20171110-version-501"></a><span data-ttu-id="8e20c-647">2017.11.10 バージョン 5.0.1</span><span class="sxs-lookup"><span data-stu-id="8e20c-647">2017.11.10 Version 5.0.1</span></span>
* <span data-ttu-id="8e20c-648">以下のモジュールで一部のコマンドレットを実行した際に失敗の原因となるアセンブリ読み込みの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-648">Fixed assembly loading issue that caused some cmdlets to fail when executing in the following modules:</span></span>
  - <span data-ttu-id="8e20c-649">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8e20c-649">AzureRM.ApiManagement</span></span>
  - <span data-ttu-id="8e20c-650">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="8e20c-650">AzureRM.Backup</span></span>
  - <span data-ttu-id="8e20c-651">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="8e20c-651">AzureRM.Batch</span></span>
  - <span data-ttu-id="8e20c-652">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-652">AzureRM.Compute</span></span>
  - <span data-ttu-id="8e20c-653">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="8e20c-653">AzureRM.DataFactories</span></span>
  - <span data-ttu-id="8e20c-654">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8e20c-654">AzureRM.HDInsight</span></span>
  - <span data-ttu-id="8e20c-655">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8e20c-655">AzureRM.KeyVault</span></span>
  - <span data-ttu-id="8e20c-656">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-656">AzureRM.RecoveryServices</span></span>
  - <span data-ttu-id="8e20c-657">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8e20c-657">AzureRM.RecoveryServices.Backup</span></span>
  - <span data-ttu-id="8e20c-658">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-658">AzureRM.RecoveryServices.SiteRecovery</span></span>
  - <span data-ttu-id="8e20c-659">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8e20c-659">AzureRM.RedisCache</span></span>
  - <span data-ttu-id="8e20c-660">AzureRM.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-660">AzureRM.SiteRecovery</span></span>
  - <span data-ttu-id="8e20c-661">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="8e20c-661">AzureRM.Sql</span></span>
  - <span data-ttu-id="8e20c-662">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-662">AzureRM.Storage</span></span>
  - <span data-ttu-id="8e20c-663">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="8e20c-663">AzureRM.StreamAnalytics</span></span>

## <a name="2017118---version-500"></a><span data-ttu-id="8e20c-664">2017.11.8 - バージョン 5.0.0</span><span class="sxs-lookup"><span data-stu-id="8e20c-664">2017.11.8 - Version 5.0.0</span></span>
* <span data-ttu-id="8e20c-665">注:これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="8e20c-665">NOTE: This is a breaking change release.</span></span> <span data-ttu-id="8e20c-666">導入された重大な変更の完全な一覧については、移行ガイド (https://aka.ms/azps-migration-guide)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e20c-666">Please see the migration guide (https://aka.ms/azps-migration-guide) for a full list of introduced breaking changes.</span></span>
* <span data-ttu-id="8e20c-667">AzureRM のコマンドレットはすべて、オンライン ヘルプをサポートするようになりました</span><span class="sxs-lookup"><span data-stu-id="8e20c-667">All cmdlets in AzureRM now support online help</span></span>
  - <span data-ttu-id="8e20c-668">-Online パラメーターを指定して Get-Help を実行すると、既定のインターネット ブラウザーでオンライン ヘルプが表示されます</span><span class="sxs-lookup"><span data-stu-id="8e20c-668">Run Get-Help with the -Online parameter to open the online help in your default Internet browser</span></span>
* <span data-ttu-id="8e20c-669">AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8e20c-669">AnalysisServices</span></span>
  * <span data-ttu-id="8e20c-670">同期のために新しい AsAzure REST API と連携するように Synchronize-AzureAsInstance コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-670">Fixed Synchronize-AzureAsInstance command to work with new AsAzure REST API for sync</span></span>
* <span data-ttu-id="8e20c-671">ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8e20c-671">ApiManagement</span></span>
  * <span data-ttu-id="8e20c-672">ApiManagement の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-672">Please see the migration guide for breaking changes made to ApiManagement this release</span></span>
  * <span data-ttu-id="8e20c-673">問題 (https://github.com/Azure/azure-powershell/issues/4510) を修正するために Get-AzureRmApiManagementUser コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-673">Updated Cmdlet Get-AzureRmApiManagementUser to fix issue https://github.com/Azure/azure-powershell/issues/4510</span></span>
  * <span data-ttu-id="8e20c-674">空のパスを持つ API (https://github.com/Azure/azure-powershell/issues/4069) を作成するために、New-AzureRmApiManagementApi コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-674">Updated Cmdlet New-AzureRmApiManagementApi to create Api with Empty Path https://github.com/Azure/azure-powershell/issues/4069</span></span>
* <span data-ttu-id="8e20c-675">ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-675">ApplicationInsights</span></span>
  * <span data-ttu-id="8e20c-676">Application Insights のリソースを取得/作成/削除するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-676">Add commands to get/create/remove applicaiton insights resource</span></span>
    - <span data-ttu-id="8e20c-677">Get-AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-677">Get-AzureRmApplicationInsights</span></span>
    - <span data-ttu-id="8e20c-678">New-AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-678">New-AzureRmApplicationInsights</span></span>
    - <span data-ttu-id="8e20c-679">Remove-AzureRmApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8e20c-679">Remove-AzureRmApplicationInsights</span></span>
  * <span data-ttu-id="8e20c-680">Application Insights のリソースの価格/日次上限を取得/更新するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-680">Add commands to get/update pricing/daily cap of applicaiton insights resource</span></span>
    - <span data-ttu-id="8e20c-681">Get-AzureRmApplicationInsights -IncludeDailyCap</span><span class="sxs-lookup"><span data-stu-id="8e20c-681">Get-AzureRmApplicationInsights -IncludeDailyCap</span></span>
    - <span data-ttu-id="8e20c-682">Set-AzureRmApplicationInsightsPricingPlan</span><span class="sxs-lookup"><span data-stu-id="8e20c-682">Set-AzureRmApplicationInsightsPricingPlan</span></span>
    - <span data-ttu-id="8e20c-683">Set-AzureRmApplicationInsightsDailyCap</span><span class="sxs-lookup"><span data-stu-id="8e20c-683">Set-AzureRmApplicationInsightsDailyCap</span></span>
  * <span data-ttu-id="8e20c-684">Application Insights のリソースの連続エクスポートを取得/作成/更新/削除するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-684">Add commands to get/create/update/remove continuous export of applicaiton insights resource</span></span>
    - <span data-ttu-id="8e20c-685">Get-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="8e20c-685">Get-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="8e20c-686">Set-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="8e20c-686">Set-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="8e20c-687">New-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="8e20c-687">New-AzureRmApplicationInsightsContinuousExport</span></span>
    - <span data-ttu-id="8e20c-688">Remove-AzureRmApplicationInsightsContinuousExport</span><span class="sxs-lookup"><span data-stu-id="8e20c-688">Remove-AzureRmApplicationInsightsContinuousExport</span></span>
  * <span data-ttu-id="8e20c-689">Application Insights のリソースの API キーを取得/作成/削除するコマンドを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-689">Add commands to get/create/remove api keys of applicaiton insights resoruce</span></span>
    - <span data-ttu-id="8e20c-690">Get-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="8e20c-690">Get-AzureRmApplicationInsightsApiKey</span></span>
    - <span data-ttu-id="8e20c-691">New-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="8e20c-691">New-AzureRmApplicationInsightsApiKey</span></span>
    - <span data-ttu-id="8e20c-692">Remove-AzureRmApplicationInsightsApiKey</span><span class="sxs-lookup"><span data-stu-id="8e20c-692">Remove-AzureRmApplicationInsightsApiKey</span></span>
* <span data-ttu-id="8e20c-693">AzureBatch</span><span class="sxs-lookup"><span data-stu-id="8e20c-693">AzureBatch</span></span>
  * <span data-ttu-id="8e20c-694">新しいパラメーターを `New-AzureRmBatchAccount` に追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-694">Added new parameters to `New-AzureRmBatchAccount`.</span></span>
    - <span data-ttu-id="8e20c-695">`PoolAllocationMode`:Batch アカウントでプールを作成するために使用する割り当てモード。</span><span class="sxs-lookup"><span data-stu-id="8e20c-695">`PoolAllocationMode`: The allocation mode to use for creating pools in the Batch account.</span></span> <span data-ttu-id="8e20c-696">ユーザーのサブスクリプションにプール ノードを割り当てる Batch アカウントを作成するには、これを `UserSubscription` に設定します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-696">To create a Batch account which allocates pool nodes in the user's subscription, set this to `UserSubscription`.</span></span>
    - <span data-ttu-id="8e20c-697">`KeyVaultId`:Batch アカウントに関連付けられている Azure キー コンテナーのリソース ID。</span><span class="sxs-lookup"><span data-stu-id="8e20c-697">`KeyVaultId`: The resource ID of the Azure key vault associated with the Batch account.</span></span>
    - <span data-ttu-id="8e20c-698">`KeyVaultUrl`:Batch アカウントに関連付けられている Azure キー コンテナーの URL。</span><span class="sxs-lookup"><span data-stu-id="8e20c-698">`KeyVaultUrl`: The URL of the Azure key vault associated with the Batch account.</span></span>
  * <span data-ttu-id="8e20c-699">`New-AzureBatchTask` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-699">Updated parameters to `New-AzureBatchTask`.</span></span>
    - <span data-ttu-id="8e20c-700">`RunElevated` スイッチを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-700">Removed the `RunElevated` switch.</span></span> <span data-ttu-id="8e20c-701">`RunElevated` の代わりに `UserIdentity` パラメーターを追加しました。以下のように `PSUserIdentity` を作成することにより同じ動作を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-701">The `UserIdentity` parameter has been added to replace `RunElevated`, and the equivalent behavior can be achieved by constructing a `PSUserIdentity` as shown below:</span></span>
      - <span data-ttu-id="8e20c-702">$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")</span><span class="sxs-lookup"><span data-stu-id="8e20c-702">$autoUser = New-Object Microsoft.Azure.Commands.Batch.Models.PSAutoUserSpecification -ArgumentList @("Task", "Admin")</span></span>
      - <span data-ttu-id="8e20c-703">$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser</span><span class="sxs-lookup"><span data-stu-id="8e20c-703">$userIdentity = New-Object Microsoft.Azure.Commands.Batch.Models.PSUserIdentity $autoUser</span></span>
    - <span data-ttu-id="8e20c-704">`AuthenticationTokenSettings` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-704">Added the `AuthenticationTokenSettings` parameter.</span></span> <span data-ttu-id="8e20c-705">このパラメーターを使用すると、タスクの実行時に認証トークンを提供するようバッチ サービスに要求でき、バッチ サービスに要求を出すためにバッチ アカウント キーをタスクに渡す必要がなくなります。</span><span class="sxs-lookup"><span data-stu-id="8e20c-705">This parameter allows you to request the Batch service provide an authentication token to the task when it runs, avoiding the need to pass Batch account keys to the task in order to issue requests to the Batch service.</span></span>
    - <span data-ttu-id="8e20c-706">`ContainerSettings` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-706">Added the `ContainerSettings` parameter.</span></span>
      - <span data-ttu-id="8e20c-707">このパラメーターを使用すると、コンテナー内部でタスクを実行するよう Batch サービスに要求できます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-707">This parameter allows you to request the Batch service run the task inside a container.</span></span>
    - <span data-ttu-id="8e20c-708">`OutputFiles` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-708">Added the `OutputFiles` parameter.</span></span>
      - <span data-ttu-id="8e20c-709">このパラメーターを使用すると、タスクの終了後に Azure Storage にファイルをアップロードするようにタスクを構成できます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-709">This parameter allows you to configure the task to upload files to Azure Storage after it has finished.</span></span>
  * <span data-ttu-id="8e20c-710">`New-AzureBatchPool` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-710">Updated parameters to `New-AzureBatchPool`.</span></span>
    - <span data-ttu-id="8e20c-711">`UserAccounts` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-711">Added the `UserAccounts` parameter.</span></span>
      - <span data-ttu-id="8e20c-712">このパラメーターは、プール内の各ノードで作成されたユーザー アカウントを定義します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-712">This parameter defines user accounts created on each node in the pool.</span></span>
    - <span data-ttu-id="8e20c-713">`TargetLowPriorityComputeNodes` を追加し、`TargetDedicated` を `TargetDedicatedComputeNodes` に名前変更しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-713">Added `TargetLowPriorityComputeNodes` and renamed `TargetDedicated` to `TargetDedicatedComputeNodes`.</span></span>
      - <span data-ttu-id="8e20c-714">`TargetDedicatedComputeNodes` パラメーター用に `TargetDedicated` の別名を作成しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-714">A `TargetDedicated` alias was created for the `TargetDedicatedComputeNodes` parameter.</span></span>
    - <span data-ttu-id="8e20c-715">`NetworkConfiguration` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-715">Added the `NetworkConfiguration` parameter.</span></span>
      - <span data-ttu-id="8e20c-716">このパラメーターを使用すると、プールのネットワーク設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-716">This parameter allows you to configure the pools network settings.</span></span>
  * <span data-ttu-id="8e20c-717">`New-AzureBatchCertificate` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-717">Updated parameters to `New-AzureBatchCertificate`.</span></span>
    - <span data-ttu-id="8e20c-718">`Password` パラメーターが `SecureString` になりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-718">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="8e20c-719">`New-AzureBatchComputeNodeUser` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-719">Updated parameters to `New-AzureBatchComputeNodeUser`.</span></span>
    - <span data-ttu-id="8e20c-720">`Password` パラメーターが `SecureString` になりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-720">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="8e20c-721">`Set-AzureBatchComputeNodeUser` のパラメーターを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-721">Updated parameters to `Set-AzureBatchComputeNodeUser`.</span></span>
    - <span data-ttu-id="8e20c-722">`Password` パラメーターが `SecureString` になりました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-722">The `Password` parameter is now a `SecureString`.</span></span>
  * <span data-ttu-id="8e20c-723">`Get-AzureBatchNodeFile`、`Get-AzureBatchNodeFileContent`、および `Remove-AzureBatchNodeFile` で、`Name` パラメーターを `Path` に名前変更しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-723">Renamed the `Name` parameter to `Path` on `Get-AzureBatchNodeFile`, `Get-AzureBatchNodeFileContent`, and `Remove-AzureBatchNodeFile`.</span></span>
    - <span data-ttu-id="8e20c-724">`Path` パラメーター用に `Name` の別名を作成しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-724">A `Name` alias was created for the `Path` parameter.</span></span>
  * <span data-ttu-id="8e20c-725">オブジェクトに対する変更</span><span class="sxs-lookup"><span data-stu-id="8e20c-725">Changes to objects</span></span>
    - <span data-ttu-id="8e20c-726">完全なリストについては、Batch 変更ログを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-726">Please see the Batch change log for the full list</span></span>
  * <span data-ttu-id="8e20c-727">Azure Active Directory ベースの認証のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-727">Added support for Azure Active Directory based authentication.</span></span>
    - <span data-ttu-id="8e20c-728">Azure Active Directory 認証を使用するには、`Get-AzureRmBatchAccount` コマンドレットを使用して `BatchAccountContext` オブジェクトを取得し、この `BatchAccountContext` を Batch サービス コマンドレットの `-BatchContext` パラメーターに指定します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-728">To use Azure Active Directory authentication, retrieve a `BatchAccountContext` object using the `Get-AzureRmBatchAccount` cmdlet, and supply this `BatchAccountContext` to the `-BatchContext` parameter of a Batch service cmdlet.</span></span> <span data-ttu-id="8e20c-729">Azure Active Directory 認証は、`PoolAllocationMode = UserSubscription` のアカウントには必須です。</span><span class="sxs-lookup"><span data-stu-id="8e20c-729">Azure Active Directory authentication is mandatory for accounts with `PoolAllocationMode = UserSubscription`.</span></span>
    - <span data-ttu-id="8e20c-730">既存のアカウント、または `PoolAllocationMode = BatchService` で作成された新しいアカウントの場合、`Get-AzureRmBatchAccoutKeys` コマンドレットを使用して `BatchAccountContext` オブジェクトを取得することにより、共有キー認証の使用を継続できます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-730">For existing accounts or for new accounts created with `PoolAllocationMode = BatchService`, you may continue to use shared key authentication by retrieving a `BatchAccountContext` object using the `Get-AzureRmBatchAccoutKeys` cmdlet.</span></span>
* <span data-ttu-id="8e20c-731">Compute</span><span class="sxs-lookup"><span data-stu-id="8e20c-731">Compute</span></span>
  * <span data-ttu-id="8e20c-732">Azure Disk Encryption 拡張コマンド</span><span class="sxs-lookup"><span data-stu-id="8e20c-732">Azure Disk Encryption Extension Commands</span></span>
    - <span data-ttu-id="8e20c-733">"Set-AzureRmVmDiskEncryptionExtension" の新しいパラメーター: "-EncryptFormatAll" はデータ ディスクを暗号化フォーマットします</span><span class="sxs-lookup"><span data-stu-id="8e20c-733">New Parameter for 'Set-AzureRmVmDiskEncryptionExtension': '-EncryptFormatAll' encrypt formats data disks</span></span>
    - <span data-ttu-id="8e20c-734">"Set-AzureRmVmDiskEncryptionExtension" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます</span><span class="sxs-lookup"><span data-stu-id="8e20c-734">New Parameters for 'Set-AzureRmVmDiskEncryptionExtension': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
    - <span data-ttu-id="8e20c-735">"Disable-AzureRmVmDiskEncryption" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます</span><span class="sxs-lookup"><span data-stu-id="8e20c-735">New Parameters for 'Disable-AzureRmVmDiskEncryption': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
    - <span data-ttu-id="8e20c-736">"Get-AzureRmVmDiskEncryptionStatus" の新しいパラメーター: "-ExtensionPublisherName" および "-ExtensionType" は拡張機能の他のバージョンに切り替えることができます</span><span class="sxs-lookup"><span data-stu-id="8e20c-736">New Parameters for 'Get-AzureRmVmDiskEncryptionStatus': '-ExtensionPublisherName' and '-ExtensionType' allow switching to other versions of the extension</span></span>
* <span data-ttu-id="8e20c-737">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8e20c-737">DataLakeAnalytics</span></span>
  * <span data-ttu-id="8e20c-738">DataLakeAnalytics の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-738">Please see the migration guide for breaking changes made to DataLakeAnalytics this release</span></span>
  * <span data-ttu-id="8e20c-739">Get-AzureRmDataLakeAnalyticsAccount の 2 つの OutputTypes の 1 つを変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-739">Changed one of the two OutputTypes of Get-AzureRmDataLakeAnalyticsAccount</span></span>
    - <span data-ttu-id="8e20c-740">List\<DataLakeAnalyticsAccount> から List\<PSDataLakeAnalyticsAccountBasic></span><span class="sxs-lookup"><span data-stu-id="8e20c-740">List\<DataLakeAnalyticsAccount> to List\<PSDataLakeAnalyticsAccountBasic></span></span>
    - <span data-ttu-id="8e20c-741">PSDataLakeAnalyticsAccountBasic のプロパティは DataLakeAnalyticsAccount のプロパティの厳密なサブセットです</span><span class="sxs-lookup"><span data-stu-id="8e20c-741">The properties of PSDataLakeAnalyticsAccountBasic is a strict subset of the properties of DataLakeAnalyticsAccount</span></span>
    - <span data-ttu-id="8e20c-742">DataLakeAnalyticsAccount にある追加プロパティはサービスによって返されません。</span><span class="sxs-lookup"><span data-stu-id="8e20c-742">The additional properties that are in DataLakeAnalyticsAccount are not returned by the service.</span></span>  <span data-ttu-id="8e20c-743">そのため、この変更はこれを正確に反映するためのものです。</span><span class="sxs-lookup"><span data-stu-id="8e20c-743">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="8e20c-744">これらの追加プロパティは引き続き PSDataLakeAnalyticsAccountBasic にありますが、これらには廃止のタグが付けられます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-744">These additional properties are still in PSDataLakeAnalyticsAccountBasic, but they are tagged as Obsolete.</span></span>
  * <span data-ttu-id="8e20c-745">Get-AzureRmDataLakeAnalyticsJob の 2 つの OutputTypes の 1 つを変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-745">Changed one of the two OutputTypes of Get-AzureRmDataLakeAnalyticsJob</span></span>
    - <span data-ttu-id="8e20c-746">List\<JobInformation> から List\<PSJobInformationBasic></span><span class="sxs-lookup"><span data-stu-id="8e20c-746">List\<JobInformation> to List\<PSJobInformationBasic></span></span>
    - <span data-ttu-id="8e20c-747">PSJobInformationBasic のプロパティは JobInformation のプロパティの厳密なサブセットです</span><span class="sxs-lookup"><span data-stu-id="8e20c-747">The properties of PSJobInformationBasic is a strict subset of the properties of JobInformation</span></span>
    - <span data-ttu-id="8e20c-748">JobInformation にある追加プロパティはサービスによって返されません。</span><span class="sxs-lookup"><span data-stu-id="8e20c-748">The additional properties that are in JobInformation are not returned by the service.</span></span>  <span data-ttu-id="8e20c-749">そのため、この変更はこれを正確に反映するためのものです。</span><span class="sxs-lookup"><span data-stu-id="8e20c-749">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="8e20c-750">これらの追加プロパティは引き続き PSJobInformationBasic にありますが、これらには廃止のタグが付けられます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-750">These additional properties are still in PSJobInformationBasic, but they are tagged as Obsolete.</span></span>
* <span data-ttu-id="8e20c-751">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8e20c-751">DataLakeStore</span></span>
  * <span data-ttu-id="8e20c-752">DataLakeStore の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-752">Please see the migration guide for breaking changes made to DataLakeStore this release</span></span>
  * <span data-ttu-id="8e20c-753">Get-AzureRmDataLakeStoreAccount の 2 つの OutputTypes の 1 つを変更しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-753">Changed one of the two OutputTypes of Get-AzureRmDataLakeStoreAccount</span></span>
    - <span data-ttu-id="8e20c-754">List\<PSDataLakeStoreAccount> から List\<PSDataLakeStoreAccountBasic></span><span class="sxs-lookup"><span data-stu-id="8e20c-754">List\<PSDataLakeStoreAccount> to List\<PSDataLakeStoreAccountBasic></span></span>
    - <span data-ttu-id="8e20c-755">PSDataLakeStoreAccountBasic のプロパティは PSDataLakeStoreAccount のプロパティの厳密なサブセットです</span><span class="sxs-lookup"><span data-stu-id="8e20c-755">The properties of PSDataLakeStoreAccountBasic is a strict subset of the properties of PSDataLakeStoreAccount</span></span>
    - <span data-ttu-id="8e20c-756">PSDataLakeStoreAccount にある追加プロパティはサービスによって返されません。</span><span class="sxs-lookup"><span data-stu-id="8e20c-756">The additional properties that are in PSDataLakeStoreAccount are not returned by the service.</span></span>  <span data-ttu-id="8e20c-757">そのため、この変更はこれを正確に反映するためのものです。</span><span class="sxs-lookup"><span data-stu-id="8e20c-757">Therefore, this change is to reflect this accurately.</span></span> <span data-ttu-id="8e20c-758">これらの追加プロパティは引き続き PSDataLakeStoreAccountBasic にありますが、これらには廃止のタグが付けられます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-758">These additional properties are still in PSDataLakeStoreAccountBasic, but they are tagged as Obsolete.</span></span>
* <span data-ttu-id="8e20c-759">DNS</span><span class="sxs-lookup"><span data-stu-id="8e20c-759">Dns</span></span>
  * <span data-ttu-id="8e20c-760">Azure DNS での CAA レコードの種類のサポート</span><span class="sxs-lookup"><span data-stu-id="8e20c-760">Support for CAA record types in Azure DNS</span></span>
    - <span data-ttu-id="8e20c-761">CAA レコードの種類に対するすべての操作をサポートします</span><span class="sxs-lookup"><span data-stu-id="8e20c-761">Supports all operations on CAA record type</span></span>
* <span data-ttu-id="8e20c-762">EventHub</span><span class="sxs-lookup"><span data-stu-id="8e20c-762">EventHub</span></span>
  * <span data-ttu-id="8e20c-763">EventHub の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-763">Please see the migration guide for breaking changes made to EventHub this release</span></span>
* <span data-ttu-id="8e20c-764">洞察</span><span class="sxs-lookup"><span data-stu-id="8e20c-764">Insights</span></span>
  * <span data-ttu-id="8e20c-765">Insights の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-765">Please see the migration guide for breaking changes made to Insights this release</span></span>
* <span data-ttu-id="8e20c-766">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="8e20c-766">Network</span></span>
  * <span data-ttu-id="8e20c-767">Network の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-767">Please see the migration guide for breaking changes made to Network this release</span></span>
  * <span data-ttu-id="8e20c-768">指定された Azure リージョンで使用可能なインターネット サービス プロバイダーを一覧表示するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-768">Added cmdlet to list available internet service providers for a specified Azure region</span></span>
    - <span data-ttu-id="8e20c-769">Get-AzureRmNetworkWatcherReachabilityProvidersList</span><span class="sxs-lookup"><span data-stu-id="8e20c-769">Get-AzureRmNetworkWatcherReachabilityProvidersList</span></span>
  * <span data-ttu-id="8e20c-770">指定された場所から Azure リージョンまでのインターネット サービス プロバイダーの相対待機時間スコアを取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-770">Added cmdlet to get the relative latency score for internet service providers from a specified location to Azure regions</span></span>
    - <span data-ttu-id="8e20c-771">Get-AzureRmNetworkWatcherReachabilityReport</span><span class="sxs-lookup"><span data-stu-id="8e20c-771">Get-AzureRmNetworkWatcherReachabilityReport</span></span>
* <span data-ttu-id="8e20c-772">プロファイル</span><span class="sxs-lookup"><span data-stu-id="8e20c-772">Profile</span></span>
  - <span data-ttu-id="8e20c-773">Set-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="8e20c-773">Set-AzureRmDefault</span></span>
    - <span data-ttu-id="8e20c-774">このコマンドレットを使用して、既定のリソース グループを設定します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-774">Use this cmdlet to set a default resource group.</span></span>  <span data-ttu-id="8e20c-775">これにより、-ResourceGroup パラメーターが一部のコマンドレットで省略可能になり、リソース グループを指定しない場合に既定値が使用されます</span><span class="sxs-lookup"><span data-stu-id="8e20c-775">This will make the -ResourceGroup parameter optional for some cmdlets, and will use the default when a resource group is not specified</span></span>
    - ```Set-AzureRmDefault -ResourceGroupName "ExampleResourceGroup"```
    - <span data-ttu-id="8e20c-776">指定したリソース グループがサブスクリプションに存在する場合は、このリソース グループが既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-776">If resource group specified exists in the subscription, this resource group will be set to default.</span></span>  <span data-ttu-id="8e20c-777">それ以外の場合、リソース グループが作成され、既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-777">Otherwise, the resource group will be created and then set to default.</span></span>
  - <span data-ttu-id="8e20c-778">Get-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="8e20c-778">Get-AzureRmDefault</span></span>
    - <span data-ttu-id="8e20c-779">このコマンドレットを使用して、現在の既定のリソース グループ (および今後はその他の既定値) を取得します。</span><span class="sxs-lookup"><span data-stu-id="8e20c-779">Use this cmdlet to get the current default resource group (and other defaults in the future).</span></span>
    - ```Get-AzureRmDefault -ResourceGroup```
  - <span data-ttu-id="8e20c-780">Clear-AzureRmDefault</span><span class="sxs-lookup"><span data-stu-id="8e20c-780">Clear-AzureRmDefault</span></span>
    - <span data-ttu-id="8e20c-781">このコマンドレットを使用して、現在の既定のリソース グループを削除します</span><span class="sxs-lookup"><span data-stu-id="8e20c-781">Use this cmdlet to remove the current default resource group</span></span>
    - ```Clear-AzureRmDefault -ResourceGroup```
  - <span data-ttu-id="8e20c-782">Add-AzureRmEnvironment および Set-AzureRmEnvironment</span><span class="sxs-lookup"><span data-stu-id="8e20c-782">Add-AzureRmEnvironment and Set-AzureRmEnvironment</span></span>
    - <span data-ttu-id="8e20c-783">BatchAudience パラメーターを追加します。これにより、Batch サービスの認証トークンを取得する際に使用する Azure Batch Active Directory オーディエンスを指定できます。</span><span class="sxs-lookup"><span data-stu-id="8e20c-783">Add the BatchAudience parameter, which allows you to specify the Azure Batch Active Directory audience to use when acquiring authentication tokens for the Batch service.</span></span>
* <span data-ttu-id="8e20c-784">RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8e20c-784">RecoveryServices.Backup</span></span>
  * <span data-ttu-id="8e20c-785">インスタント ファイル回復を実行するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-785">Added cmdlets to perform instant file recovery.</span></span>
    - <span data-ttu-id="8e20c-786">Get-AzureRmRecoveryServicesBackupRPMountScript</span><span class="sxs-lookup"><span data-stu-id="8e20c-786">Get-AzureRmRecoveryServicesBackupRPMountScript</span></span>
    - <span data-ttu-id="8e20c-787">Disable-AzureRmRecoveryServicesBackupRPMountScript</span><span class="sxs-lookup"><span data-stu-id="8e20c-787">Disable-AzureRmRecoveryServicesBackupRPMountScript</span></span>
  * <span data-ttu-id="8e20c-788">RecoveryServices.Backup SDK を最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-788">Updated RecoveryServices.Backup SDK version to the latest</span></span>
  * <span data-ttu-id="8e20c-789">テスト実行に必要なすべての設定がテスト自体で行われるように、Azure VM ワークロードのテストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8e20c-789">Updated tests for the Azure VM workload so that, all setups needed for test runs are done by the tests themselves.</span></span>
  * <span data-ttu-id="8e20c-790">[https://github.com/Azure/azure-powershell/issues/3164](https://github.com/Azure/azure-powershell/issues/3164) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-790">Fixes https://github.com/Azure/azure-powershell/issues/3164</span></span>
* <span data-ttu-id="8e20c-791">RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8e20c-791">RecoveryServices.SiteRecovery</span></span>
  * <span data-ttu-id="8e20c-792">Azure Site Recovery に対する ASR VMware の変更 (コマンドレットは現在、Enterprise から Enterprise、Enterprise から Azure、HyperV から Azure の操作をサポートしています)</span><span class="sxs-lookup"><span data-stu-id="8e20c-792">Changes for ASR VMware to Azure Site Recovery (cmdlets are currently supporting operations for Enterprise to Enterprise, Enterprise to Azure, HyperV to Azure)</span></span>
    - <span data-ttu-id="8e20c-793">New-AzureRmRecoveryServicesAsrPolicy</span><span class="sxs-lookup"><span data-stu-id="8e20c-793">New-AzureRmRecoveryServicesAsrPolicy</span></span>
    - <span data-ttu-id="8e20c-794">New-AzureRmRecoveryServicesAsrProtectedItem</span><span class="sxs-lookup"><span data-stu-id="8e20c-794">New-AzureRmRecoveryServicesAsrProtectedItem</span></span>
    - <span data-ttu-id="8e20c-795">Update-AzureRmRecoveryServicesAsrPolicy</span><span class="sxs-lookup"><span data-stu-id="8e20c-795">Update-AzureRmRecoveryServicesAsrPolicy</span></span>
    - <span data-ttu-id="8e20c-796">Update-AzureRmRecoveryServicesAsrProtectionDirection</span><span class="sxs-lookup"><span data-stu-id="8e20c-796">Update-AzureRmRecoveryServicesAsrProtectionDirection</span></span>
  * <span data-ttu-id="8e20c-797">AAD ベースのコンテナーにサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-797">Added support to AAD-based vault</span></span>
  * <span data-ttu-id="8e20c-798">VCenter リソースを管理するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-798">Added cmdlets to manage VCenter resources</span></span>
    - <span data-ttu-id="8e20c-799">Get-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="8e20c-799">Get-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="8e20c-800">New-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="8e20c-800">New-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="8e20c-801">Remove-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="8e20c-801">Remove-AzureRmRecoveryServicesAsrVCenter</span></span>
    - <span data-ttu-id="8e20c-802">Update-AzureRmRecoveryServicesAsrVCenter</span><span class="sxs-lookup"><span data-stu-id="8e20c-802">Update-AzureRmRecoveryServicesAsrVCenter</span></span>
  * <span data-ttu-id="8e20c-803">その他のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8e20c-803">Added other cmdlets</span></span>
    - <span data-ttu-id="8e20c-804">Get-AzureRmRecoveryServicesAsrAlertSetting</span><span class="sxs-lookup"><span data-stu-id="8e20c-804">Get-AzureRmRecoveryServicesAsrAlertSetting</span></span>
    - <span data-ttu-id="8e20c-805">Get-AzureRmRecoveryServicesAsrEvent</span><span class="sxs-lookup"><span data-stu-id="8e20c-805">Get-AzureRmRecoveryServicesAsrEvent</span></span>
    - <span data-ttu-id="8e20c-806">New-AzureRmRecoveryServicesAsrProtectableItem</span><span class="sxs-lookup"><span data-stu-id="8e20c-806">New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
    - <span data-ttu-id="8e20c-807">Set-AzureRmRecoveryServicesAsrAlertSetting</span><span class="sxs-lookup"><span data-stu-id="8e20c-807">Set-AzureRmRecoveryServicesAsrAlertSetting</span></span>
    - <span data-ttu-id="8e20c-808">Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob</span><span class="sxs-lookup"><span data-stu-id="8e20c-808">Start-AzureRmRecoveryServicesAsrResynchronizeReplicationJob</span></span>
    - <span data-ttu-id="8e20c-809">Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob</span><span class="sxs-lookup"><span data-stu-id="8e20c-809">Start-AzureRmRecoveryServicesAsrSwitchProcessServerJob</span></span>
    - <span data-ttu-id="8e20c-810">Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob</span><span class="sxs-lookup"><span data-stu-id="8e20c-810">Start-AzureRmRecoveryServicesAsrTestFailoverCleanupJob</span></span>
    - <span data-ttu-id="8e20c-811">Update-AzureRmRecoveryServicesAsrMobilityService</span><span class="sxs-lookup"><span data-stu-id="8e20c-811">Update-AzureRmRecoveryServicesAsrMobilityService</span></span>
* <span data-ttu-id="8e20c-812">ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8e20c-812">ServiceBus</span></span>
  - <span data-ttu-id="8e20c-813">ServiceBus の、このリリースでの重大な変更については、移行ガイドを参照してください</span><span class="sxs-lookup"><span data-stu-id="8e20c-813">Please see the migration guide for breaking changes made to ServiceBus this release</span></span>
* <span data-ttu-id="8e20c-814">SQL</span><span class="sxs-lookup"><span data-stu-id="8e20c-814">Sql</span></span>
  * <span data-ttu-id="8e20c-815">データベースに対する非同期 updateslo 操作の一覧表示およびキャンセルのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-815">Adding support for list and cancel the asynchronous updateslo operation on the database</span></span>
    - <span data-ttu-id="8e20c-816">DB updateslo 操作状態を返すように既存の Get-AzureRmSqlDatabaseActivity コマンドレットを更新。</span><span class="sxs-lookup"><span data-stu-id="8e20c-816">update existing cmdlet Get-AzureRmSqlDatabaseActivity to return DB updateslo operation status.</span></span>
    - <span data-ttu-id="8e20c-817">データベースに対する非同期 updateslo 操作をキャンセルする新しい Stop-AzureRmSqlDatabaseActivity コマンドレットを追加。</span><span class="sxs-lookup"><span data-stu-id="8e20c-817">add new cmdlet Stop-AzureRmSqlDatabaseActivity for cancel the asynchronous updateslo operation on the database.</span></span>
  * <span data-ttu-id="8e20c-818">データベースとエラスティック プールのゾーン冗長性に対するサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-818">Adding support for Zone Redundancy for databases and elastic pools</span></span>
    - <span data-ttu-id="8e20c-819">ZoneRedundant スイッチ パラメーターを New-AzureRmSqlDatabase に追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-819">Adding ZoneRedundant switch parameter to New-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="8e20c-820">ZoneRedundant スイッチ パラメーターを Set-AzureRmSqlDatabase に追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-820">Adding ZoneRedundant switch parameter to Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="8e20c-821">ZoneRedundant スイッチ パラメーターを New-AzureRmSqlElasticPool に追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-821">Adding ZoneRedundant switch parameter to New-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="8e20c-822">ZoneRedundant スイッチ パラメーターを Set-AzureRmSqlElasticPool に追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-822">Adding ZoneRedundant switch parameter to Set-AzureRmSqlElasticPool</span></span>
  * <span data-ttu-id="8e20c-823">サーバー DNS エイリアスに対するサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-823">Adding support for Server DNS Aliases</span></span>
    - <span data-ttu-id="8e20c-824">サーバーとエイリアス名ごとにサーバー DNS エイリアスを取得するか、Azure SQL Server のサーバー DNS エイリアスの一覧を取得する、Get-AzureRmSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-824">Adding Get-AzureRmSqlServerDnsAlias cmdlet which gets server dns aliases by server and alias name or a list of server dns aliases for an azure Sql Server.</span></span>
    - <span data-ttu-id="8e20c-825">指定の Azure SQL Server の新しいサーバー DNS エイリアスを作成する、New-AzureRmSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-825">Adding New-AzureRmSqlServerDnsAlias cmdlet which creates new server dns alias for a given Azure Sql server</span></span>
    - <span data-ttu-id="8e20c-826">サーバー DNS エイリアスが指す Azure SQL Server を更新できる、Set-AzurermSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-826">Adding Set-AzurermSqlServerDnsAlias cmlet which allows updating a Azure Sql Server to which server dns alias is pointing</span></span>
    - <span data-ttu-id="8e20c-827">Azure SQL Server のサーバー DNS エイリアスを削除する、Remove-AzureRmSqlServerDnsAlias コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-827">Adding Remove-AzureRmSqlServerDnsAlias cmdlet which removes a server dns alias for a Azure Sql Server</span></span>
* <span data-ttu-id="8e20c-828">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8e20c-828">Azure.Storage</span></span>
  * <span data-ttu-id="8e20c-829">Azure Storage Client Library 8.5.0 および Azure Storage DataMovement Library 0.6.3 へのアップグレード</span><span class="sxs-lookup"><span data-stu-id="8e20c-829">Upgrade to Azure Storage Client Library 8.5.0 and Azure Storage DataMovement Library 0.6.3</span></span>
  * <span data-ttu-id="8e20c-830">ファイル共有スナップショット サポート機能を追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-830">Add File Share Snapshot Support Feature</span></span>
    - <span data-ttu-id="8e20c-831">"SnapshotTime" パラメーターを Get-AzureStorageShare に追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-831">Add 'SnapshotTime' parameter to Get-AzureStorageShare</span></span>
    - <span data-ttu-id="8e20c-832">"IncludeAllSnapshot" パラメーターを Remove-AzureStorageShare に追加</span><span class="sxs-lookup"><span data-stu-id="8e20c-832">Add 'IncludeAllSnapshot' parameter to Remove-AzureStorageShare</span></span>
