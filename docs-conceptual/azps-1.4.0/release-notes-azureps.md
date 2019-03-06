## <a name="140---february-2019"></a><span data-ttu-id="a312b-101">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="a312b-101">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="a312b-102">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a312b-102">Az.AnalysisServices</span></span>
* <span data-ttu-id="a312b-103">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="a312b-103">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a312b-104">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a312b-104">Az.Automation</span></span>
* <span data-ttu-id="a312b-105">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-105">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="a312b-106">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-106">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="a312b-107">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="a312b-107">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="a312b-108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a312b-108">Az.CognitiveServices</span></span>
* <span data-ttu-id="a312b-109">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="a312b-109">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-110">Az.Compute</span></span>
* <span data-ttu-id="a312b-111">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-111">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="a312b-112">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-112">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="a312b-113">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-113">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="a312b-114">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="a312b-114">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a312b-115">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-115">Az.DataLakeStore</span></span>
* <span data-ttu-id="a312b-116">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-116">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="a312b-117">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="a312b-117">Az.EventHub</span></span>
* <span data-ttu-id="a312b-118">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-118">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="a312b-119">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a312b-119">Az.KeyVault</span></span>
* <span data-ttu-id="a312b-120">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-120">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a312b-121">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a312b-121">Az.LogicApp</span></span>
* <span data-ttu-id="a312b-122">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-122">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="a312b-123">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-123">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="a312b-124">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="a312b-124">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="a312b-125">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a312b-125">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a312b-126">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a312b-126">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a312b-127">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a312b-127">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="a312b-128">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="a312b-128">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="a312b-129">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="a312b-129">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="a312b-130">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a312b-130">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a312b-131">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a312b-131">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a312b-132">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a312b-132">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="a312b-133">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="a312b-133">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="a312b-134">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-134">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="a312b-135">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a312b-135">Az.Monitor</span></span>
* <span data-ttu-id="a312b-136">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-136">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a312b-137">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-137">Az.Network</span></span>
* <span data-ttu-id="a312b-138">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-138">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="a312b-139">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a312b-139">Az.OperationalInsights</span></span>
* <span data-ttu-id="a312b-140">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-140">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="a312b-141">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-141">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="a312b-142">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-142">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="a312b-143">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-143">Az.Resources</span></span>
* <span data-ttu-id="a312b-144">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a312b-144">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a312b-145">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a312b-145">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="a312b-146">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="a312b-146">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="a312b-147">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-147">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="a312b-148">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-148">Az.Sql</span></span>
* <span data-ttu-id="a312b-149">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-149">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="a312b-150">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-150">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a312b-151">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a312b-151">Az.Websites</span></span>
* <span data-ttu-id="a312b-152">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-152">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="a312b-153">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="a312b-153">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a312b-154">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a312b-154">Az.Accounts</span></span>
* <span data-ttu-id="a312b-155">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="a312b-155">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a312b-156">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a312b-156">Az.AnalysisServices</span></span>
<span data-ttu-id="a312b-157">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="a312b-157">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-158">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-158">Az.Compute</span></span>
* <span data-ttu-id="a312b-159">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="a312b-159">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="a312b-160">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-160">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="a312b-161">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-161">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a312b-162">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a312b-162">Az.RecoveryServices</span></span>
<span data-ttu-id="a312b-163">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="a312b-163">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a312b-164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-164">Az.Resources</span></span>
* <span data-ttu-id="a312b-165">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="a312b-165">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="a312b-166">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="a312b-166">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="a312b-167">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-167">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="a312b-168">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="a312b-168">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="a312b-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-169">Az.Sql</span></span>
* <span data-ttu-id="a312b-170">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="a312b-170">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="a312b-171">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-171">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="a312b-172">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-172">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="a312b-173">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="a312b-173">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a312b-174">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a312b-174">Az.Accounts</span></span>
* <span data-ttu-id="a312b-175">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="a312b-175">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="a312b-176">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a312b-176">Az.AnalysisServices</span></span>
* <span data-ttu-id="a312b-177">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="a312b-177">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="a312b-178">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a312b-178">Az.RecoveryServices</span></span>
* <span data-ttu-id="a312b-179">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="a312b-179">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="a312b-180">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="a312b-180">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a312b-181">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a312b-181">Az.Accounts</span></span>
* <span data-ttu-id="a312b-182">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="a312b-182">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="a312b-183">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-183">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a312b-184">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="a312b-184">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="a312b-185">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="a312b-185">Az.Aks</span></span>
* <span data-ttu-id="a312b-186">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-186">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="a312b-187">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a312b-187">Az.Automation</span></span>
* <span data-ttu-id="a312b-188">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="a312b-188">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="a312b-189">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-189">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="a312b-190">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="a312b-190">Az.Cdn</span></span>
* <span data-ttu-id="a312b-191">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-191">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-192">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-192">Az.Compute</span></span>
* <span data-ttu-id="a312b-193">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="a312b-193">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="a312b-194">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="a312b-194">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="a312b-195">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="a312b-195">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="a312b-196">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a312b-196">Az.ContainerRegistry</span></span>
* <span data-ttu-id="a312b-197">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-197">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="a312b-198">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="a312b-198">Az.DataFactory</span></span>
* <span data-ttu-id="a312b-199">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="a312b-199">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a312b-200">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-200">Az.DataLakeStore</span></span>
* <span data-ttu-id="a312b-201">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="a312b-201">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="a312b-202">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="a312b-202">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="a312b-203">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-203">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a312b-204">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a312b-204">Az.IotHub</span></span>
* <span data-ttu-id="a312b-205">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="a312b-205">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="a312b-206">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a312b-206">Az.KeyVault</span></span>
* <span data-ttu-id="a312b-207">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-207">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a312b-208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-208">Az.Network</span></span>
* <span data-ttu-id="a312b-209">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-209">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="a312b-210">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-210">Az.Resources</span></span>
* <span data-ttu-id="a312b-211">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-211">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="a312b-212">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-212">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="a312b-213">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="a312b-213">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="a312b-214">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="a312b-214">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="a312b-215">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="a312b-215">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="a312b-216">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-216">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="a312b-217">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="a312b-217">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a312b-218">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a312b-218">Az.ServiceFabric</span></span>
* <span data-ttu-id="a312b-219">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="a312b-219">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="a312b-220">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="a312b-220">Fix some error messages.</span></span>
* <span data-ttu-id="a312b-221">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-221">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="a312b-222">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-222">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a312b-223">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a312b-223">Az.SignalR</span></span>
* <span data-ttu-id="a312b-224">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-224">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="a312b-225">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-225">Az.Sql</span></span>
* <span data-ttu-id="a312b-226">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-226">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a312b-227">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-227">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="a312b-228">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-228">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="a312b-229">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="a312b-229">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a312b-230">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a312b-230">Az.Storage</span></span>
* <span data-ttu-id="a312b-231">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-231">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a312b-232">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="a312b-232">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="a312b-233">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="a312b-233">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="a312b-234">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="a312b-234">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="a312b-235">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a312b-235">Az.TrafficManager</span></span>
* <span data-ttu-id="a312b-236">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-236">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a312b-237">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a312b-237">Az.Websites</span></span>
* <span data-ttu-id="a312b-238">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="a312b-238">Update incorrect online help URLs</span></span>
* <span data-ttu-id="a312b-239">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-239">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="a312b-240">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="a312b-240">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="a312b-241">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="a312b-241">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="a312b-242">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a312b-242">Az.Accounts</span></span>
* <span data-ttu-id="a312b-243">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="a312b-243">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-244">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-244">Az.Compute</span></span>
* <span data-ttu-id="a312b-245">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="a312b-245">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="a312b-246">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="a312b-246">Updated the description of ID in help files</span></span>
* <span data-ttu-id="a312b-247">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-247">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a312b-248">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-248">Az.DataLakeStore</span></span>
* <span data-ttu-id="a312b-249">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-249">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="a312b-250">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-250">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="a312b-251">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a312b-251">Az.EventGrid</span></span>
* <span data-ttu-id="a312b-252">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-252">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="a312b-253">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="a312b-253">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="a312b-254">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="a312b-254">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a312b-255">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="a312b-255">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a312b-256">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="a312b-256">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a312b-257">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="a312b-257">Dead letter endpoint.</span></span>
    - <span data-ttu-id="a312b-258">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="a312b-258">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="a312b-259">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="a312b-259">Event Time-To-Live,</span></span>
        - <span data-ttu-id="a312b-260">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="a312b-260">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="a312b-261">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="a312b-261">Dead letter endpoint.</span></span>
* <span data-ttu-id="a312b-262">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-262">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="a312b-263">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="a312b-263">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="a312b-264">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="a312b-264">Az.IotHub</span></span>
* <span data-ttu-id="a312b-265">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-265">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="a312b-266">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a312b-266">Az.LogicApp</span></span>
* <span data-ttu-id="a312b-267">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="a312b-267">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="a312b-268">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-268">Az.Resources</span></span>
* <span data-ttu-id="a312b-269">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-269">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="a312b-270">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="a312b-270">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="a312b-271">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-271">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a312b-272">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-272">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="a312b-273">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="a312b-273">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="a312b-274">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="a312b-274">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="a312b-275">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="a312b-275">Az.SignalR</span></span>
* <span data-ttu-id="a312b-276">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-276">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="a312b-277">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-277">Az.Sql</span></span>
* <span data-ttu-id="a312b-278">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="a312b-278">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="a312b-279">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a312b-279">Az.Storage</span></span>
* <span data-ttu-id="a312b-280">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="a312b-280">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="a312b-281">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="a312b-281">New-AzStorageContext</span></span>
* <span data-ttu-id="a312b-282">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-282">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="a312b-283">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="a312b-283">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a312b-284">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a312b-284">Az.Websites</span></span>
* <span data-ttu-id="a312b-285">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-285">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="a312b-286">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-286">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="a312b-287">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="a312b-287">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="a312b-288">全般</span><span class="sxs-lookup"><span data-stu-id="a312b-288">General</span></span>

- <span data-ttu-id="a312b-289">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="a312b-289">General Availability of Az Module</span></span>
- <span data-ttu-id="a312b-290">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="a312b-290">Online help for each module</span></span>
- <span data-ttu-id="a312b-291">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-291">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="a312b-292">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-292">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="a312b-293">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="a312b-293">Az.Accounts</span></span>
- <span data-ttu-id="a312b-294">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="a312b-294">Changed from Az.Profile</span></span>
- <span data-ttu-id="a312b-295">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-295">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a312b-296">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a312b-296">Az.ApiManagement</span></span>
- <span data-ttu-id="a312b-297">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="a312b-297">Fixes for #7002</span></span>
- <span data-ttu-id="a312b-298">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-298">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="a312b-299">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="a312b-299">Az.Batch</span></span>
- <span data-ttu-id="a312b-300">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-300">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="a312b-301">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="a312b-301">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="a312b-302">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-302">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="a312b-303">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="a312b-303">Az.Billing</span></span>
- <span data-ttu-id="a312b-304">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-304">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="a312b-305">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="a312b-305">Az.CognitivServices</span></span>
- <span data-ttu-id="a312b-306">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-306">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="a312b-307">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="a312b-307">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a312b-308">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a312b-308">Az.ContainerInstance</span></span>
- <span data-ttu-id="a312b-309">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-309">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="a312b-310">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a312b-310">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="a312b-311">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-311">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a312b-312">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-312">Az.DataLakeStore</span></span>
- <span data-ttu-id="a312b-313">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-313">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="a312b-314">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="a312b-314">Az.Monitor</span></span>
- <span data-ttu-id="a312b-315">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-315">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="a312b-316">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a312b-316">Az.KeyVault</span></span>
- <span data-ttu-id="a312b-317">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="a312b-317">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="a312b-318">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a312b-318">Az.MachineLearning</span></span>
- <span data-ttu-id="a312b-319">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="a312b-319">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="a312b-320">Az.Media</span><span class="sxs-lookup"><span data-stu-id="a312b-320">Az.Media</span></span>
- <span data-ttu-id="a312b-321">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="a312b-321">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a312b-322">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-322">Az.Network</span></span>
<span data-ttu-id="a312b-323">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-323">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="a312b-324">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="a312b-324">New cmdlets added:</span></span>
        - <span data-ttu-id="a312b-325">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a312b-325">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a312b-326">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a312b-326">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a312b-327">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a312b-327">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a312b-328">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a312b-328">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a312b-329">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="a312b-329">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="a312b-330">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="a312b-330">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="a312b-331">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="a312b-331">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="a312b-332">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="a312b-332">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="a312b-333">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="a312b-333">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="a312b-334">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a312b-334">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="a312b-335">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a312b-335">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a312b-336">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="a312b-336">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="a312b-337">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a312b-337">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="a312b-338">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="a312b-338">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="a312b-339">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-339">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="a312b-340">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="a312b-340">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="a312b-341">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a312b-341">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a312b-342">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a312b-342">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="a312b-343">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="a312b-343">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="a312b-344">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="a312b-344">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="a312b-345">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-345">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="a312b-346">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a312b-346">Az.OperationalInsights</span></span>
- <span data-ttu-id="a312b-347">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-347">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="a312b-348">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a312b-348">Az.Profile</span></span>
- <span data-ttu-id="a312b-349">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="a312b-349">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a312b-350">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a312b-350">Az.RecoveryServices</span></span>
- <span data-ttu-id="a312b-351">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-351">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="a312b-352">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-352">Az.Resources</span></span>
- <span data-ttu-id="a312b-353">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-353">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a312b-354">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a312b-354">Az.ServiceFabric</span></span>
- <span data-ttu-id="a312b-355">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="a312b-355">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="a312b-356">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-356">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="a312b-357">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="a312b-357">Az.SIgnalR</span></span>
- <span data-ttu-id="a312b-358">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="a312b-358">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="a312b-359">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-359">Az.Sql</span></span>
- <span data-ttu-id="a312b-360">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-360">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="a312b-361">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-361">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="a312b-362">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-362">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="a312b-363">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a312b-363">Az.Storage</span></span>
- <span data-ttu-id="a312b-364">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-364">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a312b-365">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a312b-365">Az.Websites</span></span>
- <span data-ttu-id="a312b-366">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="a312b-366">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="a312b-367">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="a312b-367">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="a312b-368">全般</span><span class="sxs-lookup"><span data-stu-id="a312b-368">General</span></span>

* <span data-ttu-id="a312b-369">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="a312b-369">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="a312b-370">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-370">Az.Compute</span></span>

* <span data-ttu-id="a312b-371">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-371">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="a312b-372">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-372">Az.DataLakeStore</span></span>

* <span data-ttu-id="a312b-373">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-373">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="a312b-374">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="a312b-374">Az.FrontDoor</span></span>

* <span data-ttu-id="a312b-375">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-375">Fixed some broken links</span></span>
    - <span data-ttu-id="a312b-376">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-376">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="a312b-377">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-377">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="a312b-378">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a312b-378">Az.RecoveryServices</span></span>

* <span data-ttu-id="a312b-379">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-379">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="a312b-380">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="a312b-380">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="a312b-381">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-381">Az.Resources</span></span>

* <span data-ttu-id="a312b-382">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="a312b-382">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="a312b-383">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-383">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="a312b-384">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-384">Az.Sql</span></span>

* <span data-ttu-id="a312b-385">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="a312b-385">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="a312b-386">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-386">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="a312b-387">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="a312b-387">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="a312b-388">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="a312b-388">Az.Storage</span></span>

* <span data-ttu-id="a312b-389">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-389">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="a312b-390">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-390">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="a312b-391">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a312b-391">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a312b-392">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="a312b-392">Support Static Website configuration</span></span>
    - <span data-ttu-id="a312b-393">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a312b-393">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="a312b-394">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="a312b-394">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="a312b-395">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a312b-395">Az.Websites</span></span>

* <span data-ttu-id="a312b-396">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="a312b-396">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="a312b-397">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-397">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="a312b-398">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="a312b-398">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="a312b-399">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="a312b-399">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="a312b-400">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a312b-400">Az.ApiManagement</span></span>
* <span data-ttu-id="a312b-401">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-401">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="a312b-402">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="a312b-402">Az.Automation</span></span>
* <span data-ttu-id="a312b-403">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="a312b-403">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="a312b-404">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-404">Added Update Management cmdlets</span></span>
* <span data-ttu-id="a312b-405">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-405">Added Source Control cmdlets</span></span>
* <span data-ttu-id="a312b-406">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-406">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="a312b-407">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-407">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="a312b-408">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-408">Az.Compute</span></span>
* <span data-ttu-id="a312b-409">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-409">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="a312b-410">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-410">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="a312b-411">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a312b-411">Az.ContainerInstance</span></span>
* <span data-ttu-id="a312b-412">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-412">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="a312b-413">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a312b-413">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="a312b-414">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-414">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="a312b-415">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-415">Az.Network</span></span>
* <span data-ttu-id="a312b-416">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-416">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="a312b-417">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-417">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="a312b-418">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-418">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="a312b-419">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-419">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="a312b-420">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a312b-420">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a312b-421">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-421">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="a312b-422">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="a312b-422">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="a312b-423">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a312b-423">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a312b-424">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-424">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="a312b-425">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-425">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="a312b-426">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="a312b-426">Az.Relay</span></span>
* <span data-ttu-id="a312b-427">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="a312b-427">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="a312b-428">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-428">Az.Resources</span></span>
* <span data-ttu-id="a312b-429">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-429">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="a312b-430">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-430">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="a312b-431">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="a312b-431">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="a312b-432">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a312b-432">Az.ServiceFabric</span></span>
* <span data-ttu-id="a312b-433">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-433">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="a312b-434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-434">Az.Sql</span></span>
* <span data-ttu-id="a312b-435">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-435">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="a312b-436">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a312b-436">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a312b-437">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a312b-437">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a312b-438">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a312b-438">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a312b-439">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="a312b-439">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="a312b-440">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a312b-440">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a312b-441">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a312b-441">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a312b-442">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a312b-442">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="a312b-443">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="a312b-443">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="a312b-444">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="a312b-444">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="a312b-445">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-445">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="a312b-446">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="a312b-446">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="a312b-447">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="a312b-447">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a312b-448">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="a312b-448">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="a312b-449">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="a312b-449">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="a312b-450">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="a312b-450">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="a312b-451">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-451">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="a312b-452">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="a312b-452">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a312b-453">全般</span><span class="sxs-lookup"><span data-stu-id="a312b-453">General</span></span>
* <span data-ttu-id="a312b-454">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="a312b-454">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="a312b-455">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a312b-455">Az.Profile</span></span>
* <span data-ttu-id="a312b-456">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-456">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="a312b-457">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-457">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="a312b-458">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="a312b-458">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="a312b-459">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-459">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="a312b-460">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-460">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="a312b-461">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-461">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="a312b-462">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-462">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="a312b-463">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a312b-463">Az.CognitiveServices</span></span>
* <span data-ttu-id="a312b-464">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-464">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-465">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-465">Az.Compute</span></span>
* <span data-ttu-id="a312b-466">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-466">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="a312b-467">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="a312b-467">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="a312b-468">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-468">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a312b-469">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-469">Az.DataLakeStore</span></span>
* <span data-ttu-id="a312b-470">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="a312b-470">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="a312b-471">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-471">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="a312b-472">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="a312b-472">Az.Insights</span></span>
* <span data-ttu-id="a312b-473">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-473">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="a312b-474">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="a312b-474">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="a312b-475">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-475">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="a312b-476">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="a312b-476">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a312b-477">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-477">Az.Network</span></span>
* <span data-ttu-id="a312b-478">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="a312b-478">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="a312b-479">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="a312b-479">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="a312b-480">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="a312b-480">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="a312b-481">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a312b-481">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="a312b-482">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="a312b-482">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="a312b-483">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="a312b-483">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="a312b-484">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="a312b-484">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="a312b-485">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a312b-485">Az.PolicyInsights</span></span>
* <span data-ttu-id="a312b-486">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-486">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="a312b-487">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-487">Az.Resources</span></span>
* <span data-ttu-id="a312b-488">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="a312b-488">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="a312b-489">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a312b-489">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="a312b-490">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a312b-490">Az.ServiceBus</span></span>
* <span data-ttu-id="a312b-491">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-491">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="a312b-492">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a312b-492">Az.ServiceFabric</span></span>
* <span data-ttu-id="a312b-493">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-493">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="a312b-494">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-494">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="a312b-495">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="a312b-495">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="a312b-496">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="a312b-496">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="a312b-497">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-497">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="a312b-498">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="a312b-498">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="a312b-499">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="a312b-499">Az.Profile</span></span>
* <span data-ttu-id="a312b-500">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-500">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="a312b-501">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-501">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-502">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-502">Az.Compute</span></span>
* <span data-ttu-id="a312b-503">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-503">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="a312b-504">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-504">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="a312b-505">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a312b-505">Az.DataLakeStore</span></span>
* <span data-ttu-id="a312b-506">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-506">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="a312b-507">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="a312b-507">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="a312b-508">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="a312b-508">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a312b-509">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="a312b-509">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="a312b-510">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="a312b-510">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a312b-511">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-511">Az.Network</span></span>
* <span data-ttu-id="a312b-512">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-512">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="a312b-513">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-513">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="a312b-514">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-514">Az.Resources</span></span>
* <span data-ttu-id="a312b-515">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-515">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="a312b-516">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-516">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="a312b-517">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="a312b-517">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="a312b-518">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a312b-518">Azure.Storage</span></span>
* <span data-ttu-id="a312b-519">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-519">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="a312b-520">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a312b-520">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="a312b-521">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a312b-521">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="a312b-522">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-522">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="a312b-523">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="a312b-523">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="a312b-524">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a312b-524">Az.CognitiveServices</span></span>
* <span data-ttu-id="a312b-525">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="a312b-525">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="a312b-526">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="a312b-526">Az.Compute</span></span>
* <span data-ttu-id="a312b-527">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-527">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="a312b-528">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-528">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="a312b-529">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-529">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="a312b-530">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a312b-530">Az.DataFactoryV2</span></span>
* <span data-ttu-id="a312b-531">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-531">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="a312b-532">Az.Network</span><span class="sxs-lookup"><span data-stu-id="a312b-532">Az.Network</span></span>
* <span data-ttu-id="a312b-533">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a312b-533">Added NetworkProfile functionality.</span></span> <span data-ttu-id="a312b-534">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="a312b-534">new cmdlets added</span></span>
    - <span data-ttu-id="a312b-535">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a312b-535">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="a312b-536">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a312b-536">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="a312b-537">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a312b-537">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="a312b-538">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a312b-538">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="a312b-539">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="a312b-539">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="a312b-540">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="a312b-540">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="a312b-541">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-541">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="a312b-542">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-542">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="a312b-543">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-543">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="a312b-544">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a312b-544">Az.RedisCache</span></span>
* <span data-ttu-id="a312b-545">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="a312b-545">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="a312b-546">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-546">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="a312b-547">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="a312b-547">Az.Resources</span></span>
* <span data-ttu-id="a312b-548">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="a312b-548">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="a312b-549">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-549">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="a312b-550">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="a312b-550">Az.Sql</span></span>
* <span data-ttu-id="a312b-551">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a312b-551">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="a312b-552">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="a312b-552">Az.Websites</span></span>
* <span data-ttu-id="a312b-553">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="a312b-553">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="a312b-554">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="a312b-554">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="a312b-555">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="a312b-555">0.2.0 - September 2018</span></span>
 <span data-ttu-id="a312b-556">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="a312b-556">Initial Release</span></span>