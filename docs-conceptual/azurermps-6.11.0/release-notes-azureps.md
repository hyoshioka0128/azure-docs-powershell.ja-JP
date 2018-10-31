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
ms.openlocfilehash: eec8b5960f787fa9ca1130b4f8b49c9d896aa99e
ms.sourcegitcommit: 5f946a535eccca0b3ddf3db8f617b32564a88938
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/25/2018
ms.locfileid: "50001509"
---
# <a name="release-notes"></a><span data-ttu-id="9730a-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="9730a-103">Release notes</span></span>

<span data-ttu-id="9730a-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="9730a-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6110---october-2018"></a><span data-ttu-id="9730a-105">6.11.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="9730a-105">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9730a-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-106">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-107">CloudShell での Get-AzureRmSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-107">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="9730a-108">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-108">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="9730a-109">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="9730a-109">AzureRM.Backup</span></span>
* <span data-ttu-id="9730a-110">Azure Backup コマンドレットを非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="9730a-110">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-111">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-111">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-112">"New-AzureRmVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-112">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="9730a-113">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-113">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9730a-114">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9730a-114">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9730a-115">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-115">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="9730a-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="9730a-116">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="9730a-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="9730a-117">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="9730a-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウントの指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="9730a-118">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="9730a-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="9730a-119">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-120">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-120">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-121">プロトコル値をバックエンドに渡すように、Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-121">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="9730a-122">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-122">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-123">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-123">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-124">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzureRMRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-124">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="9730a-125">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-125">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="9730a-126">6.10.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="9730a-126">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="9730a-127">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-127">Azure.Storage</span></span>
* <span data-ttu-id="9730a-128">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-128">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="9730a-129">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="9730a-129">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="9730a-130">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="9730a-130">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="9730a-131">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9730a-131">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="9730a-132">既存のアカウントなしでの Get-AzureRmCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="9730a-132">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-133">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-133">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-134">必要に応じて 50 を超える結果が返されるように Get-AzureRmVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-134">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="9730a-135">"SimpleParameterSet" の例を New-AzureRmVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-135">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="9730a-136">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-136">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9730a-137">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9730a-137">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9730a-138">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-138">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-139">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-139">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-140">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-140">Added NetworkProfile functionality.</span></span> <span data-ttu-id="9730a-141">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="9730a-141">new cmdlets added</span></span>
    - <span data-ttu-id="9730a-142">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9730a-142">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9730a-143">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9730a-143">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9730a-144">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9730a-144">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9730a-145">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="9730a-145">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="9730a-146">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-146">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="9730a-147">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-147">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="9730a-148">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-148">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="9730a-149">New-AzureRmVirtualNetworkTap、Get-AzureRmVirtualNetworkTap、Set-AzureRmVirtualNetworkTap、Remove-AzureRmVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-149">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="9730a-150">Set-AzureRmNEtworkInterfaceTapConfig、Get-AzureRmNEtworkInterfaceTapConfig、Remove-AzureRmNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-150">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="9730a-151">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9730a-151">AzureRM.RedisCache</span></span>
* <span data-ttu-id="9730a-152">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="9730a-152">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="9730a-153">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-153">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-154">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-154">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-155">欠落していた -Mode パラメーターを Set-AzureRmPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-155">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="9730a-156">配信元にユーザーが含まれる操作について Get-AzureRmProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-156">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9730a-157">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-157">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-158">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-158">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9730a-159">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-159">AzureRM.Storage</span></span>
* <span data-ttu-id="9730a-160">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-160">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="9730a-161">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="9730a-161">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-162">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-162">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-163">新しいコマンドレット: Get-AzureRMWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="9730a-163">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="9730a-164">新しいコマンドレット: New-AzureRMWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="9730a-164">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="9730a-165">6.9.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="9730a-165">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9730a-166">全般</span><span class="sxs-lookup"><span data-stu-id="9730a-166">General</span></span>
* <span data-ttu-id="9730a-167">AzureRM.SignalR が AzureRM ロールアップ モジュールに追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-167">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9730a-168">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-168">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-169">ストレージの一般的なコードに対する軽微な変更</span><span class="sxs-lookup"><span data-stu-id="9730a-169">Minor changes to the storage common code</span></span>
* <span data-ttu-id="9730a-170">完全なパラメーター型を含めるようにヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-170">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="9730a-171">ServicePrincipalCertificateWithSubscriptionId パラメーター セットの -ServicePrincipal を "任意" に変更しました</span><span class="sxs-lookup"><span data-stu-id="9730a-171">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="9730a-172">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-172">Azure.Storage</span></span>
* <span data-ttu-id="9730a-173">OAuth でのストレージ コンテキストの作成がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="9730a-173">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="9730a-174">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="9730a-174">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="9730a-175">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="9730a-175">AzureRM.Cdn</span></span>
* <span data-ttu-id="9730a-176">CDN 価格 SKU に Standard_Microsoft を追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-176">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-177">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-177">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-178">Keyvault および Storage への依存関係を一般的な依存関係に移動しました</span><span class="sxs-lookup"><span data-stu-id="9730a-178">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="9730a-179">より多くの仮想マシンのサイズのサポートを AEM コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-179">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="9730a-180">PublicIPPrefix パラメーターを New-AzureRmVmssIpConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-180">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="9730a-181">ResourceId パラメーターを Invoke-AzureRmVMRunCommand コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-181">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="9730a-182">Invoke-AzureRmVmssVMRunCommand コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-182">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="9730a-183">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="9730a-183">AzureRM.Dns</span></span>
* <span data-ttu-id="9730a-184">DNS レコード作成中のエイリアス レコードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-184">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9730a-185">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9730a-185">AzureRM.Insights</span></span>
* <span data-ttu-id="9730a-186">#6833 および #7102 の問題を修正しました (診断設定領域)</span><span class="sxs-lookup"><span data-stu-id="9730a-186">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="9730a-187">診断設定の作成および表示/取得中の既定の名前 ("service") に関する問題</span><span class="sxs-lookup"><span data-stu-id="9730a-187">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="9730a-188">カテゴリでの診断設定の作成に関する問題</span><span class="sxs-lookup"><span data-stu-id="9730a-188">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="9730a-189">メトリック時間グレイン パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-189">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="9730a-190">Timegrains パラメーターは引き続き利用できますが (これは破壊的変更ではありません)、PT1M のみが有効であるため、バックエンドでは無視されます</span><span class="sxs-lookup"><span data-stu-id="9730a-190">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-191">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-191">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-192">LoadBalancer コマンドレットへの変更</span><span class="sxs-lookup"><span data-stu-id="9730a-192">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="9730a-193">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes パラメーター、EnableFloatingIp パラメーター、EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-193">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="9730a-194">LoadBalancerInboundNatRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-194">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="9730a-195">LoadBalancerRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-195">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="9730a-196">LoadBalancerProbeConfig: Protocol パラメーターの "HTTPS" 値のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-196">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="9730a-197">新しい LoadBalancer のサブリソース OutboundRule について新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-197">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="9730a-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-198">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9730a-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-199">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9730a-200">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-200">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9730a-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-201">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="9730a-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-202">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="9730a-203">PSNetworkInterface の新しい HostedWorkloads プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-203">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="9730a-204">ARM 経由の Azure Firewall 機能のために新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-204">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="9730a-205">Get-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-205">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="9730a-206">Set-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-206">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="9730a-207">New-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-207">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="9730a-208">Remove-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-208">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="9730a-209">New-AzureRmFirewallApplicationRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-209">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="9730a-210">New-AzureRmFirewallApplicationRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-210">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="9730a-211">New-AzureRmFirewallNatRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-211">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="9730a-212">New-AzureRmFirewallNatRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-212">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="9730a-213">New-AzureRmFirewallNetworkRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-213">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="9730a-214">New-AzureRmFirewallNetworkRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-214">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="9730a-215">Application Gateway での信頼されたルート証明書と自動スケーリング構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-215">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="9730a-216">追加された新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="9730a-216">New Cmdlets added:</span></span>
      - <span data-ttu-id="9730a-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-217">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9730a-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-218">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9730a-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-219">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9730a-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-220">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9730a-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-221">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="9730a-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-222">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="9730a-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-223">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="9730a-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-224">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="9730a-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-225">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="9730a-226">省略可能なパラメーターで更新されたコマンドレット -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-226">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="9730a-227">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9730a-227">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="9730a-228">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9730a-228">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="9730a-229">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="9730a-229">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="9730a-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="9730a-230">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="9730a-231">省略可能なパラメーターで更新されたコマンドレット - AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-231">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="9730a-232">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9730a-232">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="9730a-233">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="9730a-233">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="9730a-234">インターフェイス エンドポイントのコマンドレット Get-AzureInterfaceEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-234">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="9730a-235">サブネットでの複数のアドレス プレフィックスのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-235">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="9730a-236">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="9730a-236">Updated cmdlets:</span></span>
  - <span data-ttu-id="9730a-237">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-237">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9730a-238">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-238">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9730a-239">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-239">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9730a-240">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-240">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="9730a-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-241">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="9730a-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-242">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="9730a-243">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-243">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="9730a-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-244">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="9730a-245">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-245">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="9730a-246">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-246">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="9730a-247">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-247">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="9730a-248">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-248">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="9730a-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-249">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="9730a-250">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-250">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="9730a-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-251">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="9730a-252">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-252">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="9730a-253">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-253">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="9730a-254">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-254">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="9730a-255">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="9730a-255">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="9730a-256">サブネット委任のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-256">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="9730a-257">New-AzureRmDelegation: 新しい委任を作成します。これはサブネットに追加できます</span><span class="sxs-lookup"><span data-stu-id="9730a-257">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="9730a-258">Remove-AzureRmDelegation: サブネットを受け取り、指定された委任の名前をそのサブネットから削除します</span><span class="sxs-lookup"><span data-stu-id="9730a-258">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="9730a-259">Add-AzureRmDelegation: サブネットを受け取り、指定されたサービス名を委任としてそのサブネットに追加します</span><span class="sxs-lookup"><span data-stu-id="9730a-259">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="9730a-260">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="9730a-260">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="9730a-261">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="9730a-261">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9730a-262">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9730a-262">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="9730a-263">管理対象のマネージド ディスクのサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-263">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="9730a-264">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9730a-264">AzureRM.RedisCache</span></span>
* <span data-ttu-id="9730a-265">Insights の依存関係を更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-265">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-266">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-266">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-267">New-AzureRmResourceGroupDeployment を新しい RollbackAction パラメーターで更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-267">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="9730a-268">新しいパラメーターを使用して OnErrorDeployment のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-268">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="9730a-269">ポリシー割り当てでマネージド ID をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9730a-269">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="9730a-270">"New-AzureRmPolicyAssignment" を指定してポリシーを割り当てるとき、既定値を持つパラメーターが不要になりました</span><span class="sxs-lookup"><span data-stu-id="9730a-270">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="9730a-271">ポリシー エイリアスを取得するための新しい Get AzureRmPolicyAlias コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-271">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-272">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-272">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-273">問題 #7161 を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-273">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="9730a-274">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="9730a-274">AzureRM.SignalR</span></span>
* <span data-ttu-id="9730a-275">SKU 名を Free_F1 および Standard_S1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-275">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="9730a-276">バージョン フィールドを PSSignalRResource オブジェクトに、接続文字列を PSSignalRKeys オブジェクトに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-276">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9730a-277">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-277">AzureRM.Storage</span></span>
* <span data-ttu-id="9730a-278">AzureRm.Storage での不変ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="9730a-278">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="9730a-279">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="9730a-279">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="9730a-280">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9730a-280">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9730a-281">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9730a-281">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9730a-282">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9730a-282">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9730a-283">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="9730a-283">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="9730a-284">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="9730a-284">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="9730a-285">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="9730a-285">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="9730a-286">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9730a-286">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="9730a-287">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9730a-287">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="9730a-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9730a-288">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="9730a-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="9730a-289">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-290">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-290">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-291">Get-AzureRmDeletedWebApp と Restore-AzureRmDeletedWebApp の 2 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-291">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="9730a-292">Windows コンテナーでの App Service プランの作成用に New-AzureRmAppServicePlan -HyperV スイッチが追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-292">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="9730a-293">Windows コンテナー アプリを作成および管理用に、New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New パラメーター (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) が追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-293">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="9730a-294">6.8.1 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="9730a-294">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9730a-295">全般</span><span class="sxs-lookup"><span data-stu-id="9730a-295">General</span></span>
* <span data-ttu-id="9730a-296">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-296">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="9730a-297">共通ランタイム アセンブリを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-297">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9730a-298">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9730a-298">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9730a-299">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-299">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="9730a-300">修正された問題 https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="9730a-300">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="9730a-301">Import-AzureRmApiManagementApi コマンドレットおよび \*-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました</span><span class="sxs-lookup"><span data-stu-id="9730a-301">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="9730a-302">修正された問題 https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="9730a-302">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="9730a-303">CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="9730a-303">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="9730a-304">4.0.4-preview NuGet へのアップグレードによって修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-304">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="9730a-305">修正された問題 https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="9730a-305">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="9730a-306">製品を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-306">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="9730a-307">修正された問題 https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="9730a-307">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="9730a-308">API を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-308">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="9730a-309">AzureMonitor ロガーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-309">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="9730a-310">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-310">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-311">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-311">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="9730a-312">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-312">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="9730a-313">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-313">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="9730a-314">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-314">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-315">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-315">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-316">コマンドレット出力の既定の表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="9730a-316">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="9730a-317">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="9730a-317">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="9730a-318">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-318">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="9730a-319">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-319">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-320">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-320">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-321">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-321">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-322">修正された問題</span><span class="sxs-lookup"><span data-stu-id="9730a-322">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9730a-323">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9730a-323">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9730a-324">複数値ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-324">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="9730a-325">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="9730a-325">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="9730a-326">サブネット ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-326">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="9730a-327">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-327">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="9730a-328">プロファイルでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-328">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="9730a-329">プロファイルでの予期される状態コード範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-329">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="9730a-330">エンドポイントでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-330">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="9730a-331">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="9730a-331">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9730a-332">全般</span><span class="sxs-lookup"><span data-stu-id="9730a-332">General</span></span>
* <span data-ttu-id="9730a-333">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-333">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9730a-334">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-334">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-335">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-335">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-336">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-336">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-337">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-337">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="9730a-338">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-338">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="9730a-339">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-339">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="9730a-340">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="9730a-340">AzureRM.IotHub</span></span>
* <span data-ttu-id="9730a-341">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-341">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-342">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-342">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-343">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="9730a-343">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="9730a-344">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="9730a-344">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="9730a-345">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-345">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-346">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-346">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-347">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-347">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-348">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-348">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-349">問題の修正</span><span class="sxs-lookup"><span data-stu-id="9730a-349">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9730a-350">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9730a-350">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9730a-351">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-351">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="9730a-352">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="9730a-352">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="9730a-353">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-353">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="9730a-354">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-354">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="9730a-355">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-355">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="9730a-356">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-356">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="9730a-357">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="9730a-357">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-358">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-358">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-359">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-359">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="9730a-360">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="9730a-360">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9730a-361">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-361">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-362">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-362">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9730a-363">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-363">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="9730a-364">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-364">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="9730a-365">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="9730a-365">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="9730a-366">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-366">Azure.Storage</span></span>
* <span data-ttu-id="9730a-367">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="9730a-367">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="9730a-368">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="9730a-368">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9730a-369">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9730a-369">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9730a-370">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-370">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="9730a-371">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9730a-371">Azure.AnalysisServices</span></span>
* <span data-ttu-id="9730a-372">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-372">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9730a-373">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9730a-373">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9730a-374">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-374">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="9730a-375">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="9730a-375">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="9730a-376">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-376">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="9730a-377">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="9730a-377">AzureRM.Automation</span></span>
* <span data-ttu-id="9730a-378">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-378">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="9730a-379">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="9730a-379">AzureRM.Backup</span></span>
* <span data-ttu-id="9730a-380">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-380">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="9730a-381">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="9730a-381">AzureRM.Batch</span></span>
* <span data-ttu-id="9730a-382">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-382">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="9730a-383">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="9730a-383">AzureRM.Billing</span></span>
* <span data-ttu-id="9730a-384">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-384">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="9730a-385">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="9730a-385">AzureRM.Cdn</span></span>
* <span data-ttu-id="9730a-386">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-386">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="9730a-387">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="9730a-387">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="9730a-388">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-389">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-389">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-390">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-390">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9730a-391">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-391">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="9730a-392">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="9730a-392">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="9730a-393">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-393">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="9730a-394">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-394">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="9730a-395">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9730a-395">AzureRM.Consumption</span></span>
* <span data-ttu-id="9730a-396">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="9730a-397">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="9730a-397">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="9730a-398">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="9730a-399">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="9730a-399">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="9730a-400">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="9730a-401">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="9730a-401">AzureRM.DataFactories</span></span>
* <span data-ttu-id="9730a-402">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9730a-403">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9730a-403">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9730a-404">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="9730a-405">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9730a-405">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="9730a-406">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9730a-407">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9730a-407">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9730a-408">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-408">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="9730a-409">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-409">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="9730a-410">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9730a-411">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-411">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="9730a-412">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="9730a-412">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="9730a-413">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-413">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="9730a-414">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="9730a-414">AzureRM.Dns</span></span>
* <span data-ttu-id="9730a-415">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-415">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="9730a-416">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9730a-416">AzureRM.EventGrid</span></span>
* <span data-ttu-id="9730a-417">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-417">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9730a-418">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9730a-418">AzureRM.EventHub</span></span>
* <span data-ttu-id="9730a-419">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-419">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="9730a-420">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="9730a-420">AzureRM.HDInsight</span></span>
* <span data-ttu-id="9730a-421">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-421">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9730a-422">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9730a-422">AzureRM.Insights</span></span>
* <span data-ttu-id="9730a-423">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="9730a-424">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="9730a-424">AzureRM.IotHub</span></span>
* <span data-ttu-id="9730a-425">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9730a-426">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9730a-426">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9730a-427">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="9730a-428">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9730a-428">AzureRM.LogicApp</span></span>
* <span data-ttu-id="9730a-429">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="9730a-430">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="9730a-430">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="9730a-431">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="9730a-432">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="9730a-432">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="9730a-433">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="9730a-434">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="9730a-434">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="9730a-435">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="9730a-436">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="9730a-436">AzureRM.Media</span></span>
* <span data-ttu-id="9730a-437">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-438">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-438">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-439">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-439">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="9730a-440">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-440">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="9730a-441">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-441">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="9730a-442">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-442">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="9730a-443">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-443">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="9730a-444">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-444">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="9730a-445">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="9730a-445">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="9730a-446">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="9730a-446">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="9730a-447">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="9730a-447">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="9730a-448">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="9730a-449">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9730a-449">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="9730a-450">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="9730a-451">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9730a-451">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="9730a-452">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="9730a-453">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="9730a-453">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="9730a-454">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="9730a-455">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="9730a-455">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="9730a-456">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-456">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9730a-457">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9730a-457">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9730a-458">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-458">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="9730a-459">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="9730a-459">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="9730a-460">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-460">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="9730a-461">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-461">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="9730a-462">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-462">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="9730a-463">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="9730a-463">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="9730a-464">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="9730a-464">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="9730a-465">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="9730a-465">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="9730a-466">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="9730a-467">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="9730a-467">AzureRM.RedisCache</span></span>
* <span data-ttu-id="9730a-468">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="9730a-469">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="9730a-469">AzureRM.Relay</span></span>
* <span data-ttu-id="9730a-470">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-471">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-471">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-472">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="9730a-472">Support template deployment at subscription scope.</span></span> <span data-ttu-id="9730a-473">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-473">Add new Cmdlets:</span></span>
    - <span data-ttu-id="9730a-474">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9730a-474">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="9730a-475">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9730a-475">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="9730a-476">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9730a-476">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="9730a-477">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9730a-477">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="9730a-478">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="9730a-478">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="9730a-479">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="9730a-479">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="9730a-480">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="9730a-480">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="9730a-481">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-481">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="9730a-482">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-482">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="9730a-483">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="9730a-484">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="9730a-484">AzureRM.Scheduler</span></span>
* <span data-ttu-id="9730a-485">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-486">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-486">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-487">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-487">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9730a-488">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9730a-488">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9730a-489">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-489">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9730a-490">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-490">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-491">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-491">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9730a-492">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-492">AzureRM.Storage</span></span>
* <span data-ttu-id="9730a-493">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-493">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="9730a-494">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="9730a-494">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="9730a-495">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-495">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="9730a-496">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9730a-496">AzureRM.Tags</span></span>
* <span data-ttu-id="9730a-497">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-497">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9730a-498">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9730a-498">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9730a-499">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-499">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="9730a-500">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="9730a-500">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="9730a-501">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-501">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-502">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-502">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-503">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-503">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="9730a-504">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="9730a-504">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9730a-505">全般</span><span class="sxs-lookup"><span data-stu-id="9730a-505">General</span></span>
* <span data-ttu-id="9730a-506">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-506">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9730a-507">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-507">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-508">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-508">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="9730a-509">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-509">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9730a-510">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-510">Azure.Storage</span></span>
* <span data-ttu-id="9730a-511">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-511">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="9730a-512">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-512">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9730a-513">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9730a-513">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9730a-514">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="9730a-514">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="9730a-515">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-515">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="9730a-516">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="9730a-516">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="9730a-517">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-517">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="9730a-518">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="9730a-518">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="9730a-519">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="9730a-519">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-520">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-520">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-521">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-521">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="9730a-522">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-522">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="9730a-523">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="9730a-523">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="9730a-524">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="9730a-524">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="9730a-525">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-525">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="9730a-526">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-526">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="9730a-527">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-527">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="9730a-528">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-528">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="9730a-529">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-529">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="9730a-530">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-530">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9730a-531">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9730a-531">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9730a-532">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-532">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="9730a-533">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="9730a-533">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="9730a-534">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-534">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="9730a-535">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-535">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9730a-536">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9730a-536">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9730a-537">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-537">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9730a-538">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9730a-538">AzureRM.EventHub</span></span>
* <span data-ttu-id="9730a-539">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-539">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="9730a-540">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="9730a-540">AzureRM.Insights</span></span>
* <span data-ttu-id="9730a-541">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-541">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="9730a-542">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="9730a-542">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9730a-543">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9730a-543">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9730a-544">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-544">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-545">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-545">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-546">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-546">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-547">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-547">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-548">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-548">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="9730a-549">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-549">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-550">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-550">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-551">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-551">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="9730a-552">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-552">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="9730a-553">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-553">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-554">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-554">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="9730a-555">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="9730a-555">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="9730a-556">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-556">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="9730a-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="9730a-557">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="9730a-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="9730a-558">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="9730a-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="9730a-559">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="9730a-560">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-560">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="9730a-561">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-561">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="9730a-562">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-562">AzureRM.Storage</span></span>
* <span data-ttu-id="9730a-563">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-563">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="9730a-564">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="9730a-564">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="9730a-565">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9730a-565">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="9730a-566">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9730a-566">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="9730a-567">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="9730a-567">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="9730a-568">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="9730a-568">AzureRM.Tags</span></span>
* <span data-ttu-id="9730a-569">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="9730a-569">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="9730a-570">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="9730a-570">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9730a-571">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-571">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-572">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-572">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9730a-573">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-573">Azure.Storage</span></span>
* <span data-ttu-id="9730a-574">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="9730a-574">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="9730a-575">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="9730a-575">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="9730a-576">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="9730a-576">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9730a-577">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9730a-577">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9730a-578">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-578">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="9730a-579">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="9730a-579">AzureRM.Automation</span></span>
* <span data-ttu-id="9730a-580">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-580">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-581">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-581">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-582">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-582">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="9730a-583">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-583">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="9730a-584">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-584">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="9730a-585">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-585">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="9730a-586">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-586">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9730a-587">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9730a-587">AzureRM.EventHub</span></span>
* <span data-ttu-id="9730a-588">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-588">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9730a-589">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9730a-589">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9730a-590">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-590">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="9730a-591">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="9730a-591">AzureRM.LogicApp</span></span>
* <span data-ttu-id="9730a-592">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-592">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-593">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-594">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="9730a-594">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="9730a-595">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-595">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="9730a-596">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-596">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="9730a-597">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-597">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="9730a-598">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-598">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="9730a-599">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="9730a-599">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="9730a-600">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="9730a-600">AzureRM.Relay</span></span>
* <span data-ttu-id="9730a-601">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-601">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-602">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-602">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-603">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-603">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="9730a-604">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="9730a-604">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="9730a-605">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-605">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="9730a-606">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-606">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="9730a-607">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-607">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-608">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-608">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-609">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-609">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="9730a-610">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-610">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="9730a-611">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9730a-611">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9730a-612">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9730a-612">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9730a-613">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9730a-613">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9730a-614">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9730a-614">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="9730a-615">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="9730a-615">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="9730a-616">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-616">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9730a-617">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9730a-617">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9730a-618">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-618">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9730a-619">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-619">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-620">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-620">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="9730a-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-621">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="9730a-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-622">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-623">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-623">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-624">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="9730a-624">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="9730a-625">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-625">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="9730a-626">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="9730a-626">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="9730a-627">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="9730a-627">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="9730a-628">全般</span><span class="sxs-lookup"><span data-stu-id="9730a-628">General</span></span>
* <span data-ttu-id="9730a-629">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-629">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="9730a-630">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-630">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-631">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-631">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-632">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-632">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-633">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="9730a-633">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="9730a-634">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-634">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="9730a-635">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-635">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="9730a-636">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="9730a-636">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="9730a-637">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-637">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="9730a-638">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="9730a-638">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="9730a-639">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="9730a-639">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="9730a-640">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="9730a-640">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="9730a-641">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="9730a-641">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="9730a-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9730a-642">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9730a-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9730a-643">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="9730a-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="9730a-644">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9730a-645">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9730a-645">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9730a-646">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="9730a-646">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="9730a-647">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="9730a-647">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9730a-648">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-648">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="9730a-649">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-649">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="9730a-650">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="9730a-650">AzureRM.EventHub</span></span>
* <span data-ttu-id="9730a-651">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-651">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="9730a-652">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-652">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="9730a-653">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="9730a-653">Provided Default Parameter set.</span></span>
* <span data-ttu-id="9730a-654">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="9730a-654">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9730a-655">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9730a-655">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9730a-656">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-656">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-657">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-657">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-658">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="9730a-658">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="9730a-659">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-659">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="9730a-660">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-660">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9730a-661">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-661">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="9730a-662">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-662">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9730a-663">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-663">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9730a-664">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-664">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="9730a-665">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-665">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="9730a-666">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-666">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="9730a-667">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-667">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9730a-668">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9730a-668">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9730a-669">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-669">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="9730a-670">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="9730a-670">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="9730a-671">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="9730a-671">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-672">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-672">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-673">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-673">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="9730a-674">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="9730a-674">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="9730a-675">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="9730a-675">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="9730a-676">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-676">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="9730a-677">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-677">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="9730a-678">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-678">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9730a-679">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-679">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9730a-680">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-680">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="9730a-681">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-681">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="9730a-682">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-682">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="9730a-683">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-683">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="9730a-684">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-684">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="9730a-685">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-685">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="9730a-686">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="9730a-686">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="9730a-687">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="9730a-687">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9730a-688">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-688">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-689">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="9730a-689">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="9730a-690">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-690">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="9730a-691">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="9730a-691">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9730a-692">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-692">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-693">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-693">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="9730a-694">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="9730a-694">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="9730a-695">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="9730a-695">Azure.Storage</span></span>
* <span data-ttu-id="9730a-696">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-696">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-697">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-697">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-698">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-698">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="9730a-699">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-699">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="9730a-700">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9730a-700">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9730a-701">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9730a-701">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9730a-702">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="9730a-702">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="9730a-703">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-703">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="9730a-704">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9730a-704">Start-AzureRmVM</span></span>
    - <span data-ttu-id="9730a-705">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9730a-705">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="9730a-706">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9730a-706">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="9730a-707">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="9730a-707">Set-AzureRmVM</span></span>
    - <span data-ttu-id="9730a-708">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="9730a-708">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="9730a-709">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9730a-709">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="9730a-710">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="9730a-710">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="9730a-711">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="9730a-711">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="9730a-712">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9730a-712">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="9730a-713">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9730a-713">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="9730a-714">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9730a-714">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="9730a-715">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="9730a-715">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="9730a-716">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="9730a-716">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="9730a-717">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="9730a-717">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="9730a-718">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="9730a-718">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="9730a-719">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="9730a-719">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="9730a-720">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="9730a-720">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="9730a-721">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="9730a-721">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="9730a-722">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="9730a-722">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="9730a-723">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="9730a-723">AzureRM.EventGrid</span></span>
* <span data-ttu-id="9730a-724">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="9730a-724">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="9730a-725">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9730a-725">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9730a-726">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-726">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="9730a-727">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="9730a-727">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="9730a-728">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="9730a-728">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="9730a-729">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="9730a-729">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="9730a-730">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-730">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="9730a-731">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="9730a-731">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="9730a-732">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-732">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="9730a-733">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="9730a-733">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9730a-734">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-734">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-735">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-735">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9730a-736">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9730a-736">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9730a-737">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-737">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-738">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-738">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-739">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="9730a-739">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="9730a-740">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="9730a-740">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="9730a-741">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="9730a-741">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="9730a-742">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="9730a-742">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="9730a-743">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-743">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="9730a-744">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="9730a-744">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9730a-745">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-745">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-746">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-746">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="9730a-747">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="9730a-747">AzureRM.Compute</span></span>
* <span data-ttu-id="9730a-748">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="9730a-748">VMSS VM Update feature</span></span>
    - <span data-ttu-id="9730a-749">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-749">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="9730a-750">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-750">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="9730a-751">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="9730a-751">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="9730a-752">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-752">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="9730a-753">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-753">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="9730a-754">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-754">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="9730a-755">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-755">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="9730a-756">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="9730a-756">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="9730a-757">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="9730a-757">AzureRM.KeyVault</span></span>
* <span data-ttu-id="9730a-758">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-758">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="9730a-759">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-759">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-760">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="9730a-760">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="9730a-761">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="9730a-761">AzureRM.Resources</span></span>
* <span data-ttu-id="9730a-762">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-762">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="9730a-763">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="9730a-763">AzureRM.Scheduler</span></span>
* <span data-ttu-id="9730a-764">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="9730a-764">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="9730a-765">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-765">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-766">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="9730a-766">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="9730a-767">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9730a-767">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9730a-768">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9730a-768">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9730a-769">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9730a-769">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9730a-770">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9730a-770">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9730a-771">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9730a-771">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="9730a-772">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="9730a-772">AzureRM.Websites</span></span>
* <span data-ttu-id="9730a-773">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="9730a-773">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="9730a-774">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="9730a-774">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="9730a-775">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="9730a-775">AzureRM.Profile</span></span>
* <span data-ttu-id="9730a-776">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-776">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="9730a-777">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="9730a-777">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="9730a-778">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="9730a-778">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="9730a-779">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="9730a-779">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="9730a-780">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-780">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="9730a-781">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-781">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="9730a-782">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-782">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="9730a-783">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="9730a-783">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="9730a-784">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-784">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="9730a-785">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-785">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="9730a-786">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-786">Added support for MSI identity</span></span>
* <span data-ttu-id="9730a-787">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="9730a-787">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="9730a-788">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="9730a-788">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="9730a-789">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-789">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="9730a-790">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="9730a-790">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="9730a-791">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="9730a-791">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="9730a-792">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="9730a-792">AzureRM.Batch</span></span>
* <span data-ttu-id="9730a-793">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="9730a-793">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="9730a-794">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="9730a-794">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="9730a-795">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="9730a-795">AzureRM.Consumption</span></span>
* <span data-ttu-id="9730a-796">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-796">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="9730a-797">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="9730a-797">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="9730a-798">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-798">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="9730a-799">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-799">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="9730a-800">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-800">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="9730a-801">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="9730a-801">AzureRM.Network</span></span>
* <span data-ttu-id="9730a-802">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-802">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="9730a-803">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-803">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="9730a-804">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="9730a-804">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="9730a-805">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-805">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="9730a-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-806">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9730a-807">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-807">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="9730a-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-808">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="9730a-809">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-809">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="9730a-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="9730a-810">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="9730a-811">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="9730a-811">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="9730a-812">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="9730a-812">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="9730a-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="9730a-813">AzureRM.Sql</span></span>
* <span data-ttu-id="9730a-814">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="9730a-814">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="9730a-815">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="9730a-815">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="9730a-816">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="9730a-816">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="9730a-817">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="9730a-817">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="9730a-818">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="9730a-818">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="9730a-819">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9730a-819">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="9730a-820">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="9730a-820">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="9730a-821">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="9730a-821">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="9730a-822">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="9730a-822">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="9730a-823">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="9730a-823">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="9730a-824">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="9730a-824">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="9730a-825">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="9730a-825">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
