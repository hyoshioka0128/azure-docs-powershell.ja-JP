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
ms.openlocfilehash: 7f517f0b3768a2075557b131158ee1264ea9ab3f
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153452"
---
# <a name="release-notes"></a><span data-ttu-id="55ac5-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="55ac5-103">Release notes</span></span>

<span data-ttu-id="55ac5-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="55ac5-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6130---november-2018"></a><span data-ttu-id="55ac5-105">6.13.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-105">6.13.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-106">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-106">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-107">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-107">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="55ac5-108">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55ac5-108">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="55ac5-109">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-109">Update dependencies for type mapping issue</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="55ac5-110">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="55ac5-110">AzureRM.Automation</span></span>
* <span data-ttu-id="55ac5-111">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="55ac5-111">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="55ac5-112">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-112">Added Update Management cmdlets</span></span>
* <span data-ttu-id="55ac5-113">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-113">Added Source Control cmdlets</span></span>
* <span data-ttu-id="55ac5-114">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-114">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="55ac5-115">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-115">Fixed the DSC Register Node command</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-116">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-116">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-117">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-117">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="55ac5-118">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-118">Update dependencies for type mapping issue</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="55ac5-119">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="55ac5-119">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="55ac5-120">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-120">Update dependencies for type mapping issue</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="55ac5-121">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="55ac5-121">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="55ac5-122">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-122">update the examples description for marketplace cmdlets</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-123">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-123">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-124">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-124">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="55ac5-125">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-125">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="55ac5-126">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-126">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="55ac5-127">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-127">Fix issues with memory usage in VirtualNetwork map</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="55ac5-128">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-128">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="55ac5-129">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-129">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="55ac5-130">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-130">Converted policy timezone to uppercase.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="55ac5-131">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="55ac5-131">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="55ac5-132">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-132">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="55ac5-133">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-133">Update dependencies for type mapping issue</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="55ac5-134">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="55ac5-134">AzureRM.Relay</span></span>
* <span data-ttu-id="55ac5-135">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="55ac5-135">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-136">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-136">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-137">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-137">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="55ac5-138">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-138">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="55ac5-139">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="55ac5-139">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="55ac5-140">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="55ac5-140">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="55ac5-141">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-141">Add deprecation messages for upcoming breaking changes</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-142">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-142">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-143">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-143">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="55ac5-144">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="55ac5-144">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="55ac5-145">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="55ac5-145">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="55ac5-146">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="55ac5-146">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="55ac5-147">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="55ac5-147">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="55ac5-148">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-148">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="55ac5-149">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-149">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="55ac5-150">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-150">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="55ac5-151">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-151">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="55ac5-152">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="55ac5-152">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="55ac5-153">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-153">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="55ac5-154">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-154">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="55ac5-155">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="55ac5-155">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="55ac5-156">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="55ac5-156">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="55ac5-157">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="55ac5-157">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="55ac5-158">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="55ac5-158">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="55ac5-159">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-159">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="6120---november-2018"></a><span data-ttu-id="55ac5-160">6.12.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-160">6.12.0 - November 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-161">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-161">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-162">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-162">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="55ac5-163">Connect-AzureRmAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-163">Rename param TenantId in cmdlet Connect-AzureRmAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="55ac5-164">Connect-AzureRmAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-164">Updated TenantId description for Connect-AzureRmAccount</span></span>
* <span data-ttu-id="55ac5-165">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-165">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="55ac5-166">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-166">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="55ac5-167">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-167">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="55ac5-168">接続されていない場合に "Disconnect-AzureRmAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-168">Fix issue where 'Disconnect-AzureRmAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azurermautomation"></a><span data-ttu-id="55ac5-169">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="55ac5-169">AzureRM.Automation</span></span>
* <span data-ttu-id="55ac5-170">コマンドレット DLL ファイルの名前を Microsoft.Azure.Commands.Automation.dll に変更しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-170">Renamed cmdlet DLL filename to Microsoft.Azure.Commands.Automation.dll</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="55ac5-171">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-171">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="55ac5-172">Get-AzureRmCognitiveServicesAccountSkus 操作を追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-172">Add Get-AzureRmCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-173">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-173">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-174">Add-AzureRmVmssVMDataDisk および Remove-AzureRmVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-174">Add Add-AzureRmVmssVMDataDisk and Remove-AzureRmVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="55ac5-175">Get-AzureRmVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="55ac5-175">Get-AzureRmVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="55ac5-176">SetAzureRmVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式では設定されません。</span><span class="sxs-lookup"><span data-stu-id="55ac5-176">Fixed SetAzureRmVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="55ac5-177">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="55ac5-177">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="55ac5-178">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-178">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="55ac5-179">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-179">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="55ac5-180">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="55ac5-180">AzureRM.Insights</span></span>
* <span data-ttu-id="55ac5-181">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-181">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="55ac5-182">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="55ac5-182">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="55ac5-183">Set-AzureRMDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-183">Fixed issue #7513 [Insights] Set-AzureRMDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="55ac5-184">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="55ac5-184">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-185">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-185">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-186">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="55ac5-186">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="55ac5-187">Get-AzureRmExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="55ac5-187">Get-AzureRmExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="55ac5-188">Get-AzureRmExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="55ac5-188">Get-AzureRmExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="55ac5-189">Get-AzureRmExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="55ac5-189">Get-AzureRmExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="55ac5-190">Get-AzureRMExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="55ac5-190">Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="55ac5-191">Get-AzureRMExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="55ac5-191">Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="55ac5-192">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="55ac5-192">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="55ac5-193">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="55ac5-193">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="55ac5-194">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-194">Added policy remediation cmdlets</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="55ac5-195">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-195">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="55ac5-196">Recovery Services で Azure ファイル共有のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-196">Added support for azure file shares in recovery services.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-197">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-197">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-198"> https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="55ac5-198">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="55ac5-199">"Get-AzureRmResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-199">Allow listing resources using the '-ResourceId' parameter for 'Get-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-200">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-200">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-201">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-201">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="55ac5-202">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="55ac5-202">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="55ac5-203">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-203">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="55ac5-204">"Add-AzureRmServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-204">Fix 'Add-AzureRmServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="55ac5-205">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="55ac5-205">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="55ac5-206">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="55ac5-206">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="55ac5-207">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzureRmServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-207">Fix 'Update-AzureRmServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="6110---october-2018"></a><span data-ttu-id="55ac5-208">6.11.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-208">6.11.0 - October 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-209">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-209">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-210">CloudShell での Get-AzureRmSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-210">Fix issue with Get-AzureRmSubscription in CloudShell</span></span>
* <span data-ttu-id="55ac5-211">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-211">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="55ac5-212">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-212">AzureRM.Backup</span></span>
* <span data-ttu-id="55ac5-213">Azure Backup コマンドレットを非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-213">Deprecated Azure Backup cmdlets.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-214">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-214">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-215">"New-AzureRmVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-215">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzureRmVm'</span></span>
* <span data-ttu-id="55ac5-216">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-216">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="55ac5-217">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="55ac5-217">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="55ac5-218">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-218">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="55ac5-219">Get-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="55ac5-219">Get-AzureRmDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="55ac5-220">Add-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="55ac5-220">Add-AzureRmDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="55ac5-221">Set-AzureRmDataLakeStoreVirtualNetworkRule: 指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="55ac5-221">Set-AzureRmDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="55ac5-222">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="55ac5-222">Remove-AzureRmDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-223">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-223">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-224">プロトコル値をバックエンドに渡すように、Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-224">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="55ac5-225">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-225">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-226">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-226">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-227">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzureRMRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-227">Fix isssue where Get-AzureRMRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="55ac5-228">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-228">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="6100---october-2018"></a><span data-ttu-id="55ac5-229">6.10.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-229">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="55ac5-230">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-230">Azure.Storage</span></span>
* <span data-ttu-id="55ac5-231">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-231">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="55ac5-232">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="55ac5-232">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="55ac5-233">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="55ac5-233">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="55ac5-234">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-234">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="55ac5-235">既存のアカウントなしでの Get-AzureRmCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-235">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-236">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-236">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-237">必要に応じて 50 を超える結果が返されるように Get-AzureRmVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-237">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="55ac5-238">"SimpleParameterSet" の例を New-AzureRmVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-238">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="55ac5-239">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-239">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="55ac5-240">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="55ac5-240">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="55ac5-241">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-241">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-242">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-242">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-243">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-243">Added NetworkProfile functionality.</span></span> <span data-ttu-id="55ac5-244">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="55ac5-244">new cmdlets added</span></span>
    - <span data-ttu-id="55ac5-245">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="55ac5-245">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="55ac5-246">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="55ac5-246">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="55ac5-247">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="55ac5-247">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="55ac5-248">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="55ac5-248">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="55ac5-249">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-249">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="55ac5-250">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-250">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="55ac5-251">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-251">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="55ac5-252">New-AzureRmVirtualNetworkTap、Get-AzureRmVirtualNetworkTap、Set-AzureRmVirtualNetworkTap、Remove-AzureRmVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-252">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="55ac5-253">Set-AzureRmNEtworkInterfaceTapConfig、Get-AzureRmNEtworkInterfaceTapConfig、Remove-AzureRmNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-253">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="55ac5-254">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="55ac5-254">AzureRM.RedisCache</span></span>
* <span data-ttu-id="55ac5-255">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-255">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="55ac5-256">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-256">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-257">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-257">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-258">欠落していた -Mode パラメーターを Set-AzureRmPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-258">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="55ac5-259">配信元にユーザーが含まれる操作について Get-AzureRmProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-259">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-260">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-260">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-261">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-261">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="55ac5-262">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-262">AzureRM.Storage</span></span>
* <span data-ttu-id="55ac5-263">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-263">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="55ac5-264">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="55ac5-264">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-265">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-265">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-266">新しいコマンドレット: Get-AzureRMWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="55ac5-266">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="55ac5-267">新しいコマンドレット: New-AzureRMWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="55ac5-267">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="55ac5-268">6.9.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-268">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="55ac5-269">全般</span><span class="sxs-lookup"><span data-stu-id="55ac5-269">General</span></span>
* <span data-ttu-id="55ac5-270">AzureRM.SignalR が AzureRM ロールアップ モジュールに追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-270">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-271">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-271">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-272">ストレージの一般的なコードに対する軽微な変更</span><span class="sxs-lookup"><span data-stu-id="55ac5-272">Minor changes to the storage common code</span></span>
* <span data-ttu-id="55ac5-273">完全なパラメーター型を含めるようにヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-273">Updated help files to include full parameter types.</span></span>
* <span data-ttu-id="55ac5-274">ServicePrincipalCertificateWithSubscriptionId パラメーター セットの -ServicePrincipal を "任意" に変更しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-274">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="55ac5-275">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-275">Azure.Storage</span></span>
* <span data-ttu-id="55ac5-276">OAuth でのストレージ コンテキストの作成がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-276">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="55ac5-277">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="55ac5-277">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="55ac5-278">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="55ac5-278">AzureRM.Cdn</span></span>
* <span data-ttu-id="55ac5-279">CDN 価格 SKU に Standard_Microsoft を追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-279">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-280">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-280">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-281">Keyvault および Storage への依存関係を一般的な依存関係に移動しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-281">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="55ac5-282">より多くの仮想マシンのサイズのサポートを AEM コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-282">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="55ac5-283">PublicIPPrefix パラメーターを New-AzureRmVmssIpConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-283">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="55ac5-284">ResourceId パラメーターを Invoke-AzureRmVMRunCommand コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-284">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="55ac5-285">Invoke-AzureRmVmssVMRunCommand コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-285">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="55ac5-286">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="55ac5-286">AzureRM.Dns</span></span>
* <span data-ttu-id="55ac5-287">DNS レコード作成中のエイリアス レコードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-287">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="55ac5-288">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="55ac5-288">AzureRM.Insights</span></span>
* <span data-ttu-id="55ac5-289">#6833 および #7102 の問題を修正しました (診断設定領域)</span><span class="sxs-lookup"><span data-stu-id="55ac5-289">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="55ac5-290">診断設定の作成および表示/取得中の既定の名前 ("service") に関する問題</span><span class="sxs-lookup"><span data-stu-id="55ac5-290">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="55ac5-291">カテゴリでの診断設定の作成に関する問題</span><span class="sxs-lookup"><span data-stu-id="55ac5-291">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="55ac5-292">メトリック時間グレイン パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-292">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="55ac5-293">Timegrains パラメーターは引き続き利用できますが (これは破壊的変更ではありません)、PT1M のみが有効であるため、バックエンドでは無視されます</span><span class="sxs-lookup"><span data-stu-id="55ac5-293">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-294">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-295">LoadBalancer コマンドレットへの変更</span><span class="sxs-lookup"><span data-stu-id="55ac5-295">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="55ac5-296">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes パラメーター、EnableFloatingIp パラメーター、EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-296">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="55ac5-297">LoadBalancerInboundNatRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-297">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="55ac5-298">LoadBalancerRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-298">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="55ac5-299">LoadBalancerProbeConfig: Protocol パラメーターの "HTTPS" 値のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-299">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="55ac5-300">新しい LoadBalancer のサブリソース OutboundRule について新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-300">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="55ac5-301">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-301">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="55ac5-302">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-302">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="55ac5-303">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-303">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="55ac5-304">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-304">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="55ac5-305">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-305">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="55ac5-306">PSNetworkInterface の新しい HostedWorkloads プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-306">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="55ac5-307">次の機能のために新しいコマンドレットを追加しました: Azure Firewall (ARM を介して)</span><span class="sxs-lookup"><span data-stu-id="55ac5-307">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="55ac5-308">Get-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-308">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="55ac5-309">Set-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-309">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="55ac5-310">New-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-310">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="55ac5-311">Remove-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-311">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="55ac5-312">New-AzureRmFirewallApplicationRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-312">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="55ac5-313">New-AzureRmFirewallApplicationRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-313">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="55ac5-314">New-AzureRmFirewallNatRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-314">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="55ac5-315">New-AzureRmFirewallNatRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-315">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="55ac5-316">New-AzureRmFirewallNetworkRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-316">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="55ac5-317">New-AzureRmFirewallNetworkRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-317">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="55ac5-318">Application Gateway での信頼されたルート証明書と自動スケーリング構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-318">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="55ac5-319">追加された新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="55ac5-319">New Cmdlets added:</span></span>
      - <span data-ttu-id="55ac5-320">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-320">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="55ac5-321">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-321">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="55ac5-322">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-322">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="55ac5-323">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-323">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="55ac5-324">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-324">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="55ac5-325">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-325">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="55ac5-326">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-326">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="55ac5-327">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-327">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="55ac5-328">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-328">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="55ac5-329">省略可能なパラメーターで更新されたコマンドレット -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-329">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="55ac5-330">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="55ac5-330">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="55ac5-331">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="55ac5-331">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="55ac5-332">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="55ac5-332">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="55ac5-333">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="55ac5-333">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="55ac5-334">省略可能なパラメーターで更新されたコマンドレット - AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-334">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="55ac5-335">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="55ac5-335">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="55ac5-336">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="55ac5-336">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="55ac5-337">インターフェイス エンドポイントのコマンドレット Get-AzureInterfaceEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-337">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="55ac5-338">サブネットでの複数のアドレス プレフィックスのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-338">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="55ac5-339">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="55ac5-339">Updated cmdlets:</span></span>
  - <span data-ttu-id="55ac5-340">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-340">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="55ac5-341">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-341">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="55ac5-342">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-342">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="55ac5-343">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-343">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="55ac5-344">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-344">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="55ac5-345">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-345">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="55ac5-346">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-346">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="55ac5-347">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-347">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="55ac5-348">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-348">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="55ac5-349">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-349">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="55ac5-350">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-350">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="55ac5-351">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-351">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="55ac5-352">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-352">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="55ac5-353">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-353">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="55ac5-354">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-354">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="55ac5-355">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-355">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="55ac5-356">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-356">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="55ac5-357">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-357">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="55ac5-358">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="55ac5-358">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="55ac5-359">サブネット委任のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-359">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="55ac5-360">New-AzureRmDelegation: 新しい委任を作成します。これはサブネットに追加できます</span><span class="sxs-lookup"><span data-stu-id="55ac5-360">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="55ac5-361">Remove-AzureRmDelegation: サブネットを受け取り、指定された委任の名前をそのサブネットから削除します</span><span class="sxs-lookup"><span data-stu-id="55ac5-361">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="55ac5-362">Add-AzureRmDelegation: サブネットを受け取り、指定されたサービス名を委任としてそのサブネットに追加します</span><span class="sxs-lookup"><span data-stu-id="55ac5-362">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="55ac5-363">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="55ac5-363">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="55ac5-364">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="55ac5-364">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="55ac5-365">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="55ac5-365">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="55ac5-366">管理対象のマネージド ディスクのサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-366">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="55ac5-367">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="55ac5-367">AzureRM.RedisCache</span></span>
* <span data-ttu-id="55ac5-368">Insights の依存関係を更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-368">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-369">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-369">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-370">New-AzureRmResourceGroupDeployment を新しい RollbackAction パラメーターで更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-370">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="55ac5-371">新しいパラメーターを使用して OnErrorDeployment のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-371">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="55ac5-372">ポリシー割り当てでマネージド ID をサポートします。</span><span class="sxs-lookup"><span data-stu-id="55ac5-372">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="55ac5-373">"New-AzureRmPolicyAssignment" を指定してポリシーを割り当てるとき、既定値を持つパラメーターが不要になりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-373">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="55ac5-374">ポリシー エイリアスを取得するための新しい Get AzureRmPolicyAlias コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-374">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-375">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-375">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-376">問題 #7161 を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-376">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="55ac5-377">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="55ac5-377">AzureRM.SignalR</span></span>
* <span data-ttu-id="55ac5-378">SKU 名を Free_F1 および Standard_S1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-378">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="55ac5-379">バージョン フィールドを PSSignalRResource オブジェクトに、接続文字列を PSSignalRKeys オブジェクトに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-379">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="55ac5-380">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-380">AzureRM.Storage</span></span>
* <span data-ttu-id="55ac5-381">AzureRm.Storage での不変ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="55ac5-381">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="55ac5-382">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="55ac5-382">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="55ac5-383">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="55ac5-383">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="55ac5-384">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="55ac5-384">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="55ac5-385">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="55ac5-385">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="55ac5-386">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="55ac5-386">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="55ac5-387">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="55ac5-387">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="55ac5-388">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="55ac5-388">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="55ac5-389">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="55ac5-389">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="55ac5-390">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="55ac5-390">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="55ac5-391">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="55ac5-391">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="55ac5-392">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="55ac5-392">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-393">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-393">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-394">追加された 2 つの新しいコマンドレット: Get-AzureRmDeletedWebApp および Restore-AzureRmDeletedWebApp</span><span class="sxs-lookup"><span data-stu-id="55ac5-394">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="55ac5-395">Windows コンテナーでの App Service プランの作成用に New-AzureRmAppServicePlan -HyperV スイッチが追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-395">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="55ac5-396">Windows コンテナー アプリを作成および管理用に、New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New パラメーター (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) が追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-396">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="55ac5-397">6.8.1 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-397">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="55ac5-398">全般</span><span class="sxs-lookup"><span data-stu-id="55ac5-398">General</span></span>
* <span data-ttu-id="55ac5-399">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-399">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="55ac5-400">共通ランタイム アセンブリを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-400">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="55ac5-401">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55ac5-401">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="55ac5-402">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-402">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="55ac5-403">修正された問題 https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="55ac5-403">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="55ac5-404">Import-AzureRmApiManagementApi コマンドレットおよび \*-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-404">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="55ac5-405">修正された問題 https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="55ac5-405">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="55ac5-406">CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="55ac5-406">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="55ac5-407">4.0.4-preview NuGet へのアップグレードによって修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-407">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="55ac5-408">修正された問題 https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="55ac5-408">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="55ac5-409">製品を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-409">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="55ac5-410">修正された問題 https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="55ac5-410">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="55ac5-411">API を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-411">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="55ac5-412">AzureMonitor ロガーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-412">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-413">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-413">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-414">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-414">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="55ac5-415">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-415">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="55ac5-416">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-416">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="55ac5-417">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-417">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-418">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-418">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-419">コマンドレット出力の既定の表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-419">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="55ac5-420">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="55ac5-420">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="55ac5-421">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-421">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="55ac5-422">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-422">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-423">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-423">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-424">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-424">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-425">修正された問題</span><span class="sxs-lookup"><span data-stu-id="55ac5-425">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="55ac5-426">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="55ac5-426">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="55ac5-427">複数値ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-427">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="55ac5-428">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="55ac5-428">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="55ac5-429">サブネット ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-429">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="55ac5-430">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-430">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="55ac5-431">プロファイルでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-431">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="55ac5-432">プロファイルでの予期される状態コード範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-432">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="55ac5-433">エンドポイントでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-433">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="55ac5-434">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-434">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="55ac5-435">全般</span><span class="sxs-lookup"><span data-stu-id="55ac5-435">General</span></span>
* <span data-ttu-id="55ac5-436">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-436">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-437">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-437">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-438">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-438">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-439">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-439">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-440">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-440">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="55ac5-441">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-441">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="55ac5-442">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-442">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="55ac5-443">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="55ac5-443">AzureRM.IotHub</span></span>
* <span data-ttu-id="55ac5-444">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-444">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-445">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-445">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-446">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-446">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="55ac5-447">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="55ac5-447">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="55ac5-448">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-448">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-449">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-449">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-450">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-450">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-451">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-451">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-452">問題の修正</span><span class="sxs-lookup"><span data-stu-id="55ac5-452">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="55ac5-453">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="55ac5-453">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="55ac5-454">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-454">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="55ac5-455">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="55ac5-455">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="55ac5-456">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-456">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="55ac5-457">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-457">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="55ac5-458">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-458">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="55ac5-459">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-459">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="55ac5-460">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="55ac5-460">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-461">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-461">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-462">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-462">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="55ac5-463">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-463">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-464">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-464">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-465">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-465">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="55ac5-466">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-466">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="55ac5-467">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-467">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="55ac5-468">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="55ac5-468">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="55ac5-469">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-469">Azure.Storage</span></span>
* <span data-ttu-id="55ac5-470">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-470">Remove the 5TB limitation for Azure File Share quota</span></span>
* <span data-ttu-id="55ac5-471">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="55ac5-471">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="55ac5-472">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-472">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="55ac5-473">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-473">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="55ac5-474">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-474">Azure.AnalysisServices</span></span>
* <span data-ttu-id="55ac5-475">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-475">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="55ac5-476">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55ac5-476">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="55ac5-477">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-477">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="55ac5-478">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="55ac5-478">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="55ac5-479">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-479">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="55ac5-480">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="55ac5-480">AzureRM.Automation</span></span>
* <span data-ttu-id="55ac5-481">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-481">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="55ac5-482">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-482">AzureRM.Backup</span></span>
* <span data-ttu-id="55ac5-483">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-483">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="55ac5-484">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="55ac5-484">AzureRM.Batch</span></span>
* <span data-ttu-id="55ac5-485">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-485">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="55ac5-486">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="55ac5-486">AzureRM.Billing</span></span>
* <span data-ttu-id="55ac5-487">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-487">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="55ac5-488">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="55ac5-488">AzureRM.Cdn</span></span>
* <span data-ttu-id="55ac5-489">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-489">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="55ac5-490">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-490">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="55ac5-491">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-491">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-492">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-492">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-493">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-493">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="55ac5-494">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-494">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="55ac5-495">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="55ac5-495">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="55ac5-496">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-496">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="55ac5-497">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-497">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="55ac5-498">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="55ac5-498">AzureRM.Consumption</span></span>
* <span data-ttu-id="55ac5-499">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-499">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="55ac5-500">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="55ac5-500">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="55ac5-501">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-501">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="55ac5-502">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="55ac5-502">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="55ac5-503">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-503">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="55ac5-504">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="55ac5-504">AzureRM.DataFactories</span></span>
* <span data-ttu-id="55ac5-505">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-505">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="55ac5-506">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="55ac5-506">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="55ac5-507">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-507">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="55ac5-508">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="55ac5-508">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="55ac5-509">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-509">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="55ac5-510">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="55ac5-510">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="55ac5-511">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-511">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="55ac5-512">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-512">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="55ac5-513">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-513">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="55ac5-514">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-514">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="55ac5-515">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="55ac5-515">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="55ac5-516">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-516">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="55ac5-517">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="55ac5-517">AzureRM.Dns</span></span>
* <span data-ttu-id="55ac5-518">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-518">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="55ac5-519">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="55ac5-519">AzureRM.EventGrid</span></span>
* <span data-ttu-id="55ac5-520">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-520">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="55ac5-521">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="55ac5-521">AzureRM.EventHub</span></span>
* <span data-ttu-id="55ac5-522">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-522">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="55ac5-523">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="55ac5-523">AzureRM.HDInsight</span></span>
* <span data-ttu-id="55ac5-524">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-524">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="55ac5-525">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="55ac5-525">AzureRM.Insights</span></span>
* <span data-ttu-id="55ac5-526">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-526">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="55ac5-527">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="55ac5-527">AzureRM.IotHub</span></span>
* <span data-ttu-id="55ac5-528">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-528">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="55ac5-529">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55ac5-529">AzureRM.KeyVault</span></span>
* <span data-ttu-id="55ac5-530">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-530">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="55ac5-531">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="55ac5-531">AzureRM.LogicApp</span></span>
* <span data-ttu-id="55ac5-532">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-532">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="55ac5-533">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="55ac5-533">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="55ac5-534">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-534">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="55ac5-535">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="55ac5-535">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="55ac5-536">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-536">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="55ac5-537">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="55ac5-537">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="55ac5-538">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-538">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="55ac5-539">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="55ac5-539">AzureRM.Media</span></span>
* <span data-ttu-id="55ac5-540">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-540">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-541">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-541">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-542">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-542">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="55ac5-543">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-543">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="55ac5-544">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-544">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="55ac5-545">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-545">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="55ac5-546">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-546">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="55ac5-547">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-547">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="55ac5-548">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-548">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="55ac5-549">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-549">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="55ac5-550">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="55ac5-550">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="55ac5-551">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-551">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="55ac5-552">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="55ac5-552">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="55ac5-553">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-553">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="55ac5-554">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="55ac5-554">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="55ac5-555">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-555">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="55ac5-556">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="55ac5-556">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="55ac5-557">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-557">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="55ac5-558">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-558">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="55ac5-559">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-559">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="55ac5-560">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-560">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="55ac5-561">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-561">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="55ac5-562">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-562">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="55ac5-563">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-563">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="55ac5-564">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-564">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="55ac5-565">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-565">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="55ac5-566">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="55ac5-566">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="55ac5-567">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-567">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="55ac5-568">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="55ac5-568">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="55ac5-569">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-569">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="55ac5-570">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="55ac5-570">AzureRM.RedisCache</span></span>
* <span data-ttu-id="55ac5-571">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-571">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="55ac5-572">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="55ac5-572">AzureRM.Relay</span></span>
* <span data-ttu-id="55ac5-573">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-573">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-574">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-574">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-575">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="55ac5-575">Support template deployment at subscription scope.</span></span> <span data-ttu-id="55ac5-576">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-576">Add new Cmdlets:</span></span>
    - <span data-ttu-id="55ac5-577">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="55ac5-577">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="55ac5-578">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="55ac5-578">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="55ac5-579">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="55ac5-579">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="55ac5-580">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="55ac5-580">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="55ac5-581">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="55ac5-581">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="55ac5-582">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="55ac5-582">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="55ac5-583">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="55ac5-583">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="55ac5-584">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-584">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="55ac5-585">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-585">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="55ac5-586">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-586">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="55ac5-587">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="55ac5-587">AzureRM.Scheduler</span></span>
* <span data-ttu-id="55ac5-588">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-588">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-589">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-589">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-590">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-590">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="55ac5-591">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="55ac5-591">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="55ac5-592">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-592">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-593">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-593">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-594">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-594">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="55ac5-595">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-595">AzureRM.Storage</span></span>
* <span data-ttu-id="55ac5-596">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-596">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="55ac5-597">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="55ac5-597">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="55ac5-598">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-598">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="55ac5-599">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="55ac5-599">AzureRM.Tags</span></span>
* <span data-ttu-id="55ac5-600">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-600">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="55ac5-601">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="55ac5-601">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="55ac5-602">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-602">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="55ac5-603">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="55ac5-603">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="55ac5-604">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-604">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-605">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-605">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-606">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-606">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="55ac5-607">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-607">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="55ac5-608">全般</span><span class="sxs-lookup"><span data-stu-id="55ac5-608">General</span></span>
* <span data-ttu-id="55ac5-609">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-609">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-610">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-610">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-611">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-611">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="55ac5-612">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-612">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="55ac5-613">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-613">Azure.Storage</span></span>
* <span data-ttu-id="55ac5-614">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-614">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="55ac5-615">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-615">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="55ac5-616">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55ac5-616">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="55ac5-617">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="55ac5-617">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="55ac5-618">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-618">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="55ac5-619">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="55ac5-619">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="55ac5-620">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-620">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="55ac5-621">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="55ac5-621">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="55ac5-622">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-622">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-623">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-623">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-624">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-624">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="55ac5-625">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-625">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="55ac5-626">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="55ac5-626">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="55ac5-627">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="55ac5-627">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="55ac5-628">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-628">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="55ac5-629">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-629">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="55ac5-630">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-630">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="55ac5-631">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-631">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="55ac5-632">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-632">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="55ac5-633">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-633">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="55ac5-634">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="55ac5-634">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="55ac5-635">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-635">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="55ac5-636">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-636">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="55ac5-637">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-637">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="55ac5-638">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-638">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="55ac5-639">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="55ac5-639">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="55ac5-640">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-640">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="55ac5-641">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="55ac5-641">AzureRM.EventHub</span></span>
* <span data-ttu-id="55ac5-642">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-642">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="55ac5-643">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="55ac5-643">AzureRM.Insights</span></span>
* <span data-ttu-id="55ac5-644">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-644">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="55ac5-645">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="55ac5-645">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="55ac5-646">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55ac5-646">AzureRM.KeyVault</span></span>
* <span data-ttu-id="55ac5-647">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-647">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-648">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-648">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-649">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-649">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-650">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-650">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-651">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-651">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="55ac5-652">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-652">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-653">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-653">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-654">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-654">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="55ac5-655">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-655">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-656">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-656">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-657">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-657">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="55ac5-658">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="55ac5-658">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="55ac5-659">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-659">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="55ac5-660">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="55ac5-660">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="55ac5-661">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="55ac5-661">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="55ac5-662">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="55ac5-662">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="55ac5-663">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-663">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="55ac5-664">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-664">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="55ac5-665">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-665">AzureRM.Storage</span></span>
* <span data-ttu-id="55ac5-666">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-666">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="55ac5-667">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="55ac5-667">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="55ac5-668">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="55ac5-668">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="55ac5-669">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="55ac5-669">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="55ac5-670">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="55ac5-670">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="55ac5-671">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="55ac5-671">AzureRM.Tags</span></span>
* <span data-ttu-id="55ac5-672">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-672">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="55ac5-673">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-673">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-674">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-674">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-675">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-675">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="55ac5-676">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-676">Azure.Storage</span></span>
* <span data-ttu-id="55ac5-677">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="55ac5-677">Support Upload Blob or File with write only Sas token</span></span>
* <span data-ttu-id="55ac5-678">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="55ac5-678">Set-AzureStorageBlobContent</span></span>
* <span data-ttu-id="55ac5-679">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="55ac5-679">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="55ac5-680">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-680">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="55ac5-681">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-681">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="55ac5-682">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="55ac5-682">AzureRM.Automation</span></span>
* <span data-ttu-id="55ac5-683">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-683">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-684">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-684">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-685">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-685">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="55ac5-686">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-686">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="55ac5-687">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-687">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="55ac5-688">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-688">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="55ac5-689">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-689">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="55ac5-690">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="55ac5-690">AzureRM.EventHub</span></span>
* <span data-ttu-id="55ac5-691">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-691">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="55ac5-692">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55ac5-692">AzureRM.KeyVault</span></span>
* <span data-ttu-id="55ac5-693">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-693">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="55ac5-694">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="55ac5-694">AzureRM.LogicApp</span></span>
* <span data-ttu-id="55ac5-695">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-695">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-696">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-696">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-697">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="55ac5-697">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="55ac5-698">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-698">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="55ac5-699">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-699">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="55ac5-700">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-700">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="55ac5-701">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-701">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="55ac5-702">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-702">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="55ac5-703">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="55ac5-703">AzureRM.Relay</span></span>
* <span data-ttu-id="55ac5-704">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-704">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-705">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-705">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-706">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-706">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="55ac5-707">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-707">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="55ac5-708">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-708">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="55ac5-709">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-709">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="55ac5-710">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-710">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-711">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-711">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-712">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-712">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="55ac5-713">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-713">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="55ac5-714">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="55ac5-714">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="55ac5-715">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="55ac5-715">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="55ac5-716">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="55ac5-716">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="55ac5-717">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="55ac5-717">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="55ac5-718">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="55ac5-718">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="55ac5-719">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-719">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="55ac5-720">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="55ac5-720">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="55ac5-721">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-721">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-722">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-722">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-723">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-723">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="55ac5-724">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-724">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="55ac5-725">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-725">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-726">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-726">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-727">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="55ac5-727">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="55ac5-728">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-728">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="55ac5-729">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="55ac5-729">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="55ac5-730">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-730">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="55ac5-731">全般</span><span class="sxs-lookup"><span data-stu-id="55ac5-731">General</span></span>
* <span data-ttu-id="55ac5-732">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-732">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-733">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-733">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-734">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-734">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-735">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-735">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-736">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="55ac5-736">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="55ac5-737">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-737">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="55ac5-738">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-738">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="55ac5-739">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="55ac5-739">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="55ac5-740">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-740">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="55ac5-741">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="55ac5-741">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="55ac5-742">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-742">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="55ac5-743">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="55ac5-743">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="55ac5-744">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-744">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="55ac5-745">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="55ac5-745">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="55ac5-746">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="55ac5-746">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="55ac5-747">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="55ac5-747">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="55ac5-748">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="55ac5-748">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="55ac5-749">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-749">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="55ac5-750">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-750">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="55ac5-751">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-751">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="55ac5-752">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-752">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="55ac5-753">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="55ac5-753">AzureRM.EventHub</span></span>
* <span data-ttu-id="55ac5-754">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-754">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="55ac5-755">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-755">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="55ac5-756">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-756">Provided Default Parameter set.</span></span>
* <span data-ttu-id="55ac5-757">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-757">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="55ac5-758">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55ac5-758">AzureRM.KeyVault</span></span>
* <span data-ttu-id="55ac5-759">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-759">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-760">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-760">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-761">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-761">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="55ac5-762">次の機能のために新しいコマンドを追加しました: ExpressRoute Partner API (ARM を介して)</span><span class="sxs-lookup"><span data-stu-id="55ac5-762">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="55ac5-763">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-763">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="55ac5-764">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-764">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="55ac5-765">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-765">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="55ac5-766">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-766">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="55ac5-767">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-767">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="55ac5-768">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-768">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="55ac5-769">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-769">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="55ac5-770">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-770">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="55ac5-771">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-771">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="55ac5-772">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-772">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="55ac5-773">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="55ac5-773">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="55ac5-774">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-774">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-775">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-775">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-776">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-776">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="55ac5-777">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-777">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="55ac5-778">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="55ac5-778">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="55ac5-779">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-779">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="55ac5-780">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-780">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="55ac5-781">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-781">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="55ac5-782">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-782">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="55ac5-783">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-783">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="55ac5-784">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-784">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="55ac5-785">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-785">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="55ac5-786">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-786">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="55ac5-787">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-787">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="55ac5-788">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-788">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="55ac5-789">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="55ac5-789">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="55ac5-790">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-790">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-791">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-791">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-792">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-792">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="55ac5-793">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-793">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="55ac5-794">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-794">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-795">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-795">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-796">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-796">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="55ac5-797">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="55ac5-797">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="55ac5-798">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="55ac5-798">Azure.Storage</span></span>
* <span data-ttu-id="55ac5-799">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-799">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-800">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-800">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-801">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-801">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="55ac5-802">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-802">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="55ac5-803">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="55ac5-803">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="55ac5-804">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="55ac5-804">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="55ac5-805">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="55ac5-805">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="55ac5-806">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-806">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="55ac5-807">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="55ac5-807">Start-AzureRmVM</span></span>
    - <span data-ttu-id="55ac5-808">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="55ac5-808">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="55ac5-809">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="55ac5-809">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="55ac5-810">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="55ac5-810">Set-AzureRmVM</span></span>
    - <span data-ttu-id="55ac5-811">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="55ac5-811">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="55ac5-812">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="55ac5-812">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="55ac5-813">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="55ac5-813">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="55ac5-814">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="55ac5-814">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="55ac5-815">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="55ac5-815">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="55ac5-816">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="55ac5-816">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="55ac5-817">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="55ac5-817">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="55ac5-818">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="55ac5-818">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="55ac5-819">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="55ac5-819">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="55ac5-820">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="55ac5-820">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="55ac5-821">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="55ac5-821">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="55ac5-822">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="55ac5-822">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="55ac5-823">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="55ac5-823">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="55ac5-824">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="55ac5-824">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="55ac5-825">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="55ac5-825">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="55ac5-826">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="55ac5-826">AzureRM.EventGrid</span></span>
* <span data-ttu-id="55ac5-827">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-827">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="55ac5-828">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55ac5-828">AzureRM.KeyVault</span></span>
* <span data-ttu-id="55ac5-829">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-829">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="55ac5-830">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="55ac5-830">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="55ac5-831">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="55ac5-831">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="55ac5-832">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="55ac5-832">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="55ac5-833">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-833">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="55ac5-834">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="55ac5-834">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="55ac5-835">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-835">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="55ac5-836">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-836">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-837">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-837">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-838">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-838">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="55ac5-839">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="55ac5-839">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="55ac5-840">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-840">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-841">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-841">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-842">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-842">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="55ac5-843">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="55ac5-843">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="55ac5-844">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-844">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="55ac5-845">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="55ac5-845">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="55ac5-846">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-846">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="55ac5-847">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-847">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-848">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-848">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-849">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-849">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="55ac5-850">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="55ac5-850">AzureRM.Compute</span></span>
* <span data-ttu-id="55ac5-851">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="55ac5-851">VMSS VM Update feature</span></span>
    - <span data-ttu-id="55ac5-852">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-852">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="55ac5-853">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-853">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="55ac5-854">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="55ac5-854">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="55ac5-855">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-855">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="55ac5-856">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-856">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="55ac5-857">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-857">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="55ac5-858">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-858">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="55ac5-859">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-859">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="55ac5-860">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="55ac5-860">AzureRM.KeyVault</span></span>
* <span data-ttu-id="55ac5-861">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-861">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-862">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-862">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-863">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="55ac5-863">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="55ac5-864">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="55ac5-864">AzureRM.Resources</span></span>
* <span data-ttu-id="55ac5-865">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-865">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="55ac5-866">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="55ac5-866">AzureRM.Scheduler</span></span>
* <span data-ttu-id="55ac5-867">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-867">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="55ac5-868">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-868">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-869">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="55ac5-869">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="55ac5-870">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-870">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="55ac5-871">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="55ac5-871">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="55ac5-872">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="55ac5-872">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="55ac5-873">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="55ac5-873">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="55ac5-874">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-874">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="55ac5-875">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="55ac5-875">AzureRM.Websites</span></span>
* <span data-ttu-id="55ac5-876">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-876">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="55ac5-877">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="55ac5-877">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="55ac5-878">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="55ac5-878">AzureRM.Profile</span></span>
* <span data-ttu-id="55ac5-879">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-879">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="55ac5-880">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="55ac5-880">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="55ac5-881">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="55ac5-881">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="55ac5-882">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="55ac5-882">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="55ac5-883">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-883">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="55ac5-884">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-884">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="55ac5-885">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-885">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="55ac5-886">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-886">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="55ac5-887">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-887">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="55ac5-888">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-888">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="55ac5-889">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-889">Added support for MSI identity</span></span>
* <span data-ttu-id="55ac5-890">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です</span><span class="sxs-lookup"><span data-stu-id="55ac5-890">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="55ac5-891">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="55ac5-891">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="55ac5-892">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-892">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="55ac5-893">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="55ac5-893">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="55ac5-894">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="55ac5-894">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="55ac5-895">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="55ac5-895">AzureRM.Batch</span></span>
* <span data-ttu-id="55ac5-896">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-896">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="55ac5-897">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-897">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="55ac5-898">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="55ac5-898">AzureRM.Consumption</span></span>
* <span data-ttu-id="55ac5-899">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-899">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="55ac5-900">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="55ac5-900">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="55ac5-901">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-901">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="55ac5-902">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-902">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="55ac5-903">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-903">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="55ac5-904">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="55ac5-904">AzureRM.Network</span></span>
* <span data-ttu-id="55ac5-905">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-905">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="55ac5-906">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-906">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="55ac5-907">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="55ac5-907">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="55ac5-908">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-908">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="55ac5-909">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-909">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="55ac5-910">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-910">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="55ac5-911">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-911">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="55ac5-912">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-912">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="55ac5-913">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="55ac5-913">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="55ac5-914">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="55ac5-914">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="55ac5-915">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="55ac5-915">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="55ac5-916">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="55ac5-916">AzureRM.Sql</span></span>
* <span data-ttu-id="55ac5-917">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-917">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="55ac5-918">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="55ac5-918">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="55ac5-919">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-919">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="55ac5-920">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="55ac5-920">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="55ac5-921">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="55ac5-921">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="55ac5-922">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-922">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="55ac5-923">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="55ac5-923">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="55ac5-924">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="55ac5-924">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="55ac5-925">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="55ac5-925">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="55ac5-926">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="55ac5-926">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="55ac5-927">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="55ac5-927">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="55ac5-928">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="55ac5-928">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
