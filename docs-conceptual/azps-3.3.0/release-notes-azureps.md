---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 3806a1c609a71c53c0bddc5bafd51d845c0c296e
ms.sourcegitcommit: 16904e0a72c55fb81248e0252769defb86c50f36
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/10/2020
ms.locfileid: "75831646"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="08e76-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="08e76-103">Azure PowerShell release notes</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="08e76-104">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="08e76-104">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-105">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-105">Az.Accounts</span></span>
* <span data-ttu-id="08e76-106">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-106">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08e76-107">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-107">Az.Cdn</span></span>
* <span data-ttu-id="08e76-108">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="08e76-108">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-109">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-109">Az.Compute</span></span>
* <span data-ttu-id="08e76-110">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-110">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="08e76-111">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-111">Az.ContainerInstance</span></span>
* <span data-ttu-id="08e76-112">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-112">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="08e76-113">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="08e76-113">Az.DataBoxEdge</span></span>
* <span data-ttu-id="08e76-114">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-114">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="08e76-115">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-115">Get the Edge Storage Container</span></span>
* <span data-ttu-id="08e76-116">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-116">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="08e76-117">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-117">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="08e76-118">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-118">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="08e76-119">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-119">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="08e76-120">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-120">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="08e76-121">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="08e76-121">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="08e76-122">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-122">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="08e76-123">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-123">Get the Edge Storage Account</span></span>
* <span data-ttu-id="08e76-124">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-124">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="08e76-125">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-125">Create new Edge Storage Account</span></span>
* <span data-ttu-id="08e76-126">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-126">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="08e76-127">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-127">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="08e76-128">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="08e76-128">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="08e76-129">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="08e76-129">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="08e76-130">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-130">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="08e76-131">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="08e76-131">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-132">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-132">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-133">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-133">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="08e76-134">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-134">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="08e76-135">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="08e76-135">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="08e76-136">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="08e76-136">Az.DevTestLabs</span></span>
* <span data-ttu-id="08e76-137">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-137">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-138">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-138">Az.EventHub</span></span>
* <span data-ttu-id="08e76-139">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-139">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="08e76-140">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08e76-140">Az.HDInsight</span></span>
* <span data-ttu-id="08e76-141">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-141">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="08e76-142">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="08e76-142">Az.MachineLearning</span></span>
* <span data-ttu-id="08e76-143">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-143">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="08e76-144">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="08e76-144">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="08e76-145">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="08e76-145">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="08e76-146">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="08e76-146">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="08e76-147">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="08e76-147">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="08e76-148">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="08e76-148">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="08e76-149">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="08e76-149">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="08e76-150">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="08e76-150">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-151">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-151">Az.Network</span></span>
* <span data-ttu-id="08e76-152">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="08e76-152">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-153">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-153">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-154">Azure Site Recovery は、Azure to Azure プロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="08e76-154">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed leys for Azure to Azure provider.</span></span>
* <span data-ttu-id="08e76-155">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-155">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="08e76-156">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-156">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="08e76-157">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-157">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-158">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-158">Az.Resources</span></span>
* <span data-ttu-id="08e76-159">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-159">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-160">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-160">Az.Sql</span></span>
* <span data-ttu-id="08e76-161">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-161">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="08e76-162">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-162">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="08e76-163">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="08e76-163">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="08e76-164">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-164">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-165">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-165">Az.Storage</span></span>
* <span data-ttu-id="08e76-166">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-166">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="08e76-167">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-167">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="08e76-168">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-168">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="08e76-169">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-169">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="08e76-170">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="08e76-170">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="08e76-171">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-171">General</span></span>
* <span data-ttu-id="08e76-172">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-172">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08e76-173">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-173">Az.Accounts</span></span>
* <span data-ttu-id="08e76-174">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="08e76-174">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="08e76-175">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="08e76-175">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="08e76-176">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08e76-176">Az.Batch</span></span>
* <span data-ttu-id="08e76-177">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="08e76-177">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-178">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-178">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-179">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-179">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="08e76-180">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08e76-180">Az.FrontDoor</span></span>
* <span data-ttu-id="08e76-181">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-181">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="08e76-182">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-182">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="08e76-183">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="08e76-183">Az.HealthcareApis</span></span>
* <span data-ttu-id="08e76-184">例外処理</span><span class="sxs-lookup"><span data-stu-id="08e76-184">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08e76-185">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-185">Az.KeyVault</span></span>
* <span data-ttu-id="08e76-186">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-186">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="08e76-187">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="08e76-187">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="08e76-188">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-188">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-189">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-189">Az.Monitor</span></span>
* <span data-ttu-id="08e76-190">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="08e76-190">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="08e76-191">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="08e76-191">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="08e76-192">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="08e76-192">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-193">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-193">Az.Network</span></span>
* <span data-ttu-id="08e76-194">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="08e76-194">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-195">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-195">Az.Resources</span></span>
* <span data-ttu-id="08e76-196">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-196">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="08e76-197">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-197">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-198">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-198">Az.Sql</span></span>
* <span data-ttu-id="08e76-199">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="08e76-199">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-200">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-200">Az.Storage</span></span>
* <span data-ttu-id="08e76-201">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-201">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="08e76-202">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="08e76-202">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="08e76-203">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="08e76-203">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="08e76-204">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="08e76-204">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="08e76-205">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="08e76-205">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="08e76-206">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-206">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="08e76-207">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-207">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="08e76-208">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="08e76-208">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="08e76-209">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="08e76-209">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="08e76-210">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-210">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="08e76-211">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="08e76-211">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="08e76-212">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-212">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="08e76-213">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="08e76-213">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="08e76-214">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="08e76-214">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08e76-215">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="08e76-215">Highlights since the last major release</span></span>
* <span data-ttu-id="08e76-216">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="08e76-216">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="08e76-217">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="08e76-217">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-218">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-218">Az.Compute</span></span>
* <span data-ttu-id="08e76-219">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="08e76-219">VM Reapply feature</span></span>
    - <span data-ttu-id="08e76-220">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-220">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="08e76-221">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="08e76-221">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="08e76-222">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="08e76-222">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="08e76-223">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="08e76-223">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="08e76-224">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-224">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="08e76-225">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-225">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="08e76-226">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="08e76-226">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="08e76-227">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-227">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="08e76-228">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-228">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="08e76-229">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-229">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="08e76-230">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="08e76-230">Az.DataBoxEdge</span></span>
* <span data-ttu-id="08e76-231">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-231">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="08e76-232">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-232">Get the Order</span></span>
* <span data-ttu-id="08e76-233">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-233">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="08e76-234">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-234">Create new Order</span></span>
* <span data-ttu-id="08e76-235">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-235">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="08e76-236">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-236">Remove the Order</span></span>
* <span data-ttu-id="08e76-237">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="08e76-237">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="08e76-238">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="08e76-238">Now creates Local Share</span></span>
* <span data-ttu-id="08e76-239">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-239">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="08e76-240">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-240">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="08e76-241">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-241">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="08e76-242">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="08e76-242">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="08e76-243">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-243">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="08e76-244">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-244">Gets the information about Triggers</span></span>
* <span data-ttu-id="08e76-245">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-245">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="08e76-246">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-246">Create new Triggers</span></span>
* <span data-ttu-id="08e76-247">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-247">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="08e76-248">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-248">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-249">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-249">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-250">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-250">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="08e76-251">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-251">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-252">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-252">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-253">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-253">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-254">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-254">Az.EventHub</span></span>
* <span data-ttu-id="08e76-255">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-255">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="08e76-256">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08e76-256">Az.FrontDoor</span></span>
* <span data-ttu-id="08e76-257">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-257">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="08e76-258">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-258">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="08e76-259">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-259">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="08e76-260">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="08e76-260">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-261">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-261">Az.Network</span></span>
* <span data-ttu-id="08e76-262">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="08e76-262">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="08e76-263">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="08e76-263">Az.PrivateDns</span></span>
* <span data-ttu-id="08e76-264">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-264">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-265">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-265">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-266">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="08e76-266">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="08e76-267">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="08e76-267">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="08e76-268">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="08e76-268">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="08e76-269">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="08e76-269">Az.RedisCache</span></span>
* <span data-ttu-id="08e76-270">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-270">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="08e76-271">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-271">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="08e76-272">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-272">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-273">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-273">Az.Resources</span></span>
- <span data-ttu-id="08e76-274">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-274">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="08e76-275">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-275">Updated create policy definition help example</span></span>
- <span data-ttu-id="08e76-276">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-276">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="08e76-277">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-277">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="08e76-278">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="08e76-278">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-279">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-279">Az.Sql</span></span>
* <span data-ttu-id="08e76-280">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-280">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="08e76-281">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-281">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="08e76-282">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="08e76-282">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="08e76-283">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-283">General</span></span>
* <span data-ttu-id="08e76-284">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="08e76-284">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08e76-285">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-285">Az.Accounts</span></span>
* <span data-ttu-id="08e76-286">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-286">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="08e76-287">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="08e76-287">Az.Advisor</span></span>
* <span data-ttu-id="08e76-288">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-288">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="08e76-289">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08e76-289">Az.Batch</span></span>
* <span data-ttu-id="08e76-290">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-290">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="08e76-291">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="08e76-291">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="08e76-292">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="08e76-292">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="08e76-293">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="08e76-293">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="08e76-294">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="08e76-294">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="08e76-295">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="08e76-295">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="08e76-296">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="08e76-296">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="08e76-297">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="08e76-297">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="08e76-298">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="08e76-298">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="08e76-299">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-299">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="08e76-300">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="08e76-300">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="08e76-301">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="08e76-301">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="08e76-302">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-302">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="08e76-303">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-303">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="08e76-304">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-304">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="08e76-305">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-305">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="08e76-306">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-306">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="08e76-307">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-307">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="08e76-308">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-308">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="08e76-309">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08e76-309">This operation is no longer supported.</span></span>
* <span data-ttu-id="08e76-310">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-310">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="08e76-311">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-311">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="08e76-312">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-312">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="08e76-313">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="08e76-313">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="08e76-314">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="08e76-314">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="08e76-315">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-315">New non-verified images are also now returned.</span></span> <span data-ttu-id="08e76-316">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="08e76-316">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="08e76-317">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-317">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="08e76-318">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-318">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="08e76-319">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="08e76-319">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="08e76-320">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-320">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="08e76-321">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="08e76-321">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="08e76-322">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-322">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="08e76-323">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="08e76-323">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="08e76-324">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="08e76-324">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="08e76-325">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="08e76-325">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08e76-326">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-326">Az.Cdn</span></span>
* <span data-ttu-id="08e76-327">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-327">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="08e76-328">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-328">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-329">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-329">Az.Compute</span></span>
* <span data-ttu-id="08e76-330">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="08e76-330">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="08e76-331">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="08e76-331">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="08e76-332">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="08e76-332">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="08e76-333">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="08e76-333">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="08e76-334">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-334">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="08e76-335">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-335">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="08e76-336">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="08e76-336">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="08e76-337">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-337">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="08e76-338">重大な変更</span><span class="sxs-lookup"><span data-stu-id="08e76-338">Breaking changes</span></span>
    - <span data-ttu-id="08e76-339">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="08e76-339">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="08e76-340">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="08e76-340">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-341">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-341">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-342">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-342">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-343">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-343">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-344">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="08e76-344">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="08e76-345">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="08e76-345">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="08e76-346">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="08e76-346">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="08e76-347">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-347">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="08e76-348">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-348">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="08e76-349">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-349">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="08e76-350">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08e76-350">Az.FrontDoor</span></span>
* <span data-ttu-id="08e76-351">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-351">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="08e76-352">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08e76-352">Az.HDInsight</span></span>
* <span data-ttu-id="08e76-353">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-353">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="08e76-354">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="08e76-354">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="08e76-355">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-355">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="08e76-356">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-356">Removed five cmdlets:</span></span>
    - <span data-ttu-id="08e76-357">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="08e76-357">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="08e76-358">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="08e76-358">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="08e76-359">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="08e76-359">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="08e76-360">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="08e76-360">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="08e76-361">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="08e76-361">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="08e76-362">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-362">Added three cmdlets:</span></span>
    - <span data-ttu-id="08e76-363">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="08e76-363">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="08e76-364">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="08e76-364">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="08e76-365">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="08e76-365">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="08e76-366">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-366">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="08e76-367">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-367">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="08e76-368">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-368">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="08e76-369">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="08e76-369">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="08e76-370">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-370">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="08e76-371">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-371">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="08e76-372">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-372">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="08e76-373">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-373">Added some scenario test cases.</span></span>
* <span data-ttu-id="08e76-374">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="08e76-374">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-375">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-375">Az.IotHub</span></span>
* <span data-ttu-id="08e76-376">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="08e76-376">Breaking changes:</span></span>
    - <span data-ttu-id="08e76-377">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="08e76-377">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="08e76-378">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-378">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="08e76-379">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="08e76-379">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="08e76-380">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-380">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="08e76-381">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-381">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="08e76-382">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-382">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="08e76-383">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-383">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="08e76-384">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-384">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="08e76-385">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="08e76-385">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="08e76-386">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-386">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="08e76-387">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="08e76-387">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="08e76-388">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-388">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-389">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-389">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-390">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-390">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-391">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-391">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="08e76-392">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-392">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="08e76-393">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-393">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-394">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-394">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-395">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-395">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-396">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-396">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-397">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-397">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-398">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-398">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-399">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-399">Az.Resources</span></span>
* <span data-ttu-id="08e76-400">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-400">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-401">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-401">Az.Network</span></span>
* <span data-ttu-id="08e76-402">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="08e76-402">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="08e76-403">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-403">Updated cmdlet:</span></span>
        - <span data-ttu-id="08e76-404">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-404">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-405">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-405">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-406">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-406">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-407">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-407">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-408">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-408">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="08e76-409">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="08e76-409">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="08e76-410">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-410">New cmdlet:</span></span>
        - <span data-ttu-id="08e76-411">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="08e76-411">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="08e76-412">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-412">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="08e76-413">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-413">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="08e76-414">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-414">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="08e76-415">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-415">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="08e76-416">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-416">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="08e76-417">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-417">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="08e76-418">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-418">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="08e76-419">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-419">New cmdlets added:</span></span>
        - <span data-ttu-id="08e76-420">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="08e76-420">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="08e76-421">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="08e76-421">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="08e76-422">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="08e76-422">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="08e76-423">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="08e76-423">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="08e76-424">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="08e76-424">Set-AzVirtualHub</span></span>
* <span data-ttu-id="08e76-425">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-425">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="08e76-426">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="08e76-426">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="08e76-427">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-427">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="08e76-428">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-428">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="08e76-429">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-429">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="08e76-430">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-430">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="08e76-431">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-431">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="08e76-432">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-432">New cmdlets added:</span></span>
        - <span data-ttu-id="08e76-433">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-433">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="08e76-434">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="08e76-434">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="08e76-435">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-435">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="08e76-436">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-436">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="08e76-437">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-437">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="08e76-438">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-438">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="08e76-439">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-439">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="08e76-440">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-440">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="08e76-441">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-441">New cmdlets added:</span></span>
        - <span data-ttu-id="08e76-442">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="08e76-442">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="08e76-443">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="08e76-443">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="08e76-444">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="08e76-444">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="08e76-445">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="08e76-445">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="08e76-446">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="08e76-446">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="08e76-447">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-447">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="08e76-448">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="08e76-448">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="08e76-449">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-449">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="08e76-450">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-450">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="08e76-451">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-451">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="08e76-452">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-452">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="08e76-453">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="08e76-453">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="08e76-454">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-454">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="08e76-455">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-455">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="08e76-456">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-456">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="08e76-457">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-457">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="08e76-458">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-458">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="08e76-459">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-459">New cmdlets added:</span></span>
        - <span data-ttu-id="08e76-460">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="08e76-460">New-AzIpGroup</span></span>
        - <span data-ttu-id="08e76-461">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="08e76-461">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="08e76-462">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="08e76-462">Get-AzIpGroup</span></span>
        - <span data-ttu-id="08e76-463">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="08e76-463">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-464">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-464">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-465">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="08e76-465">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-466">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-466">Az.Sql</span></span>
* <span data-ttu-id="08e76-467">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-467">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="08e76-468">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-468">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="08e76-469">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-469">Removed deprecated aliases:</span></span>
* <span data-ttu-id="08e76-470">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="08e76-470">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="08e76-471">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="08e76-471">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="08e76-472">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-472">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="08e76-473">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-473">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="08e76-474">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="08e76-474">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="08e76-475">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-475">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-476">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-476">Az.Storage</span></span>
* <span data-ttu-id="08e76-477">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-477">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="08e76-478">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-478">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="08e76-479">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-479">Set-AzStorageAccount</span></span>
* <span data-ttu-id="08e76-480">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="08e76-480">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="08e76-481">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="08e76-481">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="08e76-482">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="08e76-482">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="08e76-483">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="08e76-483">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="08e76-484">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-484">General</span></span>
* <span data-ttu-id="08e76-485">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="08e76-485">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08e76-486">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-486">Az.Accounts</span></span>
* <span data-ttu-id="08e76-487">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-487">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="08e76-488">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-488">Az.ApiManagement</span></span>
* <span data-ttu-id="08e76-489">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-489">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="08e76-490">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="08e76-490">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-491">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-491">Az.Automation</span></span>
* <span data-ttu-id="08e76-492">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-492">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="08e76-493">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08e76-493">Az.Batch</span></span>
* <span data-ttu-id="08e76-494">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="08e76-494">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-495">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-495">Az.Compute</span></span>
* <span data-ttu-id="08e76-496">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-496">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="08e76-497">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-497">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="08e76-498">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-498">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="08e76-499">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-499">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-500">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-500">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-501">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="08e76-501">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="08e76-502">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="08e76-502">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="08e76-503">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-503">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-504">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-505">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-505">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="08e76-506">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="08e76-506">Az.HealthcareApis</span></span>
* <span data-ttu-id="08e76-507">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-507">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="08e76-508">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-508">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="08e76-509">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-509">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="08e76-510">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-510">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-511">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-511">Az.IotHub</span></span>
* <span data-ttu-id="08e76-512">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="08e76-512">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="08e76-513">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="08e76-513">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="08e76-514">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-514">Az.Monitor</span></span>
* <span data-ttu-id="08e76-515">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="08e76-515">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="08e76-516">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="08e76-516">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="08e76-517">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="08e76-517">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="08e76-518">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-518">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-519">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-519">Az.Network</span></span>
* <span data-ttu-id="08e76-520">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-520">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="08e76-521">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-521">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="08e76-522">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-522">New cmdlets added:</span></span>
        - <span data-ttu-id="08e76-523">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-523">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="08e76-524">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-524">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="08e76-525">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-525">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="08e76-526">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-526">Updated cmdlets:</span></span>
        - <span data-ttu-id="08e76-527">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-527">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="08e76-528">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-528">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="08e76-529">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-529">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="08e76-530">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="08e76-530">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="08e76-531">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="08e76-531">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="08e76-532">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="08e76-532">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="08e76-533">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="08e76-533">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="08e76-534">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="08e76-534">Az.RedisCache</span></span>
* <span data-ttu-id="08e76-535">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-535">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-536">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-536">Az.Sql</span></span>
* <span data-ttu-id="08e76-537">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-537">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-538">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-538">Az.Storage</span></span>
* <span data-ttu-id="08e76-539">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="08e76-539">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="08e76-540">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="08e76-540">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="08e76-541">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="08e76-541">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="08e76-542">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="08e76-542">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="08e76-543">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-543">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="08e76-544">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="08e76-544">Az.StorageSync</span></span>
* <span data-ttu-id="08e76-545">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-545">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-546">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-546">Az.Websites</span></span>
* <span data-ttu-id="08e76-547">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="08e76-547">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="08e76-548">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="08e76-548">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="08e76-549">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-549">Az.ApiManagement</span></span>
* <span data-ttu-id="08e76-550">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-550">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="08e76-551">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-551">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="08e76-552">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="08e76-552">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-553">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-553">Az.Automation</span></span>
* <span data-ttu-id="08e76-554">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-554">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="08e76-555">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-555">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="08e76-556">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-556">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-557">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-557">Az.Compute</span></span>
* <span data-ttu-id="08e76-558">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-558">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="08e76-559">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-559">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="08e76-560">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-560">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="08e76-561">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="08e76-561">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="08e76-562">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="08e76-562">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="08e76-563">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-563">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="08e76-564">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-564">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="08e76-565">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-565">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="08e76-566">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-566">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-567">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-567">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-568">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-568">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="08e76-569">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-569">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="08e76-570">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08e76-570">Az.HDInsight</span></span>
* <span data-ttu-id="08e76-571">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="08e76-571">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-572">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-572">Az.IotHub</span></span>
* <span data-ttu-id="08e76-573">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-573">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="08e76-574">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-574">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="08e76-575">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="08e76-575">New cmdlets are:</span></span>
    - <span data-ttu-id="08e76-576">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="08e76-576">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="08e76-577">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="08e76-577">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="08e76-578">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="08e76-578">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="08e76-579">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="08e76-579">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-580">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-580">Az.Monitor</span></span>
* <span data-ttu-id="08e76-581">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="08e76-581">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="08e76-582">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="08e76-582">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="08e76-583">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="08e76-583">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="08e76-584">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="08e76-584">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="08e76-585">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-585">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="08e76-586">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-586">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="08e76-587">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="08e76-587">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="08e76-588">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="08e76-588">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="08e76-589">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-589">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="08e76-590">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="08e76-590">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="08e76-591">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-591">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="08e76-592">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="08e76-592">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="08e76-593">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-593">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="08e76-594">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-594">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="08e76-595">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-595">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="08e76-596">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="08e76-596">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="08e76-597">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="08e76-597">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="08e76-598">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="08e76-598">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="08e76-599">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-599">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="08e76-600">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="08e76-600">Overall improved help files</span></span>
* <span data-ttu-id="08e76-601">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-601">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-602">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-602">Az.Network</span></span>
* <span data-ttu-id="08e76-603">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-603">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="08e76-604">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-604">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="08e76-605">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="08e76-605">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="08e76-606">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="08e76-606">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="08e76-607">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="08e76-607">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="08e76-608">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-608">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="08e76-609">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-609">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="08e76-610">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-610">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="08e76-611">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-611">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="08e76-612">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-612">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="08e76-613">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-613">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="08e76-614">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-614">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="08e76-615">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-615">New cmdlets</span></span>
        - <span data-ttu-id="08e76-616">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="08e76-616">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="08e76-617">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-617">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="08e76-618">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-618">Updated cmdlet:</span></span>
        - <span data-ttu-id="08e76-619">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="08e76-619">New-VpnSite</span></span>
        - <span data-ttu-id="08e76-620">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="08e76-620">Update-VpnSite</span></span>
        - <span data-ttu-id="08e76-621">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-621">New-VpnConnection</span></span>
        - <span data-ttu-id="08e76-622">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-622">Update-VpnConnection</span></span>
* <span data-ttu-id="08e76-623">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-623">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-624">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-624">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-625">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-625">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="08e76-626">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-626">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-627">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-627">Az.Resources</span></span>
* <span data-ttu-id="08e76-628">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-628">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-629">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-629">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-630">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-630">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="08e76-631">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-631">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="08e76-632">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="08e76-632">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="08e76-633">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="08e76-633">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="08e76-634">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="08e76-634">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="08e76-635">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="08e76-635">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="08e76-636">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="08e76-636">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="08e76-637">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="08e76-637">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="08e76-638">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="08e76-638">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="08e76-639">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="08e76-639">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="08e76-640">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="08e76-640">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="08e76-641">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="08e76-641">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="08e76-642">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="08e76-642">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="08e76-643">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="08e76-643">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="08e76-644">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="08e76-644">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="08e76-645">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="08e76-645">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="08e76-646">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="08e76-646">Az.SignalR</span></span>
* <span data-ttu-id="08e76-647">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="08e76-647">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-648">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-648">Az.Sql</span></span>
* <span data-ttu-id="08e76-649">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-649">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="08e76-650">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-650">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="08e76-651">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-651">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="08e76-652">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-652">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="08e76-653">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="08e76-653">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-654">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-654">Az.Storage</span></span>
* <span data-ttu-id="08e76-655">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-655">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="08e76-656">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-656">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="08e76-657">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="08e76-657">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="08e76-658">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="08e76-658">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="08e76-659">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="08e76-659">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="08e76-660">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="08e76-660">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="08e76-661">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-661">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="08e76-662">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="08e76-662">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="08e76-663">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="08e76-663">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="08e76-664">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="08e76-664">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="08e76-665">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="08e76-665">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-666">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-666">Az.Websites</span></span>
* <span data-ttu-id="08e76-667">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-667">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="08e76-668">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="08e76-668">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="08e76-669">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-669">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="08e76-670">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="08e76-670">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="08e76-671">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-671">General</span></span>
* <span data-ttu-id="08e76-672">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-672">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08e76-673">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-673">Az.Accounts</span></span>
* <span data-ttu-id="08e76-674">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="08e76-674">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="08e76-675">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="08e76-675">Az.Aks</span></span>
* <span data-ttu-id="08e76-676">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-676">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="08e76-677">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="08e76-677">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="08e76-678">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-678">Az.ApiManagement</span></span>
* <span data-ttu-id="08e76-679">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="08e76-679">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="08e76-680">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="08e76-680">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="08e76-681">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-681">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="08e76-682">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="08e76-682">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="08e76-683">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-683">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="08e76-684">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08e76-684">Az.Batch</span></span>
* <span data-ttu-id="08e76-685">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-685">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08e76-686">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-686">Az.Cdn</span></span>
* <span data-ttu-id="08e76-687">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-687">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-688">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-688">Az.Compute</span></span>
* <span data-ttu-id="08e76-689">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-689">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="08e76-690">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-690">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="08e76-691">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-691">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="08e76-692">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-692">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="08e76-693">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="08e76-693">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="08e76-694">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="08e76-694">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="08e76-695">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-695">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="08e76-696">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-696">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-697">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-697">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-698">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-698">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="08e76-699">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-699">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="08e76-700">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="08e76-700">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="08e76-701">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-701">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-702">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-702">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-703">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-703">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-704">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-704">Az.EventHub</span></span>
* <span data-ttu-id="08e76-705">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="08e76-705">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="08e76-706">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="08e76-706">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="08e76-707">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-707">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="08e76-708">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="08e76-708">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="08e76-709">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="08e76-709">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="08e76-710">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-710">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-711">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-711">Az.Monitor</span></span>
* <span data-ttu-id="08e76-712">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-712">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-713">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-713">Az.Network</span></span>
* <span data-ttu-id="08e76-714">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-714">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="08e76-715">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-715">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="08e76-716">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-716">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="08e76-717">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-717">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="08e76-718">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="08e76-718">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="08e76-719">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-719">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="08e76-720">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-720">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-721">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-721">Az.OperationalInsights</span></span>
* <span data-ttu-id="08e76-722">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-722">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="08e76-723">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-723">Added example</span></span>
    - <span data-ttu-id="08e76-724">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-724">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="08e76-725">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-725">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="08e76-726">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-726">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-727">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-727">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-728">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-728">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-729">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-729">Az.Resources</span></span>
* <span data-ttu-id="08e76-730">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-730">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="08e76-731">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-731">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="08e76-732">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="08e76-732">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="08e76-733">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-733">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08e76-734">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08e76-734">Az.ServiceBus</span></span>
* <span data-ttu-id="08e76-735">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="08e76-735">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="08e76-736">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="08e76-736">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="08e76-737">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-737">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-738">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-738">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-739">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-739">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="08e76-740">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="08e76-740">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="08e76-741">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="08e76-741">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="08e76-742">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-742">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="08e76-743">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="08e76-743">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="08e76-744">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-744">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-745">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-745">Az.Sql</span></span>
* <span data-ttu-id="08e76-746">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-746">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-747">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-747">Az.Storage</span></span>
* <span data-ttu-id="08e76-748">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-748">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="08e76-749">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-749">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="08e76-750">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="08e76-750">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="08e76-751">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="08e76-751">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="08e76-752">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-752">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="08e76-753">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="08e76-753">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-754">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-754">Az.Websites</span></span>
* <span data-ttu-id="08e76-755">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-755">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="08e76-756">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="08e76-756">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-757">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-757">Az.Accounts</span></span>
* <span data-ttu-id="08e76-758">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-758">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="08e76-759">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-759">Az.ApplicationInsights</span></span>
* <span data-ttu-id="08e76-760">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-760">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="08e76-761">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-761">Az.Automation</span></span>
* <span data-ttu-id="08e76-762">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-762">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="08e76-763">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08e76-763">Az.CognitiveServices</span></span>
* <span data-ttu-id="08e76-764">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-764">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-765">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-765">Az.Compute</span></span>
* <span data-ttu-id="08e76-766">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-766">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="08e76-767">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="08e76-767">Az.ContainerRegistry</span></span>
* <span data-ttu-id="08e76-768">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-768">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="08e76-769">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="08e76-769">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-770">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-770">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-771">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-771">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="08e76-772">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-772">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-773">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-773">Az.EventHub</span></span>
* <span data-ttu-id="08e76-774">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="08e76-774">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="08e76-775">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-775">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08e76-776">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-776">Az.KeyVault</span></span>
* <span data-ttu-id="08e76-777">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-777">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08e76-778">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08e76-778">Az.LogicApp</span></span>
* <span data-ttu-id="08e76-779">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-779">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="08e76-780">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-780">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="08e76-781">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="08e76-781">Az.ManagedServices</span></span>
* <span data-ttu-id="08e76-782">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-782">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-783">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-783">Az.Network</span></span>
* <span data-ttu-id="08e76-784">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-784">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="08e76-785">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-785">New cmdlets</span></span>
        - <span data-ttu-id="08e76-786">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="08e76-786">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="08e76-787">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="08e76-787">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="08e76-788">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-788">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-789">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-789">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-790">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-790">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-791">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-791">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="08e76-792">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="08e76-792">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="08e76-793">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="08e76-793">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="08e76-794">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="08e76-794">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="08e76-795">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-795">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="08e76-796">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-796">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="08e76-797">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-797">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="08e76-798">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="08e76-798">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="08e76-799">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-799">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="08e76-800">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-800">Updated cmdlets</span></span>
        - <span data-ttu-id="08e76-801">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-801">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="08e76-802">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-802">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="08e76-803">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-803">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="08e76-804">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-804">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="08e76-805">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-805">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="08e76-806">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-806">Updated cmdlet:</span></span>
        - <span data-ttu-id="08e76-807">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-807">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="08e76-808">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-808">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="08e76-809">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-809">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="08e76-810">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="08e76-810">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="08e76-811">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-811">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="08e76-812">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="08e76-812">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-813">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-813">Az.OperationalInsights</span></span>
* <span data-ttu-id="08e76-814">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-814">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="08e76-815">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-815">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-816">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-816">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-817">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-817">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="08e76-818">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-818">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="08e76-819">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-819">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="08e76-820">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-820">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="08e76-821">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-821">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="08e76-822">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-822">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="08e76-823">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-823">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="08e76-824">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-824">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="08e76-825">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-825">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="08e76-826">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-826">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-827">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-827">Az.Resources</span></span>
- <span data-ttu-id="08e76-828">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-828">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="08e76-829">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-829">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08e76-830">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08e76-830">Az.ServiceBus</span></span>
* <span data-ttu-id="08e76-831">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="08e76-831">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="08e76-832">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-832">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-833">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-833">Az.Sql</span></span>
* <span data-ttu-id="08e76-834">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-834">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="08e76-835">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-835">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="08e76-836">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-836">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-837">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-837">Az.Storage</span></span>
* <span data-ttu-id="08e76-838">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-838">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="08e76-839">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="08e76-839">Az.StorageSync</span></span>
* <span data-ttu-id="08e76-840">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-840">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="08e76-841">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-841">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-842">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-842">Az.Websites</span></span>
* <span data-ttu-id="08e76-843">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-843">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="08e76-844">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-844">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="08e76-845">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-845">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="08e76-846">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="08e76-846">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-847">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-847">Az.Accounts</span></span>
* <span data-ttu-id="08e76-848">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="08e76-848">Add support for profile cmdlets</span></span>
* <span data-ttu-id="08e76-849">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="08e76-849">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="08e76-850">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="08e76-850">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="08e76-851">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="08e76-851">Az.Advisor</span></span>
* <span data-ttu-id="08e76-852">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="08e76-852">GA release of Az.Advisor</span></span>
* <span data-ttu-id="08e76-853">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-853">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="08e76-854">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-854">Az.ApiManagement</span></span>
* <span data-ttu-id="08e76-855">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="08e76-855">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="08e76-856">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="08e76-856">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="08e76-857">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-857">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="08e76-858">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-858">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="08e76-859">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-859">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="08e76-860">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="08e76-860">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="08e76-861">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-861">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-862">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-862">Az.Automation</span></span>
* <span data-ttu-id="08e76-863">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-863">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-864">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-864">Az.Compute</span></span>
* <span data-ttu-id="08e76-865">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="08e76-865">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-866">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-866">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-867">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="08e76-867">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="08e76-868">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="08e76-868">Az.EventGrid</span></span>
* <span data-ttu-id="08e76-869">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-869">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-870">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-870">Az.IotHub</span></span>
* <span data-ttu-id="08e76-871">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-871">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-872">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-872">Az.Network</span></span>
* <span data-ttu-id="08e76-873">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-873">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="08e76-874">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="08e76-874">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08e76-875">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-875">Az.PolicyInsights</span></span>
* <span data-ttu-id="08e76-876">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-876">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="08e76-877">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="08e76-877">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-878">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-878">Az.OperationalInsights</span></span>
* <span data-ttu-id="08e76-879">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-879">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-880">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-880">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-881">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-881">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-882">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-882">Az.Resources</span></span>
    - <span data-ttu-id="08e76-883">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-883">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="08e76-884">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-884">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="08e76-885">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-885">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="08e76-886">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-886">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08e76-887">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08e76-887">Az.ServiceBus</span></span>
* <span data-ttu-id="08e76-888">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="08e76-888">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-889">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-889">Az.Sql</span></span>
* <span data-ttu-id="08e76-890">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-890">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="08e76-891">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-891">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="08e76-892">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="08e76-892">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="08e76-893">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="08e76-893">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="08e76-894">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="08e76-894">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="08e76-895">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="08e76-895">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="08e76-896">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="08e76-896">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="08e76-897">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="08e76-897">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="08e76-898">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-898">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-899">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-899">Az.Storage</span></span>
* <span data-ttu-id="08e76-900">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-900">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="08e76-901">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="08e76-901">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="08e76-902">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-902">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="08e76-903">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="08e76-903">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="08e76-904">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-904">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="08e76-905">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-905">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="08e76-906">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-906">Set-AzStorageAccount</span></span>
* <span data-ttu-id="08e76-907">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-907">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="08e76-908">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="08e76-908">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="08e76-909">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="08e76-909">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="08e76-910">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="08e76-910">Az.StorageSync</span></span>
* <span data-ttu-id="08e76-911">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-911">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="08e76-912">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="08e76-912">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-913">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-913">Az.Accounts</span></span>
* <span data-ttu-id="08e76-914">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-914">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="08e76-915">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="08e76-915">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="08e76-916">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-916">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="08e76-917">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="08e76-917">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="08e76-918">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="08e76-918">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-919">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-919">Az.Compute</span></span>
* <span data-ttu-id="08e76-920">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-920">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="08e76-921">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-921">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="08e76-922">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="08e76-922">Az.Dns</span></span>
* <span data-ttu-id="08e76-923">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-923">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="08e76-924">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="08e76-924">Az.EventGrid</span></span>
* <span data-ttu-id="08e76-925">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-925">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="08e76-926">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-926">New cmdlets:</span></span>
    - <span data-ttu-id="08e76-927">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="08e76-927">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="08e76-928">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="08e76-928">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="08e76-929">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="08e76-929">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="08e76-930">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="08e76-930">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="08e76-931">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="08e76-931">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="08e76-932">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="08e76-932">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="08e76-933">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="08e76-933">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="08e76-934">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="08e76-934">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="08e76-935">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="08e76-935">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="08e76-936">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="08e76-936">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="08e76-937">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="08e76-937">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="08e76-938">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="08e76-938">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="08e76-939">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="08e76-939">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="08e76-940">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="08e76-940">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="08e76-941">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="08e76-941">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="08e76-942">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="08e76-942">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="08e76-943">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-943">Updated cmdlets:</span></span>
    - <span data-ttu-id="08e76-944">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="08e76-944">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="08e76-945">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-945">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="08e76-946">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-946">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="08e76-947">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="08e76-947">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="08e76-948">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="08e76-948">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="08e76-949">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="08e76-949">Event subscription expiration date,</span></span>
            - <span data-ttu-id="08e76-950">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="08e76-950">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="08e76-951">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-951">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="08e76-952">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="08e76-952">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="08e76-953">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="08e76-953">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="08e76-954">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-954">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="08e76-955">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="08e76-955">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="08e76-956">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-956">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="08e76-957">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-957">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="08e76-958">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08e76-958">Az.FrontDoor</span></span>
* <span data-ttu-id="08e76-959">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="08e76-959">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="08e76-960">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-960">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="08e76-961">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="08e76-961">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="08e76-962">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-962">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-963">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-963">Az.Network</span></span>
* <span data-ttu-id="08e76-964">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-964">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="08e76-965">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-965">New cmdlets</span></span>
        - <span data-ttu-id="08e76-966">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="08e76-966">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="08e76-967">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-967">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="08e76-968">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-968">New cmdlets</span></span> 
        - <span data-ttu-id="08e76-969">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="08e76-969">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="08e76-970">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-970">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="08e76-971">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-971">New cmdlets</span></span> 
        - <span data-ttu-id="08e76-972">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="08e76-972">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="08e76-973">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="08e76-973">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="08e76-974">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="08e76-974">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="08e76-975">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-975">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="08e76-976">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-976">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="08e76-977">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-977">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="08e76-978">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-978">New cmdlets</span></span>
        - <span data-ttu-id="08e76-979">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="08e76-979">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="08e76-980">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="08e76-980">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="08e76-981">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="08e76-981">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="08e76-982">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="08e76-982">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="08e76-983">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="08e76-983">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="08e76-984">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-984">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="08e76-985">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-985">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="08e76-986">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-986">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="08e76-987">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-987">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="08e76-988">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-988">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="08e76-989">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-989">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="08e76-990">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-990">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="08e76-991">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-991">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="08e76-992">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-992">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="08e76-993">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-993">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="08e76-994">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-994">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="08e76-995">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-995">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="08e76-996">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-996">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="08e76-997">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="08e76-997">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="08e76-998">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-998">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="08e76-999">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-999">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="08e76-1000">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="08e76-1000">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="08e76-1001">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="08e76-1001">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="08e76-1002">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1002">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="08e76-1003">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1003">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="08e76-1004">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1004">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="08e76-1005">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1005">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-1006">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1006">Az.OperationalInsights</span></span>
* <span data-ttu-id="08e76-1007">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1007">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1008">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1008">Az.Resources</span></span>
* <span data-ttu-id="08e76-1009">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="08e76-1009">Support for additional Template Export options</span></span>
    - <span data-ttu-id="08e76-1010">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1010">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="08e76-1011">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1011">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="08e76-1012">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1012">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-1013">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1013">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-1014">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1014">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1015">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1015">Az.Sql</span></span>
* <span data-ttu-id="08e76-1016">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1016">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="08e76-1017">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1017">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="08e76-1018">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="08e76-1018">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="08e76-1019">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="08e76-1019">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="08e76-1020">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="08e76-1020">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="08e76-1021">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="08e76-1021">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="08e76-1022">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="08e76-1022">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="08e76-1023">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="08e76-1023">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1024">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1024">Az.Storage</span></span>
* <span data-ttu-id="08e76-1025">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1025">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="08e76-1026">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-1026">New-AzStorageAccount</span></span>
* <span data-ttu-id="08e76-1027">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1027">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="08e76-1028">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-1028">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1029">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1029">Az.Websites</span></span>
* <span data-ttu-id="08e76-1030">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1030">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="08e76-1031">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1031">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="08e76-1032">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1032">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="08e76-1033">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-1033">Az.Cdn</span></span>
* <span data-ttu-id="08e76-1034">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1034">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1035">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1035">Az.Compute</span></span>
* <span data-ttu-id="08e76-1036">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1036">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="08e76-1037">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="08e76-1037">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-1038">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-1038">Az.EventHub</span></span>
* <span data-ttu-id="08e76-1039">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1039">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="08e76-1040">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1040">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1041">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1041">Az.Network</span></span>
* <span data-ttu-id="08e76-1042">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1042">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="08e76-1043">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1043">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08e76-1044">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1044">Az.PolicyInsights</span></span>
* <span data-ttu-id="08e76-1045">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1045">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1046">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1046">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-1047">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1047">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08e76-1048">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08e76-1048">Az.ServiceBus</span></span>
* <span data-ttu-id="08e76-1049">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1049">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-1050">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1050">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-1051">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1051">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="08e76-1052">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1052">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1053">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1053">Az.Sql</span></span>
* <span data-ttu-id="08e76-1054">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1054">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="08e76-1055">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="08e76-1055">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="08e76-1056">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1056">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="08e76-1057">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1057">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1058">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1058">Az.Websites</span></span>
* <span data-ttu-id="08e76-1059">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1059">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="08e76-1060">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1060">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="08e76-1061">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-1061">Az.ApiManagement</span></span>
* <span data-ttu-id="08e76-1062">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1062">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="08e76-1063">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-1063">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="08e76-1064">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-1064">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="08e76-1065">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-1065">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="08e76-1066">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1066">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="08e76-1067">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-1067">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="08e76-1068">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-1068">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="08e76-1069">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-1069">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="08e76-1070">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1070">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="08e76-1071">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-1071">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="08e76-1072">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-1072">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="08e76-1073">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-1073">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="08e76-1074">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-1074">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="08e76-1075">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1075">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="08e76-1076">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="08e76-1076">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="08e76-1077">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-1077">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="08e76-1078">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="08e76-1078">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="08e76-1079">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="08e76-1079">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="08e76-1080">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1080">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="08e76-1081">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="08e76-1081">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="08e76-1082">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1082">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="08e76-1083">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1083">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="08e76-1084">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="08e76-1084">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="08e76-1085">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1085">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="08e76-1086">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1086">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="08e76-1087">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1087">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="08e76-1088">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="08e76-1088">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="08e76-1089">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="08e76-1089">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="08e76-1090">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1090">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="08e76-1091">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1091">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="08e76-1092">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1092">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="08e76-1093">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="08e76-1093">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="08e76-1094">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1094">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="08e76-1095">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1095">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="08e76-1096">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="08e76-1096">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="08e76-1097">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="08e76-1097">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="08e76-1098">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="08e76-1098">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="08e76-1099">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1099">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="08e76-1100">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1100">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="08e76-1101">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1101">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="08e76-1102">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="08e76-1102">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="08e76-1103">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="08e76-1103">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="08e76-1104">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="08e76-1104">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="08e76-1105">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1105">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="08e76-1106">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1106">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="08e76-1107">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="08e76-1107">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="08e76-1108">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="08e76-1108">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="08e76-1109">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1109">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="08e76-1110">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1110">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="08e76-1111">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="08e76-1111">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="08e76-1112">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="08e76-1112">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="08e76-1113">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="08e76-1113">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="08e76-1114">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="08e76-1114">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="08e76-1115">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1115">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="08e76-1116">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="08e76-1116">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="08e76-1117">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="08e76-1117">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="08e76-1118">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1118">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="08e76-1119">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="08e76-1119">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="08e76-1120">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="08e76-1120">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="08e76-1121">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1121">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="08e76-1122">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1122">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="08e76-1123">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="08e76-1123">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="08e76-1124">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="08e76-1124">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="08e76-1125">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1125">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="08e76-1126">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1126">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="08e76-1127">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="08e76-1127">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="08e76-1128">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="08e76-1128">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="08e76-1129">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="08e76-1129">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="08e76-1130">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="08e76-1130">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="08e76-1131">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="08e76-1131">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="08e76-1132">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="08e76-1132">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="08e76-1133">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="08e76-1133">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="08e76-1134">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="08e76-1134">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="08e76-1135">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1135">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="08e76-1136">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="08e76-1136">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="08e76-1137">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="08e76-1137">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="08e76-1138">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="08e76-1138">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-1139">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1139">Az.Automation</span></span>
* <span data-ttu-id="08e76-1140">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1140">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="08e76-1141">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="08e76-1141">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="08e76-1142">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="08e76-1142">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="08e76-1143">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1143">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="08e76-1144">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="08e76-1144">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="08e76-1145">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1145">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="08e76-1146">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1146">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1147">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1147">Az.Compute</span></span>
* <span data-ttu-id="08e76-1148">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1148">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="08e76-1149">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-1149">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1150">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1150">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1151">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1151">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-1152">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-1152">Az.Monitor</span></span>
* <span data-ttu-id="08e76-1153">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1153">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1154">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1154">Az.Network</span></span>
* <span data-ttu-id="08e76-1155">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1155">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="08e76-1156">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="08e76-1156">Updated cmdlet:</span></span>
        - <span data-ttu-id="08e76-1157">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="08e76-1157">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="08e76-1158">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1158">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1159">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1159">Az.Resources</span></span>
* <span data-ttu-id="08e76-1160">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1160">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1161">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1161">Az.Sql</span></span>
* <span data-ttu-id="08e76-1162">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-1162">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="08e76-1163">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1163">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-1164">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1164">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1165">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1165">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="08e76-1166">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1166">Az.CognitiveServices</span></span>
* <span data-ttu-id="08e76-1167">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1167">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="08e76-1168">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1168">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1169">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1169">Az.Compute</span></span>
* <span data-ttu-id="08e76-1170">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="08e76-1170">Proximity placement group feature.</span></span>
    - <span data-ttu-id="08e76-1171">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="08e76-1171">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="08e76-1172">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-1172">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="08e76-1173">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1173">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="08e76-1174">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1174">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="08e76-1175">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1175">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="08e76-1176">重大な変更</span><span class="sxs-lookup"><span data-stu-id="08e76-1176">Breaking changes</span></span>
    - <span data-ttu-id="08e76-1177">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="08e76-1177">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="08e76-1178">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="08e76-1178">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="08e76-1179">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="08e76-1179">Az.DeploymentManager</span></span>
* <span data-ttu-id="08e76-1180">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="08e76-1180">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="08e76-1181">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="08e76-1181">Az.Dns</span></span>
* <span data-ttu-id="08e76-1182">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="08e76-1182">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="08e76-1183">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="08e76-1183">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="08e76-1184">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1184">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="08e76-1185">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08e76-1185">Az.FrontDoor</span></span>
* <span data-ttu-id="08e76-1186">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="08e76-1186">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="08e76-1187">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="08e76-1187">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="08e76-1188">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08e76-1188">Az.HDInsight</span></span>
* <span data-ttu-id="08e76-1189">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1189">Removed two cmdlets:</span></span>
    - <span data-ttu-id="08e76-1190">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="08e76-1190">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="08e76-1191">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="08e76-1191">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="08e76-1192">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1192">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="08e76-1193">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1193">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="08e76-1194">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1194">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="08e76-1195">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="08e76-1195">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-1196">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-1196">Az.Monitor</span></span>
* <span data-ttu-id="08e76-1197">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="08e76-1197">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="08e76-1198">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="08e76-1198">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="08e76-1199">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="08e76-1199">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="08e76-1200">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="08e76-1200">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="08e76-1201">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="08e76-1201">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="08e76-1202">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="08e76-1202">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="08e76-1203">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="08e76-1203">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="08e76-1204">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1204">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08e76-1205">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1205">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08e76-1206">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1206">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08e76-1207">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1207">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08e76-1208">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1208">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="08e76-1209">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="08e76-1209">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="08e76-1210">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1210">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1211">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1211">Az.Network</span></span>
* <span data-ttu-id="08e76-1212">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1212">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="08e76-1213">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1213">New cmdlets</span></span>
        - <span data-ttu-id="08e76-1214">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08e76-1214">New-AzNatGateway</span></span>
        - <span data-ttu-id="08e76-1215">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08e76-1215">Get-AzNatGateway</span></span>
        - <span data-ttu-id="08e76-1216">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08e76-1216">Set-AzNatGateway</span></span>
        - <span data-ttu-id="08e76-1217">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="08e76-1217">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="08e76-1218">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1218">Updated cmdlets</span></span>
        - <span data-ttu-id="08e76-1219">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="08e76-1219">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="08e76-1220">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="08e76-1220">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="08e76-1221">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="08e76-1221">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="08e76-1222">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1222">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="08e76-1223">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1223">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08e76-1224">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1224">Az.PolicyInsights</span></span>
* <span data-ttu-id="08e76-1225">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="08e76-1225">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="08e76-1226">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1226">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="08e76-1227">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="08e76-1227">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1228">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1228">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-1229">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="08e76-1229">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="08e76-1230">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="08e76-1230">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="08e76-1231">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="08e76-1231">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="08e76-1232">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="08e76-1232">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="08e76-1233">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="08e76-1233">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="08e76-1234">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="08e76-1234">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="08e76-1235">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="08e76-1235">Az.Relay</span></span>
* <span data-ttu-id="08e76-1236">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1236">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08e76-1237">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08e76-1237">Az.ServiceBus</span></span>
* <span data-ttu-id="08e76-1238">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1238">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1239">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1239">Az.Storage</span></span>
* <span data-ttu-id="08e76-1240">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="08e76-1240">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="08e76-1241">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1241">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="08e76-1242">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1242">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="08e76-1243">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-1243">New-AzStorageAccount</span></span>
* <span data-ttu-id="08e76-1244">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="08e76-1244">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="08e76-1245">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-1245">New-AzStorageAccount</span></span>
    - <span data-ttu-id="08e76-1246">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-1246">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="08e76-1247">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="08e76-1247">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1248">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1248">Az.Websites</span></span>
* <span data-ttu-id="08e76-1249">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="08e76-1249">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="08e76-1250">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="08e76-1250">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="08e76-1251">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1251">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08e76-1252">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="08e76-1252">Highlights since the last major release</span></span>
* <span data-ttu-id="08e76-1253">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="08e76-1253">General availability of `Az` module</span></span>
* <span data-ttu-id="08e76-1254">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="08e76-1254">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="08e76-1255">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="08e76-1255">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="08e76-1256">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1256">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="08e76-1257">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1257">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08e76-1258">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1258">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="08e76-1259">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1259">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08e76-1260">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1260">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1261">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1261">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="08e76-1262">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08e76-1262">Az.Batch</span></span>
* <span data-ttu-id="08e76-1263">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1263">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08e76-1264">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-1264">Az.Cdn</span></span>
* <span data-ttu-id="08e76-1265">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1265">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="08e76-1266">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1266">Az.CognitiveServices</span></span>
* <span data-ttu-id="08e76-1267">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1267">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1268">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1268">Az.Compute</span></span>
* <span data-ttu-id="08e76-1269">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1269">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="08e76-1270">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1270">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08e76-1271">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1271">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-1272">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-1272">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-1273">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1273">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1274">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1274">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1275">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1275">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="08e76-1276">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="08e76-1276">Az.EventGrid</span></span>
* <span data-ttu-id="08e76-1277">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1277">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-1278">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-1278">Az.EventHub</span></span>
* <span data-ttu-id="08e76-1279">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1279">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="08e76-1280">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="08e76-1280">Az.HDInsight</span></span>
* <span data-ttu-id="08e76-1281">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1281">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-1282">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-1282">Az.IotHub</span></span>
* <span data-ttu-id="08e76-1283">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1283">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08e76-1284">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-1284">Az.KeyVault</span></span>
* <span data-ttu-id="08e76-1285">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1285">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08e76-1286">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1286">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="08e76-1287">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="08e76-1287">Az.MachineLearning</span></span>
* <span data-ttu-id="08e76-1288">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1288">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="08e76-1289">Az.Media</span><span class="sxs-lookup"><span data-stu-id="08e76-1289">Az.Media</span></span>
* <span data-ttu-id="08e76-1290">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1290">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-1291">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-1291">Az.Monitor</span></span>
  * <span data-ttu-id="08e76-1292">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1292">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="08e76-1293">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="08e76-1293">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="08e76-1294">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="08e76-1294">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="08e76-1295">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="08e76-1295">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="08e76-1296">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="08e76-1296">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="08e76-1297">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="08e76-1297">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="08e76-1298">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1298">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1299">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1299">Az.Network</span></span>
* <span data-ttu-id="08e76-1300">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1300">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08e76-1301">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1301">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="08e76-1302">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="08e76-1302">Az.NotificationHubs</span></span>
* <span data-ttu-id="08e76-1303">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1303">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-1304">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1304">Az.OperationalInsights</span></span>
* <span data-ttu-id="08e76-1305">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1305">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="08e76-1306">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="08e76-1306">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="08e76-1307">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1307">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1308">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1308">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-1309">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1309">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08e76-1310">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1310">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="08e76-1311">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1311">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="08e76-1312">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1312">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="08e76-1313">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="08e76-1313">Az.RedisCache</span></span>
* <span data-ttu-id="08e76-1314">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1314">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1315">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1315">Az.Resources</span></span>
* <span data-ttu-id="08e76-1316">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1316">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1317">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1317">Az.Sql</span></span>
* <span data-ttu-id="08e76-1318">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="08e76-1318">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="08e76-1319">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1319">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08e76-1320">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1320">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="08e76-1321">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1321">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="08e76-1322">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="08e76-1322">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="08e76-1323">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="08e76-1323">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="08e76-1324">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1324">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1325">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1325">Az.Websites</span></span>
* <span data-ttu-id="08e76-1326">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1326">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="08e76-1327">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1327">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="08e76-1328">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1328">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="08e76-1329">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1329">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="08e76-1330">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1330">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08e76-1331">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="08e76-1331">Highlights since the last major release</span></span>
* <span data-ttu-id="08e76-1332">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="08e76-1332">General availability of `Az` module</span></span>
* <span data-ttu-id="08e76-1333">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="08e76-1333">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="08e76-1334">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="08e76-1334">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="08e76-1335">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1335">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="08e76-1336">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1336">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08e76-1337">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1337">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="08e76-1338">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1338">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="08e76-1339">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1339">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1340">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1340">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="08e76-1341">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1341">Az.AnalysisServices</span></span>
* <span data-ttu-id="08e76-1342">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="08e76-1342">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="08e76-1343">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1343">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-1344">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1344">Az.Automation</span></span>
* <span data-ttu-id="08e76-1345">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1345">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="08e76-1346">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1346">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="08e76-1347">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1347">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1348">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1348">Az.Compute</span></span>
* <span data-ttu-id="08e76-1349">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1349">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="08e76-1350">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1350">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="08e76-1351">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1351">Az.ContainerInstance</span></span>
* <span data-ttu-id="08e76-1352">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1352">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-1353">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-1353">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-1354">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1354">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="08e76-1355">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1355">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1356">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1356">Az.Resources</span></span>
* <span data-ttu-id="08e76-1357">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1357">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="08e76-1358">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1358">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="08e76-1359">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="08e76-1359">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="08e76-1360">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="08e76-1360">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="08e76-1361">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1361">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="08e76-1362">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="08e76-1362">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1363">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1363">Az.Sql</span></span>
* <span data-ttu-id="08e76-1364">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1364">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1365">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1365">Az.Storage</span></span>
* <span data-ttu-id="08e76-1366">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="08e76-1366">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="08e76-1367">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="08e76-1367">New-AzStorageContext</span></span>
* <span data-ttu-id="08e76-1368">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="08e76-1368">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="08e76-1369">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="08e76-1369">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="08e76-1370">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="08e76-1370">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="08e76-1371">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-1371">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="08e76-1372">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-1372">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="08e76-1373">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="08e76-1373">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="08e76-1374">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="08e76-1374">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="08e76-1375">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="08e76-1375">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="08e76-1376">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="08e76-1376">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="08e76-1377">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="08e76-1377">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="08e76-1378">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1378">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="08e76-1379">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="08e76-1379">Highlights since the last major release</span></span>
* <span data-ttu-id="08e76-1380">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="08e76-1380">General availability of `Az` module</span></span>
* <span data-ttu-id="08e76-1381">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="08e76-1381">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="08e76-1382">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="08e76-1382">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="08e76-1383">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1383">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="08e76-1384">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1384">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08e76-1385">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1385">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="08e76-1386">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1386">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-1387">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1387">Az.Automation</span></span>
* <span data-ttu-id="08e76-1388">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1388">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="08e76-1389">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="08e76-1389">Dynamic grouping</span></span>
    * <span data-ttu-id="08e76-1390">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="08e76-1390">Pre-Post script</span></span>
    * <span data-ttu-id="08e76-1391">再起動設定</span><span class="sxs-lookup"><span data-stu-id="08e76-1391">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1392">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1392">Az.Compute</span></span>
* <span data-ttu-id="08e76-1393">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1393">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="08e76-1394">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1394">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08e76-1395">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-1395">Az.KeyVault</span></span>
* <span data-ttu-id="08e76-1396">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1396">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1397">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1397">Az.Network</span></span>
* <span data-ttu-id="08e76-1398">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1398">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="08e76-1399">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1399">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1400">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1400">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-1401">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1401">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="08e76-1402">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1402">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1403">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1403">Az.Resources</span></span>
* <span data-ttu-id="08e76-1404">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1404">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="08e76-1405">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1405">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1406">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1406">Az.Sql</span></span>
* <span data-ttu-id="08e76-1407">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1407">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1408">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1408">Az.Storage</span></span>
* <span data-ttu-id="08e76-1409">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-1409">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="08e76-1410">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-1410">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="08e76-1411">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-1411">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="08e76-1412">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="08e76-1412">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="08e76-1413">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="08e76-1413">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="08e76-1414">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="08e76-1414">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="08e76-1415">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1415">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1416">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1416">Az.Websites</span></span>
* <span data-ttu-id="08e76-1417">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1417">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="08e76-1418">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1418">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-1419">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1419">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1420">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1420">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="08e76-1421">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1421">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-1422">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1422">Az.Automation</span></span>
* <span data-ttu-id="08e76-1423">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1423">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="08e76-1424">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1424">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="08e76-1425">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="08e76-1425">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08e76-1426">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-1426">Az.Cdn</span></span>
* <span data-ttu-id="08e76-1427">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-1427">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1428">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1428">Az.Compute</span></span>
* <span data-ttu-id="08e76-1429">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1429">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-1430">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-1430">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-1431">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1431">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08e76-1432">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08e76-1432">Az.LogicApp</span></span>
* <span data-ttu-id="08e76-1433">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1433">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1434">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1434">Az.Network</span></span>
* <span data-ttu-id="08e76-1435">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1435">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1436">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1436">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-1437">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1437">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="08e76-1438">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1438">SDK Update</span></span>
* <span data-ttu-id="08e76-1439">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1439">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="08e76-1440">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1440">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1441">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1441">Az.Resources</span></span>
* <span data-ttu-id="08e76-1442">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1442">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="08e76-1443">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="08e76-1443">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="08e76-1444">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1444">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="08e76-1445">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="08e76-1445">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="08e76-1446">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1446">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="08e76-1447">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="08e76-1447">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1448">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1448">Az.Sql</span></span>
* <span data-ttu-id="08e76-1449">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1449">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="08e76-1450">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1450">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1451">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1451">Az.Storage</span></span>
* <span data-ttu-id="08e76-1452">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="08e76-1452">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="08e76-1453">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1453">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="08e76-1454">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1454">Az.AnalysisServices</span></span>
* <span data-ttu-id="08e76-1455">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-1455">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-1456">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1456">Az.Automation</span></span>
* <span data-ttu-id="08e76-1457">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1457">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="08e76-1458">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1458">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="08e76-1459">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1459">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="08e76-1460">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1460">Az.CognitiveServices</span></span>
* <span data-ttu-id="08e76-1461">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1461">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1462">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1462">Az.Compute</span></span>
* <span data-ttu-id="08e76-1463">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1463">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="08e76-1464">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1464">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="08e76-1465">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1465">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="08e76-1466">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="08e76-1466">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1467">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1467">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1468">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1468">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="08e76-1469">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="08e76-1469">Az.EventHub</span></span>
* <span data-ttu-id="08e76-1470">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1470">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="08e76-1471">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-1471">Az.KeyVault</span></span>
* <span data-ttu-id="08e76-1472">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1472">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08e76-1473">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08e76-1473">Az.LogicApp</span></span>
* <span data-ttu-id="08e76-1474">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1474">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="08e76-1475">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1475">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="08e76-1476">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1476">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="08e76-1477">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08e76-1477">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="08e76-1478">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08e76-1478">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="08e76-1479">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08e76-1479">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="08e76-1480">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="08e76-1480">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="08e76-1481">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1481">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="08e76-1482">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08e76-1482">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="08e76-1483">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08e76-1483">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="08e76-1484">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08e76-1484">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="08e76-1485">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="08e76-1485">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="08e76-1486">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1486">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="08e76-1487">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-1487">Az.Monitor</span></span>
* <span data-ttu-id="08e76-1488">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1488">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1489">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1489">Az.Network</span></span>
* <span data-ttu-id="08e76-1490">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1490">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-1491">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1491">Az.OperationalInsights</span></span>
* <span data-ttu-id="08e76-1492">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1492">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="08e76-1493">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1493">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="08e76-1494">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1494">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="08e76-1495">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1495">Az.Resources</span></span>
* <span data-ttu-id="08e76-1496">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="08e76-1496">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="08e76-1497">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="08e76-1497">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="08e76-1498">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="08e76-1498">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="08e76-1499">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1499">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1500">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1500">Az.Sql</span></span>
* <span data-ttu-id="08e76-1501">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1501">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="08e76-1502">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1502">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1503">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1503">Az.Websites</span></span>
* <span data-ttu-id="08e76-1504">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1504">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="08e76-1505">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1505">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-1506">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1506">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1507">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1507">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="08e76-1508">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1508">Az.AnalysisServices</span></span>
<span data-ttu-id="08e76-1509">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="08e76-1509">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1510">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1510">Az.Compute</span></span>
* <span data-ttu-id="08e76-1511">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1511">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="08e76-1512">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1512">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="08e76-1513">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1513">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1514">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1514">Az.RecoveryServices</span></span>
<span data-ttu-id="08e76-1515">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="08e76-1515">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1516">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1516">Az.Resources</span></span>
* <span data-ttu-id="08e76-1517">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1517">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="08e76-1518">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="08e76-1518">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="08e76-1519">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1519">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="08e76-1520">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="08e76-1520">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1521">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1521">Az.Sql</span></span>
* <span data-ttu-id="08e76-1522">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1522">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="08e76-1523">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1523">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="08e76-1524">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1524">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="08e76-1525">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1525">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-1526">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1526">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1527">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="08e76-1527">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="08e76-1528">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1528">Az.AnalysisServices</span></span>
* <span data-ttu-id="08e76-1529">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="08e76-1529">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1530">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1530">Az.RecoveryServices</span></span>
* <span data-ttu-id="08e76-1531">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="08e76-1531">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="08e76-1532">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1532">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-1533">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1533">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1534">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1534">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="08e76-1535">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1535">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08e76-1536">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1536">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="08e76-1537">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="08e76-1537">Az.Aks</span></span>
* <span data-ttu-id="08e76-1538">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1538">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="08e76-1539">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1539">Az.Automation</span></span>
* <span data-ttu-id="08e76-1540">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1540">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="08e76-1541">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1541">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="08e76-1542">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="08e76-1542">Az.Cdn</span></span>
* <span data-ttu-id="08e76-1543">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1543">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1544">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1544">Az.Compute</span></span>
* <span data-ttu-id="08e76-1545">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1545">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="08e76-1546">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1546">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="08e76-1547">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1547">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="08e76-1548">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="08e76-1548">Az.ContainerRegistry</span></span>
* <span data-ttu-id="08e76-1549">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1549">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="08e76-1550">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="08e76-1550">Az.DataFactory</span></span>
* <span data-ttu-id="08e76-1551">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1551">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1552">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1552">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1553">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="08e76-1553">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="08e76-1554">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="08e76-1554">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="08e76-1555">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1555">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-1556">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-1556">Az.IotHub</span></span>
* <span data-ttu-id="08e76-1557">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1557">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="08e76-1558">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-1558">Az.KeyVault</span></span>
* <span data-ttu-id="08e76-1559">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1559">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1560">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1560">Az.Network</span></span>
* <span data-ttu-id="08e76-1561">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1561">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1562">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1562">Az.Resources</span></span>
* <span data-ttu-id="08e76-1563">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1563">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="08e76-1564">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1564">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="08e76-1565">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1565">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="08e76-1566">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="08e76-1566">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="08e76-1567">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="08e76-1567">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="08e76-1568">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1568">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="08e76-1569">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="08e76-1569">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-1570">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1570">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-1571">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="08e76-1571">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="08e76-1572">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1572">Fix some error messages.</span></span>
* <span data-ttu-id="08e76-1573">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1573">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="08e76-1574">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1574">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="08e76-1575">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="08e76-1575">Az.SignalR</span></span>
* <span data-ttu-id="08e76-1576">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1576">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1577">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1577">Az.Sql</span></span>
* <span data-ttu-id="08e76-1578">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1578">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08e76-1579">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1579">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="08e76-1580">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1580">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="08e76-1581">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-1581">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1582">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1582">Az.Storage</span></span>
* <span data-ttu-id="08e76-1583">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1583">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08e76-1584">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="08e76-1584">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="08e76-1585">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="08e76-1585">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="08e76-1586">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="08e76-1586">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="08e76-1587">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="08e76-1587">Az.TrafficManager</span></span>
* <span data-ttu-id="08e76-1588">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1588">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1589">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1589">Az.Websites</span></span>
* <span data-ttu-id="08e76-1590">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1590">Update incorrect online help URLs</span></span>
* <span data-ttu-id="08e76-1591">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1591">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="08e76-1592">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="08e76-1592">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="08e76-1593">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1593">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="08e76-1594">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1594">Az.Accounts</span></span>
* <span data-ttu-id="08e76-1595">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="08e76-1595">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1596">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1596">Az.Compute</span></span>
* <span data-ttu-id="08e76-1597">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1597">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="08e76-1598">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="08e76-1598">Updated the description of ID in help files</span></span>
* <span data-ttu-id="08e76-1599">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1599">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1600">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1600">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1601">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1601">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="08e76-1602">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1602">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="08e76-1603">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="08e76-1603">Az.EventGrid</span></span>
* <span data-ttu-id="08e76-1604">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1604">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="08e76-1605">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="08e76-1605">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="08e76-1606">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="08e76-1606">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="08e76-1607">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="08e76-1607">Event Time-To-Live,</span></span>
        - <span data-ttu-id="08e76-1608">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="08e76-1608">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="08e76-1609">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="08e76-1609">Dead letter endpoint.</span></span>
    - <span data-ttu-id="08e76-1610">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="08e76-1610">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="08e76-1611">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="08e76-1611">Event Time-To-Live,</span></span>
        - <span data-ttu-id="08e76-1612">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="08e76-1612">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="08e76-1613">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="08e76-1613">Dead letter endpoint.</span></span>
* <span data-ttu-id="08e76-1614">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1614">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="08e76-1615">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1615">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="08e76-1616">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="08e76-1616">Az.IotHub</span></span>
* <span data-ttu-id="08e76-1617">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1617">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="08e76-1618">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="08e76-1618">Az.LogicApp</span></span>
* <span data-ttu-id="08e76-1619">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="08e76-1619">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1620">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1620">Az.Resources</span></span>
* <span data-ttu-id="08e76-1621">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1621">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="08e76-1622">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="08e76-1622">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="08e76-1623">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1623">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="08e76-1624">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1624">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="08e76-1625">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="08e76-1625">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="08e76-1626">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="08e76-1626">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="08e76-1627">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="08e76-1627">Az.SignalR</span></span>
* <span data-ttu-id="08e76-1628">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1628">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1629">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1629">Az.Sql</span></span>
* <span data-ttu-id="08e76-1630">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1630">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="08e76-1631">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1631">Az.Storage</span></span>
* <span data-ttu-id="08e76-1632">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="08e76-1632">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="08e76-1633">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="08e76-1633">New-AzStorageContext</span></span>
* <span data-ttu-id="08e76-1634">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1634">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="08e76-1635">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="08e76-1635">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1636">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1636">Az.Websites</span></span>
* <span data-ttu-id="08e76-1637">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1637">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="08e76-1638">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1638">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="08e76-1639">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1639">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="08e76-1640">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-1640">General</span></span>

- <span data-ttu-id="08e76-1641">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="08e76-1641">General Availability of Az Module</span></span>
- <span data-ttu-id="08e76-1642">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="08e76-1642">Online help for each module</span></span>
- <span data-ttu-id="08e76-1643">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1643">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="08e76-1644">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1644">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="08e76-1645">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="08e76-1645">Az.Accounts</span></span>
- <span data-ttu-id="08e76-1646">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1646">Changed from Az.Profile</span></span>
- <span data-ttu-id="08e76-1647">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1647">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="08e76-1648">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-1648">Az.ApiManagement</span></span>
- <span data-ttu-id="08e76-1649">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="08e76-1649">Fixes for #7002</span></span>
- <span data-ttu-id="08e76-1650">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1650">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="08e76-1651">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="08e76-1651">Az.Batch</span></span>
- <span data-ttu-id="08e76-1652">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1652">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="08e76-1653">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1653">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="08e76-1654">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1654">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="08e76-1655">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="08e76-1655">Az.Billing</span></span>
- <span data-ttu-id="08e76-1656">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1656">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="08e76-1657">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1657">Az.CognitivServices</span></span>
- <span data-ttu-id="08e76-1658">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1658">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="08e76-1659">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1659">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="08e76-1660">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1660">Az.ContainerInstance</span></span>
- <span data-ttu-id="08e76-1661">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1661">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="08e76-1662">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="08e76-1662">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="08e76-1663">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1663">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1664">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1664">Az.DataLakeStore</span></span>
- <span data-ttu-id="08e76-1665">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1665">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="08e76-1666">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="08e76-1666">Az.Monitor</span></span>
- <span data-ttu-id="08e76-1667">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1667">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="08e76-1668">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="08e76-1668">Az.KeyVault</span></span>
- <span data-ttu-id="08e76-1669">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1669">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="08e76-1670">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="08e76-1670">Az.MachineLearning</span></span>
- <span data-ttu-id="08e76-1671">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="08e76-1671">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="08e76-1672">Az.Media</span><span class="sxs-lookup"><span data-stu-id="08e76-1672">Az.Media</span></span>
- <span data-ttu-id="08e76-1673">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1673">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="08e76-1674">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1674">Az.Network</span></span>
<span data-ttu-id="08e76-1675">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1675">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="08e76-1676">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-1676">New cmdlets added:</span></span>
        - <span data-ttu-id="08e76-1677">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-1677">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08e76-1678">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-1678">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08e76-1679">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-1679">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08e76-1680">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-1680">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08e76-1681">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="08e76-1681">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="08e76-1682">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1682">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="08e76-1683">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="08e76-1683">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="08e76-1684">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="08e76-1684">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="08e76-1685">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1685">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="08e76-1686">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="08e76-1686">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="08e76-1687">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1687">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="08e76-1688">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="08e76-1688">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="08e76-1689">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-1689">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="08e76-1690">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-1690">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="08e76-1691">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1691">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="08e76-1692">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1692">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="08e76-1693">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="08e76-1693">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="08e76-1694">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="08e76-1694">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="08e76-1695">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="08e76-1695">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="08e76-1696">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1696">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="08e76-1697">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1697">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="08e76-1698">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1698">Az.OperationalInsights</span></span>
- <span data-ttu-id="08e76-1699">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1699">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="08e76-1700">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08e76-1700">Az.Profile</span></span>
- <span data-ttu-id="08e76-1701">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1701">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1702">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1702">Az.RecoveryServices</span></span>
- <span data-ttu-id="08e76-1703">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1703">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="08e76-1704">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1704">Az.Resources</span></span>
- <span data-ttu-id="08e76-1705">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1705">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="08e76-1706">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1706">Az.ServiceFabric</span></span>
- <span data-ttu-id="08e76-1707">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="08e76-1707">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="08e76-1708">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1708">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="08e76-1709">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="08e76-1709">Az.SIgnalR</span></span>
- <span data-ttu-id="08e76-1710">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="08e76-1710">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="08e76-1711">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1711">Az.Sql</span></span>
- <span data-ttu-id="08e76-1712">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1712">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="08e76-1713">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1713">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="08e76-1714">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1714">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="08e76-1715">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1715">Az.Storage</span></span>
- <span data-ttu-id="08e76-1716">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1716">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="08e76-1717">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1717">Az.Websites</span></span>
- <span data-ttu-id="08e76-1718">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="08e76-1718">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="08e76-1719">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1719">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="08e76-1720">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-1720">General</span></span>

* <span data-ttu-id="08e76-1721">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="08e76-1721">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="08e76-1722">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1722">Az.Compute</span></span>

* <span data-ttu-id="08e76-1723">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1723">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1724">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1724">Az.DataLakeStore</span></span>

* <span data-ttu-id="08e76-1725">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1725">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="08e76-1726">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="08e76-1726">Az.FrontDoor</span></span>

* <span data-ttu-id="08e76-1727">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1727">Fixed some broken links</span></span>
    - <span data-ttu-id="08e76-1728">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1728">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="08e76-1729">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1729">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="08e76-1730">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1730">Az.RecoveryServices</span></span>

* <span data-ttu-id="08e76-1731">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1731">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="08e76-1732">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1732">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="08e76-1733">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1733">Az.Resources</span></span>

* <span data-ttu-id="08e76-1734">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1734">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="08e76-1735">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1735">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="08e76-1736">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1736">Az.Sql</span></span>

* <span data-ttu-id="08e76-1737">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="08e76-1737">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="08e76-1738">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1738">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="08e76-1739">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1739">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="08e76-1740">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1740">Az.Storage</span></span>

* <span data-ttu-id="08e76-1741">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1741">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="08e76-1742">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1742">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="08e76-1743">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="08e76-1743">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="08e76-1744">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="08e76-1744">Support Static Website configuration</span></span>
    - <span data-ttu-id="08e76-1745">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="08e76-1745">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="08e76-1746">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="08e76-1746">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="08e76-1747">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1747">Az.Websites</span></span>

* <span data-ttu-id="08e76-1748">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="08e76-1748">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="08e76-1749">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1749">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="08e76-1750">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="08e76-1750">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="08e76-1751">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1751">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="08e76-1752">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="08e76-1752">Az.ApiManagement</span></span>
* <span data-ttu-id="08e76-1753">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1753">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="08e76-1754">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="08e76-1754">Az.Automation</span></span>
* <span data-ttu-id="08e76-1755">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="08e76-1755">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="08e76-1756">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1756">Added Update Management cmdlets</span></span>
* <span data-ttu-id="08e76-1757">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1757">Added Source Control cmdlets</span></span>
* <span data-ttu-id="08e76-1758">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1758">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="08e76-1759">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1759">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="08e76-1760">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1760">Az.Compute</span></span>
* <span data-ttu-id="08e76-1761">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1761">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="08e76-1762">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1762">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="08e76-1763">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1763">Az.ContainerInstance</span></span>
* <span data-ttu-id="08e76-1764">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1764">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="08e76-1765">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="08e76-1765">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="08e76-1766">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1766">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="08e76-1767">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1767">Az.Network</span></span>
* <span data-ttu-id="08e76-1768">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1768">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="08e76-1769">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1769">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="08e76-1770">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1770">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="08e76-1771">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1771">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="08e76-1772">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="08e76-1772">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="08e76-1773">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1773">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="08e76-1774">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1774">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="08e76-1775">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="08e76-1775">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="08e76-1776">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1776">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="08e76-1777">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1777">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="08e76-1778">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="08e76-1778">Az.Relay</span></span>
* <span data-ttu-id="08e76-1779">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="08e76-1779">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="08e76-1780">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1780">Az.Resources</span></span>
* <span data-ttu-id="08e76-1781">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1781">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="08e76-1782">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1782">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="08e76-1783">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="08e76-1783">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="08e76-1784">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1784">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-1785">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1785">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="08e76-1786">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1786">Az.Sql</span></span>
* <span data-ttu-id="08e76-1787">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1787">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="08e76-1788">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1788">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08e76-1789">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1789">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08e76-1790">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1790">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08e76-1791">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="08e76-1791">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="08e76-1792">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08e76-1792">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="08e76-1793">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08e76-1793">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="08e76-1794">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08e76-1794">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="08e76-1795">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="08e76-1795">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="08e76-1796">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="08e76-1796">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="08e76-1797">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1797">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="08e76-1798">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1798">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="08e76-1799">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="08e76-1799">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="08e76-1800">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="08e76-1800">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="08e76-1801">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="08e76-1801">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="08e76-1802">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="08e76-1802">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="08e76-1803">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1803">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="08e76-1804">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1804">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="08e76-1805">全般</span><span class="sxs-lookup"><span data-stu-id="08e76-1805">General</span></span>
* <span data-ttu-id="08e76-1806">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="08e76-1806">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="08e76-1807">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08e76-1807">Az.Profile</span></span>
* <span data-ttu-id="08e76-1808">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1808">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="08e76-1809">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1809">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="08e76-1810">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1810">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="08e76-1811">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1811">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="08e76-1812">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1812">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="08e76-1813">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1813">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="08e76-1814">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1814">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="08e76-1815">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1815">Az.CognitiveServices</span></span>
* <span data-ttu-id="08e76-1816">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1816">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1817">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1817">Az.Compute</span></span>
* <span data-ttu-id="08e76-1818">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1818">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="08e76-1819">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="08e76-1819">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="08e76-1820">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1820">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1821">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1821">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1822">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1822">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="08e76-1823">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1823">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="08e76-1824">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="08e76-1824">Az.Insights</span></span>
* <span data-ttu-id="08e76-1825">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1825">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="08e76-1826">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="08e76-1826">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="08e76-1827">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1827">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="08e76-1828">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="08e76-1828">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1829">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1829">Az.Network</span></span>
* <span data-ttu-id="08e76-1830">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="08e76-1830">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="08e76-1831">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="08e76-1831">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="08e76-1832">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="08e76-1832">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="08e76-1833">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="08e76-1833">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="08e76-1834">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="08e76-1834">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="08e76-1835">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="08e76-1835">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="08e76-1836">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="08e76-1836">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="08e76-1837">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="08e76-1837">Az.PolicyInsights</span></span>
* <span data-ttu-id="08e76-1838">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1838">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1839">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1839">Az.Resources</span></span>
* <span data-ttu-id="08e76-1840">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1840">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="08e76-1841">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1841">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="08e76-1842">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="08e76-1842">Az.ServiceBus</span></span>
* <span data-ttu-id="08e76-1843">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1843">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="08e76-1844">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="08e76-1844">Az.ServiceFabric</span></span>
* <span data-ttu-id="08e76-1845">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1845">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="08e76-1846">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1846">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="08e76-1847">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="08e76-1847">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="08e76-1848">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="08e76-1848">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="08e76-1849">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1849">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="08e76-1850">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1850">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="08e76-1851">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="08e76-1851">Az.Profile</span></span>
* <span data-ttu-id="08e76-1852">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1852">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="08e76-1853">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1853">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1854">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1854">Az.Compute</span></span>
* <span data-ttu-id="08e76-1855">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1855">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="08e76-1856">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1856">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="08e76-1857">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="08e76-1857">Az.DataLakeStore</span></span>
* <span data-ttu-id="08e76-1858">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1858">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="08e76-1859">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1859">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="08e76-1860">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1860">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="08e76-1861">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1861">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="08e76-1862">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="08e76-1862">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1863">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1863">Az.Network</span></span>
* <span data-ttu-id="08e76-1864">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1864">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="08e76-1865">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1865">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1866">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1866">Az.Resources</span></span>
* <span data-ttu-id="08e76-1867">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1867">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="08e76-1868">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1868">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="08e76-1869">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1869">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="08e76-1870">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="08e76-1870">Azure.Storage</span></span>
* <span data-ttu-id="08e76-1871">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1871">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="08e76-1872">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="08e76-1872">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="08e76-1873">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="08e76-1873">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="08e76-1874">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1874">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="08e76-1875">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="08e76-1875">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="08e76-1876">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="08e76-1876">Az.CognitiveServices</span></span>
* <span data-ttu-id="08e76-1877">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1877">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="08e76-1878">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="08e76-1878">Az.Compute</span></span>
* <span data-ttu-id="08e76-1879">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1879">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="08e76-1880">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1880">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="08e76-1881">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1881">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="08e76-1882">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="08e76-1882">Az.DataFactoryV2</span></span>
* <span data-ttu-id="08e76-1883">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1883">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="08e76-1884">Az.Network</span><span class="sxs-lookup"><span data-stu-id="08e76-1884">Az.Network</span></span>
* <span data-ttu-id="08e76-1885">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="08e76-1885">Added NetworkProfile functionality.</span></span> <span data-ttu-id="08e76-1886">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="08e76-1886">new cmdlets added</span></span>
    - <span data-ttu-id="08e76-1887">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08e76-1887">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="08e76-1888">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08e76-1888">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="08e76-1889">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08e76-1889">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="08e76-1890">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="08e76-1890">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="08e76-1891">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-1891">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="08e76-1892">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="08e76-1892">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="08e76-1893">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1893">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="08e76-1894">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1894">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="08e76-1895">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1895">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="08e76-1896">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="08e76-1896">Az.RedisCache</span></span>
* <span data-ttu-id="08e76-1897">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="08e76-1897">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="08e76-1898">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1898">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="08e76-1899">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="08e76-1899">Az.Resources</span></span>
* <span data-ttu-id="08e76-1900">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1900">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="08e76-1901">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1901">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="08e76-1902">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="08e76-1902">Az.Sql</span></span>
* <span data-ttu-id="08e76-1903">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="08e76-1903">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="08e76-1904">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="08e76-1904">Az.Websites</span></span>
* <span data-ttu-id="08e76-1905">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="08e76-1905">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="08e76-1906">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="08e76-1906">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="08e76-1907">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="08e76-1907">0.2.0 - September 2018</span></span>
 <span data-ttu-id="08e76-1908">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="08e76-1908">Initial Release</span></span>
