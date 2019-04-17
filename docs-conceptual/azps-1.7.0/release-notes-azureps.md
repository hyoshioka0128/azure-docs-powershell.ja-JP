---
ms.openlocfilehash: 54d7a9da878e085e90479fb229876c9be6dafd74
ms.sourcegitcommit: 89066b7c4b527357bb2024e1ad708df84c131804
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2019
ms.locfileid: "59364136"
---
## <a name="170---april-2019"></a><span data-ttu-id="328ec-101">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="328ec-101">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="328ec-102">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="328ec-102">Highlights since the last major release</span></span>
* <span data-ttu-id="328ec-103">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="328ec-103">General availability of `Az` module</span></span>
* <span data-ttu-id="328ec-104">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="328ec-104">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="328ec-105">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="328ec-105">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="328ec-106">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-106">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="328ec-107">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="328ec-107">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="328ec-108">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-108">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="328ec-109">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-109">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="328ec-110">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-110">Az.Accounts</span></span>
* <span data-ttu-id="328ec-111">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-111">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="328ec-112">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="328ec-112">Az.AnalysisServices</span></span>
* <span data-ttu-id="328ec-113">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="328ec-113">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="328ec-114">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="328ec-114">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="328ec-115">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="328ec-115">Az.Automation</span></span>
* <span data-ttu-id="328ec-116">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-116">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="328ec-117">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="328ec-117">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="328ec-118">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-118">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-119">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-119">Az.Compute</span></span>
* <span data-ttu-id="328ec-120">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-120">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="328ec-121">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="328ec-121">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="328ec-122">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-122">Az.ContainerInstance</span></span>
* <span data-ttu-id="328ec-123">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-123">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="328ec-124">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="328ec-124">Az.DataFactory</span></span>
* <span data-ttu-id="328ec-125">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-125">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="328ec-126">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-126">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-127">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-127">Az.Resources</span></span>
* <span data-ttu-id="328ec-128">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="328ec-128">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="328ec-129">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="328ec-129">Improve error handling for for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="328ec-130">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="328ec-130">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="328ec-131">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="328ec-131">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="328ec-132">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-132">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="328ec-133">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="328ec-133">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-134">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-134">Az.Sql</span></span>
* <span data-ttu-id="328ec-135">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="328ec-135">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="328ec-136">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-136">Az.Storage</span></span>
* <span data-ttu-id="328ec-137">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="328ec-137">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="328ec-138">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="328ec-138">New-AzStorageContext</span></span>
* <span data-ttu-id="328ec-139">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="328ec-139">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="328ec-140">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="328ec-140">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="328ec-141">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="328ec-141">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="328ec-142">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="328ec-142">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="328ec-143">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="328ec-143">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="328ec-144">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="328ec-144">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="328ec-145">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="328ec-145">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="328ec-146">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="328ec-146">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="328ec-147">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="328ec-147">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="328ec-148">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="328ec-148">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="328ec-149">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="328ec-149">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="328ec-150">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="328ec-150">Highlights since the last major release</span></span>
* <span data-ttu-id="328ec-151">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="328ec-151">General availability of `Az` module</span></span>
* <span data-ttu-id="328ec-152">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="328ec-152">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="328ec-153">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="328ec-153">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/en-us/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="328ec-154">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-154">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="328ec-155">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="328ec-155">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="328ec-156">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-156">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="328ec-157">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-157">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="328ec-158">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="328ec-158">Az.Automation</span></span>
* <span data-ttu-id="328ec-159">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="328ec-159">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="328ec-160">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="328ec-160">Dynamic grouping</span></span>
    * <span data-ttu-id="328ec-161">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="328ec-161">Pre-Post script</span></span>
    * <span data-ttu-id="328ec-162">再起動設定</span><span class="sxs-lookup"><span data-stu-id="328ec-162">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-163">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-163">Az.Compute</span></span>
* <span data-ttu-id="328ec-164">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-164">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="328ec-165">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-165">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="328ec-166">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="328ec-166">Az.KeyVault</span></span>
* <span data-ttu-id="328ec-167">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-167">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-168">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-168">Az.Network</span></span>
* <span data-ttu-id="328ec-169">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-169">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="328ec-170">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-170">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="328ec-171">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="328ec-171">Az.RecoveryServices</span></span>
* <span data-ttu-id="328ec-172">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-172">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="328ec-173">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-173">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-174">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-174">Az.Resources</span></span>
* <span data-ttu-id="328ec-175">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="328ec-175">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="328ec-176">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-176">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-177">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-177">Az.Sql</span></span>
* <span data-ttu-id="328ec-178">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-178">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="328ec-179">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-179">Az.Storage</span></span>
* <span data-ttu-id="328ec-180">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="328ec-180">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="328ec-181">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="328ec-181">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="328ec-182">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="328ec-182">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="328ec-183">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="328ec-183">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="328ec-184">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="328ec-184">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="328ec-185">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="328ec-185">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="328ec-186">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="328ec-186">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="328ec-187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-187">Az.Websites</span></span>
* <span data-ttu-id="328ec-188">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="328ec-188">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="328ec-189">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="328ec-189">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="328ec-190">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-190">Az.Accounts</span></span>
* <span data-ttu-id="328ec-191">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-191">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="328ec-192">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-192">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="328ec-193">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="328ec-193">Az.Automation</span></span>
* <span data-ttu-id="328ec-194">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-194">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="328ec-195">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-195">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="328ec-196">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="328ec-196">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="328ec-197">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="328ec-197">Az.Cdn</span></span>
* <span data-ttu-id="328ec-198">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="328ec-198">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-199">Az.Compute</span></span>
* <span data-ttu-id="328ec-200">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-200">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="328ec-201">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="328ec-201">Az.DataFactory</span></span>
* <span data-ttu-id="328ec-202">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-202">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="328ec-203">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="328ec-203">Az.LogicApp</span></span>
* <span data-ttu-id="328ec-204">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-204">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-205">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-205">Az.Network</span></span>
* <span data-ttu-id="328ec-206">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-206">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="328ec-207">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="328ec-207">Az.RecoveryServices</span></span>
* <span data-ttu-id="328ec-208">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-208">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="328ec-209">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="328ec-209">SDK Update</span></span>
* <span data-ttu-id="328ec-210">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="328ec-210">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="328ec-211">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-211">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-212">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-212">Az.Resources</span></span>
* <span data-ttu-id="328ec-213">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-213">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="328ec-214">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="328ec-214">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="328ec-215">`Get-AzResource` の結果をパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-215">Fix issue when piping the result of `Get-AzResource` to</span></span> `Set-AzResource`
    - <span data-ttu-id="328ec-216">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="328ec-216">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="328ec-217">実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-217">Fix issue with JSON data type change when running</span></span> `Set-AzResource`
    - <span data-ttu-id="328ec-218">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="328ec-218">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-219">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-219">Az.Sql</span></span>
* <span data-ttu-id="328ec-220">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-220">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="328ec-221">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-221">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="328ec-222">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-222">Az.Storage</span></span>
* <span data-ttu-id="328ec-223">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="328ec-223">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="328ec-224">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="328ec-224">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="328ec-225">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="328ec-225">Az.AnalysisServices</span></span>
* <span data-ttu-id="328ec-226">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="328ec-226">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="328ec-227">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="328ec-227">Az.Automation</span></span>
* <span data-ttu-id="328ec-228">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-228">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="328ec-229">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-229">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="328ec-230">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="328ec-230">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="328ec-231">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="328ec-231">Az.CognitiveServices</span></span>
* <span data-ttu-id="328ec-232">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="328ec-232">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-233">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-233">Az.Compute</span></span>
* <span data-ttu-id="328ec-234">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-234">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="328ec-235">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-235">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="328ec-236">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-236">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="328ec-237">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="328ec-237">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="328ec-238">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-238">Az.DataLakeStore</span></span>
* <span data-ttu-id="328ec-239">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-239">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="328ec-240">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="328ec-240">Az.EventHub</span></span>
* <span data-ttu-id="328ec-241">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-241">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="328ec-242">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="328ec-242">Az.KeyVault</span></span>
* <span data-ttu-id="328ec-243">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-243">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="328ec-244">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="328ec-244">Az.LogicApp</span></span>
* <span data-ttu-id="328ec-245">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-245">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="328ec-246">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-246">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="328ec-247">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-247">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="328ec-248">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="328ec-248">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="328ec-249">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="328ec-249">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="328ec-250">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="328ec-250">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="328ec-251">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="328ec-251">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="328ec-252">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-252">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="328ec-253">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="328ec-253">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="328ec-254">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="328ec-254">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="328ec-255">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="328ec-255">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="328ec-256">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="328ec-256">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="328ec-257">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-257">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="328ec-258">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="328ec-258">Az.Monitor</span></span>
* <span data-ttu-id="328ec-259">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-259">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-260">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-260">Az.Network</span></span>
* <span data-ttu-id="328ec-261">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-261">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="328ec-262">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="328ec-262">Az.OperationalInsights</span></span>
* <span data-ttu-id="328ec-263">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-263">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="328ec-264">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-264">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="328ec-265">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-265">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="328ec-266">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-266">Az.Resources</span></span>
* <span data-ttu-id="328ec-267">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="328ec-267">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="328ec-268">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="328ec-268">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="328ec-269">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="328ec-269">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="328ec-270">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-270">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-271">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-271">Az.Sql</span></span>
* <span data-ttu-id="328ec-272">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-272">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="328ec-273">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-273">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="328ec-274">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-274">Az.Websites</span></span>
* <span data-ttu-id="328ec-275">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-275">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="328ec-276">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="328ec-276">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="328ec-277">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-277">Az.Accounts</span></span>
* <span data-ttu-id="328ec-278">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="328ec-278">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="328ec-279">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="328ec-279">Az.AnalysisServices</span></span>
<span data-ttu-id="328ec-280">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="328ec-280">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-281">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-281">Az.Compute</span></span>
* <span data-ttu-id="328ec-282">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-282">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="328ec-283">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-283">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="328ec-284">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-284">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="328ec-285">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="328ec-285">Az.RecoveryServices</span></span>
<span data-ttu-id="328ec-286">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="328ec-286">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-287">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-287">Az.Resources</span></span>
* <span data-ttu-id="328ec-288">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="328ec-288">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="328ec-289">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="328ec-289">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="328ec-290">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-290">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="328ec-291">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="328ec-291">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-292">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-292">Az.Sql</span></span>
* <span data-ttu-id="328ec-293">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="328ec-293">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="328ec-294">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-294">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="328ec-295">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-295">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="328ec-296">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="328ec-296">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="328ec-297">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-297">Az.Accounts</span></span>
* <span data-ttu-id="328ec-298">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="328ec-298">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="328ec-299">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="328ec-299">Az.AnalysisServices</span></span>
* <span data-ttu-id="328ec-300">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="328ec-300">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="328ec-301">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="328ec-301">Az.RecoveryServices</span></span>
* <span data-ttu-id="328ec-302">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="328ec-302">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="328ec-303">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="328ec-303">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="328ec-304">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-304">Az.Accounts</span></span>
* <span data-ttu-id="328ec-305">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="328ec-305">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="328ec-306">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-306">Update incorrect online help URLs</span></span>
* <span data-ttu-id="328ec-307">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-307">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="328ec-308">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="328ec-308">Az.Aks</span></span>
* <span data-ttu-id="328ec-309">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-309">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="328ec-310">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="328ec-310">Az.Automation</span></span>
* <span data-ttu-id="328ec-311">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-311">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="328ec-312">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-312">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="328ec-313">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="328ec-313">Az.Cdn</span></span>
* <span data-ttu-id="328ec-314">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-314">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-315">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-315">Az.Compute</span></span>
* <span data-ttu-id="328ec-316">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="328ec-316">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="328ec-317">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="328ec-317">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="328ec-318">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="328ec-318">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="328ec-319">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="328ec-319">Az.ContainerRegistry</span></span>
* <span data-ttu-id="328ec-320">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-320">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="328ec-321">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="328ec-321">Az.DataFactory</span></span>
* <span data-ttu-id="328ec-322">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="328ec-322">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="328ec-323">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-323">Az.DataLakeStore</span></span>
* <span data-ttu-id="328ec-324">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="328ec-324">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="328ec-325">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="328ec-325">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="328ec-326">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-326">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="328ec-327">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="328ec-327">Az.IotHub</span></span>
* <span data-ttu-id="328ec-328">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="328ec-328">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="328ec-329">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="328ec-329">Az.KeyVault</span></span>
* <span data-ttu-id="328ec-330">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-330">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-331">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-331">Az.Network</span></span>
* <span data-ttu-id="328ec-332">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-332">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-333">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-333">Az.Resources</span></span>
* <span data-ttu-id="328ec-334">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-334">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="328ec-335">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-335">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="328ec-336">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="328ec-336">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="328ec-337">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="328ec-337">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="328ec-338">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="328ec-338">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="328ec-339">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-339">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="328ec-340">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="328ec-340">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="328ec-341">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="328ec-341">Az.ServiceFabric</span></span>
* <span data-ttu-id="328ec-342">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="328ec-342">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="328ec-343">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="328ec-343">Fix some error messages.</span></span>
* <span data-ttu-id="328ec-344">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-344">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="328ec-345">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-345">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="328ec-346">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="328ec-346">Az.SignalR</span></span>
* <span data-ttu-id="328ec-347">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-347">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-348">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-348">Az.Sql</span></span>
* <span data-ttu-id="328ec-349">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-349">Update incorrect online help URLs</span></span>
* <span data-ttu-id="328ec-350">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-350">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="328ec-351">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-351">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="328ec-352">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="328ec-352">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="328ec-353">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-353">Az.Storage</span></span>
* <span data-ttu-id="328ec-354">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-354">Update incorrect online help URLs</span></span>
* <span data-ttu-id="328ec-355">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="328ec-355">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="328ec-356">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="328ec-356">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="328ec-357">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="328ec-357">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="328ec-358">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="328ec-358">Az.TrafficManager</span></span>
* <span data-ttu-id="328ec-359">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-359">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="328ec-360">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-360">Az.Websites</span></span>
* <span data-ttu-id="328ec-361">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="328ec-361">Update incorrect online help URLs</span></span>
* <span data-ttu-id="328ec-362">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-362">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="328ec-363">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="328ec-363">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="328ec-364">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="328ec-364">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="328ec-365">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-365">Az.Accounts</span></span>
* <span data-ttu-id="328ec-366">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="328ec-366">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-367">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-367">Az.Compute</span></span>
* <span data-ttu-id="328ec-368">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="328ec-368">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="328ec-369">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="328ec-369">Updated the description of ID in help files</span></span>
* <span data-ttu-id="328ec-370">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-370">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="328ec-371">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-371">Az.DataLakeStore</span></span>
* <span data-ttu-id="328ec-372">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-372">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="328ec-373">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-373">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="328ec-374">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="328ec-374">Az.EventGrid</span></span>
* <span data-ttu-id="328ec-375">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-375">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="328ec-376">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="328ec-376">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="328ec-377">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="328ec-377">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="328ec-378">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="328ec-378">Event Time-To-Live,</span></span>
        - <span data-ttu-id="328ec-379">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="328ec-379">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="328ec-380">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="328ec-380">Dead letter endpoint.</span></span>
    - <span data-ttu-id="328ec-381">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="328ec-381">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="328ec-382">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="328ec-382">Event Time-To-Live,</span></span>
        - <span data-ttu-id="328ec-383">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="328ec-383">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="328ec-384">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="328ec-384">Dead letter endpoint.</span></span>
* <span data-ttu-id="328ec-385">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-385">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="328ec-386">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="328ec-386">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="328ec-387">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="328ec-387">Az.IotHub</span></span>
* <span data-ttu-id="328ec-388">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-388">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="328ec-389">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="328ec-389">Az.LogicApp</span></span>
* <span data-ttu-id="328ec-390">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="328ec-390">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-391">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-391">Az.Resources</span></span>
* <span data-ttu-id="328ec-392">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-392">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="328ec-393">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="328ec-393">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="328ec-394">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-394">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="328ec-395">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-395">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="328ec-396">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="328ec-396">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="328ec-397">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="328ec-397">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="328ec-398">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="328ec-398">Az.SignalR</span></span>
* <span data-ttu-id="328ec-399">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-399">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-400">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-400">Az.Sql</span></span>
* <span data-ttu-id="328ec-401">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="328ec-401">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="328ec-402">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-402">Az.Storage</span></span>
* <span data-ttu-id="328ec-403">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="328ec-403">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="328ec-404">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="328ec-404">New-AzStorageContext</span></span>
* <span data-ttu-id="328ec-405">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-405">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="328ec-406">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="328ec-406">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="328ec-407">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-407">Az.Websites</span></span>
* <span data-ttu-id="328ec-408">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-408">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="328ec-409">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-409">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="328ec-410">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="328ec-410">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="328ec-411">全般</span><span class="sxs-lookup"><span data-stu-id="328ec-411">General</span></span>

- <span data-ttu-id="328ec-412">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="328ec-412">General Availability of Az Module</span></span>
- <span data-ttu-id="328ec-413">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="328ec-413">Online help for each module</span></span>
- <span data-ttu-id="328ec-414">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-414">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="328ec-415">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-415">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="328ec-416">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="328ec-416">Az.Accounts</span></span>
- <span data-ttu-id="328ec-417">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="328ec-417">Changed from Az.Profile</span></span>
- <span data-ttu-id="328ec-418">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-418">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="328ec-419">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="328ec-419">Az.ApiManagement</span></span>
- <span data-ttu-id="328ec-420">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="328ec-420">Fixes for #7002</span></span>
- <span data-ttu-id="328ec-421">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-421">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="328ec-422">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="328ec-422">Az.Batch</span></span>
- <span data-ttu-id="328ec-423">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-423">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="328ec-424">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="328ec-424">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="328ec-425">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-425">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="328ec-426">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="328ec-426">Az.Billing</span></span>
- <span data-ttu-id="328ec-427">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-427">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="328ec-428">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="328ec-428">Az.CognitivServices</span></span>
- <span data-ttu-id="328ec-429">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-429">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="328ec-430">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="328ec-430">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="328ec-431">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-431">Az.ContainerInstance</span></span>
- <span data-ttu-id="328ec-432">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-432">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="328ec-433">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="328ec-433">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="328ec-434">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-434">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="328ec-435">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-435">Az.DataLakeStore</span></span>
- <span data-ttu-id="328ec-436">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-436">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="328ec-437">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="328ec-437">Az.Monitor</span></span>
- <span data-ttu-id="328ec-438">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-438">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="328ec-439">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="328ec-439">Az.KeyVault</span></span>
- <span data-ttu-id="328ec-440">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="328ec-440">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="328ec-441">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="328ec-441">Az.MachineLearning</span></span>
- <span data-ttu-id="328ec-442">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="328ec-442">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="328ec-443">Az.Media</span><span class="sxs-lookup"><span data-stu-id="328ec-443">Az.Media</span></span>
- <span data-ttu-id="328ec-444">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="328ec-444">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="328ec-445">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-445">Az.Network</span></span>
<span data-ttu-id="328ec-446">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-446">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="328ec-447">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="328ec-447">New cmdlets added:</span></span>
        - <span data-ttu-id="328ec-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="328ec-448">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="328ec-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="328ec-449">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="328ec-450">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="328ec-450">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="328ec-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="328ec-451">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="328ec-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="328ec-452">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="328ec-453">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="328ec-453">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="328ec-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="328ec-454">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="328ec-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="328ec-455">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="328ec-456">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-456">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="328ec-457">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="328ec-457">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="328ec-458">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="328ec-458">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="328ec-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="328ec-459">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="328ec-460">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="328ec-460">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="328ec-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="328ec-461">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="328ec-462">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-462">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="328ec-463">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-463">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="328ec-464">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="328ec-464">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="328ec-465">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="328ec-465">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="328ec-466">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="328ec-466">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="328ec-467">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-467">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="328ec-468">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-468">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="328ec-469">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="328ec-469">Az.OperationalInsights</span></span>
- <span data-ttu-id="328ec-470">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-470">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="328ec-471">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="328ec-471">Az.Profile</span></span>
- <span data-ttu-id="328ec-472">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="328ec-472">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="328ec-473">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="328ec-473">Az.RecoveryServices</span></span>
- <span data-ttu-id="328ec-474">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-474">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="328ec-475">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-475">Az.Resources</span></span>
- <span data-ttu-id="328ec-476">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-476">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="328ec-477">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="328ec-477">Az.ServiceFabric</span></span>
- <span data-ttu-id="328ec-478">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="328ec-478">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="328ec-479">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-479">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="328ec-480">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="328ec-480">Az.SIgnalR</span></span>
- <span data-ttu-id="328ec-481">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="328ec-481">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="328ec-482">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-482">Az.Sql</span></span>
- <span data-ttu-id="328ec-483">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-483">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="328ec-484">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-484">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="328ec-485">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-485">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="328ec-486">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-486">Az.Storage</span></span>
- <span data-ttu-id="328ec-487">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-487">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="328ec-488">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-488">Az.Websites</span></span>
- <span data-ttu-id="328ec-489">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="328ec-489">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="328ec-490">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="328ec-490">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="328ec-491">全般</span><span class="sxs-lookup"><span data-stu-id="328ec-491">General</span></span>

* <span data-ttu-id="328ec-492">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="328ec-492">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="328ec-493">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-493">Az.Compute</span></span>

* <span data-ttu-id="328ec-494">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-494">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="328ec-495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-495">Az.DataLakeStore</span></span>

* <span data-ttu-id="328ec-496">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-496">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="328ec-497">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="328ec-497">Az.FrontDoor</span></span>

* <span data-ttu-id="328ec-498">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-498">Fixed some broken links</span></span>
    - <span data-ttu-id="328ec-499">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-499">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="328ec-500">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-500">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="328ec-501">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="328ec-501">Az.RecoveryServices</span></span>

* <span data-ttu-id="328ec-502">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-502">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="328ec-503">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="328ec-503">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="328ec-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-504">Az.Resources</span></span>

* <span data-ttu-id="328ec-505">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="328ec-505">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="328ec-506">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-506">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="328ec-507">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-507">Az.Sql</span></span>

* <span data-ttu-id="328ec-508">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="328ec-508">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="328ec-509">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-509">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="328ec-510">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="328ec-510">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="328ec-511">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-511">Az.Storage</span></span>

* <span data-ttu-id="328ec-512">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-512">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="328ec-513">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-513">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="328ec-514">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="328ec-514">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="328ec-515">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="328ec-515">Support Static Website configuration</span></span>
    - <span data-ttu-id="328ec-516">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="328ec-516">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="328ec-517">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="328ec-517">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="328ec-518">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-518">Az.Websites</span></span>

* <span data-ttu-id="328ec-519">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="328ec-519">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="328ec-520">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-520">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="328ec-521">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="328ec-521">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="328ec-522">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="328ec-522">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="328ec-523">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="328ec-523">Az.ApiManagement</span></span>
* <span data-ttu-id="328ec-524">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-524">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="328ec-525">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="328ec-525">Az.Automation</span></span>
* <span data-ttu-id="328ec-526">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="328ec-526">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="328ec-527">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-527">Added Update Management cmdlets</span></span>
* <span data-ttu-id="328ec-528">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-528">Added Source Control cmdlets</span></span>
* <span data-ttu-id="328ec-529">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-529">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="328ec-530">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-530">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="328ec-531">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-531">Az.Compute</span></span>
* <span data-ttu-id="328ec-532">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-532">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="328ec-533">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-533">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="328ec-534">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-534">Az.ContainerInstance</span></span>
* <span data-ttu-id="328ec-535">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-535">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="328ec-536">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="328ec-536">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="328ec-537">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-537">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="328ec-538">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-538">Az.Network</span></span>
* <span data-ttu-id="328ec-539">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-539">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="328ec-540">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-540">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="328ec-541">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-541">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="328ec-542">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-542">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="328ec-543">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="328ec-543">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="328ec-544">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-544">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="328ec-545">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="328ec-545">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="328ec-546">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="328ec-546">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="328ec-547">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-547">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="328ec-548">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-548">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="328ec-549">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="328ec-549">Az.Relay</span></span>
* <span data-ttu-id="328ec-550">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="328ec-550">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="328ec-551">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-551">Az.Resources</span></span>
* <span data-ttu-id="328ec-552">`New-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-552">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and</span></span> `Set-AzureRmPolicyAssignment`
* <span data-ttu-id="328ec-553">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-553">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="328ec-554">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="328ec-554">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="328ec-555">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="328ec-555">Az.ServiceFabric</span></span>
* <span data-ttu-id="328ec-556">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-556">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="328ec-557">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-557">Az.Sql</span></span>
* <span data-ttu-id="328ec-558">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-558">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="328ec-559">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-559">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="328ec-560">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-560">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="328ec-561">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-561">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="328ec-562">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="328ec-562">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="328ec-563">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="328ec-563">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="328ec-564">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="328ec-564">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="328ec-565">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="328ec-565">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="328ec-566">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="328ec-566">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="328ec-567">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="328ec-567">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="328ec-568">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-568">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="328ec-569">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="328ec-569">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="328ec-570">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="328ec-570">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="328ec-571">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="328ec-571">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="328ec-572">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="328ec-572">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="328ec-573">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="328ec-573">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="328ec-574">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-574">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="328ec-575">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="328ec-575">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="328ec-576">全般</span><span class="sxs-lookup"><span data-stu-id="328ec-576">General</span></span>
* <span data-ttu-id="328ec-577">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="328ec-577">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="328ec-578">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="328ec-578">Az.Profile</span></span>
* <span data-ttu-id="328ec-579">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-579">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="328ec-580">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-580">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="328ec-581">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="328ec-581">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="328ec-582">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-582">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="328ec-583">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-583">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="328ec-584">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-584">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="328ec-585">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-585">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="328ec-586">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="328ec-586">Az.CognitiveServices</span></span>
* <span data-ttu-id="328ec-587">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-587">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-588">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-588">Az.Compute</span></span>
* <span data-ttu-id="328ec-589">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-589">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="328ec-590">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="328ec-590">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="328ec-591">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-591">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="328ec-592">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-592">Az.DataLakeStore</span></span>
* <span data-ttu-id="328ec-593">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="328ec-593">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="328ec-594">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-594">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="328ec-595">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="328ec-595">Az.Insights</span></span>
* <span data-ttu-id="328ec-596">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-596">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="328ec-597">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="328ec-597">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="328ec-598">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-598">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="328ec-599">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="328ec-599">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-600">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-600">Az.Network</span></span>
* <span data-ttu-id="328ec-601">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="328ec-601">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="328ec-602">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="328ec-602">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="328ec-603">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="328ec-603">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="328ec-604">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="328ec-604">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="328ec-605">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="328ec-605">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="328ec-606">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="328ec-606">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="328ec-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="328ec-607">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="328ec-608">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="328ec-608">Az.PolicyInsights</span></span>
* <span data-ttu-id="328ec-609">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-609">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-610">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-610">Az.Resources</span></span>
* <span data-ttu-id="328ec-611">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="328ec-611">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="328ec-612">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="328ec-612">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="328ec-613">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="328ec-613">Az.ServiceBus</span></span>
* <span data-ttu-id="328ec-614">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-614">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="328ec-615">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="328ec-615">Az.ServiceFabric</span></span>
* <span data-ttu-id="328ec-616">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-616">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="328ec-617">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-617">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="328ec-618">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="328ec-618">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="328ec-619">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="328ec-619">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="328ec-620">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-620">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="328ec-621">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="328ec-621">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="328ec-622">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="328ec-622">Az.Profile</span></span>
* <span data-ttu-id="328ec-623">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-623">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="328ec-624">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-624">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-625">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-625">Az.Compute</span></span>
* <span data-ttu-id="328ec-626">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-626">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="328ec-627">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-627">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="328ec-628">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="328ec-628">Az.DataLakeStore</span></span>
* <span data-ttu-id="328ec-629">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-629">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="328ec-630">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="328ec-630">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="328ec-631">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="328ec-631">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="328ec-632">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="328ec-632">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="328ec-633">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="328ec-633">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-634">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-634">Az.Network</span></span>
* <span data-ttu-id="328ec-635">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-635">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="328ec-636">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-636">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-637">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-637">Az.Resources</span></span>
* <span data-ttu-id="328ec-638">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-638">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="328ec-639">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-639">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="328ec-640">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="328ec-640">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="328ec-641">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="328ec-641">Azure.Storage</span></span>
* <span data-ttu-id="328ec-642">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-642">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="328ec-643">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="328ec-643">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="328ec-644">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="328ec-644">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="328ec-645">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-645">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="328ec-646">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="328ec-646">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="328ec-647">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="328ec-647">Az.CognitiveServices</span></span>
* <span data-ttu-id="328ec-648">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="328ec-648">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="328ec-649">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="328ec-649">Az.Compute</span></span>
* <span data-ttu-id="328ec-650">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-650">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="328ec-651">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-651">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="328ec-652">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-652">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="328ec-653">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="328ec-653">Az.DataFactoryV2</span></span>
* <span data-ttu-id="328ec-654">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-654">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="328ec-655">Az.Network</span><span class="sxs-lookup"><span data-stu-id="328ec-655">Az.Network</span></span>
* <span data-ttu-id="328ec-656">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="328ec-656">Added NetworkProfile functionality.</span></span> <span data-ttu-id="328ec-657">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="328ec-657">new cmdlets added</span></span>
    - <span data-ttu-id="328ec-658">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="328ec-658">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="328ec-659">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="328ec-659">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="328ec-660">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="328ec-660">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="328ec-661">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="328ec-661">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="328ec-662">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="328ec-662">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="328ec-663">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="328ec-663">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="328ec-664">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-664">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="328ec-665">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-665">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="328ec-666">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-666">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="328ec-667">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="328ec-667">Az.RedisCache</span></span>
* <span data-ttu-id="328ec-668">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="328ec-668">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="328ec-669">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-669">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="328ec-670">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="328ec-670">Az.Resources</span></span>
* <span data-ttu-id="328ec-671">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="328ec-671">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="328ec-672">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-672">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="328ec-673">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="328ec-673">Az.Sql</span></span>
* <span data-ttu-id="328ec-674">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="328ec-674">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="328ec-675">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="328ec-675">Az.Websites</span></span>
* <span data-ttu-id="328ec-676">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="328ec-676">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="328ec-677">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="328ec-677">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="328ec-678">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="328ec-678">0.2.0 - September 2018</span></span>
 <span data-ttu-id="328ec-679">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="328ec-679">Initial Release</span></span>