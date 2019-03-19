---
ms.openlocfilehash: 9915ff37e59a73c1d226a216213fd9016b55d3d4
ms.sourcegitcommit: 447276d46ffeeb37f0c07a570536665e36c5ddb8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "57882474"
---
## <a name="150---march-2019"></a><span data-ttu-id="6643d-101">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="6643d-101">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6643d-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6643d-102">Az.Accounts</span></span>
* <span data-ttu-id="6643d-103">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-103">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="6643d-104">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-104">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6643d-105">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6643d-105">Az.Automation</span></span>
* <span data-ttu-id="6643d-106">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-106">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="6643d-107">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-107">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="6643d-108">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="6643d-108">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6643d-109">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6643d-109">Az.Cdn</span></span>
* <span data-ttu-id="6643d-110">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="6643d-110">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-111">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-111">Az.Compute</span></span>
* <span data-ttu-id="6643d-112">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-112">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6643d-113">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6643d-113">Az.DataFactory</span></span>
* <span data-ttu-id="6643d-114">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-114">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6643d-115">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6643d-115">Az.LogicApp</span></span>
* <span data-ttu-id="6643d-116">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-116">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6643d-117">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-117">Az.Network</span></span>
* <span data-ttu-id="6643d-118">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-118">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6643d-119">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6643d-119">Az.RecoveryServices</span></span>
* <span data-ttu-id="6643d-120">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-120">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="6643d-121">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="6643d-121">SDK Update</span></span>
* <span data-ttu-id="6643d-122">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="6643d-122">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="6643d-123">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-123">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-124">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-124">Az.Resources</span></span>
* <span data-ttu-id="6643d-125">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-125">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="6643d-126">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="6643d-126">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="6643d-127">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-127">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="6643d-128">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="6643d-128">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="6643d-129">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-129">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="6643d-130">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="6643d-130">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="6643d-131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-131">Az.Sql</span></span>
* <span data-ttu-id="6643d-132">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-132">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="6643d-133">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-133">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6643d-134">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6643d-134">Az.Storage</span></span>
* <span data-ttu-id="6643d-135">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="6643d-135">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="6643d-136">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="6643d-136">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="6643d-137">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6643d-137">Az.AnalysisServices</span></span>
* <span data-ttu-id="6643d-138">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="6643d-138">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6643d-139">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6643d-139">Az.Automation</span></span>
* <span data-ttu-id="6643d-140">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-140">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="6643d-141">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-141">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="6643d-142">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="6643d-142">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="6643d-143">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6643d-143">Az.CognitiveServices</span></span>
* <span data-ttu-id="6643d-144">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="6643d-144">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-145">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-145">Az.Compute</span></span>
* <span data-ttu-id="6643d-146">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-146">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="6643d-147">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-147">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="6643d-148">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-148">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="6643d-149">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="6643d-149">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6643d-150">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-150">Az.DataLakeStore</span></span>
* <span data-ttu-id="6643d-151">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-151">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="6643d-152">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="6643d-152">Az.EventHub</span></span>
* <span data-ttu-id="6643d-153">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-153">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="6643d-154">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6643d-154">Az.KeyVault</span></span>
* <span data-ttu-id="6643d-155">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-155">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6643d-156">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6643d-156">Az.LogicApp</span></span>
* <span data-ttu-id="6643d-157">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-157">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="6643d-158">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-158">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="6643d-159">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6643d-159">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="6643d-160">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6643d-160">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="6643d-161">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6643d-161">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="6643d-162">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6643d-162">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="6643d-163">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="6643d-163">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="6643d-164">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6643d-164">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="6643d-165">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6643d-165">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="6643d-166">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6643d-166">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="6643d-167">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6643d-167">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="6643d-168">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="6643d-168">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="6643d-169">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-169">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="6643d-170">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6643d-170">Az.Monitor</span></span>
* <span data-ttu-id="6643d-171">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-171">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6643d-172">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-172">Az.Network</span></span>
* <span data-ttu-id="6643d-173">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-173">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="6643d-174">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6643d-174">Az.OperationalInsights</span></span>
* <span data-ttu-id="6643d-175">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-175">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="6643d-176">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-176">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="6643d-177">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-177">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="6643d-178">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-178">Az.Resources</span></span>
* <span data-ttu-id="6643d-179">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="6643d-179">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="6643d-180">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="6643d-180">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="6643d-181">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="6643d-181">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="6643d-182">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-182">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="6643d-183">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-183">Az.Sql</span></span>
* <span data-ttu-id="6643d-184">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-184">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="6643d-185">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-185">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6643d-186">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6643d-186">Az.Websites</span></span>
* <span data-ttu-id="6643d-187">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-187">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="6643d-188">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="6643d-188">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6643d-189">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6643d-189">Az.Accounts</span></span>
* <span data-ttu-id="6643d-190">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="6643d-190">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="6643d-191">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6643d-191">Az.AnalysisServices</span></span>
<span data-ttu-id="6643d-192">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="6643d-192">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-193">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-193">Az.Compute</span></span>
* <span data-ttu-id="6643d-194">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6643d-194">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="6643d-195">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-195">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="6643d-196">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-196">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6643d-197">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6643d-197">Az.RecoveryServices</span></span>
<span data-ttu-id="6643d-198">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="6643d-198">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-199">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-199">Az.Resources</span></span>
* <span data-ttu-id="6643d-200">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="6643d-200">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="6643d-201">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="6643d-201">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="6643d-202">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-202">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="6643d-203">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="6643d-203">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="6643d-204">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-204">Az.Sql</span></span>
* <span data-ttu-id="6643d-205">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="6643d-205">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="6643d-206">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-206">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="6643d-207">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-207">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="6643d-208">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="6643d-208">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6643d-209">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6643d-209">Az.Accounts</span></span>
* <span data-ttu-id="6643d-210">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="6643d-210">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="6643d-211">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="6643d-211">Az.AnalysisServices</span></span>
* <span data-ttu-id="6643d-212">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="6643d-212">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="6643d-213">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6643d-213">Az.RecoveryServices</span></span>
* <span data-ttu-id="6643d-214">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="6643d-214">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="6643d-215">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="6643d-215">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6643d-216">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6643d-216">Az.Accounts</span></span>
* <span data-ttu-id="6643d-217">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="6643d-217">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="6643d-218">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-218">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6643d-219">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="6643d-219">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="6643d-220">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="6643d-220">Az.Aks</span></span>
* <span data-ttu-id="6643d-221">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-221">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="6643d-222">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6643d-222">Az.Automation</span></span>
* <span data-ttu-id="6643d-223">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="6643d-223">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="6643d-224">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-224">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="6643d-225">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="6643d-225">Az.Cdn</span></span>
* <span data-ttu-id="6643d-226">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-226">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-227">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-227">Az.Compute</span></span>
* <span data-ttu-id="6643d-228">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="6643d-228">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="6643d-229">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="6643d-229">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="6643d-230">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="6643d-230">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="6643d-231">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="6643d-231">Az.ContainerRegistry</span></span>
* <span data-ttu-id="6643d-232">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-232">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="6643d-233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="6643d-233">Az.DataFactory</span></span>
* <span data-ttu-id="6643d-234">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="6643d-234">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6643d-235">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-235">Az.DataLakeStore</span></span>
* <span data-ttu-id="6643d-236">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="6643d-236">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="6643d-237">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="6643d-237">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="6643d-238">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-238">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6643d-239">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6643d-239">Az.IotHub</span></span>
* <span data-ttu-id="6643d-240">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="6643d-240">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="6643d-241">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6643d-241">Az.KeyVault</span></span>
* <span data-ttu-id="6643d-242">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-242">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6643d-243">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-243">Az.Network</span></span>
* <span data-ttu-id="6643d-244">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-244">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-245">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-245">Az.Resources</span></span>
* <span data-ttu-id="6643d-246">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-246">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="6643d-247">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-247">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="6643d-248">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="6643d-248">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="6643d-249">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="6643d-249">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="6643d-250">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="6643d-250">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="6643d-251">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-251">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="6643d-252">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="6643d-252">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6643d-253">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6643d-253">Az.ServiceFabric</span></span>
* <span data-ttu-id="6643d-254">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="6643d-254">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="6643d-255">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="6643d-255">Fix some error messages.</span></span>
* <span data-ttu-id="6643d-256">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-256">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="6643d-257">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-257">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="6643d-258">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="6643d-258">Az.SignalR</span></span>
* <span data-ttu-id="6643d-259">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-259">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="6643d-260">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-260">Az.Sql</span></span>
* <span data-ttu-id="6643d-261">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-261">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6643d-262">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-262">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="6643d-263">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-263">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="6643d-264">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="6643d-264">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6643d-265">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6643d-265">Az.Storage</span></span>
* <span data-ttu-id="6643d-266">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-266">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6643d-267">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="6643d-267">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="6643d-268">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="6643d-268">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="6643d-269">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="6643d-269">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="6643d-270">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="6643d-270">Az.TrafficManager</span></span>
* <span data-ttu-id="6643d-271">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-271">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6643d-272">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6643d-272">Az.Websites</span></span>
* <span data-ttu-id="6643d-273">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="6643d-273">Update incorrect online help URLs</span></span>
* <span data-ttu-id="6643d-274">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-274">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="6643d-275">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="6643d-275">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="6643d-276">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="6643d-276">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="6643d-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6643d-277">Az.Accounts</span></span>
* <span data-ttu-id="6643d-278">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="6643d-278">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-279">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-279">Az.Compute</span></span>
* <span data-ttu-id="6643d-280">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="6643d-280">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="6643d-281">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="6643d-281">Updated the description of ID in help files</span></span>
* <span data-ttu-id="6643d-282">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-282">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6643d-283">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-283">Az.DataLakeStore</span></span>
* <span data-ttu-id="6643d-284">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-284">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="6643d-285">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-285">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="6643d-286">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="6643d-286">Az.EventGrid</span></span>
* <span data-ttu-id="6643d-287">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-287">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="6643d-288">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="6643d-288">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="6643d-289">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="6643d-289">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="6643d-290">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="6643d-290">Event Time-To-Live,</span></span>
        - <span data-ttu-id="6643d-291">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="6643d-291">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="6643d-292">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="6643d-292">Dead letter endpoint.</span></span>
    - <span data-ttu-id="6643d-293">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="6643d-293">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="6643d-294">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="6643d-294">Event Time-To-Live,</span></span>
        - <span data-ttu-id="6643d-295">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="6643d-295">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="6643d-296">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="6643d-296">Dead letter endpoint.</span></span>
* <span data-ttu-id="6643d-297">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-297">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="6643d-298">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="6643d-298">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="6643d-299">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="6643d-299">Az.IotHub</span></span>
* <span data-ttu-id="6643d-300">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-300">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="6643d-301">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="6643d-301">Az.LogicApp</span></span>
* <span data-ttu-id="6643d-302">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="6643d-302">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-303">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-303">Az.Resources</span></span>
* <span data-ttu-id="6643d-304">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-304">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="6643d-305">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="6643d-305">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="6643d-306">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-306">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="6643d-307">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-307">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="6643d-308">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="6643d-308">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="6643d-309">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="6643d-309">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="6643d-310">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="6643d-310">Az.SignalR</span></span>
* <span data-ttu-id="6643d-311">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-311">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="6643d-312">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-312">Az.Sql</span></span>
* <span data-ttu-id="6643d-313">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="6643d-313">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="6643d-314">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6643d-314">Az.Storage</span></span>
* <span data-ttu-id="6643d-315">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="6643d-315">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="6643d-316">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="6643d-316">New-AzStorageContext</span></span>
* <span data-ttu-id="6643d-317">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-317">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="6643d-318">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="6643d-318">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6643d-319">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6643d-319">Az.Websites</span></span>
* <span data-ttu-id="6643d-320">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-320">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="6643d-321">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-321">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="6643d-322">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="6643d-322">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="6643d-323">全般</span><span class="sxs-lookup"><span data-stu-id="6643d-323">General</span></span>

- <span data-ttu-id="6643d-324">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="6643d-324">General Availability of Az Module</span></span>
- <span data-ttu-id="6643d-325">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="6643d-325">Online help for each module</span></span>
- <span data-ttu-id="6643d-326">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-326">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="6643d-327">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-327">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="6643d-328">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="6643d-328">Az.Accounts</span></span>
- <span data-ttu-id="6643d-329">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="6643d-329">Changed from Az.Profile</span></span>
- <span data-ttu-id="6643d-330">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-330">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="6643d-331">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6643d-331">Az.ApiManagement</span></span>
- <span data-ttu-id="6643d-332">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="6643d-332">Fixes for #7002</span></span>
- <span data-ttu-id="6643d-333">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-333">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="6643d-334">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="6643d-334">Az.Batch</span></span>
- <span data-ttu-id="6643d-335">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-335">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="6643d-336">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="6643d-336">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="6643d-337">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-337">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="6643d-338">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="6643d-338">Az.Billing</span></span>
- <span data-ttu-id="6643d-339">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-339">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="6643d-340">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="6643d-340">Az.CognitivServices</span></span>
- <span data-ttu-id="6643d-341">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-341">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="6643d-342">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="6643d-342">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="6643d-343">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="6643d-343">Az.ContainerInstance</span></span>
- <span data-ttu-id="6643d-344">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-344">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="6643d-345">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="6643d-345">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="6643d-346">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-346">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="6643d-347">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-347">Az.DataLakeStore</span></span>
- <span data-ttu-id="6643d-348">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-348">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="6643d-349">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="6643d-349">Az.Monitor</span></span>
- <span data-ttu-id="6643d-350">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-350">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="6643d-351">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="6643d-351">Az.KeyVault</span></span>
- <span data-ttu-id="6643d-352">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="6643d-352">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="6643d-353">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="6643d-353">Az.MachineLearning</span></span>
- <span data-ttu-id="6643d-354">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="6643d-354">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="6643d-355">Az.Media</span><span class="sxs-lookup"><span data-stu-id="6643d-355">Az.Media</span></span>
- <span data-ttu-id="6643d-356">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="6643d-356">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="6643d-357">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-357">Az.Network</span></span>
<span data-ttu-id="6643d-358">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-358">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="6643d-359">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6643d-359">New cmdlets added:</span></span>
        - <span data-ttu-id="6643d-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6643d-360">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6643d-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6643d-361">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6643d-362">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6643d-362">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6643d-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6643d-363">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6643d-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="6643d-364">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="6643d-365">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="6643d-365">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="6643d-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="6643d-366">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="6643d-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="6643d-367">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="6643d-368">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6643d-368">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="6643d-369">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="6643d-369">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="6643d-370">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="6643d-370">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="6643d-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="6643d-371">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="6643d-372">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="6643d-372">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="6643d-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="6643d-373">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="6643d-374">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-374">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="6643d-375">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="6643d-375">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="6643d-376">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="6643d-376">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="6643d-377">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="6643d-377">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="6643d-378">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="6643d-378">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="6643d-379">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="6643d-379">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="6643d-380">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-380">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="6643d-381">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="6643d-381">Az.OperationalInsights</span></span>
- <span data-ttu-id="6643d-382">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-382">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="6643d-383">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="6643d-383">Az.Profile</span></span>
- <span data-ttu-id="6643d-384">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="6643d-384">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="6643d-385">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6643d-385">Az.RecoveryServices</span></span>
- <span data-ttu-id="6643d-386">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="6643d-387">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-387">Az.Resources</span></span>
- <span data-ttu-id="6643d-388">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="6643d-389">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6643d-389">Az.ServiceFabric</span></span>
- <span data-ttu-id="6643d-390">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="6643d-390">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="6643d-391">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-391">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="6643d-392">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="6643d-392">Az.SIgnalR</span></span>
- <span data-ttu-id="6643d-393">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="6643d-393">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="6643d-394">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-394">Az.Sql</span></span>
- <span data-ttu-id="6643d-395">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-395">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="6643d-396">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-396">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="6643d-397">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-397">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="6643d-398">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6643d-398">Az.Storage</span></span>
- <span data-ttu-id="6643d-399">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-399">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="6643d-400">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6643d-400">Az.Websites</span></span>
- <span data-ttu-id="6643d-401">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="6643d-401">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="6643d-402">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="6643d-402">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="6643d-403">全般</span><span class="sxs-lookup"><span data-stu-id="6643d-403">General</span></span>

* <span data-ttu-id="6643d-404">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="6643d-404">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="6643d-405">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-405">Az.Compute</span></span>

* <span data-ttu-id="6643d-406">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-406">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="6643d-407">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-407">Az.DataLakeStore</span></span>

* <span data-ttu-id="6643d-408">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-408">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="6643d-409">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="6643d-409">Az.FrontDoor</span></span>

* <span data-ttu-id="6643d-410">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-410">Fixed some broken links</span></span>
    - <span data-ttu-id="6643d-411">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-411">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="6643d-412">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-412">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="6643d-413">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="6643d-413">Az.RecoveryServices</span></span>

* <span data-ttu-id="6643d-414">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-414">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="6643d-415">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="6643d-415">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="6643d-416">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-416">Az.Resources</span></span>

* <span data-ttu-id="6643d-417">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="6643d-417">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="6643d-418">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-418">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="6643d-419">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-419">Az.Sql</span></span>

* <span data-ttu-id="6643d-420">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="6643d-420">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="6643d-421">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-421">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="6643d-422">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="6643d-422">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="6643d-423">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="6643d-423">Az.Storage</span></span>

* <span data-ttu-id="6643d-424">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-424">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="6643d-425">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-425">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="6643d-426">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="6643d-426">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="6643d-427">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="6643d-427">Support Static Website configuration</span></span>
    - <span data-ttu-id="6643d-428">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="6643d-428">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="6643d-429">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="6643d-429">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="6643d-430">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6643d-430">Az.Websites</span></span>

* <span data-ttu-id="6643d-431">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="6643d-431">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="6643d-432">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-432">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="6643d-433">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="6643d-433">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="6643d-434">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="6643d-434">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="6643d-435">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="6643d-435">Az.ApiManagement</span></span>
* <span data-ttu-id="6643d-436">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-436">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="6643d-437">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="6643d-437">Az.Automation</span></span>
* <span data-ttu-id="6643d-438">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="6643d-438">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="6643d-439">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-439">Added Update Management cmdlets</span></span>
* <span data-ttu-id="6643d-440">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-440">Added Source Control cmdlets</span></span>
* <span data-ttu-id="6643d-441">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-441">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="6643d-442">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-442">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="6643d-443">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-443">Az.Compute</span></span>
* <span data-ttu-id="6643d-444">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-444">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="6643d-445">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-445">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="6643d-446">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="6643d-446">Az.ContainerInstance</span></span>
* <span data-ttu-id="6643d-447">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-447">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="6643d-448">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="6643d-448">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="6643d-449">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-449">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="6643d-450">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-450">Az.Network</span></span>
* <span data-ttu-id="6643d-451">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-451">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="6643d-452">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-452">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="6643d-453">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-453">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="6643d-454">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-454">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="6643d-455">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="6643d-455">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="6643d-456">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-456">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="6643d-457">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="6643d-457">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="6643d-458">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="6643d-458">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="6643d-459">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-459">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="6643d-460">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-460">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="6643d-461">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="6643d-461">Az.Relay</span></span>
* <span data-ttu-id="6643d-462">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="6643d-462">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="6643d-463">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-463">Az.Resources</span></span>
* <span data-ttu-id="6643d-464">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-464">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="6643d-465">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-465">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="6643d-466">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="6643d-466">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="6643d-467">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6643d-467">Az.ServiceFabric</span></span>
* <span data-ttu-id="6643d-468">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-468">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="6643d-469">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-469">Az.Sql</span></span>
* <span data-ttu-id="6643d-470">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-470">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="6643d-471">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6643d-471">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6643d-472">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6643d-472">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6643d-473">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6643d-473">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6643d-474">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="6643d-474">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="6643d-475">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6643d-475">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="6643d-476">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6643d-476">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="6643d-477">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6643d-477">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="6643d-478">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="6643d-478">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="6643d-479">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="6643d-479">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="6643d-480">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-480">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="6643d-481">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="6643d-481">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="6643d-482">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="6643d-482">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="6643d-483">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="6643d-483">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="6643d-484">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="6643d-484">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="6643d-485">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="6643d-485">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="6643d-486">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-486">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="6643d-487">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="6643d-487">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="6643d-488">全般</span><span class="sxs-lookup"><span data-stu-id="6643d-488">General</span></span>
* <span data-ttu-id="6643d-489">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="6643d-489">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="6643d-490">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="6643d-490">Az.Profile</span></span>
* <span data-ttu-id="6643d-491">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-491">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="6643d-492">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-492">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="6643d-493">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="6643d-493">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="6643d-494">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-494">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="6643d-495">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-495">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="6643d-496">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-496">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="6643d-497">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-497">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="6643d-498">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6643d-498">Az.CognitiveServices</span></span>
* <span data-ttu-id="6643d-499">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-499">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-500">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-500">Az.Compute</span></span>
* <span data-ttu-id="6643d-501">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-501">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="6643d-502">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="6643d-502">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="6643d-503">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-503">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6643d-504">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-504">Az.DataLakeStore</span></span>
* <span data-ttu-id="6643d-505">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="6643d-505">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="6643d-506">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-506">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="6643d-507">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="6643d-507">Az.Insights</span></span>
* <span data-ttu-id="6643d-508">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-508">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="6643d-509">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="6643d-509">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="6643d-510">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-510">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="6643d-511">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="6643d-511">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6643d-512">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-512">Az.Network</span></span>
* <span data-ttu-id="6643d-513">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="6643d-513">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="6643d-514">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="6643d-514">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="6643d-515">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="6643d-515">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="6643d-516">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="6643d-516">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="6643d-517">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="6643d-517">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="6643d-518">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="6643d-518">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="6643d-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="6643d-519">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="6643d-520">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="6643d-520">Az.PolicyInsights</span></span>
* <span data-ttu-id="6643d-521">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-521">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-522">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-522">Az.Resources</span></span>
* <span data-ttu-id="6643d-523">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="6643d-523">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="6643d-524">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="6643d-524">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="6643d-525">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="6643d-525">Az.ServiceBus</span></span>
* <span data-ttu-id="6643d-526">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-526">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="6643d-527">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="6643d-527">Az.ServiceFabric</span></span>
* <span data-ttu-id="6643d-528">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-528">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="6643d-529">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-529">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="6643d-530">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="6643d-530">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="6643d-531">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="6643d-531">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="6643d-532">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-532">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="6643d-533">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="6643d-533">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="6643d-534">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="6643d-534">Az.Profile</span></span>
* <span data-ttu-id="6643d-535">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-535">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="6643d-536">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-536">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-537">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-537">Az.Compute</span></span>
* <span data-ttu-id="6643d-538">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-538">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="6643d-539">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-539">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="6643d-540">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="6643d-540">Az.DataLakeStore</span></span>
* <span data-ttu-id="6643d-541">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-541">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="6643d-542">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="6643d-542">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="6643d-543">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="6643d-543">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="6643d-544">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="6643d-544">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="6643d-545">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="6643d-545">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6643d-546">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-546">Az.Network</span></span>
* <span data-ttu-id="6643d-547">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-547">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="6643d-548">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-548">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-549">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-549">Az.Resources</span></span>
* <span data-ttu-id="6643d-550">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-550">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="6643d-551">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-551">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="6643d-552">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="6643d-552">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="6643d-553">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="6643d-553">Azure.Storage</span></span>
* <span data-ttu-id="6643d-554">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-554">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="6643d-555">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="6643d-555">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="6643d-556">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="6643d-556">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="6643d-557">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-557">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="6643d-558">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="6643d-558">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="6643d-559">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="6643d-559">Az.CognitiveServices</span></span>
* <span data-ttu-id="6643d-560">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="6643d-560">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="6643d-561">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="6643d-561">Az.Compute</span></span>
* <span data-ttu-id="6643d-562">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-562">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="6643d-563">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-563">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="6643d-564">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-564">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="6643d-565">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="6643d-565">Az.DataFactoryV2</span></span>
* <span data-ttu-id="6643d-566">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-566">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="6643d-567">Az.Network</span><span class="sxs-lookup"><span data-stu-id="6643d-567">Az.Network</span></span>
* <span data-ttu-id="6643d-568">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="6643d-568">Added NetworkProfile functionality.</span></span> <span data-ttu-id="6643d-569">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="6643d-569">new cmdlets added</span></span>
    - <span data-ttu-id="6643d-570">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6643d-570">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="6643d-571">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6643d-571">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="6643d-572">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6643d-572">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="6643d-573">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="6643d-573">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="6643d-574">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="6643d-574">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="6643d-575">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="6643d-575">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="6643d-576">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-576">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="6643d-577">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-577">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="6643d-578">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-578">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="6643d-579">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="6643d-579">Az.RedisCache</span></span>
* <span data-ttu-id="6643d-580">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="6643d-580">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="6643d-581">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-581">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="6643d-582">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="6643d-582">Az.Resources</span></span>
* <span data-ttu-id="6643d-583">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="6643d-583">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="6643d-584">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-584">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="6643d-585">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="6643d-585">Az.Sql</span></span>
* <span data-ttu-id="6643d-586">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="6643d-586">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="6643d-587">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="6643d-587">Az.Websites</span></span>
* <span data-ttu-id="6643d-588">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="6643d-588">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="6643d-589">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="6643d-589">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="6643d-590">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="6643d-590">0.2.0 - September 2018</span></span>
 <span data-ttu-id="6643d-591">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="6643d-591">Initial Release</span></span>