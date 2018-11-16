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
ms.openlocfilehash: 8a7b184ed06eb078956229fa67d02840014e3aaf
ms.sourcegitcommit: 4afdba3cd7e1d348876ce59f3503fdcd258f79ab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/15/2018
ms.locfileid: "51574534"
---
# <a name="release-notes"></a><span data-ttu-id="2eb97-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="2eb97-103">Release notes</span></span>

<span data-ttu-id="2eb97-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="2eb97-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6120---november-2018"></a><span data-ttu-id="2eb97-105">6.12.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-105">6.12.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-106">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-107">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-107">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="2eb97-108">Connect-AzureRmAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-108">Rename param TenantId in cmdlet Connect-AzureRmAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="2eb97-109">Connect-AzureRmAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-109">Updated TenantId description for Connect-AzureRmAccount</span></span>
* <span data-ttu-id="2eb97-110">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-110">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="2eb97-111">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-111">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="2eb97-112">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-112">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="2eb97-113">接続されていない場合に "Disconnect-AzureRmAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-113">Fix issue where 'Disconnect-AzureRmAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a><span data-ttu-id="2eb97-114">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="2eb97-114">AzureRM.Automation</span></span>
* <span data-ttu-id="2eb97-115">コマンドレット DLL ファイルの名前を Microsoft.Azure.Commands.Automation.dll に変更しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-115">Renamed cmdlet DLL filename to Microsoft.Azure.Commands.Automation.dll</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="2eb97-116">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-116">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="2eb97-117">Get-AzureRmCognitiveServicesAccountSkus 操作を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-117">Add Get-AzureRmCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-118">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-118">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-119">Add-AzureRmVmssVMDataDisk および Remove-AzureRmVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-119">Add Add-AzureRmVmssVMDataDisk and Remove-AzureRmVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="2eb97-120">Get-AzureRmVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="2eb97-120">Get-AzureRmVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="2eb97-121">SetAzureRmVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式では設定されません。</span><span class="sxs-lookup"><span data-stu-id="2eb97-121">Fixed SetAzureRmVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="2eb97-122">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2eb97-122">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="2eb97-123">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-123">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="2eb97-124">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-124">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="2eb97-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="2eb97-125">AzureRM.Insights</span></span>
* <span data-ttu-id="2eb97-126">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-126">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="2eb97-127">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="2eb97-127">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="2eb97-128">Set-AzureRMDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-128">Fixed issue #7513 [Insights] Set-AzureRMDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="2eb97-129">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="2eb97-129">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-130">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-130">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-131">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="2eb97-131">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="2eb97-132">Get-AzureRmExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="2eb97-132">Get-AzureRmExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="2eb97-133">Get-AzureRmExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="2eb97-133">Get-AzureRmExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="2eb97-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="2eb97-134">Get-AzureRmExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="2eb97-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="2eb97-135">Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="2eb97-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="2eb97-136">Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="2eb97-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="2eb97-137">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="2eb97-138">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2eb97-138">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="2eb97-139">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-139">Added policy remediation cmdlets</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="2eb97-140">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2eb97-140">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="2eb97-141">Recovery Services で Azure ファイル共有のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-141">Added support for azure file shares in recovery services.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-142">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-142">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-143">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-143">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="2eb97-144">"Get-AzureRmResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-144">Allow listing resources using the '-ResourceId' parameter for 'Get-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-145">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-145">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-146">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-146">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="2eb97-147">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2eb97-147">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="2eb97-148">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-148">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="2eb97-149">"Add-AzureRmServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-149">Fix 'Add-AzureRmServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="2eb97-150">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="2eb97-150">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="2eb97-151">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="2eb97-151">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="2eb97-152">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzureRmServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-152">Fix 'Update-AzureRmServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="6110---october-2018"></a><span data-ttu-id="2eb97-153">6.11.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-153">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-154">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-154">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-155">CloudShell での Get-AzureRmSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-155">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="2eb97-156">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-156">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="2eb97-157">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="2eb97-157">AzureRM.Backup</span></span>
* <span data-ttu-id="2eb97-158">Azure Backup コマンドレットを非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-158">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-159">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-159">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-160">"New-AzureRmVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-160">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="2eb97-161">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-161">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="2eb97-162">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2eb97-162">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="2eb97-163">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-163">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="2eb97-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2eb97-164">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="2eb97-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="2eb97-165">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="2eb97-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウントの指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="2eb97-166">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="2eb97-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="2eb97-167">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-168">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-168">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-169">プロトコル値をバックエンドに渡すように、Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-169">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="2eb97-170">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-170">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-171">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-171">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-172">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzureRMRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-172">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="2eb97-173">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-173">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="2eb97-174">6.10.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-174">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="2eb97-175">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-175">Azure.Storage</span></span>
* <span data-ttu-id="2eb97-176">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-176">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="2eb97-177">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="2eb97-177">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="2eb97-178">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="2eb97-178">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="2eb97-179">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-179">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="2eb97-180">既存のアカウントなしでの Get-AzureRmCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-180">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-181">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-181">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-182">必要に応じて 50 を超える結果が返されるように Get-AzureRmVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-182">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="2eb97-183">"SimpleParameterSet" の例を New-AzureRmVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-183">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="2eb97-184">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-184">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="2eb97-185">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2eb97-185">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="2eb97-186">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-186">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-187">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-187">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-188">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-188">Added NetworkProfile functionality.</span></span> <span data-ttu-id="2eb97-189">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2eb97-189">new cmdlets added</span></span>
    - <span data-ttu-id="2eb97-190">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2eb97-190">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="2eb97-191">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2eb97-191">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="2eb97-192">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2eb97-192">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="2eb97-193">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2eb97-193">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="2eb97-194">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-194">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="2eb97-195">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-195">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="2eb97-196">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-196">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="2eb97-197">New-AzureRmVirtualNetworkTap、Get-AzureRmVirtualNetworkTap、Set-AzureRmVirtualNetworkTap、Remove-AzureRmVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-197">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="2eb97-198">Set-AzureRmNEtworkInterfaceTapConfig、Get-AzureRmNEtworkInterfaceTapConfig、Remove-AzureRmNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-198">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="2eb97-199">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2eb97-199">AzureRM.RedisCache</span></span>
* <span data-ttu-id="2eb97-200">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-200">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="2eb97-201">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-201">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-202">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-202">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-203">欠落していた -Mode パラメーターを Set-AzureRmPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-203">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="2eb97-204">配信元にユーザーが含まれる操作について Get-AzureRmProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-204">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-205">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-205">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-206">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-206">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="2eb97-207">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-207">AzureRM.Storage</span></span>
* <span data-ttu-id="2eb97-208">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-208">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="2eb97-209">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="2eb97-209">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-210">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-210">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-211">新しいコマンドレット: Get-AzureRMWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="2eb97-211">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="2eb97-212">新しいコマンドレット: New-AzureRMWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="2eb97-212">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="2eb97-213">6.9.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-213">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2eb97-214">全般</span><span class="sxs-lookup"><span data-stu-id="2eb97-214">General</span></span>
* <span data-ttu-id="2eb97-215">AzureRM.SignalR が AzureRM ロールアップ モジュールに追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-215">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-216">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-216">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-217">ストレージの一般的なコードに対する軽微な変更</span><span class="sxs-lookup"><span data-stu-id="2eb97-217">Minor changes to the storage common code</span></span>
* <span data-ttu-id="2eb97-218">完全なパラメーター型を含めるようにヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-218">Updated help files to include full parameter types.</span></span>
* <span data-ttu-id="2eb97-219">ServicePrincipalCertificateWithSubscriptionId パラメーター セットの -ServicePrincipal を "任意" に変更しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-219">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="2eb97-220">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-220">Azure.Storage</span></span>
* <span data-ttu-id="2eb97-221">OAuth でのストレージ コンテキストの作成がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-221">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="2eb97-222">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="2eb97-222">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="2eb97-223">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="2eb97-223">AzureRM.Cdn</span></span>
* <span data-ttu-id="2eb97-224">CDN 価格 SKU に Standard_Microsoft を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-224">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-225">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-225">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-226">Keyvault および Storage への依存関係を一般的な依存関係に移動しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-226">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="2eb97-227">より多くの仮想マシンのサイズのサポートを AEM コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-227">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="2eb97-228">PublicIPPrefix パラメーターを New-AzureRmVmssIpConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-228">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="2eb97-229">ResourceId パラメーターを Invoke-AzureRmVMRunCommand コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-229">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="2eb97-230">Invoke-AzureRmVmssVMRunCommand コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-230">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="2eb97-231">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="2eb97-231">AzureRM.Dns</span></span>
* <span data-ttu-id="2eb97-232">DNS レコード作成中のエイリアス レコードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-232">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="2eb97-233">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="2eb97-233">AzureRM.Insights</span></span>
* <span data-ttu-id="2eb97-234">#6833 および #7102 の問題を修正しました (診断設定領域)</span><span class="sxs-lookup"><span data-stu-id="2eb97-234">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="2eb97-235">診断設定の作成および表示/取得中の既定の名前 ("service") に関する問題</span><span class="sxs-lookup"><span data-stu-id="2eb97-235">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="2eb97-236">カテゴリでの診断設定の作成に関する問題</span><span class="sxs-lookup"><span data-stu-id="2eb97-236">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="2eb97-237">メトリック時間グレイン パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-237">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="2eb97-238">Timegrains パラメーターは引き続き利用できますが (これは破壊的変更ではありません)、PT1M のみが有効であるため、バックエンドでは無視されます</span><span class="sxs-lookup"><span data-stu-id="2eb97-238">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-239">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-239">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-240">LoadBalancer コマンドレットへの変更</span><span class="sxs-lookup"><span data-stu-id="2eb97-240">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="2eb97-241">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes パラメーター、EnableFloatingIp パラメーター、EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-241">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="2eb97-242">LoadBalancerInboundNatRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-242">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="2eb97-243">LoadBalancerRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-243">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="2eb97-244">LoadBalancerProbeConfig: Protocol パラメーターの "HTTPS" 値のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-244">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="2eb97-245">新しい LoadBalancer のサブリソース OutboundRule について新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-245">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="2eb97-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-246">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="2eb97-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-247">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="2eb97-248">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-248">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="2eb97-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-249">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="2eb97-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-250">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="2eb97-251">PSNetworkInterface の新しい HostedWorkloads プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-251">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="2eb97-252">ARM 経由の Azure Firewall 機能のために新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-252">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="2eb97-253">Get-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-253">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="2eb97-254">Set-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-254">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="2eb97-255">New-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-255">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="2eb97-256">Remove-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-256">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="2eb97-257">New-AzureRmFirewallApplicationRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-257">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="2eb97-258">New-AzureRmFirewallApplicationRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-258">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="2eb97-259">New-AzureRmFirewallNatRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-259">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="2eb97-260">New-AzureRmFirewallNatRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-260">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="2eb97-261">New-AzureRmFirewallNetworkRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-261">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="2eb97-262">New-AzureRmFirewallNetworkRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-262">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="2eb97-263">Application Gateway での信頼されたルート証明書と自動スケーリング構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-263">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="2eb97-264">追加された新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2eb97-264">New Cmdlets added:</span></span>
      - <span data-ttu-id="2eb97-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-265">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="2eb97-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-266">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="2eb97-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-267">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="2eb97-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-268">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="2eb97-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-269">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="2eb97-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-270">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="2eb97-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-271">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="2eb97-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-272">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="2eb97-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-273">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="2eb97-274">省略可能なパラメーターで更新されたコマンドレット -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-274">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="2eb97-275">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="2eb97-275">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="2eb97-276">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="2eb97-276">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="2eb97-277">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="2eb97-277">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="2eb97-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="2eb97-278">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="2eb97-279">省略可能なパラメーターで更新されたコマンドレット - AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-279">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="2eb97-280">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="2eb97-280">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="2eb97-281">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="2eb97-281">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="2eb97-282">インターフェイス エンドポイントのコマンドレット Get-AzureInterfaceEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-282">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="2eb97-283">サブネットでの複数のアドレス プレフィックスのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-283">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="2eb97-284">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2eb97-284">Updated cmdlets:</span></span>
  - <span data-ttu-id="2eb97-285">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-285">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="2eb97-286">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-286">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="2eb97-287">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-287">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="2eb97-288">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-288">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="2eb97-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-289">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="2eb97-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-290">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="2eb97-291">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-291">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="2eb97-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-292">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="2eb97-293">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-293">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="2eb97-294">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-294">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="2eb97-295">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-295">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="2eb97-296">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-296">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="2eb97-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-297">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="2eb97-298">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-298">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="2eb97-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-299">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="2eb97-300">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-300">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="2eb97-301">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-301">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="2eb97-302">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-302">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="2eb97-303">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="2eb97-303">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="2eb97-304">サブネット委任のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-304">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="2eb97-305">New-AzureRmDelegation: 新しい委任を作成します。これはサブネットに追加できます</span><span class="sxs-lookup"><span data-stu-id="2eb97-305">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="2eb97-306">Remove-AzureRmDelegation: サブネットを受け取り、指定された委任の名前をそのサブネットから削除します</span><span class="sxs-lookup"><span data-stu-id="2eb97-306">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="2eb97-307">Add-AzureRmDelegation: サブネットを受け取り、指定されたサービス名を委任としてそのサブネットに追加します</span><span class="sxs-lookup"><span data-stu-id="2eb97-307">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="2eb97-308">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="2eb97-308">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="2eb97-309">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="2eb97-309">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="2eb97-310">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="2eb97-310">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="2eb97-311">管理対象のマネージド ディスクのサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-311">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="2eb97-312">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2eb97-312">AzureRM.RedisCache</span></span>
* <span data-ttu-id="2eb97-313">Insights の依存関係を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-313">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-314">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-314">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-315">New-AzureRmResourceGroupDeployment を新しい RollbackAction パラメーターで更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-315">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="2eb97-316">新しいパラメーターを使用して OnErrorDeployment のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-316">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="2eb97-317">ポリシー割り当てでマネージド ID をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2eb97-317">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="2eb97-318">"New-AzureRmPolicyAssignment" を指定してポリシーを割り当てるとき、既定値を持つパラメーターが不要になりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-318">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="2eb97-319">ポリシー エイリアスを取得するための新しい Get AzureRmPolicyAlias コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-319">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-320">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-320">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-321">問題 #7161 を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-321">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="2eb97-322">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="2eb97-322">AzureRM.SignalR</span></span>
* <span data-ttu-id="2eb97-323">SKU 名を Free_F1 および Standard_S1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-323">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="2eb97-324">バージョン フィールドを PSSignalRResource オブジェクトに、接続文字列を PSSignalRKeys オブジェクトに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-324">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="2eb97-325">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-325">AzureRM.Storage</span></span>
* <span data-ttu-id="2eb97-326">AzureRm.Storage での不変ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="2eb97-326">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="2eb97-327">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="2eb97-327">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="2eb97-328">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="2eb97-328">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="2eb97-329">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="2eb97-329">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="2eb97-330">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="2eb97-330">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="2eb97-331">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="2eb97-331">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="2eb97-332">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="2eb97-332">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="2eb97-333">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="2eb97-333">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="2eb97-334">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="2eb97-334">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="2eb97-335">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="2eb97-335">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="2eb97-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="2eb97-336">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="2eb97-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="2eb97-337">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-338">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-338">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-339">Get-AzureRmDeletedWebApp と Restore-AzureRmDeletedWebApp の 2 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-339">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="2eb97-340">Windows コンテナーでの App Service プランの作成用に New-AzureRmAppServicePlan -HyperV スイッチが追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-340">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="2eb97-341">Windows コンテナー アプリを作成および管理用に、New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New パラメーター (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) が追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-341">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="2eb97-342">6.8.1 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-342">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2eb97-343">全般</span><span class="sxs-lookup"><span data-stu-id="2eb97-343">General</span></span>
* <span data-ttu-id="2eb97-344">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-344">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="2eb97-345">共通ランタイム アセンブリを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-345">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="2eb97-346">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2eb97-346">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="2eb97-347">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-347">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="2eb97-348">修正された問題 https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="2eb97-348">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="2eb97-349">Import-AzureRmApiManagementApi コマンドレットおよび \*-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-349">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="2eb97-350">修正された問題 https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="2eb97-350">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="2eb97-351">CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="2eb97-351">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="2eb97-352">4.0.4-preview NuGet へのアップグレードによって修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-352">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="2eb97-353">修正された問題 https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="2eb97-353">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="2eb97-354">製品を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-354">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="2eb97-355">修正された問題 https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="2eb97-355">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="2eb97-356">API を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-356">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="2eb97-357">AzureMonitor ロガーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-357">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-358">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-358">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-359">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-359">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="2eb97-360">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-360">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="2eb97-361">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-361">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="2eb97-362">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-362">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-363">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-363">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-364">コマンドレット出力の既定の表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-364">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="2eb97-365">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="2eb97-365">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="2eb97-366">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-366">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="2eb97-367">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-367">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-368">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-368">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-369">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-369">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-370">修正された問題</span><span class="sxs-lookup"><span data-stu-id="2eb97-370">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="2eb97-371">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2eb97-371">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="2eb97-372">複数値ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-372">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="2eb97-373">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="2eb97-373">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="2eb97-374">サブネット ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-374">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="2eb97-375">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-375">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="2eb97-376">プロファイルでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-376">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="2eb97-377">プロファイルでの予期される状態コード範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-377">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="2eb97-378">エンドポイントでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-378">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="2eb97-379">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-379">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2eb97-380">全般</span><span class="sxs-lookup"><span data-stu-id="2eb97-380">General</span></span>
* <span data-ttu-id="2eb97-381">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-381">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-382">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-382">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-383">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-383">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-384">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-384">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-385">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-385">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="2eb97-386">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-386">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="2eb97-387">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-387">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="2eb97-388">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="2eb97-388">AzureRM.IotHub</span></span>
* <span data-ttu-id="2eb97-389">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-389">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-390">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-390">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-391">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-391">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="2eb97-392">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="2eb97-392">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="2eb97-393">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-393">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-394">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-394">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-395">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-395">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-396">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-396">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-397">問題の修正</span><span class="sxs-lookup"><span data-stu-id="2eb97-397">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="2eb97-398">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2eb97-398">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="2eb97-399">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-399">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="2eb97-400">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="2eb97-400">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="2eb97-401">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-401">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="2eb97-402">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-402">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="2eb97-403">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-403">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="2eb97-404">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-404">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="2eb97-405">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="2eb97-405">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-406">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-406">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-407">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-407">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="2eb97-408">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-408">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-409">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-409">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-410">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-410">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="2eb97-411">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-411">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="2eb97-412">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-412">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="2eb97-413">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="2eb97-413">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="2eb97-414">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-414">Azure.Storage</span></span>
* <span data-ttu-id="2eb97-415">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-415">Remove the 5TB limitation for Azure File Share quota</span></span>
* <span data-ttu-id="2eb97-416">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="2eb97-416">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="2eb97-417">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-417">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="2eb97-418">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-418">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="2eb97-419">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-419">Azure.AnalysisServices</span></span>
* <span data-ttu-id="2eb97-420">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-420">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="2eb97-421">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2eb97-421">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="2eb97-422">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-422">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="2eb97-423">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="2eb97-423">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="2eb97-424">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-424">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="2eb97-425">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="2eb97-425">AzureRM.Automation</span></span>
* <span data-ttu-id="2eb97-426">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-426">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="2eb97-427">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="2eb97-427">AzureRM.Backup</span></span>
* <span data-ttu-id="2eb97-428">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-428">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="2eb97-429">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="2eb97-429">AzureRM.Batch</span></span>
* <span data-ttu-id="2eb97-430">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-430">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="2eb97-431">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="2eb97-431">AzureRM.Billing</span></span>
* <span data-ttu-id="2eb97-432">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-432">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="2eb97-433">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="2eb97-433">AzureRM.Cdn</span></span>
* <span data-ttu-id="2eb97-434">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-434">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="2eb97-435">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-435">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="2eb97-436">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-436">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-437">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-437">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-438">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-438">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="2eb97-439">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-439">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="2eb97-440">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="2eb97-440">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="2eb97-441">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-441">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="2eb97-442">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-442">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="2eb97-443">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="2eb97-443">AzureRM.Consumption</span></span>
* <span data-ttu-id="2eb97-444">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-444">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="2eb97-445">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2eb97-445">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="2eb97-446">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-446">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="2eb97-447">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="2eb97-447">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="2eb97-448">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-448">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="2eb97-449">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="2eb97-449">AzureRM.DataFactories</span></span>
* <span data-ttu-id="2eb97-450">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-450">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="2eb97-451">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2eb97-451">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="2eb97-452">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-452">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="2eb97-453">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="2eb97-453">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="2eb97-454">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-454">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="2eb97-455">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2eb97-455">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="2eb97-456">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-456">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="2eb97-457">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-457">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="2eb97-458">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-458">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="2eb97-459">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-459">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="2eb97-460">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="2eb97-460">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="2eb97-461">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-461">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="2eb97-462">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="2eb97-462">AzureRM.Dns</span></span>
* <span data-ttu-id="2eb97-463">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-463">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="2eb97-464">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="2eb97-464">AzureRM.EventGrid</span></span>
* <span data-ttu-id="2eb97-465">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-465">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="2eb97-466">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="2eb97-466">AzureRM.EventHub</span></span>
* <span data-ttu-id="2eb97-467">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-467">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="2eb97-468">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2eb97-468">AzureRM.HDInsight</span></span>
* <span data-ttu-id="2eb97-469">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-469">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="2eb97-470">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="2eb97-470">AzureRM.Insights</span></span>
* <span data-ttu-id="2eb97-471">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-471">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="2eb97-472">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="2eb97-472">AzureRM.IotHub</span></span>
* <span data-ttu-id="2eb97-473">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-473">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="2eb97-474">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2eb97-474">AzureRM.KeyVault</span></span>
* <span data-ttu-id="2eb97-475">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-475">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="2eb97-476">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="2eb97-476">AzureRM.LogicApp</span></span>
* <span data-ttu-id="2eb97-477">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-477">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="2eb97-478">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="2eb97-478">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="2eb97-479">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-479">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="2eb97-480">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="2eb97-480">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="2eb97-481">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-481">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="2eb97-482">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="2eb97-482">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="2eb97-483">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="2eb97-484">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="2eb97-484">AzureRM.Media</span></span>
* <span data-ttu-id="2eb97-485">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-486">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-486">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-487">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-487">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="2eb97-488">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-488">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="2eb97-489">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-489">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="2eb97-490">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-490">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="2eb97-491">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-491">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="2eb97-492">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-492">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="2eb97-493">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-493">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="2eb97-494">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-494">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="2eb97-495">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="2eb97-495">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="2eb97-496">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-496">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="2eb97-497">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2eb97-497">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="2eb97-498">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-498">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="2eb97-499">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2eb97-499">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="2eb97-500">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-500">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="2eb97-501">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="2eb97-501">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="2eb97-502">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-502">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="2eb97-503">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-503">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="2eb97-504">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-504">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="2eb97-505">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2eb97-505">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="2eb97-506">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-506">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="2eb97-507">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-507">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="2eb97-508">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-508">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="2eb97-509">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-509">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="2eb97-510">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-510">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="2eb97-511">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="2eb97-511">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="2eb97-512">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-512">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="2eb97-513">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="2eb97-513">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="2eb97-514">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-514">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="2eb97-515">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2eb97-515">AzureRM.RedisCache</span></span>
* <span data-ttu-id="2eb97-516">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-516">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="2eb97-517">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="2eb97-517">AzureRM.Relay</span></span>
* <span data-ttu-id="2eb97-518">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-518">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-519">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-519">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-520">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2eb97-520">Support template deployment at subscription scope.</span></span> <span data-ttu-id="2eb97-521">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-521">Add new Cmdlets:</span></span>
    - <span data-ttu-id="2eb97-522">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="2eb97-522">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="2eb97-523">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="2eb97-523">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="2eb97-524">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="2eb97-524">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="2eb97-525">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="2eb97-525">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="2eb97-526">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="2eb97-526">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="2eb97-527">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="2eb97-527">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="2eb97-528">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="2eb97-528">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="2eb97-529">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-529">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="2eb97-530">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-530">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="2eb97-531">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-531">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="2eb97-532">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="2eb97-532">AzureRM.Scheduler</span></span>
* <span data-ttu-id="2eb97-533">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-533">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-534">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-534">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-535">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-535">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="2eb97-536">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2eb97-536">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="2eb97-537">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-537">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-538">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-538">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-539">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-539">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="2eb97-540">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-540">AzureRM.Storage</span></span>
* <span data-ttu-id="2eb97-541">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-541">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="2eb97-542">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="2eb97-542">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="2eb97-543">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-543">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="2eb97-544">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="2eb97-544">AzureRM.Tags</span></span>
* <span data-ttu-id="2eb97-545">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-545">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="2eb97-546">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2eb97-546">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="2eb97-547">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-547">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="2eb97-548">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="2eb97-548">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="2eb97-549">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-549">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-550">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-550">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-551">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-551">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="2eb97-552">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-552">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2eb97-553">全般</span><span class="sxs-lookup"><span data-stu-id="2eb97-553">General</span></span>
* <span data-ttu-id="2eb97-554">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-554">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-555">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-555">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-556">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-556">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="2eb97-557">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-557">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="2eb97-558">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-558">Azure.Storage</span></span>
* <span data-ttu-id="2eb97-559">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-559">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="2eb97-560">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-560">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="2eb97-561">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2eb97-561">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="2eb97-562">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="2eb97-562">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="2eb97-563">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-563">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="2eb97-564">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="2eb97-564">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="2eb97-565">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-565">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="2eb97-566">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="2eb97-566">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="2eb97-567">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-567">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-568">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-568">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-569">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-569">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="2eb97-570">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-570">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="2eb97-571">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="2eb97-571">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="2eb97-572">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="2eb97-572">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="2eb97-573">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-573">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="2eb97-574">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-574">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="2eb97-575">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-575">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="2eb97-576">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-576">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="2eb97-577">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-577">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="2eb97-578">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-578">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="2eb97-579">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2eb97-579">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="2eb97-580">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-580">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="2eb97-581">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-581">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="2eb97-582">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-582">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="2eb97-583">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-583">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="2eb97-584">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2eb97-584">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="2eb97-585">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-585">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="2eb97-586">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="2eb97-586">AzureRM.EventHub</span></span>
* <span data-ttu-id="2eb97-587">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-587">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="2eb97-588">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="2eb97-588">AzureRM.Insights</span></span>
* <span data-ttu-id="2eb97-589">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-589">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="2eb97-590">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="2eb97-590">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="2eb97-591">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2eb97-591">AzureRM.KeyVault</span></span>
* <span data-ttu-id="2eb97-592">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-592">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-593">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-593">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-594">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-594">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-595">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-595">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-596">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-596">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="2eb97-597">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-597">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-598">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-598">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-599">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-599">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="2eb97-600">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-600">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-601">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-601">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-602">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-602">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="2eb97-603">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="2eb97-603">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="2eb97-604">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-604">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="2eb97-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="2eb97-605">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="2eb97-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="2eb97-606">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="2eb97-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="2eb97-607">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="2eb97-608">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-608">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="2eb97-609">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-609">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="2eb97-610">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-610">AzureRM.Storage</span></span>
* <span data-ttu-id="2eb97-611">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-611">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="2eb97-612">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="2eb97-612">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="2eb97-613">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2eb97-613">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="2eb97-614">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2eb97-614">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="2eb97-615">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2eb97-615">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="2eb97-616">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="2eb97-616">AzureRM.Tags</span></span>
* <span data-ttu-id="2eb97-617">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-617">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="2eb97-618">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-618">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-619">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-619">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-620">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-620">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="2eb97-621">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-621">Azure.Storage</span></span>
* <span data-ttu-id="2eb97-622">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="2eb97-622">Support Upload Blob or File with write only Sas token</span></span>
* <span data-ttu-id="2eb97-623">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="2eb97-623">Set-AzureStorageBlobContent</span></span>
* <span data-ttu-id="2eb97-624">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="2eb97-624">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="2eb97-625">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-625">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="2eb97-626">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-626">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="2eb97-627">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="2eb97-627">AzureRM.Automation</span></span>
* <span data-ttu-id="2eb97-628">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-628">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-629">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-629">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-630">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-630">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="2eb97-631">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-631">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="2eb97-632">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-632">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="2eb97-633">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-633">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="2eb97-634">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-634">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="2eb97-635">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="2eb97-635">AzureRM.EventHub</span></span>
* <span data-ttu-id="2eb97-636">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-636">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="2eb97-637">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2eb97-637">AzureRM.KeyVault</span></span>
* <span data-ttu-id="2eb97-638">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-638">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="2eb97-639">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="2eb97-639">AzureRM.LogicApp</span></span>
* <span data-ttu-id="2eb97-640">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-640">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-641">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-641">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-642">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="2eb97-642">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="2eb97-643">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-643">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="2eb97-644">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-644">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="2eb97-645">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-645">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="2eb97-646">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-646">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="2eb97-647">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-647">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="2eb97-648">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="2eb97-648">AzureRM.Relay</span></span>
* <span data-ttu-id="2eb97-649">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-649">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-650">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-650">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-651">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-651">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="2eb97-652">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-652">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="2eb97-653">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-653">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="2eb97-654">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-654">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="2eb97-655">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-655">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-656">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-656">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-657">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-657">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="2eb97-658">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-658">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="2eb97-659">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="2eb97-659">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="2eb97-660">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="2eb97-660">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="2eb97-661">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="2eb97-661">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="2eb97-662">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="2eb97-662">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="2eb97-663">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="2eb97-663">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="2eb97-664">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-664">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="2eb97-665">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2eb97-665">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="2eb97-666">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-666">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-667">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-668">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-668">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="2eb97-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-669">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="2eb97-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-670">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-671">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-671">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-672">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="2eb97-672">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="2eb97-673">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-673">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="2eb97-674">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="2eb97-674">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="2eb97-675">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-675">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2eb97-676">全般</span><span class="sxs-lookup"><span data-stu-id="2eb97-676">General</span></span>
* <span data-ttu-id="2eb97-677">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-677">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-678">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-678">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-679">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-679">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-680">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-680">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-681">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="2eb97-681">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="2eb97-682">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-682">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="2eb97-683">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-683">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="2eb97-684">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="2eb97-684">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="2eb97-685">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-685">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="2eb97-686">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="2eb97-686">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="2eb97-687">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-687">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="2eb97-688">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="2eb97-688">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="2eb97-689">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-689">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="2eb97-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="2eb97-690">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="2eb97-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="2eb97-691">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="2eb97-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="2eb97-692">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="2eb97-693">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2eb97-693">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="2eb97-694">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-694">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="2eb97-695">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-695">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="2eb97-696">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-696">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="2eb97-697">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-697">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="2eb97-698">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="2eb97-698">AzureRM.EventHub</span></span>
* <span data-ttu-id="2eb97-699">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-699">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="2eb97-700">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-700">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="2eb97-701">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-701">Provided Default Parameter set.</span></span>
* <span data-ttu-id="2eb97-702">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-702">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="2eb97-703">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2eb97-703">AzureRM.KeyVault</span></span>
* <span data-ttu-id="2eb97-704">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-704">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-705">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-705">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-706">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-706">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="2eb97-707">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-707">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="2eb97-708">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-708">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="2eb97-709">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-709">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="2eb97-710">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-710">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="2eb97-711">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-711">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="2eb97-712">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-712">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="2eb97-713">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-713">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="2eb97-714">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-714">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="2eb97-715">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-715">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="2eb97-716">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2eb97-716">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="2eb97-717">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-717">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="2eb97-718">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="2eb97-718">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="2eb97-719">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-719">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-720">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-720">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-721">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-721">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="2eb97-722">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-722">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="2eb97-723">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="2eb97-723">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="2eb97-724">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-724">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="2eb97-725">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-725">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="2eb97-726">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-726">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="2eb97-727">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-727">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="2eb97-728">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-728">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="2eb97-729">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-729">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="2eb97-730">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-730">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="2eb97-731">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-731">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="2eb97-732">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-732">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="2eb97-733">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-733">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="2eb97-734">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2eb97-734">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="2eb97-735">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-735">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-736">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-736">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-737">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-737">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="2eb97-738">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-738">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="2eb97-739">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-739">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-740">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-740">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-741">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-741">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="2eb97-742">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="2eb97-742">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="2eb97-743">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2eb97-743">Azure.Storage</span></span>
* <span data-ttu-id="2eb97-744">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-744">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-745">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-745">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-746">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-746">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="2eb97-747">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-747">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="2eb97-748">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="2eb97-748">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="2eb97-749">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="2eb97-749">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="2eb97-750">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="2eb97-750">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="2eb97-751">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-751">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="2eb97-752">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="2eb97-752">Start-AzureRmVM</span></span>
    - <span data-ttu-id="2eb97-753">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="2eb97-753">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="2eb97-754">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="2eb97-754">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="2eb97-755">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="2eb97-755">Set-AzureRmVM</span></span>
    - <span data-ttu-id="2eb97-756">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="2eb97-756">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="2eb97-757">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="2eb97-757">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="2eb97-758">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="2eb97-758">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="2eb97-759">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="2eb97-759">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="2eb97-760">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="2eb97-760">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="2eb97-761">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="2eb97-761">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="2eb97-762">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="2eb97-762">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="2eb97-763">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="2eb97-763">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="2eb97-764">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="2eb97-764">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="2eb97-765">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="2eb97-765">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="2eb97-766">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="2eb97-766">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="2eb97-767">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="2eb97-767">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="2eb97-768">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="2eb97-768">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="2eb97-769">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="2eb97-769">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="2eb97-770">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="2eb97-770">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="2eb97-771">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="2eb97-771">AzureRM.EventGrid</span></span>
* <span data-ttu-id="2eb97-772">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-772">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="2eb97-773">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2eb97-773">AzureRM.KeyVault</span></span>
* <span data-ttu-id="2eb97-774">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-774">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="2eb97-775">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2eb97-775">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="2eb97-776">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="2eb97-776">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="2eb97-777">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="2eb97-777">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="2eb97-778">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-778">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="2eb97-779">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2eb97-779">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="2eb97-780">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-780">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="2eb97-781">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-781">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-782">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-782">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-783">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-783">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="2eb97-784">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2eb97-784">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="2eb97-785">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-785">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-786">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-786">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-787">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-787">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="2eb97-788">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="2eb97-788">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="2eb97-789">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-789">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="2eb97-790">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2eb97-790">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="2eb97-791">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-791">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="2eb97-792">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-792">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-793">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-793">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-794">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-794">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="2eb97-795">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="2eb97-795">AzureRM.Compute</span></span>
* <span data-ttu-id="2eb97-796">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="2eb97-796">VMSS VM Update feature</span></span>
    - <span data-ttu-id="2eb97-797">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-797">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="2eb97-798">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-798">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="2eb97-799">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2eb97-799">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="2eb97-800">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-800">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="2eb97-801">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-801">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="2eb97-802">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-802">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="2eb97-803">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-803">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="2eb97-804">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-804">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="2eb97-805">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2eb97-805">AzureRM.KeyVault</span></span>
* <span data-ttu-id="2eb97-806">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-806">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-807">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-807">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-808">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="2eb97-808">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="2eb97-809">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="2eb97-809">AzureRM.Resources</span></span>
* <span data-ttu-id="2eb97-810">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-810">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="2eb97-811">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="2eb97-811">AzureRM.Scheduler</span></span>
* <span data-ttu-id="2eb97-812">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-812">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="2eb97-813">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-813">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-814">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2eb97-814">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="2eb97-815">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="2eb97-815">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="2eb97-816">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="2eb97-816">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="2eb97-817">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="2eb97-817">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="2eb97-818">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="2eb97-818">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="2eb97-819">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="2eb97-819">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="2eb97-820">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="2eb97-820">AzureRM.Websites</span></span>
* <span data-ttu-id="2eb97-821">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-821">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="2eb97-822">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="2eb97-822">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="2eb97-823">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="2eb97-823">AzureRM.Profile</span></span>
* <span data-ttu-id="2eb97-824">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-824">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="2eb97-825">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2eb97-825">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="2eb97-826">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2eb97-826">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="2eb97-827">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2eb97-827">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="2eb97-828">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-828">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="2eb97-829">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-829">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="2eb97-830">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-830">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="2eb97-831">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-831">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="2eb97-832">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-832">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="2eb97-833">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-833">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="2eb97-834">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-834">Added support for MSI identity</span></span>
* <span data-ttu-id="2eb97-835">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="2eb97-835">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="2eb97-836">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="2eb97-836">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="2eb97-837">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-837">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="2eb97-838">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="2eb97-838">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="2eb97-839">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="2eb97-839">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="2eb97-840">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="2eb97-840">AzureRM.Batch</span></span>
* <span data-ttu-id="2eb97-841">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-841">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="2eb97-842">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-842">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="2eb97-843">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="2eb97-843">AzureRM.Consumption</span></span>
* <span data-ttu-id="2eb97-844">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-844">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="2eb97-845">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2eb97-845">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="2eb97-846">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-846">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="2eb97-847">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-847">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="2eb97-848">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-848">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="2eb97-849">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="2eb97-849">AzureRM.Network</span></span>
* <span data-ttu-id="2eb97-850">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-850">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="2eb97-851">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-851">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="2eb97-852">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="2eb97-852">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="2eb97-853">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-853">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="2eb97-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-854">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="2eb97-855">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-855">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="2eb97-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-856">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="2eb97-857">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-857">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="2eb97-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="2eb97-858">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="2eb97-859">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2eb97-859">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="2eb97-860">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="2eb97-860">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="2eb97-861">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="2eb97-861">AzureRM.Sql</span></span>
* <span data-ttu-id="2eb97-862">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-862">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="2eb97-863">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="2eb97-863">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="2eb97-864">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-864">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="2eb97-865">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="2eb97-865">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="2eb97-866">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2eb97-866">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="2eb97-867">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="2eb97-867">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="2eb97-868">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="2eb97-868">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="2eb97-869">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="2eb97-869">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="2eb97-870">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="2eb97-870">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="2eb97-871">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="2eb97-871">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="2eb97-872">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2eb97-872">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="2eb97-873">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="2eb97-873">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
