---
ms.openlocfilehash: 2db9810e20254373a487013de50d4297d4ec50d5
ms.sourcegitcommit: 8f59e11e5c991543964154d63648aa1e6ae22512
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "58475392"
---
## <a name="160---march-2019"></a><span data-ttu-id="3bdfb-101">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-101">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="3bdfb-102">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="3bdfb-102">Highlights since the last major release</span></span>
* <span data-ttu-id="3bdfb-103">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="3bdfb-103">General availability of `Az` module</span></span>
* <span data-ttu-id="3bdfb-104">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="3bdfb-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="3bdfb-105">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="3bdfb-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="3bdfb-106">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="3bdfb-107">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="3bdfb-108">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="3bdfb-109">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="3bdfb-110">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="3bdfb-110">Az.Automation</span></span>
* <span data-ttu-id="3bdfb-111">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-111">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="3bdfb-112">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="3bdfb-112">Dynamic grouping</span></span>
    * <span data-ttu-id="3bdfb-113">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="3bdfb-113">Pre-Post script</span></span>
    * <span data-ttu-id="3bdfb-114">再起動設定</span><span class="sxs-lookup"><span data-stu-id="3bdfb-114">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-115">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-115">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-116">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-116">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="3bdfb-117">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-117">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="3bdfb-118">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="3bdfb-118">Az.KeyVault</span></span>
* <span data-ttu-id="3bdfb-119">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-119">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-120">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-120">Az.Network</span></span>
* <span data-ttu-id="3bdfb-121">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-121">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="3bdfb-122">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-122">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="3bdfb-123">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-123">Az.RecoveryServices</span></span>
* <span data-ttu-id="3bdfb-124">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-124">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="3bdfb-125">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-125">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-126">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-126">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-127">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-127">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="3bdfb-128">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-128">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-129">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-129">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-130">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-130">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="3bdfb-131">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-131">Az.Storage</span></span>
* <span data-ttu-id="3bdfb-132">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="3bdfb-132">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="3bdfb-133">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="3bdfb-133">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="3bdfb-134">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="3bdfb-134">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="3bdfb-135">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="3bdfb-135">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="3bdfb-136">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="3bdfb-136">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="3bdfb-137">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="3bdfb-137">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="3bdfb-138">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="3bdfb-138">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="3bdfb-139">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-139">Az.Websites</span></span>
* <span data-ttu-id="3bdfb-140">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-140">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="3bdfb-141">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-141">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="3bdfb-142">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="3bdfb-142">Az.Accounts</span></span>
* <span data-ttu-id="3bdfb-143">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-143">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="3bdfb-144">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-144">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="3bdfb-145">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="3bdfb-145">Az.Automation</span></span>
* <span data-ttu-id="3bdfb-146">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-146">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="3bdfb-147">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-147">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="3bdfb-148">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-148">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="3bdfb-149">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="3bdfb-149">Az.Cdn</span></span>
* <span data-ttu-id="3bdfb-150">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-150">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-151">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-151">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-152">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-152">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="3bdfb-153">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="3bdfb-153">Az.DataFactory</span></span>
* <span data-ttu-id="3bdfb-154">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-154">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="3bdfb-155">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="3bdfb-155">Az.LogicApp</span></span>
* <span data-ttu-id="3bdfb-156">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-156">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-157">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-157">Az.Network</span></span>
* <span data-ttu-id="3bdfb-158">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-158">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="3bdfb-159">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-159">Az.RecoveryServices</span></span>
* <span data-ttu-id="3bdfb-160">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-160">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="3bdfb-161">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-161">SDK Update</span></span>
* <span data-ttu-id="3bdfb-162">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-162">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="3bdfb-163">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-163">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-164">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-164">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-165">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-165">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="3bdfb-166">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="3bdfb-166">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="3bdfb-167">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-167">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="3bdfb-168">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="3bdfb-168">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="3bdfb-169">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-169">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="3bdfb-170">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="3bdfb-170">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-171">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-171">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-172">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-172">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="3bdfb-173">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-173">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="3bdfb-174">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-174">Az.Storage</span></span>
* <span data-ttu-id="3bdfb-175">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-175">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="3bdfb-176">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-176">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="3bdfb-177">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-177">Az.AnalysisServices</span></span>
* <span data-ttu-id="3bdfb-178">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-178">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="3bdfb-179">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="3bdfb-179">Az.Automation</span></span>
* <span data-ttu-id="3bdfb-180">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-180">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="3bdfb-181">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-181">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="3bdfb-182">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-182">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="3bdfb-183">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-183">Az.CognitiveServices</span></span>
* <span data-ttu-id="3bdfb-184">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-184">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-185">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-185">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-186">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-186">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="3bdfb-187">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-187">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="3bdfb-188">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-188">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="3bdfb-189">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-189">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-190">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-190">Az.DataLakeStore</span></span>
* <span data-ttu-id="3bdfb-191">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-191">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="3bdfb-192">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="3bdfb-192">Az.EventHub</span></span>
* <span data-ttu-id="3bdfb-193">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-193">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="3bdfb-194">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="3bdfb-194">Az.KeyVault</span></span>
* <span data-ttu-id="3bdfb-195">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-195">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="3bdfb-196">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="3bdfb-196">Az.LogicApp</span></span>
* <span data-ttu-id="3bdfb-197">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-197">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="3bdfb-198">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-198">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="3bdfb-199">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-199">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="3bdfb-200">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="3bdfb-200">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="3bdfb-201">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="3bdfb-201">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="3bdfb-202">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="3bdfb-202">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="3bdfb-203">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="3bdfb-203">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="3bdfb-204">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-204">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="3bdfb-205">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bdfb-205">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="3bdfb-206">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bdfb-206">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="3bdfb-207">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bdfb-207">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="3bdfb-208">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bdfb-208">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="3bdfb-209">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-209">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="3bdfb-210">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="3bdfb-210">Az.Monitor</span></span>
* <span data-ttu-id="3bdfb-211">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-211">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-212">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-212">Az.Network</span></span>
* <span data-ttu-id="3bdfb-213">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-213">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="3bdfb-214">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="3bdfb-214">Az.OperationalInsights</span></span>
* <span data-ttu-id="3bdfb-215">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-215">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="3bdfb-216">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-216">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="3bdfb-217">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-217">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="3bdfb-218">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-218">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-219">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="3bdfb-219">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="3bdfb-220">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="3bdfb-220">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="3bdfb-221">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="3bdfb-221">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="3bdfb-222">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-222">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-223">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-223">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-224">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-224">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="3bdfb-225">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-225">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="3bdfb-226">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-226">Az.Websites</span></span>
* <span data-ttu-id="3bdfb-227">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-227">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="3bdfb-228">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-228">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="3bdfb-229">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="3bdfb-229">Az.Accounts</span></span>
* <span data-ttu-id="3bdfb-230">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-230">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="3bdfb-231">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-231">Az.AnalysisServices</span></span>
<span data-ttu-id="3bdfb-232">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="3bdfb-232">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-233">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-234">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-234">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="3bdfb-235">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-235">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="3bdfb-236">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-236">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="3bdfb-237">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-237">Az.RecoveryServices</span></span>
<span data-ttu-id="3bdfb-238">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="3bdfb-238">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-239">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-239">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-240">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-240">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="3bdfb-241">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="3bdfb-241">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="3bdfb-242">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-242">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="3bdfb-243">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="3bdfb-243">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-244">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-244">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-245">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-245">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="3bdfb-246">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-246">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="3bdfb-247">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-247">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="3bdfb-248">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-248">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="3bdfb-249">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="3bdfb-249">Az.Accounts</span></span>
* <span data-ttu-id="3bdfb-250">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="3bdfb-250">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="3bdfb-251">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-251">Az.AnalysisServices</span></span>
* <span data-ttu-id="3bdfb-252">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="3bdfb-252">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="3bdfb-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="3bdfb-254">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="3bdfb-254">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="3bdfb-255">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-255">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="3bdfb-256">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="3bdfb-256">Az.Accounts</span></span>
* <span data-ttu-id="3bdfb-257">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-257">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="3bdfb-258">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-258">Update incorrect online help URLs</span></span>
* <span data-ttu-id="3bdfb-259">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-259">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="3bdfb-260">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="3bdfb-260">Az.Aks</span></span>
* <span data-ttu-id="3bdfb-261">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-261">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="3bdfb-262">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="3bdfb-262">Az.Automation</span></span>
* <span data-ttu-id="3bdfb-263">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-263">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="3bdfb-264">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-264">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="3bdfb-265">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="3bdfb-265">Az.Cdn</span></span>
* <span data-ttu-id="3bdfb-266">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-266">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-267">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-267">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-268">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-268">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="3bdfb-269">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-269">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="3bdfb-270">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-270">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="3bdfb-271">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="3bdfb-271">Az.ContainerRegistry</span></span>
* <span data-ttu-id="3bdfb-272">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-272">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="3bdfb-273">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="3bdfb-273">Az.DataFactory</span></span>
* <span data-ttu-id="3bdfb-274">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-274">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-275">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-275">Az.DataLakeStore</span></span>
* <span data-ttu-id="3bdfb-276">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="3bdfb-276">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="3bdfb-277">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="3bdfb-277">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="3bdfb-278">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-278">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="3bdfb-279">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="3bdfb-279">Az.IotHub</span></span>
* <span data-ttu-id="3bdfb-280">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-280">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="3bdfb-281">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="3bdfb-281">Az.KeyVault</span></span>
* <span data-ttu-id="3bdfb-282">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-282">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-283">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-283">Az.Network</span></span>
* <span data-ttu-id="3bdfb-284">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-284">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-285">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-285">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-286">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-286">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="3bdfb-287">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-287">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="3bdfb-288">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-288">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="3bdfb-289">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="3bdfb-289">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="3bdfb-290">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="3bdfb-290">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="3bdfb-291">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-291">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="3bdfb-292">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="3bdfb-292">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="3bdfb-293">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3bdfb-293">Az.ServiceFabric</span></span>
* <span data-ttu-id="3bdfb-294">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="3bdfb-294">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="3bdfb-295">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-295">Fix some error messages.</span></span>
* <span data-ttu-id="3bdfb-296">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-296">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="3bdfb-297">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-297">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="3bdfb-298">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="3bdfb-298">Az.SignalR</span></span>
* <span data-ttu-id="3bdfb-299">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-299">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-300">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-300">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-301">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-301">Update incorrect online help URLs</span></span>
* <span data-ttu-id="3bdfb-302">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-302">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="3bdfb-303">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-303">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="3bdfb-304">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="3bdfb-304">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="3bdfb-305">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-305">Az.Storage</span></span>
* <span data-ttu-id="3bdfb-306">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="3bdfb-307">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="3bdfb-307">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="3bdfb-308">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="3bdfb-308">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="3bdfb-309">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="3bdfb-309">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="3bdfb-310">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="3bdfb-310">Az.TrafficManager</span></span>
* <span data-ttu-id="3bdfb-311">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-311">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="3bdfb-312">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-312">Az.Websites</span></span>
* <span data-ttu-id="3bdfb-313">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-313">Update incorrect online help URLs</span></span>
* <span data-ttu-id="3bdfb-314">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-314">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="3bdfb-315">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="3bdfb-315">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="3bdfb-316">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-316">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="3bdfb-317">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="3bdfb-317">Az.Accounts</span></span>
* <span data-ttu-id="3bdfb-318">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="3bdfb-318">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-319">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-319">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-320">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-320">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="3bdfb-321">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-321">Updated the description of ID in help files</span></span>
* <span data-ttu-id="3bdfb-322">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-322">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="3bdfb-324">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-324">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="3bdfb-325">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-325">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="3bdfb-326">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="3bdfb-326">Az.EventGrid</span></span>
* <span data-ttu-id="3bdfb-327">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-327">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="3bdfb-328">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="3bdfb-328">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="3bdfb-329">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="3bdfb-329">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="3bdfb-330">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="3bdfb-330">Event Time-To-Live,</span></span>
        - <span data-ttu-id="3bdfb-331">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="3bdfb-331">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="3bdfb-332">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="3bdfb-332">Dead letter endpoint.</span></span>
    - <span data-ttu-id="3bdfb-333">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="3bdfb-333">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="3bdfb-334">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="3bdfb-334">Event Time-To-Live,</span></span>
        - <span data-ttu-id="3bdfb-335">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="3bdfb-335">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="3bdfb-336">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="3bdfb-336">Dead letter endpoint.</span></span>
* <span data-ttu-id="3bdfb-337">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-337">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="3bdfb-338">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-338">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="3bdfb-339">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="3bdfb-339">Az.IotHub</span></span>
* <span data-ttu-id="3bdfb-340">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-340">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="3bdfb-341">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="3bdfb-341">Az.LogicApp</span></span>
* <span data-ttu-id="3bdfb-342">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="3bdfb-342">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-343">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-343">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-344">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-344">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="3bdfb-345">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="3bdfb-345">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="3bdfb-346">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-346">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="3bdfb-347">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-347">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="3bdfb-348">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-348">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="3bdfb-349">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="3bdfb-349">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="3bdfb-350">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="3bdfb-350">Az.SignalR</span></span>
* <span data-ttu-id="3bdfb-351">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-351">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-352">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-352">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-353">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-353">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="3bdfb-354">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-354">Az.Storage</span></span>
* <span data-ttu-id="3bdfb-355">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="3bdfb-355">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="3bdfb-356">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="3bdfb-356">New-AzStorageContext</span></span>
* <span data-ttu-id="3bdfb-357">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-357">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="3bdfb-358">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="3bdfb-358">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="3bdfb-359">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-359">Az.Websites</span></span>
* <span data-ttu-id="3bdfb-360">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-360">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="3bdfb-361">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-361">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="3bdfb-362">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-362">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="3bdfb-363">全般</span><span class="sxs-lookup"><span data-stu-id="3bdfb-363">General</span></span>

- <span data-ttu-id="3bdfb-364">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="3bdfb-364">General Availability of Az Module</span></span>
- <span data-ttu-id="3bdfb-365">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="3bdfb-365">Online help for each module</span></span>
- <span data-ttu-id="3bdfb-366">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-366">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="3bdfb-367">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-367">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="3bdfb-368">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="3bdfb-368">Az.Accounts</span></span>
- <span data-ttu-id="3bdfb-369">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-369">Changed from Az.Profile</span></span>
- <span data-ttu-id="3bdfb-370">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-370">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="3bdfb-371">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="3bdfb-371">Az.ApiManagement</span></span>
- <span data-ttu-id="3bdfb-372">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="3bdfb-372">Fixes for #7002</span></span>
- <span data-ttu-id="3bdfb-373">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-373">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="3bdfb-374">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="3bdfb-374">Az.Batch</span></span>
- <span data-ttu-id="3bdfb-375">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-375">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="3bdfb-376">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-376">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="3bdfb-377">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-377">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="3bdfb-378">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="3bdfb-378">Az.Billing</span></span>
- <span data-ttu-id="3bdfb-379">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-379">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="3bdfb-380">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-380">Az.CognitivServices</span></span>
- <span data-ttu-id="3bdfb-381">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-381">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="3bdfb-382">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-382">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="3bdfb-383">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="3bdfb-383">Az.ContainerInstance</span></span>
- <span data-ttu-id="3bdfb-384">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-384">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="3bdfb-385">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="3bdfb-385">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="3bdfb-386">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-386">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-387">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-387">Az.DataLakeStore</span></span>
- <span data-ttu-id="3bdfb-388">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-388">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="3bdfb-389">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="3bdfb-389">Az.Monitor</span></span>
- <span data-ttu-id="3bdfb-390">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-390">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="3bdfb-391">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="3bdfb-391">Az.KeyVault</span></span>
- <span data-ttu-id="3bdfb-392">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-392">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="3bdfb-393">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="3bdfb-393">Az.MachineLearning</span></span>
- <span data-ttu-id="3bdfb-394">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-394">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="3bdfb-395">Az.Media</span><span class="sxs-lookup"><span data-stu-id="3bdfb-395">Az.Media</span></span>
- <span data-ttu-id="3bdfb-396">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-396">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="3bdfb-397">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-397">Az.Network</span></span>
<span data-ttu-id="3bdfb-398">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-398">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="3bdfb-399">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="3bdfb-399">New cmdlets added:</span></span>
        - <span data-ttu-id="3bdfb-400">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="3bdfb-400">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="3bdfb-401">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="3bdfb-401">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="3bdfb-402">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="3bdfb-402">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="3bdfb-403">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="3bdfb-403">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="3bdfb-404">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="3bdfb-404">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="3bdfb-405">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="3bdfb-405">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="3bdfb-406">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="3bdfb-406">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="3bdfb-407">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="3bdfb-407">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="3bdfb-408">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-408">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="3bdfb-409">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="3bdfb-409">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="3bdfb-410">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="3bdfb-410">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="3bdfb-411">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="3bdfb-411">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="3bdfb-412">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="3bdfb-412">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="3bdfb-413">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="3bdfb-413">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="3bdfb-414">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-414">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="3bdfb-415">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-415">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="3bdfb-416">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="3bdfb-416">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="3bdfb-417">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="3bdfb-417">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="3bdfb-418">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="3bdfb-418">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="3bdfb-419">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-419">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="3bdfb-420">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-420">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="3bdfb-421">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="3bdfb-421">Az.OperationalInsights</span></span>
- <span data-ttu-id="3bdfb-422">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-422">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="3bdfb-423">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-423">Az.Profile</span></span>
- <span data-ttu-id="3bdfb-424">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-424">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="3bdfb-425">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-425">Az.RecoveryServices</span></span>
- <span data-ttu-id="3bdfb-426">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-426">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="3bdfb-427">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-427">Az.Resources</span></span>
- <span data-ttu-id="3bdfb-428">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-428">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="3bdfb-429">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3bdfb-429">Az.ServiceFabric</span></span>
- <span data-ttu-id="3bdfb-430">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="3bdfb-430">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="3bdfb-431">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-431">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="3bdfb-432">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="3bdfb-432">Az.SIgnalR</span></span>
- <span data-ttu-id="3bdfb-433">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="3bdfb-433">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="3bdfb-434">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-434">Az.Sql</span></span>
- <span data-ttu-id="3bdfb-435">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-435">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="3bdfb-436">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-436">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="3bdfb-437">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-437">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="3bdfb-438">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-438">Az.Storage</span></span>
- <span data-ttu-id="3bdfb-439">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-439">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="3bdfb-440">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-440">Az.Websites</span></span>
- <span data-ttu-id="3bdfb-441">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="3bdfb-441">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="3bdfb-442">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-442">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="3bdfb-443">全般</span><span class="sxs-lookup"><span data-stu-id="3bdfb-443">General</span></span>

* <span data-ttu-id="3bdfb-444">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="3bdfb-444">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="3bdfb-445">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-445">Az.Compute</span></span>

* <span data-ttu-id="3bdfb-446">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-446">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-447">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-447">Az.DataLakeStore</span></span>

* <span data-ttu-id="3bdfb-448">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-448">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="3bdfb-449">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="3bdfb-449">Az.FrontDoor</span></span>

* <span data-ttu-id="3bdfb-450">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-450">Fixed some broken links</span></span>
    - <span data-ttu-id="3bdfb-451">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-451">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="3bdfb-452">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-452">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="3bdfb-453">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-453">Az.RecoveryServices</span></span>

* <span data-ttu-id="3bdfb-454">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-454">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="3bdfb-455">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-455">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="3bdfb-456">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-456">Az.Resources</span></span>

* <span data-ttu-id="3bdfb-457">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="3bdfb-457">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="3bdfb-458">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-458">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="3bdfb-459">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-459">Az.Sql</span></span>

* <span data-ttu-id="3bdfb-460">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="3bdfb-460">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="3bdfb-461">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-461">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="3bdfb-462">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-462">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="3bdfb-463">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-463">Az.Storage</span></span>

* <span data-ttu-id="3bdfb-464">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-464">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="3bdfb-465">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-465">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="3bdfb-466">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="3bdfb-466">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="3bdfb-467">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="3bdfb-467">Support Static Website configuration</span></span>
    - <span data-ttu-id="3bdfb-468">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="3bdfb-468">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="3bdfb-469">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="3bdfb-469">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="3bdfb-470">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-470">Az.Websites</span></span>

* <span data-ttu-id="3bdfb-471">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="3bdfb-471">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="3bdfb-472">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-472">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="3bdfb-473">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="3bdfb-473">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="3bdfb-474">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-474">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="3bdfb-475">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="3bdfb-475">Az.ApiManagement</span></span>
* <span data-ttu-id="3bdfb-476">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-476">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="3bdfb-477">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="3bdfb-477">Az.Automation</span></span>
* <span data-ttu-id="3bdfb-478">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="3bdfb-478">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="3bdfb-479">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-479">Added Update Management cmdlets</span></span>
* <span data-ttu-id="3bdfb-480">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-480">Added Source Control cmdlets</span></span>
* <span data-ttu-id="3bdfb-481">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-481">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="3bdfb-482">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-482">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="3bdfb-483">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-483">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-484">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-484">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="3bdfb-485">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-485">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="3bdfb-486">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="3bdfb-486">Az.ContainerInstance</span></span>
* <span data-ttu-id="3bdfb-487">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-487">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="3bdfb-488">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="3bdfb-488">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="3bdfb-489">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-489">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="3bdfb-490">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-490">Az.Network</span></span>
* <span data-ttu-id="3bdfb-491">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-491">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="3bdfb-492">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-492">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="3bdfb-493">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-493">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="3bdfb-494">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-494">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="3bdfb-495">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="3bdfb-495">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="3bdfb-496">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-496">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="3bdfb-497">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-497">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="3bdfb-498">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="3bdfb-498">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="3bdfb-499">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-499">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="3bdfb-500">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-500">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="3bdfb-501">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="3bdfb-501">Az.Relay</span></span>
* <span data-ttu-id="3bdfb-502">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="3bdfb-502">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="3bdfb-503">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-503">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-504">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-504">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="3bdfb-505">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-505">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="3bdfb-506">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="3bdfb-506">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="3bdfb-507">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3bdfb-507">Az.ServiceFabric</span></span>
* <span data-ttu-id="3bdfb-508">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-508">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="3bdfb-509">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-509">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-510">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-510">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="3bdfb-511">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="3bdfb-511">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="3bdfb-512">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="3bdfb-512">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="3bdfb-513">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="3bdfb-513">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="3bdfb-514">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="3bdfb-514">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="3bdfb-515">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="3bdfb-515">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="3bdfb-516">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="3bdfb-516">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="3bdfb-517">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="3bdfb-517">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="3bdfb-518">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="3bdfb-518">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="3bdfb-519">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-519">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="3bdfb-520">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-520">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="3bdfb-521">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-521">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="3bdfb-522">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="3bdfb-522">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="3bdfb-523">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="3bdfb-523">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="3bdfb-524">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="3bdfb-524">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="3bdfb-525">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="3bdfb-525">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="3bdfb-526">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-526">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="3bdfb-527">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-527">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="3bdfb-528">全般</span><span class="sxs-lookup"><span data-stu-id="3bdfb-528">General</span></span>
* <span data-ttu-id="3bdfb-529">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="3bdfb-529">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="3bdfb-530">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-530">Az.Profile</span></span>
* <span data-ttu-id="3bdfb-531">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-531">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="3bdfb-532">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-532">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="3bdfb-533">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-533">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="3bdfb-534">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-534">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="3bdfb-535">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-535">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="3bdfb-536">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-536">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="3bdfb-537">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-537">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="3bdfb-538">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-538">Az.CognitiveServices</span></span>
* <span data-ttu-id="3bdfb-539">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-539">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-540">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-540">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-541">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-541">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="3bdfb-542">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="3bdfb-542">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="3bdfb-543">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-543">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-544">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-544">Az.DataLakeStore</span></span>
* <span data-ttu-id="3bdfb-545">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-545">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="3bdfb-546">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-546">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="3bdfb-547">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="3bdfb-547">Az.Insights</span></span>
* <span data-ttu-id="3bdfb-548">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-548">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="3bdfb-549">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-549">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="3bdfb-550">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-550">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="3bdfb-551">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="3bdfb-551">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-552">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-552">Az.Network</span></span>
* <span data-ttu-id="3bdfb-553">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="3bdfb-553">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="3bdfb-554">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="3bdfb-554">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="3bdfb-555">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="3bdfb-555">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="3bdfb-556">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="3bdfb-556">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="3bdfb-557">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="3bdfb-557">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="3bdfb-558">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="3bdfb-558">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="3bdfb-559">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="3bdfb-559">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="3bdfb-560">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="3bdfb-560">Az.PolicyInsights</span></span>
* <span data-ttu-id="3bdfb-561">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-561">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-562">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-562">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-563">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="3bdfb-563">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="3bdfb-564">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-564">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="3bdfb-565">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="3bdfb-565">Az.ServiceBus</span></span>
* <span data-ttu-id="3bdfb-566">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-566">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="3bdfb-567">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="3bdfb-567">Az.ServiceFabric</span></span>
* <span data-ttu-id="3bdfb-568">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-568">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="3bdfb-569">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-569">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="3bdfb-570">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-570">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="3bdfb-571">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-571">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="3bdfb-572">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-572">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="3bdfb-573">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-573">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="3bdfb-574">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-574">Az.Profile</span></span>
* <span data-ttu-id="3bdfb-575">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-575">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="3bdfb-576">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-576">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-577">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-577">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-578">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-578">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="3bdfb-579">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-579">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="3bdfb-580">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="3bdfb-580">Az.DataLakeStore</span></span>
* <span data-ttu-id="3bdfb-581">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-581">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="3bdfb-582">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-582">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="3bdfb-583">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-583">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="3bdfb-584">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-584">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="3bdfb-585">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-585">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-586">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-586">Az.Network</span></span>
* <span data-ttu-id="3bdfb-587">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-587">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="3bdfb-588">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-588">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-589">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-589">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-590">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-590">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="3bdfb-591">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-591">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="3bdfb-592">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-592">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="3bdfb-593">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-593">Azure.Storage</span></span>
* <span data-ttu-id="3bdfb-594">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-594">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="3bdfb-595">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="3bdfb-595">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="3bdfb-596">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="3bdfb-596">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="3bdfb-597">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-597">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="3bdfb-598">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="3bdfb-598">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="3bdfb-599">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="3bdfb-599">Az.CognitiveServices</span></span>
* <span data-ttu-id="3bdfb-600">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-600">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="3bdfb-601">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="3bdfb-601">Az.Compute</span></span>
* <span data-ttu-id="3bdfb-602">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-602">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="3bdfb-603">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-603">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="3bdfb-604">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-604">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="3bdfb-605">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="3bdfb-605">Az.DataFactoryV2</span></span>
* <span data-ttu-id="3bdfb-606">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-606">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="3bdfb-607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="3bdfb-607">Az.Network</span></span>
* <span data-ttu-id="3bdfb-608">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-608">Added NetworkProfile functionality.</span></span> <span data-ttu-id="3bdfb-609">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="3bdfb-609">new cmdlets added</span></span>
    - <span data-ttu-id="3bdfb-610">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-610">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="3bdfb-611">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-611">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="3bdfb-612">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-612">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="3bdfb-613">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="3bdfb-613">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="3bdfb-614">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="3bdfb-614">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="3bdfb-615">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="3bdfb-615">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="3bdfb-616">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-616">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="3bdfb-617">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-617">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="3bdfb-618">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-618">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="3bdfb-619">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="3bdfb-619">Az.RedisCache</span></span>
* <span data-ttu-id="3bdfb-620">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="3bdfb-620">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="3bdfb-621">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-621">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="3bdfb-622">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="3bdfb-622">Az.Resources</span></span>
* <span data-ttu-id="3bdfb-623">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-623">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="3bdfb-624">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-624">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="3bdfb-625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="3bdfb-625">Az.Sql</span></span>
* <span data-ttu-id="3bdfb-626">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="3bdfb-626">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="3bdfb-627">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="3bdfb-627">Az.Websites</span></span>
* <span data-ttu-id="3bdfb-628">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="3bdfb-628">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="3bdfb-629">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="3bdfb-629">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="3bdfb-630">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="3bdfb-630">0.2.0 - September 2018</span></span>
 <span data-ttu-id="3bdfb-631">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="3bdfb-631">Initial Release</span></span>