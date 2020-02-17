---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/09/2020
ms.openlocfilehash: 694439934afb41b465a89188d59bc964db3c0032
ms.sourcegitcommit: 9181f20c2c5eaa271150de9e25b9cb30ba5e6cb0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/04/2020
ms.locfileid: "77002675"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="cf51e-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="cf51e-103">Azure PowerShell release notes</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="cf51e-104">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-104">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cf51e-105">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cf51e-105">Highlights since the last major release</span></span>
* <span data-ttu-id="cf51e-106">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-106">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="cf51e-107">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-107">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-108">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-108">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-109">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="cf51e-109">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="cf51e-110">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-110">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="cf51e-111">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-111">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-112">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="cf51e-112">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="cf51e-113">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="cf51e-113">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="cf51e-114">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-114">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="cf51e-115">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-115">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-116">Az.Compute</span></span>
* <span data-ttu-id="cf51e-117">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-117">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="cf51e-118">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-118">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="cf51e-119">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-119">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="cf51e-120">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-120">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="cf51e-121">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-121">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-122">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-122">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-123">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-123">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="cf51e-124">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="cf51e-124">Az.DeploymentManager</span></span>
* <span data-ttu-id="cf51e-125">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-125">Adds LIST operations for resources</span></span>
* <span data-ttu-id="cf51e-126">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-126">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="cf51e-127">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cf51e-127">Az.HDInsight</span></span>
* <span data-ttu-id="cf51e-128">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-128">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-129">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-129">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-130">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-130">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-131">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-131">Az.Network</span></span>
* <span data-ttu-id="cf51e-132">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-132">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="cf51e-133">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="cf51e-133">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="cf51e-134">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="cf51e-134">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="cf51e-135">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-135">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="cf51e-136">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="cf51e-136">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="cf51e-137">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-137">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="cf51e-138">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-138">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="cf51e-139">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-139">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="cf51e-140">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-140">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-141">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf51e-141">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="cf51e-142">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-142">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="cf51e-143">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-143">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="cf51e-144">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-144">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cf51e-145">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-145">Az.PolicyInsights</span></span>
* <span data-ttu-id="cf51e-146">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-146">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="cf51e-147">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-147">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="cf51e-148">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-148">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="cf51e-149">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-149">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-150">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-150">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-151">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-151">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="cf51e-152">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-152">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-153">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-153">Az.Resources</span></span>
* <span data-ttu-id="cf51e-154">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="cf51e-154">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="cf51e-155">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-155">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-156">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-156">Az.Sql</span></span>
<span data-ttu-id="cf51e-157">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-157">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-158">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-158">Az.Storage</span></span>
* <span data-ttu-id="cf51e-159">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-159">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="cf51e-160">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-160">New-AzStorageAccount</span></span>
* <span data-ttu-id="cf51e-161">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="cf51e-161">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="cf51e-162">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-162">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-163">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-163">Az.Websites</span></span>
* <span data-ttu-id="cf51e-164">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-164">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="cf51e-165">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-165">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="cf51e-166">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-166">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-167">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-167">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-168">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-168">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cf51e-169">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-169">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-170">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="cf51e-170">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-171">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-171">Az.Compute</span></span>
* <span data-ttu-id="cf51e-172">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-172">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="cf51e-173">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-173">Az.ContainerInstance</span></span>
* <span data-ttu-id="cf51e-174">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-174">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="cf51e-175">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="cf51e-175">Az.DataBoxEdge</span></span>
* <span data-ttu-id="cf51e-176">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-176">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="cf51e-177">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-177">Get the Edge Storage Container</span></span>
* <span data-ttu-id="cf51e-178">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-178">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="cf51e-179">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-179">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="cf51e-180">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-180">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="cf51e-181">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-181">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="cf51e-182">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-182">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="cf51e-183">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="cf51e-183">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="cf51e-184">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-184">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="cf51e-185">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-185">Get the Edge Storage Account</span></span>
* <span data-ttu-id="cf51e-186">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-186">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="cf51e-187">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-187">Create new Edge Storage Account</span></span>
* <span data-ttu-id="cf51e-188">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-188">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="cf51e-189">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-189">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="cf51e-190">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="cf51e-190">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="cf51e-191">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="cf51e-191">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="cf51e-192">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-192">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="cf51e-193">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="cf51e-193">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-194">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-194">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-195">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-195">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="cf51e-196">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-196">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="cf51e-197">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-197">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="cf51e-198">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="cf51e-198">Az.DevTestLabs</span></span>
* <span data-ttu-id="cf51e-199">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-199">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-200">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-200">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-201">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-201">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="cf51e-202">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cf51e-202">Az.HDInsight</span></span>
* <span data-ttu-id="cf51e-203">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-203">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="cf51e-204">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cf51e-204">Az.MachineLearning</span></span>
* <span data-ttu-id="cf51e-205">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-205">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="cf51e-206">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="cf51e-206">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="cf51e-207">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="cf51e-207">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="cf51e-208">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="cf51e-208">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="cf51e-209">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="cf51e-209">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="cf51e-210">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="cf51e-210">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="cf51e-211">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="cf51e-211">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="cf51e-212">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="cf51e-212">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-213">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-213">Az.Network</span></span>
* <span data-ttu-id="cf51e-214">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="cf51e-214">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-215">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-215">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-216">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-216">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="cf51e-217">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-217">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="cf51e-218">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-218">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="cf51e-219">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-219">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-220">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-220">Az.Resources</span></span>
* <span data-ttu-id="cf51e-221">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-221">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-222">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-222">Az.Sql</span></span>
* <span data-ttu-id="cf51e-223">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-223">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="cf51e-224">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-224">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="cf51e-225">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="cf51e-225">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="cf51e-226">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-226">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-227">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-227">Az.Storage</span></span>
* <span data-ttu-id="cf51e-228">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-228">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="cf51e-229">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-229">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="cf51e-230">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-230">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span> 
    - <span data-ttu-id="cf51e-231">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-231">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="cf51e-232">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-232">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="cf51e-233">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-233">General</span></span>
* <span data-ttu-id="cf51e-234">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-234">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-235">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-235">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-236">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="cf51e-236">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="cf51e-237">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="cf51e-237">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="cf51e-238">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cf51e-238">Az.Batch</span></span>
* <span data-ttu-id="cf51e-239">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="cf51e-239">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-240">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-240">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-241">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-241">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="cf51e-242">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cf51e-242">Az.FrontDoor</span></span>
* <span data-ttu-id="cf51e-243">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-243">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="cf51e-244">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-244">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="cf51e-245">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="cf51e-245">Az.HealthcareApis</span></span>
* <span data-ttu-id="cf51e-246">例外処理</span><span class="sxs-lookup"><span data-stu-id="cf51e-246">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-247">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-247">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-248">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-248">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="cf51e-249">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="cf51e-249">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="cf51e-250">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-250">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-251">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-251">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-252">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-252">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="cf51e-253">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="cf51e-253">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="cf51e-254">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="cf51e-254">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-255">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-255">Az.Network</span></span>
* <span data-ttu-id="cf51e-256">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-256">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-257">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-257">Az.Resources</span></span>
* <span data-ttu-id="cf51e-258">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-258">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="cf51e-259">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-259">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-260">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-260">Az.Sql</span></span>
* <span data-ttu-id="cf51e-261">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-261">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-262">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-262">Az.Storage</span></span>
* <span data-ttu-id="cf51e-263">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-263">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="cf51e-264">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="cf51e-264">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="cf51e-265">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="cf51e-265">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="cf51e-266">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="cf51e-266">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="cf51e-267">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="cf51e-267">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="cf51e-268">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-268">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="cf51e-269">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-269">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span> 
    - <span data-ttu-id="cf51e-270">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="cf51e-270">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="cf51e-271">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="cf51e-271">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="cf51e-272">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-272">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="cf51e-273">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="cf51e-273">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="cf51e-274">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-274">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="cf51e-275">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="cf51e-275">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="cf51e-276">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-276">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cf51e-277">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cf51e-277">Highlights since the last major release</span></span>
* <span data-ttu-id="cf51e-278">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-278">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="cf51e-279">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-279">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-280">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-280">Az.Compute</span></span>
* <span data-ttu-id="cf51e-281">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="cf51e-281">VM Reapply feature</span></span>
    - <span data-ttu-id="cf51e-282">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-282">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="cf51e-283">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="cf51e-283">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="cf51e-284">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="cf51e-284">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="cf51e-285">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-285">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="cf51e-286">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-286">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="cf51e-287">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-287">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="cf51e-288">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="cf51e-288">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="cf51e-289">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-289">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="cf51e-290">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-290">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="cf51e-291">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-291">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="cf51e-292">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="cf51e-292">Az.DataBoxEdge</span></span>
* <span data-ttu-id="cf51e-293">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-293">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="cf51e-294">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-294">Get the Order</span></span>
* <span data-ttu-id="cf51e-295">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-295">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="cf51e-296">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-296">Create new Order</span></span>
* <span data-ttu-id="cf51e-297">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-297">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="cf51e-298">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-298">Remove the Order</span></span>
* <span data-ttu-id="cf51e-299">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="cf51e-299">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="cf51e-300">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="cf51e-300">Now creates Local Share</span></span>
* <span data-ttu-id="cf51e-301">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-301">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="cf51e-302">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-302">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="cf51e-303">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-303">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="cf51e-304">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="cf51e-304">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="cf51e-305">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-305">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="cf51e-306">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-306">Gets the information about Triggers</span></span>
* <span data-ttu-id="cf51e-307">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-307">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="cf51e-308">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-308">Create new Triggers</span></span>
* <span data-ttu-id="cf51e-309">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-309">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="cf51e-310">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-310">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-311">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-311">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-312">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-312">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="cf51e-313">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-313">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-314">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-314">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-315">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-315">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-316">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-316">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-317">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-317">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="cf51e-318">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cf51e-318">Az.FrontDoor</span></span>
* <span data-ttu-id="cf51e-319">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-319">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="cf51e-320">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-320">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="cf51e-321">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-321">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="cf51e-322">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="cf51e-322">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-323">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-323">Az.Network</span></span>
* <span data-ttu-id="cf51e-324">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-324">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="cf51e-325">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="cf51e-325">Az.PrivateDns</span></span>
* <span data-ttu-id="cf51e-326">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-326">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-327">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-327">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-328">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-328">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="cf51e-329">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="cf51e-329">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="cf51e-330">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-330">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cf51e-331">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cf51e-331">Az.RedisCache</span></span>
* <span data-ttu-id="cf51e-332">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-332">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="cf51e-333">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-333">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="cf51e-334">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-334">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-335">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-335">Az.Resources</span></span>
- <span data-ttu-id="cf51e-336">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-336">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="cf51e-337">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-337">Updated create policy definition help example</span></span>
- <span data-ttu-id="cf51e-338">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-338">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="cf51e-339">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-339">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="cf51e-340">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-340">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-341">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-341">Az.Sql</span></span>
* <span data-ttu-id="cf51e-342">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-342">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="cf51e-343">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-343">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="cf51e-344">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-344">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="cf51e-345">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-345">General</span></span>
* <span data-ttu-id="cf51e-346">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-346">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-347">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-347">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-348">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-348">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="cf51e-349">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="cf51e-349">Az.Advisor</span></span>
* <span data-ttu-id="cf51e-350">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-350">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="cf51e-351">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cf51e-351">Az.Batch</span></span>
* <span data-ttu-id="cf51e-352">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-352">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="cf51e-353">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="cf51e-353">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="cf51e-354">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-354">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="cf51e-355">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-355">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="cf51e-356">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="cf51e-356">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="cf51e-357">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-357">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="cf51e-358">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-358">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="cf51e-359">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-359">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="cf51e-360">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-360">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="cf51e-361">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-361">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="cf51e-362">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-362">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="cf51e-363">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-363">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="cf51e-364">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-364">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="cf51e-365">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-365">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="cf51e-366">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-366">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="cf51e-367">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-367">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="cf51e-368">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-368">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="cf51e-369">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-369">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="cf51e-370">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-370">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="cf51e-371">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf51e-371">This operation is no longer supported.</span></span>
* <span data-ttu-id="cf51e-372">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-372">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="cf51e-373">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-373">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="cf51e-374">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-374">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="cf51e-375">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-375">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span> 
  - <span data-ttu-id="cf51e-376">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-376">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="cf51e-377">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-377">New non-verified images are also now returned.</span></span> <span data-ttu-id="cf51e-378">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-378">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="cf51e-379">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-379">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="cf51e-380">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-380">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="cf51e-381">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-381">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="cf51e-382">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-382">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="cf51e-383">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-383">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="cf51e-384">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-384">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="cf51e-385">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-385">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="cf51e-386">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-386">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="cf51e-387">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-387">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cf51e-388">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-388">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-389">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-389">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="cf51e-390">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-390">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-391">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-391">Az.Compute</span></span>
* <span data-ttu-id="cf51e-392">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="cf51e-392">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="cf51e-393">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-393">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="cf51e-394">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile</span><span class="sxs-lookup"><span data-stu-id="cf51e-394">DiskEncryptionSetId parameter is added to the following cmdlets: Set-AzImageOSDisk Set-AzVMOSDisk Set-AzVmssStorageProfile</span></span>        
        <span data-ttu-id="cf51e-395">Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="cf51e-395">Add-AzImageDataDisk New-AzVMDataDisk Set-AzVMDataDisk Add-AzVMDataDisk Add-AzVmssDataDisk Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="cf51e-396">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-396">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="cf51e-397">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-397">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="cf51e-398">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="cf51e-398">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="cf51e-399">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-399">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="cf51e-400">重大な変更</span><span class="sxs-lookup"><span data-stu-id="cf51e-400">Breaking changes</span></span>
    - <span data-ttu-id="cf51e-401">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="cf51e-401">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="cf51e-402">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="cf51e-402">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-403">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-403">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-404">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-404">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-405">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-405">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-406">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="cf51e-406">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="cf51e-407">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-407">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="cf51e-408">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="cf51e-408">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="cf51e-409">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-409">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="cf51e-410">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-410">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="cf51e-411">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-411">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="cf51e-412">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cf51e-412">Az.FrontDoor</span></span>
* <span data-ttu-id="cf51e-413">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-413">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="cf51e-414">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cf51e-414">Az.HDInsight</span></span>
* <span data-ttu-id="cf51e-415">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-415">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="cf51e-416">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-416">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="cf51e-417">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-417">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="cf51e-418">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-418">Removed five cmdlets:</span></span>
    - <span data-ttu-id="cf51e-419">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="cf51e-419">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="cf51e-420">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="cf51e-420">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="cf51e-421">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="cf51e-421">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="cf51e-422">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="cf51e-422">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="cf51e-423">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="cf51e-423">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="cf51e-424">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-424">Added three cmdlets:</span></span>
    - <span data-ttu-id="cf51e-425">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-425">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="cf51e-426">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-426">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="cf51e-427">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-427">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="cf51e-428">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-428">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="cf51e-429">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-429">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="cf51e-430">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-430">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="cf51e-431">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="cf51e-431">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="cf51e-432">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-432">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="cf51e-433">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-433">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="cf51e-434">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-434">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="cf51e-435">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-435">Added some scenario test cases.</span></span>
* <span data-ttu-id="cf51e-436">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="cf51e-436">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-437">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-437">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-438">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="cf51e-438">Breaking changes:</span></span>
    - <span data-ttu-id="cf51e-439">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-439">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="cf51e-440">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-440">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="cf51e-441">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-441">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="cf51e-442">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-442">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="cf51e-443">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-443">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="cf51e-444">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-444">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="cf51e-445">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-445">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="cf51e-446">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-446">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="cf51e-447">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-447">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="cf51e-448">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-448">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="cf51e-449">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-449">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="cf51e-450">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-450">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-451">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-451">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-452">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-452">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-453">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-453">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="cf51e-454">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-454">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="cf51e-455">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-455">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-456">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-456">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-457">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-457">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-458">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-458">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-459">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-459">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-460">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-460">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-461">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-461">Az.Resources</span></span>
* <span data-ttu-id="cf51e-462">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-462">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-463">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-463">Az.Network</span></span>
* <span data-ttu-id="cf51e-464">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-464">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="cf51e-465">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-465">Updated cmdlet:</span></span>
        - <span data-ttu-id="cf51e-466">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-466">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-467">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-467">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-468">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-468">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-469">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-469">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-470">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-470">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="cf51e-471">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="cf51e-471">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="cf51e-472">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-472">New cmdlet:</span></span>
        - <span data-ttu-id="cf51e-473">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="cf51e-473">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="cf51e-474">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-474">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="cf51e-475">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-475">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="cf51e-476">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-476">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="cf51e-477">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-477">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="cf51e-478">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-478">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="cf51e-479">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-479">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="cf51e-480">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-480">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="cf51e-481">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-481">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-482">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="cf51e-482">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="cf51e-483">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-483">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="cf51e-484">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-484">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="cf51e-485">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-485">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="cf51e-486">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-486">Set-AzVirtualHub</span></span>
* <span data-ttu-id="cf51e-487">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-487">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="cf51e-488">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cf51e-488">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="cf51e-489">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-489">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="cf51e-490">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-490">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="cf51e-491">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-491">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="cf51e-492">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-492">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="cf51e-493">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-493">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="cf51e-494">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-494">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-495">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-495">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="cf51e-496">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cf51e-496">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="cf51e-497">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-497">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="cf51e-498">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-498">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="cf51e-499">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-499">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="cf51e-500">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-500">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="cf51e-501">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-501">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="cf51e-502">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-502">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="cf51e-503">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-503">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-504">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="cf51e-504">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="cf51e-505">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="cf51e-505">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="cf51e-506">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="cf51e-506">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="cf51e-507">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="cf51e-507">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="cf51e-508">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-508">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="cf51e-509">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-509">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="cf51e-510">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cf51e-510">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="cf51e-511">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-511">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="cf51e-512">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-512">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="cf51e-513">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-513">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="cf51e-514">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-514">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="cf51e-515">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cf51e-515">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="cf51e-516">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-516">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="cf51e-517">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-517">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="cf51e-518">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-518">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="cf51e-519">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-519">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="cf51e-520">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-520">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="cf51e-521">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-521">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-522">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="cf51e-522">New-AzIpGroup</span></span>
        - <span data-ttu-id="cf51e-523">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="cf51e-523">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="cf51e-524">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="cf51e-524">Get-AzIpGroup</span></span>
        - <span data-ttu-id="cf51e-525">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="cf51e-525">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-526">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-526">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-527">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-527">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-528">Az.Sql</span></span>
* <span data-ttu-id="cf51e-529">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-529">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="cf51e-530">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-530">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="cf51e-531">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-531">Removed deprecated aliases:</span></span>
* <span data-ttu-id="cf51e-532">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="cf51e-532">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="cf51e-533">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="cf51e-533">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="cf51e-534">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-534">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="cf51e-535">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-535">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="cf51e-536">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="cf51e-536">Deprecate Advanced Threat Detection Settings cmdlets</span></span> 
* <span data-ttu-id="cf51e-537">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-537">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-538">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-538">Az.Storage</span></span>
* <span data-ttu-id="cf51e-539">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-539">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="cf51e-540">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-540">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="cf51e-541">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-541">Set-AzStorageAccount</span></span>
* <span data-ttu-id="cf51e-542">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="cf51e-542">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="cf51e-543">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="cf51e-543">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="cf51e-544">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="cf51e-544">Close-AzStorageFileHandle</span></span>
    
## <a name="280---october-2019"></a><span data-ttu-id="cf51e-545">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-545">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="cf51e-546">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-546">General</span></span>
* <span data-ttu-id="cf51e-547">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-547">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-548">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-548">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-549">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-549">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="cf51e-550">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-550">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-551">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-551">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="cf51e-552">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="cf51e-552">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-553">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-553">Az.Automation</span></span>
* <span data-ttu-id="cf51e-554">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-554">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span> 

#### <a name="azbatch"></a><span data-ttu-id="cf51e-555">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cf51e-555">Az.Batch</span></span>
* <span data-ttu-id="cf51e-556">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-556">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-557">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-557">Az.Compute</span></span>
* <span data-ttu-id="cf51e-558">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-558">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="cf51e-559">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-559">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="cf51e-560">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-560">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span> 
* <span data-ttu-id="cf51e-561">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-561">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-562">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-562">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-563">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="cf51e-563">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="cf51e-564">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="cf51e-564">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="cf51e-565">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-565">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-566">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-566">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-567">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-567">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="cf51e-568">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="cf51e-568">Az.HealthcareApis</span></span>
* <span data-ttu-id="cf51e-569">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-569">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="cf51e-570">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-570">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="cf51e-571">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-571">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="cf51e-572">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-572">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-573">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-573">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-574">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="cf51e-574">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="cf51e-575">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="cf51e-575">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span> 

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-576">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-576">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-577">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="cf51e-577">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="cf51e-578">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-578">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="cf51e-579">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="cf51e-579">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="cf51e-580">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-580">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-581">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-581">Az.Network</span></span>
* <span data-ttu-id="cf51e-582">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-582">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="cf51e-583">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-583">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="cf51e-584">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-584">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-585">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-585">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="cf51e-586">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-586">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="cf51e-587">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-587">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="cf51e-588">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-588">Updated cmdlets:</span></span>
        - <span data-ttu-id="cf51e-589">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-589">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="cf51e-590">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-590">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="cf51e-591">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-591">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="cf51e-592">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="cf51e-592">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="cf51e-593">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="cf51e-593">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="cf51e-594">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-594">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="cf51e-595">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-595">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cf51e-596">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cf51e-596">Az.RedisCache</span></span>
* <span data-ttu-id="cf51e-597">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-597">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-598">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-598">Az.Sql</span></span>
* <span data-ttu-id="cf51e-599">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-599">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-600">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-600">Az.Storage</span></span>
* <span data-ttu-id="cf51e-601">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="cf51e-601">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="cf51e-602">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cf51e-602">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="cf51e-603">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="cf51e-603">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="cf51e-604">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cf51e-604">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="cf51e-605">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-605">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="cf51e-606">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="cf51e-606">Az.StorageSync</span></span>
* <span data-ttu-id="cf51e-607">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-607">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-608">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-608">Az.Websites</span></span>
* <span data-ttu-id="cf51e-609">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="cf51e-609">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="cf51e-610">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-610">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="cf51e-611">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-611">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-612">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-612">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="cf51e-613">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-613">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="cf51e-614">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="cf51e-614">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-615">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-615">Az.Automation</span></span>
* <span data-ttu-id="cf51e-616">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-616">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="cf51e-617">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-617">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="cf51e-618">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-618">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-619">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-619">Az.Compute</span></span>
* <span data-ttu-id="cf51e-620">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-620">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="cf51e-621">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-621">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="cf51e-622">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-622">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="cf51e-623">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-623">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="cf51e-624">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-624">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="cf51e-625">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-625">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="cf51e-626">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-626">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="cf51e-627">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-627">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="cf51e-628">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-628">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-629">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-629">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-630">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-630">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="cf51e-631">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-631">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="cf51e-632">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cf51e-632">Az.HDInsight</span></span>
* <span data-ttu-id="cf51e-633">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="cf51e-633">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-634">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-634">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-635">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-635">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="cf51e-636">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-636">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="cf51e-637">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cf51e-637">New cmdlets are:</span></span>
    - <span data-ttu-id="cf51e-638">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="cf51e-638">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="cf51e-639">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="cf51e-639">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="cf51e-640">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="cf51e-640">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="cf51e-641">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="cf51e-641">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-642">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-642">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-643">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="cf51e-643">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="cf51e-644">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-644">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="cf51e-645">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="cf51e-645">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="cf51e-646">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-646">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="cf51e-647">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-647">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="cf51e-648">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-648">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="cf51e-649">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-649">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="cf51e-650">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="cf51e-650">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="cf51e-651">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-651">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="cf51e-652">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-652">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="cf51e-653">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-653">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="cf51e-654">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="cf51e-654">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="cf51e-655">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-655">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="cf51e-656">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-656">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="cf51e-657">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-657">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="cf51e-658">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="cf51e-658">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="cf51e-659">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-659">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="cf51e-660">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-660">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="cf51e-661">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-661">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="cf51e-662">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-662">Overall improved help files</span></span>
* <span data-ttu-id="cf51e-663">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-663">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-664">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-664">Az.Network</span></span>
* <span data-ttu-id="cf51e-665">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-665">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span> 
* <span data-ttu-id="cf51e-666">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-666">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="cf51e-667">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-667">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="cf51e-668">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-668">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="cf51e-669">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-669">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="cf51e-670">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-670">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="cf51e-671">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-671">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="cf51e-672">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-672">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="cf51e-673">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-673">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="cf51e-674">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-674">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="cf51e-675">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-675">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="cf51e-676">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-676">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="cf51e-677">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-677">New cmdlets</span></span>
        - <span data-ttu-id="cf51e-678">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="cf51e-678">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="cf51e-679">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-679">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="cf51e-680">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-680">Updated cmdlet:</span></span>
        - <span data-ttu-id="cf51e-681">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="cf51e-681">New-VpnSite</span></span>
        - <span data-ttu-id="cf51e-682">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="cf51e-682">Update-VpnSite</span></span>
        - <span data-ttu-id="cf51e-683">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-683">New-VpnConnection</span></span>
        - <span data-ttu-id="cf51e-684">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-684">Update-VpnConnection</span></span>
* <span data-ttu-id="cf51e-685">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-685">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-686">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-686">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-687">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-687">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="cf51e-688">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-688">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-689">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-689">Az.Resources</span></span>
* <span data-ttu-id="cf51e-690">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-690">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-691">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-691">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-692">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-692">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="cf51e-693">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-693">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="cf51e-694">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="cf51e-694">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="cf51e-695">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="cf51e-695">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="cf51e-696">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="cf51e-696">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="cf51e-697">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="cf51e-697">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="cf51e-698">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="cf51e-698">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="cf51e-699">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="cf51e-699">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="cf51e-700">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="cf51e-700">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="cf51e-701">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="cf51e-701">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="cf51e-702">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="cf51e-702">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="cf51e-703">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="cf51e-703">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="cf51e-704">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="cf51e-704">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="cf51e-705">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="cf51e-705">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="cf51e-706">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="cf51e-706">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="cf51e-707">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-707">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cf51e-708">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cf51e-708">Az.SignalR</span></span>
* <span data-ttu-id="cf51e-709">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="cf51e-709">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-710">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-710">Az.Sql</span></span>
* <span data-ttu-id="cf51e-711">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-711">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="cf51e-712">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-712">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="cf51e-713">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-713">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="cf51e-714">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-714">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="cf51e-715">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-715">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-716">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-716">Az.Storage</span></span>
* <span data-ttu-id="cf51e-717">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-717">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="cf51e-718">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-718">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="cf51e-719">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-719">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="cf51e-720">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-720">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="cf51e-721">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-721">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="cf51e-722">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-722">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="cf51e-723">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-723">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="cf51e-724">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="cf51e-724">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="cf51e-725">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="cf51e-725">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="cf51e-726">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="cf51e-726">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="cf51e-727">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="cf51e-727">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-728">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-728">Az.Websites</span></span>
* <span data-ttu-id="cf51e-729">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-729">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="cf51e-730">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="cf51e-730">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="cf51e-731">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-731">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="cf51e-732">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-732">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="cf51e-733">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-733">General</span></span>
* <span data-ttu-id="cf51e-734">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-734">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-735">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-735">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-736">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="cf51e-736">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="cf51e-737">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="cf51e-737">Az.Aks</span></span>
* <span data-ttu-id="cf51e-738">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-738">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="cf51e-739">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="cf51e-739">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="cf51e-740">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-740">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-741">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="cf51e-741">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="cf51e-742">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="cf51e-742">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="cf51e-743">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-743">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="cf51e-744">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="cf51e-744">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="cf51e-745">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-745">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="cf51e-746">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cf51e-746">Az.Batch</span></span>
* <span data-ttu-id="cf51e-747">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-747">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cf51e-748">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-748">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-749">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-749">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-750">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-750">Az.Compute</span></span>
* <span data-ttu-id="cf51e-751">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-751">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="cf51e-752">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-752">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="cf51e-753">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-753">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="cf51e-754">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-754">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="cf51e-755">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="cf51e-755">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="cf51e-756">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="cf51e-756">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="cf51e-757">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-757">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="cf51e-758">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-758">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-759">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-759">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-760">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-760">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="cf51e-761">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-761">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="cf51e-762">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-762">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="cf51e-763">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-763">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-764">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-764">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-765">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-765">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-766">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-766">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-767">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="cf51e-767">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="cf51e-768">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="cf51e-768">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="cf51e-769">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-769">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="cf51e-770">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="cf51e-770">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="cf51e-771">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="cf51e-771">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="cf51e-772">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-772">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-773">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-773">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-774">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-774">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-775">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-775">Az.Network</span></span>
* <span data-ttu-id="cf51e-776">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-776">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="cf51e-777">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-777">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="cf51e-778">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-778">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="cf51e-779">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-779">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="cf51e-780">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-780">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span> 
* <span data-ttu-id="cf51e-781">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-781">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="cf51e-782">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-782">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-783">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-783">Az.OperationalInsights</span></span>
* <span data-ttu-id="cf51e-784">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-784">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="cf51e-785">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-785">Added example</span></span>
    - <span data-ttu-id="cf51e-786">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-786">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="cf51e-787">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-787">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="cf51e-788">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-788">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-789">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-789">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-790">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-790">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-791">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-791">Az.Resources</span></span>
* <span data-ttu-id="cf51e-792">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-792">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="cf51e-793">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-793">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="cf51e-794">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="cf51e-794">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="cf51e-795">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-795">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cf51e-796">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cf51e-796">Az.ServiceBus</span></span>
* <span data-ttu-id="cf51e-797">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="cf51e-797">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="cf51e-798">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="cf51e-798">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="cf51e-799">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-799">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span> 

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-800">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-800">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-801">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-801">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="cf51e-802">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="cf51e-802">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="cf51e-803">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="cf51e-803">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="cf51e-804">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-804">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="cf51e-805">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="cf51e-805">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="cf51e-806">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-806">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-807">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-807">Az.Sql</span></span>
* <span data-ttu-id="cf51e-808">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-808">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-809">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-809">Az.Storage</span></span>
* <span data-ttu-id="cf51e-810">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-810">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="cf51e-811">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-811">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="cf51e-812">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-812">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="cf51e-813">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="cf51e-813">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="cf51e-814">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-814">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="cf51e-815">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="cf51e-815">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-816">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-816">Az.Websites</span></span>
* <span data-ttu-id="cf51e-817">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-817">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="cf51e-818">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-818">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-819">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-819">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-820">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-820">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="cf51e-821">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-821">Az.ApplicationInsights</span></span>
* <span data-ttu-id="cf51e-822">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-822">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="cf51e-823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-823">Az.Automation</span></span>
* <span data-ttu-id="cf51e-824">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-824">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="cf51e-825">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-825">Az.CognitiveServices</span></span>
* <span data-ttu-id="cf51e-826">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-826">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-827">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-827">Az.Compute</span></span>
* <span data-ttu-id="cf51e-828">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-828">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="cf51e-829">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="cf51e-829">Az.ContainerRegistry</span></span>
* <span data-ttu-id="cf51e-830">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-830">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="cf51e-831">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="cf51e-831">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-832">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-832">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-833">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-833">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="cf51e-834">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-834">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-835">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-835">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-836">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="cf51e-836">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="cf51e-837">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-837">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-838">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-838">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-839">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-839">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cf51e-840">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cf51e-840">Az.LogicApp</span></span>
* <span data-ttu-id="cf51e-841">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-841">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="cf51e-842">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-842">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="cf51e-843">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-843">Az.ManagedServices</span></span>
* <span data-ttu-id="cf51e-844">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-844">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-845">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-845">Az.Network</span></span>
* <span data-ttu-id="cf51e-846">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-846">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="cf51e-847">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-847">New cmdlets</span></span>
        - <span data-ttu-id="cf51e-848">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="cf51e-848">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="cf51e-849">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="cf51e-849">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="cf51e-850">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-850">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-851">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-851">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-852">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-852">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-853">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-853">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="cf51e-854">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="cf51e-854">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="cf51e-855">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="cf51e-855">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="cf51e-856">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="cf51e-856">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="cf51e-857">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-857">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="cf51e-858">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-858">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="cf51e-859">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-859">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="cf51e-860">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="cf51e-860">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="cf51e-861">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-861">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="cf51e-862">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-862">Updated cmdlets</span></span>
        - <span data-ttu-id="cf51e-863">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-863">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="cf51e-864">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-864">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="cf51e-865">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-865">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="cf51e-866">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-866">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="cf51e-867">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-867">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="cf51e-868">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-868">Updated cmdlet:</span></span>
        - <span data-ttu-id="cf51e-869">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-869">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="cf51e-870">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-870">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="cf51e-871">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-871">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="cf51e-872">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-872">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="cf51e-873">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-873">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="cf51e-874">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-874">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-875">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-875">Az.OperationalInsights</span></span>
* <span data-ttu-id="cf51e-876">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-876">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="cf51e-877">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-877">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-878">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-878">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-879">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-879">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="cf51e-880">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-880">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="cf51e-881">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-881">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="cf51e-882">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-882">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="cf51e-883">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-883">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="cf51e-884">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-884">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="cf51e-885">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-885">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="cf51e-886">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-886">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="cf51e-887">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-887">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="cf51e-888">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-888">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-889">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-889">Az.Resources</span></span>
- <span data-ttu-id="cf51e-890">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-890">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="cf51e-891">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-891">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cf51e-892">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cf51e-892">Az.ServiceBus</span></span>
* <span data-ttu-id="cf51e-893">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="cf51e-893">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="cf51e-894">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-894">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-895">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-895">Az.Sql</span></span>
* <span data-ttu-id="cf51e-896">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-896">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="cf51e-897">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-897">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="cf51e-898">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-898">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-899">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-899">Az.Storage</span></span>
* <span data-ttu-id="cf51e-900">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-900">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="cf51e-901">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="cf51e-901">Az.StorageSync</span></span>
* <span data-ttu-id="cf51e-902">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-902">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="cf51e-903">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-903">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-904">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-904">Az.Websites</span></span>
* <span data-ttu-id="cf51e-905">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-905">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="cf51e-906">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-906">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="cf51e-907">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-907">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="cf51e-908">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-908">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-909">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-909">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-910">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-910">Add support for profile cmdlets</span></span>
* <span data-ttu-id="cf51e-911">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-911">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="cf51e-912">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-912">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="cf51e-913">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="cf51e-913">Az.Advisor</span></span>
* <span data-ttu-id="cf51e-914">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-914">GA release of Az.Advisor</span></span>
* <span data-ttu-id="cf51e-915">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-915">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="cf51e-916">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-916">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-917">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="cf51e-917">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="cf51e-918">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="cf51e-918">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="cf51e-919">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-919">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="cf51e-920">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-920">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="cf51e-921">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-921">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="cf51e-922">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="cf51e-922">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="cf51e-923">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-923">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-924">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-924">Az.Automation</span></span>
* <span data-ttu-id="cf51e-925">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-925">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-926">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-926">Az.Compute</span></span>
* <span data-ttu-id="cf51e-927">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-927">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-928">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-928">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-929">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-929">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cf51e-930">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cf51e-930">Az.EventGrid</span></span>
* <span data-ttu-id="cf51e-931">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-931">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-932">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-932">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-933">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-933">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-934">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-934">Az.Network</span></span>
* <span data-ttu-id="cf51e-935">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-935">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="cf51e-936">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-936">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cf51e-937">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-937">Az.PolicyInsights</span></span>
* <span data-ttu-id="cf51e-938">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-938">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="cf51e-939">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="cf51e-939">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-940">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-940">Az.OperationalInsights</span></span>
* <span data-ttu-id="cf51e-941">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-941">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-942">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-942">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-943">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-943">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-944">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-944">Az.Resources</span></span>
    - <span data-ttu-id="cf51e-945">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-945">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="cf51e-946">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-946">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="cf51e-947">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-947">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="cf51e-948">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-948">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cf51e-949">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cf51e-949">Az.ServiceBus</span></span>
* <span data-ttu-id="cf51e-950">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="cf51e-950">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-951">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-951">Az.Sql</span></span>
* <span data-ttu-id="cf51e-952">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-952">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="cf51e-953">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-953">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="cf51e-954">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="cf51e-954">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="cf51e-955">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="cf51e-955">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="cf51e-956">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="cf51e-956">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="cf51e-957">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="cf51e-957">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="cf51e-958">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="cf51e-958">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="cf51e-959">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="cf51e-959">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="cf51e-960">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-960">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-961">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-961">Az.Storage</span></span>
* <span data-ttu-id="cf51e-962">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-962">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="cf51e-963">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cf51e-963">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="cf51e-964">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-964">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="cf51e-965">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="cf51e-965">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="cf51e-966">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-966">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="cf51e-967">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-967">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="cf51e-968">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-968">Set-AzStorageAccount</span></span>
* <span data-ttu-id="cf51e-969">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-969">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="cf51e-970">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="cf51e-970">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="cf51e-971">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="cf51e-971">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="cf51e-972">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="cf51e-972">Az.StorageSync</span></span>
* <span data-ttu-id="cf51e-973">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-973">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="cf51e-974">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-974">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-975">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-975">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-976">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-976">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="cf51e-977">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="cf51e-977">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="cf51e-978">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-978">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="cf51e-979">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="cf51e-979">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="cf51e-980">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="cf51e-980">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-981">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-981">Az.Compute</span></span>
* <span data-ttu-id="cf51e-982">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-982">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="cf51e-983">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-983">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="cf51e-984">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="cf51e-984">Az.Dns</span></span>
* <span data-ttu-id="cf51e-985">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-985">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cf51e-986">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cf51e-986">Az.EventGrid</span></span>
* <span data-ttu-id="cf51e-987">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-987">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="cf51e-988">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-988">New cmdlets:</span></span>
    - <span data-ttu-id="cf51e-989">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="cf51e-989">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="cf51e-990">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-990">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="cf51e-991">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="cf51e-991">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="cf51e-992">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-992">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="cf51e-993">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="cf51e-993">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="cf51e-994">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-994">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="cf51e-995">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="cf51e-995">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="cf51e-996">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-996">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="cf51e-997">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="cf51e-997">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="cf51e-998">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-998">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="cf51e-999">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="cf51e-999">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="cf51e-1000">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1000">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="cf51e-1001">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="cf51e-1001">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="cf51e-1002">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1002">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="cf51e-1003">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1003">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="cf51e-1004">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1004">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="cf51e-1005">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1005">Updated cmdlets:</span></span>
    - <span data-ttu-id="cf51e-1006">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1006">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="cf51e-1007">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1007">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="cf51e-1008">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1008">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="cf51e-1009">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1009">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="cf51e-1010">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1010">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="cf51e-1011">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="cf51e-1011">Event subscription expiration date,</span></span>
            - <span data-ttu-id="cf51e-1012">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="cf51e-1012">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="cf51e-1013">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1013">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="cf51e-1014">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1014">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="cf51e-1015">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1015">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="cf51e-1016">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1016">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="cf51e-1017">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="cf51e-1017">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="cf51e-1018">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1018">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="cf51e-1019">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1019">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="cf51e-1020">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1020">Az.FrontDoor</span></span>
* <span data-ttu-id="cf51e-1021">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="cf51e-1021">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="cf51e-1022">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1022">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="cf51e-1023">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="cf51e-1023">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="cf51e-1024">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1024">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1025">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1025">Az.Network</span></span>
* <span data-ttu-id="cf51e-1026">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1026">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="cf51e-1027">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1027">New cmdlets</span></span>
        - <span data-ttu-id="cf51e-1028">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="cf51e-1028">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="cf51e-1029">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1029">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="cf51e-1030">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1030">New cmdlets</span></span> 
        - <span data-ttu-id="cf51e-1031">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="cf51e-1031">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="cf51e-1032">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1032">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="cf51e-1033">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1033">New cmdlets</span></span> 
        - <span data-ttu-id="cf51e-1034">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="cf51e-1034">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="cf51e-1035">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="cf51e-1035">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="cf51e-1036">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="cf51e-1036">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="cf51e-1037">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-1037">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="cf51e-1038">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-1038">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="cf51e-1039">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1039">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="cf51e-1040">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1040">New cmdlets</span></span>
        - <span data-ttu-id="cf51e-1041">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="cf51e-1041">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="cf51e-1042">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="cf51e-1042">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="cf51e-1043">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="cf51e-1043">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="cf51e-1044">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="cf51e-1044">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="cf51e-1045">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="cf51e-1045">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="cf51e-1046">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1046">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="cf51e-1047">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1047">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="cf51e-1048">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1048">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="cf51e-1049">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1049">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="cf51e-1050">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1050">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="cf51e-1051">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1051">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="cf51e-1052">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1052">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="cf51e-1053">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1053">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="cf51e-1054">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1054">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="cf51e-1055">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1055">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="cf51e-1056">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1056">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="cf51e-1057">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1057">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="cf51e-1058">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1058">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="cf51e-1059">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1059">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="cf51e-1060">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1060">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="cf51e-1061">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1061">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="cf51e-1062">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="cf51e-1062">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="cf51e-1063">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1063">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="cf51e-1064">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1064">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="cf51e-1065">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1065">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="cf51e-1066">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1066">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="cf51e-1067">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1067">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-1068">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1068">Az.OperationalInsights</span></span>
* <span data-ttu-id="cf51e-1069">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1069">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1070">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1070">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1071">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1071">Support for additional Template Export options</span></span>
    - <span data-ttu-id="cf51e-1072">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1072">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="cf51e-1073">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1073">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="cf51e-1074">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1074">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-1075">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1075">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-1076">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1076">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1077">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1077">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1078">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1078">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="cf51e-1079">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1079">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="cf51e-1080">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1080">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="cf51e-1081">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="cf51e-1081">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="cf51e-1082">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="cf51e-1082">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="cf51e-1083">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="cf51e-1083">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="cf51e-1084">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="cf51e-1084">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="cf51e-1085">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="cf51e-1085">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1086">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1086">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1087">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1087">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="cf51e-1088">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-1088">New-AzStorageAccount</span></span>
* <span data-ttu-id="cf51e-1089">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1089">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="cf51e-1090">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1090">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1091">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1091">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1092">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1092">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="cf51e-1093">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1093">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="cf51e-1094">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1094">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="cf51e-1095">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-1095">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-1096">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1096">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1097">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1097">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1098">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1098">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="cf51e-1099">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="cf51e-1099">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-1100">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-1100">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-1101">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1101">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="cf51e-1102">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1102">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1103">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1103">Az.Network</span></span>
* <span data-ttu-id="cf51e-1104">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1104">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="cf51e-1105">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1105">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cf51e-1106">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1106">Az.PolicyInsights</span></span>
* <span data-ttu-id="cf51e-1107">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1107">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1108">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1108">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-1109">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1109">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cf51e-1110">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cf51e-1110">Az.ServiceBus</span></span>
* <span data-ttu-id="cf51e-1111">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1111">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-1112">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1112">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-1113">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1113">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="cf51e-1114">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1114">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1115">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1115">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1116">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1116">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="cf51e-1117">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="cf51e-1117">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="cf51e-1118">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1118">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="cf51e-1119">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1119">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1120">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1120">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1121">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1121">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="cf51e-1122">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1122">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="cf51e-1123">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-1123">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-1124">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1124">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="cf51e-1125">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1125">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="cf51e-1126">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1126">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="cf51e-1127">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1127">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="cf51e-1128">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1128">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="cf51e-1129">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1129">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="cf51e-1130">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1130">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="cf51e-1131">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1131">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="cf51e-1132">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1132">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="cf51e-1133">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1133">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="cf51e-1134">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1134">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="cf51e-1135">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1135">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="cf51e-1136">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1136">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="cf51e-1137">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1137">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="cf51e-1138">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1138">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="cf51e-1139">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1139">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="cf51e-1140">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1140">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="cf51e-1141">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1141">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="cf51e-1142">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1142">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="cf51e-1143">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="cf51e-1143">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="cf51e-1144">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1144">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="cf51e-1145">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1145">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="cf51e-1146">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1146">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="cf51e-1147">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1147">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="cf51e-1148">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1148">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="cf51e-1149">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1149">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="cf51e-1150">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1150">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="cf51e-1151">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1151">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="cf51e-1152">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1152">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="cf51e-1153">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1153">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="cf51e-1154">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1154">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="cf51e-1155">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="cf51e-1155">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="cf51e-1156">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1156">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="cf51e-1157">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1157">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="cf51e-1158">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="cf51e-1158">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="cf51e-1159">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1159">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="cf51e-1160">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1160">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="cf51e-1161">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1161">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="cf51e-1162">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1162">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="cf51e-1163">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1163">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="cf51e-1164">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1164">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="cf51e-1165">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1165">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="cf51e-1166">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1166">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="cf51e-1167">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1167">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="cf51e-1168">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1168">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="cf51e-1169">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1169">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="cf51e-1170">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1170">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="cf51e-1171">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1171">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="cf51e-1172">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1172">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="cf51e-1173">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1173">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="cf51e-1174">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1174">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="cf51e-1175">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1175">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="cf51e-1176">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1176">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="cf51e-1177">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1177">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="cf51e-1178">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1178">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="cf51e-1179">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1179">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="cf51e-1180">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1180">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="cf51e-1181">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1181">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="cf51e-1182">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1182">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="cf51e-1183">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1183">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="cf51e-1184">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1184">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="cf51e-1185">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1185">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="cf51e-1186">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="cf51e-1186">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="cf51e-1187">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1187">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="cf51e-1188">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1188">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="cf51e-1189">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1189">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="cf51e-1190">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="cf51e-1190">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="cf51e-1191">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1191">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="cf51e-1192">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="cf51e-1192">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="cf51e-1193">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1193">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="cf51e-1194">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="cf51e-1194">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="cf51e-1195">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1195">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="cf51e-1196">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1196">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="cf51e-1197">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1197">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="cf51e-1198">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1198">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="cf51e-1199">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1199">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="cf51e-1200">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="cf51e-1200">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-1201">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1201">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1202">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1202">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="cf51e-1203">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="cf51e-1203">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="cf51e-1204">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="cf51e-1204">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="cf51e-1205">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1205">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="cf51e-1206">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="cf51e-1206">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="cf51e-1207">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1207">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="cf51e-1208">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1208">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1209">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1209">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1210">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1210">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="cf51e-1211">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1211">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1212">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1212">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1213">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1213">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-1214">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1214">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-1215">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1215">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1216">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1216">Az.Network</span></span>
* <span data-ttu-id="cf51e-1217">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1217">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="cf51e-1218">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1218">Updated cmdlet:</span></span>
        - <span data-ttu-id="cf51e-1219">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-1219">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="cf51e-1220">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1220">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1221">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1221">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1222">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1222">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1223">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1223">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1224">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1224">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="cf51e-1225">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1225">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1226">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1226">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1227">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1227">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cf51e-1228">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1228">Az.CognitiveServices</span></span>
* <span data-ttu-id="cf51e-1229">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1229">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="cf51e-1230">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1230">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1231">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1231">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1232">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1232">Proximity placement group feature.</span></span>
    - <span data-ttu-id="cf51e-1233">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="cf51e-1233">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="cf51e-1234">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-1234">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="cf51e-1235">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1235">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="cf51e-1236">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1236">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="cf51e-1237">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1237">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="cf51e-1238">重大な変更</span><span class="sxs-lookup"><span data-stu-id="cf51e-1238">Breaking changes</span></span>
    - <span data-ttu-id="cf51e-1239">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1239">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="cf51e-1240">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1240">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="cf51e-1241">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="cf51e-1241">Az.DeploymentManager</span></span>
* <span data-ttu-id="cf51e-1242">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-1242">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="cf51e-1243">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="cf51e-1243">Az.Dns</span></span>
* <span data-ttu-id="cf51e-1244">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="cf51e-1244">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="cf51e-1245">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1245">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="cf51e-1246">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1246">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="cf51e-1247">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1247">Az.FrontDoor</span></span>
* <span data-ttu-id="cf51e-1248">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-1248">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="cf51e-1249">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1249">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="cf51e-1250">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cf51e-1250">Az.HDInsight</span></span>
* <span data-ttu-id="cf51e-1251">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1251">Removed two cmdlets:</span></span>
    - <span data-ttu-id="cf51e-1252">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="cf51e-1252">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="cf51e-1253">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="cf51e-1253">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="cf51e-1254">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1254">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="cf51e-1255">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1255">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="cf51e-1256">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1256">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="cf51e-1257">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1257">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-1258">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1258">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-1259">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="cf51e-1259">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="cf51e-1260">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="cf51e-1260">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="cf51e-1261">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="cf51e-1261">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="cf51e-1262">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="cf51e-1262">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="cf51e-1263">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1263">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="cf51e-1264">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="cf51e-1264">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="cf51e-1265">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="cf51e-1265">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="cf51e-1266">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1266">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="cf51e-1267">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1267">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="cf51e-1268">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1268">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="cf51e-1269">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1269">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="cf51e-1270">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1270">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="cf51e-1271">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="cf51e-1271">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="cf51e-1272">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1272">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1273">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1273">Az.Network</span></span>
* <span data-ttu-id="cf51e-1274">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1274">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="cf51e-1275">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1275">New cmdlets</span></span>
        - <span data-ttu-id="cf51e-1276">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="cf51e-1276">New-AzNatGateway</span></span>
        - <span data-ttu-id="cf51e-1277">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="cf51e-1277">Get-AzNatGateway</span></span>
        - <span data-ttu-id="cf51e-1278">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="cf51e-1278">Set-AzNatGateway</span></span>
        - <span data-ttu-id="cf51e-1279">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="cf51e-1279">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="cf51e-1280">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1280">Updated cmdlets</span></span>
        - <span data-ttu-id="cf51e-1281">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="cf51e-1281">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="cf51e-1282">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="cf51e-1282">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="cf51e-1283">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1283">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="cf51e-1284">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1284">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="cf51e-1285">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1285">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cf51e-1286">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1286">Az.PolicyInsights</span></span>
* <span data-ttu-id="cf51e-1287">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1287">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="cf51e-1288">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1288">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="cf51e-1289">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1289">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1290">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1290">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-1291">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1291">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="cf51e-1292">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1292">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="cf51e-1293">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1293">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="cf51e-1294">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1294">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="cf51e-1295">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1295">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="cf51e-1296">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1296">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="cf51e-1297">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="cf51e-1297">Az.Relay</span></span>
* <span data-ttu-id="cf51e-1298">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1298">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cf51e-1299">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cf51e-1299">Az.ServiceBus</span></span>
* <span data-ttu-id="cf51e-1300">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1300">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1301">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1301">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1302">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="cf51e-1302">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="cf51e-1303">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1303">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="cf51e-1304">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1304">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="cf51e-1305">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-1305">New-AzStorageAccount</span></span>
* <span data-ttu-id="cf51e-1306">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="cf51e-1306">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="cf51e-1307">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-1307">New-AzStorageAccount</span></span>
    - <span data-ttu-id="cf51e-1308">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-1308">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="cf51e-1309">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="cf51e-1309">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1310">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1310">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1311">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="cf51e-1311">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="cf51e-1312">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1312">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="cf51e-1313">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1313">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cf51e-1314">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cf51e-1314">Highlights since the last major release</span></span>
* <span data-ttu-id="cf51e-1315">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="cf51e-1315">General availability of `Az` module</span></span>
* <span data-ttu-id="cf51e-1316">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="cf51e-1316">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cf51e-1317">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="cf51e-1317">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cf51e-1318">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1318">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cf51e-1319">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1319">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cf51e-1320">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1320">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cf51e-1321">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1321">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1322">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1322">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1323">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1323">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="cf51e-1324">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cf51e-1324">Az.Batch</span></span>
* <span data-ttu-id="cf51e-1325">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1325">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cf51e-1326">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-1326">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-1327">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1327">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cf51e-1328">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1328">Az.CognitiveServices</span></span>
* <span data-ttu-id="cf51e-1329">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1329">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1330">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1330">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1331">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1331">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="cf51e-1332">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1332">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cf51e-1333">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1333">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-1334">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-1334">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-1335">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1335">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1336">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1336">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1337">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1337">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cf51e-1338">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cf51e-1338">Az.EventGrid</span></span>
* <span data-ttu-id="cf51e-1339">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1339">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-1340">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-1340">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-1341">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1341">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="cf51e-1342">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="cf51e-1342">Az.HDInsight</span></span>
* <span data-ttu-id="cf51e-1343">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1343">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-1344">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-1344">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-1345">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1345">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-1346">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-1346">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-1347">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1347">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cf51e-1348">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1348">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="cf51e-1349">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cf51e-1349">Az.MachineLearning</span></span>
* <span data-ttu-id="cf51e-1350">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1350">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="cf51e-1351">Az.Media</span><span class="sxs-lookup"><span data-stu-id="cf51e-1351">Az.Media</span></span>
* <span data-ttu-id="cf51e-1352">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1352">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-1353">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1353">Az.Monitor</span></span>
  * <span data-ttu-id="cf51e-1354">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1354">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="cf51e-1355">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="cf51e-1355">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="cf51e-1356">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="cf51e-1356">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="cf51e-1357">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="cf51e-1357">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="cf51e-1358">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="cf51e-1358">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="cf51e-1359">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="cf51e-1359">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="cf51e-1360">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1360">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1361">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1361">Az.Network</span></span>
* <span data-ttu-id="cf51e-1362">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1362">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cf51e-1363">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1363">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="cf51e-1364">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="cf51e-1364">Az.NotificationHubs</span></span>
* <span data-ttu-id="cf51e-1365">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1365">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-1366">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1366">Az.OperationalInsights</span></span>
* <span data-ttu-id="cf51e-1367">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1367">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="cf51e-1368">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="cf51e-1368">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="cf51e-1369">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1369">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1370">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1370">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-1371">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1371">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cf51e-1372">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1372">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="cf51e-1373">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1373">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="cf51e-1374">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1374">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cf51e-1375">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cf51e-1375">Az.RedisCache</span></span>
* <span data-ttu-id="cf51e-1376">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1376">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1377">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1377">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1378">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1378">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1379">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1379">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1380">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="cf51e-1380">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="cf51e-1381">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1381">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cf51e-1382">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1382">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="cf51e-1383">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1383">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="cf51e-1384">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1384">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="cf51e-1385">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1385">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="cf51e-1386">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1386">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1387">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1387">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1388">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1388">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="cf51e-1389">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1389">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="cf51e-1390">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1390">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="cf51e-1391">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1391">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="cf51e-1392">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1392">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cf51e-1393">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cf51e-1393">Highlights since the last major release</span></span>
* <span data-ttu-id="cf51e-1394">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="cf51e-1394">General availability of `Az` module</span></span>
* <span data-ttu-id="cf51e-1395">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="cf51e-1395">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cf51e-1396">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="cf51e-1396">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cf51e-1397">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1397">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cf51e-1398">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1398">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cf51e-1399">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1399">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cf51e-1400">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1400">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1401">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1401">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1402">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1402">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cf51e-1403">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1403">Az.AnalysisServices</span></span>
* <span data-ttu-id="cf51e-1404">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="cf51e-1404">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="cf51e-1405">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1405">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-1406">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1406">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1407">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1407">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="cf51e-1408">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1408">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="cf51e-1409">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1409">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1410">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1410">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1411">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1411">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="cf51e-1412">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1412">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="cf51e-1413">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1413">Az.ContainerInstance</span></span>
* <span data-ttu-id="cf51e-1414">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1414">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-1415">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-1415">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-1416">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1416">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="cf51e-1417">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1417">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1418">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1418">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1419">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1419">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="cf51e-1420">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1420">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="cf51e-1421">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1421">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="cf51e-1422">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="cf51e-1422">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="cf51e-1423">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1423">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="cf51e-1424">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="cf51e-1424">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1425">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1425">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1426">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1426">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1427">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1427">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1428">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="cf51e-1428">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="cf51e-1429">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cf51e-1429">New-AzStorageContext</span></span>
* <span data-ttu-id="cf51e-1430">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1430">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="cf51e-1431">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="cf51e-1431">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="cf51e-1432">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="cf51e-1432">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="cf51e-1433">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1433">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="cf51e-1434">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1434">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="cf51e-1435">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1435">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="cf51e-1436">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-1436">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="cf51e-1437">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-1437">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="cf51e-1438">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-1438">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="cf51e-1439">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="cf51e-1439">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="cf51e-1440">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1440">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="cf51e-1441">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="cf51e-1441">Highlights since the last major release</span></span>
* <span data-ttu-id="cf51e-1442">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="cf51e-1442">General availability of `Az` module</span></span>
* <span data-ttu-id="cf51e-1443">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="cf51e-1443">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="cf51e-1444">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="cf51e-1444">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="cf51e-1445">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1445">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="cf51e-1446">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1446">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cf51e-1447">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1447">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="cf51e-1448">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1448">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-1449">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1449">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1450">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1450">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="cf51e-1451">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="cf51e-1451">Dynamic grouping</span></span>
    * <span data-ttu-id="cf51e-1452">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="cf51e-1452">Pre-Post script</span></span>
    * <span data-ttu-id="cf51e-1453">再起動設定</span><span class="sxs-lookup"><span data-stu-id="cf51e-1453">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1454">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1454">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1455">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1455">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="cf51e-1456">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1456">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-1457">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-1457">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-1458">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1458">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1459">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1459">Az.Network</span></span>
* <span data-ttu-id="cf51e-1460">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1460">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="cf51e-1461">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1461">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1462">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1462">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-1463">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1463">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="cf51e-1464">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1464">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1465">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1465">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1466">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1466">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="cf51e-1467">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1467">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1468">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1468">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1469">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1469">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1470">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1470">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1471">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-1471">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="cf51e-1472">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1472">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cf51e-1473">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1473">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cf51e-1474">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1474">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="cf51e-1475">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="cf51e-1475">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="cf51e-1476">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="cf51e-1476">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="cf51e-1477">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1477">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1478">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1478">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1479">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1479">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="cf51e-1480">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1480">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1481">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1481">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1482">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1482">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="cf51e-1483">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1483">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-1484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1484">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1485">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1485">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="cf51e-1486">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1486">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="cf51e-1487">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1487">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cf51e-1488">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-1488">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-1489">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1489">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1490">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1490">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1491">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1491">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-1492">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-1492">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-1493">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1493">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cf51e-1494">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cf51e-1494">Az.LogicApp</span></span>
* <span data-ttu-id="cf51e-1495">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1495">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1496">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1496">Az.Network</span></span>
* <span data-ttu-id="cf51e-1497">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1497">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1498">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1498">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-1499">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1499">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="cf51e-1500">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1500">SDK Update</span></span>
* <span data-ttu-id="cf51e-1501">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1501">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="cf51e-1502">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1502">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1503">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1503">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1504">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1504">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="cf51e-1505">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="cf51e-1505">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="cf51e-1506">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1506">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="cf51e-1507">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="cf51e-1507">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="cf51e-1508">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1508">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="cf51e-1509">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="cf51e-1509">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1510">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1510">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1511">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1511">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="cf51e-1512">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1512">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1513">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1513">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1514">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1514">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="cf51e-1515">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1515">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="cf51e-1516">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1516">Az.AnalysisServices</span></span>
* <span data-ttu-id="cf51e-1517">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1517">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-1518">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1518">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1519">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1519">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="cf51e-1520">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1520">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="cf51e-1521">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1521">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="cf51e-1522">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1522">Az.CognitiveServices</span></span>
* <span data-ttu-id="cf51e-1523">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1523">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1524">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1524">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1525">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1525">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="cf51e-1526">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1526">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="cf51e-1527">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1527">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="cf51e-1528">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1528">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1529">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1529">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1530">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1530">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="cf51e-1531">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-1531">Az.EventHub</span></span>
* <span data-ttu-id="cf51e-1532">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1532">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-1533">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-1533">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-1534">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1534">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cf51e-1535">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cf51e-1535">Az.LogicApp</span></span>
* <span data-ttu-id="cf51e-1536">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1536">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="cf51e-1537">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1537">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="cf51e-1538">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1538">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="cf51e-1539">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cf51e-1539">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cf51e-1540">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cf51e-1540">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cf51e-1541">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cf51e-1541">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="cf51e-1542">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="cf51e-1542">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="cf51e-1543">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1543">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="cf51e-1544">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf51e-1544">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cf51e-1545">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf51e-1545">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cf51e-1546">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf51e-1546">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="cf51e-1547">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf51e-1547">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="cf51e-1548">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1548">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="cf51e-1549">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1549">Az.Monitor</span></span>
* <span data-ttu-id="cf51e-1550">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1550">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1551">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1551">Az.Network</span></span>
* <span data-ttu-id="cf51e-1552">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1552">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-1553">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1553">Az.OperationalInsights</span></span>
* <span data-ttu-id="cf51e-1554">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1554">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="cf51e-1555">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1555">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="cf51e-1556">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1556">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="cf51e-1557">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1557">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1558">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="cf51e-1558">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cf51e-1559">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="cf51e-1559">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="cf51e-1560">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="cf51e-1560">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="cf51e-1561">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1561">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1562">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1562">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1563">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1563">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="cf51e-1564">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1564">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1565">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1565">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1566">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1566">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="cf51e-1567">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1567">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1568">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1568">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1569">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1569">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cf51e-1570">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1570">Az.AnalysisServices</span></span>
<span data-ttu-id="cf51e-1571">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="cf51e-1571">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1572">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1572">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1573">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1573">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="cf51e-1574">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1574">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="cf51e-1575">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1575">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1576">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1576">Az.RecoveryServices</span></span>
<span data-ttu-id="cf51e-1577">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="cf51e-1577">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1578">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1578">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1579">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1579">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="cf51e-1580">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="cf51e-1580">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="cf51e-1581">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1581">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="cf51e-1582">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="cf51e-1582">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1583">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1583">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1584">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1584">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="cf51e-1585">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1585">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="cf51e-1586">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1586">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="cf51e-1587">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1587">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1588">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1588">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1589">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-1589">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="cf51e-1590">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1590">Az.AnalysisServices</span></span>
* <span data-ttu-id="cf51e-1591">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-1591">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1592">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1592">Az.RecoveryServices</span></span>
* <span data-ttu-id="cf51e-1593">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-1593">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="cf51e-1594">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1594">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1595">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1595">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1596">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1596">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="cf51e-1597">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1597">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cf51e-1598">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1598">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="cf51e-1599">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="cf51e-1599">Az.Aks</span></span>
* <span data-ttu-id="cf51e-1600">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1600">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="cf51e-1601">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1601">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1602">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1602">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="cf51e-1603">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1603">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="cf51e-1604">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="cf51e-1604">Az.Cdn</span></span>
* <span data-ttu-id="cf51e-1605">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1605">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1606">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1606">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1607">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1607">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="cf51e-1608">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1608">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="cf51e-1609">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1609">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="cf51e-1610">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="cf51e-1610">Az.ContainerRegistry</span></span>
* <span data-ttu-id="cf51e-1611">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1611">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="cf51e-1612">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="cf51e-1612">Az.DataFactory</span></span>
* <span data-ttu-id="cf51e-1613">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1613">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1614">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1614">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1615">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="cf51e-1615">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="cf51e-1616">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="cf51e-1616">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="cf51e-1617">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1617">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-1618">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-1618">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-1619">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1619">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="cf51e-1620">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-1620">Az.KeyVault</span></span>
* <span data-ttu-id="cf51e-1621">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1621">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1622">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1622">Az.Network</span></span>
* <span data-ttu-id="cf51e-1623">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1623">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1624">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1624">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1625">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1625">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="cf51e-1626">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1626">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="cf51e-1627">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1627">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="cf51e-1628">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="cf51e-1628">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="cf51e-1629">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="cf51e-1629">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="cf51e-1630">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1630">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="cf51e-1631">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="cf51e-1631">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-1632">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1632">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-1633">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="cf51e-1633">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="cf51e-1634">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1634">Fix some error messages.</span></span>
* <span data-ttu-id="cf51e-1635">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1635">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="cf51e-1636">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1636">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cf51e-1637">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cf51e-1637">Az.SignalR</span></span>
* <span data-ttu-id="cf51e-1638">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1638">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1639">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1639">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1640">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1640">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cf51e-1641">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1641">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="cf51e-1642">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1642">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="cf51e-1643">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-1643">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1644">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1644">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1645">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1645">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cf51e-1646">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="cf51e-1646">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="cf51e-1647">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="cf51e-1647">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="cf51e-1648">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="cf51e-1648">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="cf51e-1649">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="cf51e-1649">Az.TrafficManager</span></span>
* <span data-ttu-id="cf51e-1650">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1650">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1651">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1651">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1652">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1652">Update incorrect online help URLs</span></span>
* <span data-ttu-id="cf51e-1653">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1653">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="cf51e-1654">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="cf51e-1654">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="cf51e-1655">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1655">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="cf51e-1656">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1656">Az.Accounts</span></span>
* <span data-ttu-id="cf51e-1657">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="cf51e-1657">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1658">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1658">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1659">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1659">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="cf51e-1660">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1660">Updated the description of ID in help files</span></span>
* <span data-ttu-id="cf51e-1661">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1661">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1662">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1662">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1663">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1663">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="cf51e-1664">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1664">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="cf51e-1665">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="cf51e-1665">Az.EventGrid</span></span>
* <span data-ttu-id="cf51e-1666">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1666">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="cf51e-1667">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="cf51e-1667">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="cf51e-1668">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1668">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cf51e-1669">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="cf51e-1669">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cf51e-1670">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="cf51e-1670">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cf51e-1671">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="cf51e-1671">Dead letter endpoint.</span></span>
    - <span data-ttu-id="cf51e-1672">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1672">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="cf51e-1673">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="cf51e-1673">Event Time-To-Live,</span></span>
        - <span data-ttu-id="cf51e-1674">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="cf51e-1674">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="cf51e-1675">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="cf51e-1675">Dead letter endpoint.</span></span>
* <span data-ttu-id="cf51e-1676">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1676">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="cf51e-1677">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1677">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="cf51e-1678">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="cf51e-1678">Az.IotHub</span></span>
* <span data-ttu-id="cf51e-1679">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1679">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="cf51e-1680">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="cf51e-1680">Az.LogicApp</span></span>
* <span data-ttu-id="cf51e-1681">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="cf51e-1681">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1682">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1682">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1683">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1683">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="cf51e-1684">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="cf51e-1684">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="cf51e-1685">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1685">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cf51e-1686">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1686">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="cf51e-1687">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1687">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="cf51e-1688">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="cf51e-1688">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="cf51e-1689">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="cf51e-1689">Az.SignalR</span></span>
* <span data-ttu-id="cf51e-1690">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1690">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1691">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1691">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1692">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1692">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="cf51e-1693">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1693">Az.Storage</span></span>
* <span data-ttu-id="cf51e-1694">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1694">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="cf51e-1695">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="cf51e-1695">New-AzStorageContext</span></span>
* <span data-ttu-id="cf51e-1696">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1696">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="cf51e-1697">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="cf51e-1697">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1698">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1698">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1699">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1699">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="cf51e-1700">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1700">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="cf51e-1701">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1701">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="cf51e-1702">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-1702">General</span></span>

- <span data-ttu-id="cf51e-1703">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="cf51e-1703">General Availability of Az Module</span></span>
- <span data-ttu-id="cf51e-1704">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="cf51e-1704">Online help for each module</span></span>
- <span data-ttu-id="cf51e-1705">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1705">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="cf51e-1706">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1706">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="cf51e-1707">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="cf51e-1707">Az.Accounts</span></span>
- <span data-ttu-id="cf51e-1708">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1708">Changed from Az.Profile</span></span>
- <span data-ttu-id="cf51e-1709">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1709">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cf51e-1710">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-1710">Az.ApiManagement</span></span>
- <span data-ttu-id="cf51e-1711">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="cf51e-1711">Fixes for #7002</span></span>
- <span data-ttu-id="cf51e-1712">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1712">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="cf51e-1713">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="cf51e-1713">Az.Batch</span></span>
- <span data-ttu-id="cf51e-1714">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1714">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="cf51e-1715">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1715">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="cf51e-1716">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1716">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="cf51e-1717">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="cf51e-1717">Az.Billing</span></span>
- <span data-ttu-id="cf51e-1718">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1718">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="cf51e-1719">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1719">Az.CognitivServices</span></span>
- <span data-ttu-id="cf51e-1720">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1720">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="cf51e-1721">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1721">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cf51e-1722">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1722">Az.ContainerInstance</span></span>
- <span data-ttu-id="cf51e-1723">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1723">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="cf51e-1724">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="cf51e-1724">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="cf51e-1725">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1725">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1726">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1726">Az.DataLakeStore</span></span>
- <span data-ttu-id="cf51e-1727">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1727">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="cf51e-1728">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1728">Az.Monitor</span></span>
- <span data-ttu-id="cf51e-1729">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1729">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="cf51e-1730">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="cf51e-1730">Az.KeyVault</span></span>
- <span data-ttu-id="cf51e-1731">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1731">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="cf51e-1732">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="cf51e-1732">Az.MachineLearning</span></span>
- <span data-ttu-id="cf51e-1733">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1733">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="cf51e-1734">Az.Media</span><span class="sxs-lookup"><span data-stu-id="cf51e-1734">Az.Media</span></span>
- <span data-ttu-id="cf51e-1735">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1735">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cf51e-1736">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1736">Az.Network</span></span>
<span data-ttu-id="cf51e-1737">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1737">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="cf51e-1738">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-1738">New cmdlets added:</span></span>
        - <span data-ttu-id="cf51e-1739">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-1739">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cf51e-1740">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-1740">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cf51e-1741">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-1741">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cf51e-1742">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-1742">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cf51e-1743">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-1743">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="cf51e-1744">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1744">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="cf51e-1745">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="cf51e-1745">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="cf51e-1746">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="cf51e-1746">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="cf51e-1747">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1747">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="cf51e-1748">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="cf51e-1748">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="cf51e-1749">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1749">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cf51e-1750">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="cf51e-1750">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="cf51e-1751">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-1751">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="cf51e-1752">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-1752">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="cf51e-1753">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1753">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="cf51e-1754">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1754">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="cf51e-1755">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cf51e-1755">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cf51e-1756">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cf51e-1756">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="cf51e-1757">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="cf51e-1757">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="cf51e-1758">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1758">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="cf51e-1759">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1759">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="cf51e-1760">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1760">Az.OperationalInsights</span></span>
- <span data-ttu-id="cf51e-1761">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1761">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="cf51e-1762">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1762">Az.Profile</span></span>
- <span data-ttu-id="cf51e-1763">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1763">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1764">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1764">Az.RecoveryServices</span></span>
- <span data-ttu-id="cf51e-1765">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1765">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="cf51e-1766">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1766">Az.Resources</span></span>
- <span data-ttu-id="cf51e-1767">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1767">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cf51e-1768">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1768">Az.ServiceFabric</span></span>
- <span data-ttu-id="cf51e-1769">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="cf51e-1769">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="cf51e-1770">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1770">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="cf51e-1771">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="cf51e-1771">Az.SIgnalR</span></span>
- <span data-ttu-id="cf51e-1772">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="cf51e-1772">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="cf51e-1773">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1773">Az.Sql</span></span>
- <span data-ttu-id="cf51e-1774">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1774">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="cf51e-1775">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1775">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="cf51e-1776">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1776">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="cf51e-1777">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1777">Az.Storage</span></span>
- <span data-ttu-id="cf51e-1778">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1778">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cf51e-1779">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1779">Az.Websites</span></span>
- <span data-ttu-id="cf51e-1780">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="cf51e-1780">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="cf51e-1781">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1781">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="cf51e-1782">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-1782">General</span></span>

* <span data-ttu-id="cf51e-1783">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="cf51e-1783">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="cf51e-1784">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1784">Az.Compute</span></span>

* <span data-ttu-id="cf51e-1785">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1785">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1786">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1786">Az.DataLakeStore</span></span>

* <span data-ttu-id="cf51e-1787">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1787">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="cf51e-1788">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="cf51e-1788">Az.FrontDoor</span></span>

* <span data-ttu-id="cf51e-1789">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1789">Fixed some broken links</span></span>
    - <span data-ttu-id="cf51e-1790">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1790">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="cf51e-1791">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1791">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="cf51e-1792">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1792">Az.RecoveryServices</span></span>

* <span data-ttu-id="cf51e-1793">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1793">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="cf51e-1794">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1794">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="cf51e-1795">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1795">Az.Resources</span></span>

* <span data-ttu-id="cf51e-1796">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1796">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="cf51e-1797">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1797">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="cf51e-1798">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1798">Az.Sql</span></span>

* <span data-ttu-id="cf51e-1799">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="cf51e-1799">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="cf51e-1800">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1800">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="cf51e-1801">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1801">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="cf51e-1802">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1802">Az.Storage</span></span>

* <span data-ttu-id="cf51e-1803">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1803">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="cf51e-1804">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1804">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="cf51e-1805">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1805">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cf51e-1806">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="cf51e-1806">Support Static Website configuration</span></span>
    - <span data-ttu-id="cf51e-1807">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cf51e-1807">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="cf51e-1808">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="cf51e-1808">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="cf51e-1809">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1809">Az.Websites</span></span>

* <span data-ttu-id="cf51e-1810">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="cf51e-1810">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="cf51e-1811">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1811">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="cf51e-1812">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1812">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="cf51e-1813">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1813">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="cf51e-1814">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="cf51e-1814">Az.ApiManagement</span></span>
* <span data-ttu-id="cf51e-1815">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1815">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="cf51e-1816">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="cf51e-1816">Az.Automation</span></span>
* <span data-ttu-id="cf51e-1817">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="cf51e-1817">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="cf51e-1818">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1818">Added Update Management cmdlets</span></span>
* <span data-ttu-id="cf51e-1819">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1819">Added Source Control cmdlets</span></span>
* <span data-ttu-id="cf51e-1820">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1820">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="cf51e-1821">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1821">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="cf51e-1822">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1822">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1823">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1823">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="cf51e-1824">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1824">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="cf51e-1825">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1825">Az.ContainerInstance</span></span>
* <span data-ttu-id="cf51e-1826">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1826">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="cf51e-1827">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="cf51e-1827">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="cf51e-1828">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1828">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="cf51e-1829">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1829">Az.Network</span></span>
* <span data-ttu-id="cf51e-1830">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1830">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="cf51e-1831">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1831">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="cf51e-1832">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1832">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="cf51e-1833">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1833">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="cf51e-1834">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="cf51e-1834">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="cf51e-1835">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1835">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="cf51e-1836">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1836">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="cf51e-1837">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="cf51e-1837">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="cf51e-1838">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1838">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="cf51e-1839">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1839">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="cf51e-1840">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="cf51e-1840">Az.Relay</span></span>
* <span data-ttu-id="cf51e-1841">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="cf51e-1841">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="cf51e-1842">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1842">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1843">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1843">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="cf51e-1844">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1844">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="cf51e-1845">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="cf51e-1845">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="cf51e-1846">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1846">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-1847">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1847">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="cf51e-1848">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1848">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1849">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1849">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="cf51e-1850">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1850">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cf51e-1851">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1851">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cf51e-1852">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1852">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cf51e-1853">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="cf51e-1853">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="cf51e-1854">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cf51e-1854">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cf51e-1855">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cf51e-1855">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cf51e-1856">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cf51e-1856">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="cf51e-1857">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="cf51e-1857">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="cf51e-1858">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1858">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="cf51e-1859">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1859">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="cf51e-1860">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1860">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="cf51e-1861">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="cf51e-1861">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cf51e-1862">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="cf51e-1862">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="cf51e-1863">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="cf51e-1863">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="cf51e-1864">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="cf51e-1864">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="cf51e-1865">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1865">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="cf51e-1866">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1866">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="cf51e-1867">全般</span><span class="sxs-lookup"><span data-stu-id="cf51e-1867">General</span></span>
* <span data-ttu-id="cf51e-1868">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="cf51e-1868">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="cf51e-1869">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1869">Az.Profile</span></span>
* <span data-ttu-id="cf51e-1870">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1870">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="cf51e-1871">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1871">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="cf51e-1872">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1872">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="cf51e-1873">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1873">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="cf51e-1874">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1874">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="cf51e-1875">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1875">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="cf51e-1876">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1876">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="cf51e-1877">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1877">Az.CognitiveServices</span></span>
* <span data-ttu-id="cf51e-1878">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1878">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1879">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1879">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1880">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1880">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="cf51e-1881">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="cf51e-1881">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="cf51e-1882">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1882">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1883">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1883">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1884">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1884">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="cf51e-1885">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1885">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="cf51e-1886">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1886">Az.Insights</span></span>
* <span data-ttu-id="cf51e-1887">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1887">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="cf51e-1888">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1888">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="cf51e-1889">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1889">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="cf51e-1890">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1890">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1891">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1891">Az.Network</span></span>
* <span data-ttu-id="cf51e-1892">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="cf51e-1892">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="cf51e-1893">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-1893">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="cf51e-1894">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-1894">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="cf51e-1895">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cf51e-1895">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="cf51e-1896">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-1896">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="cf51e-1897">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="cf51e-1897">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="cf51e-1898">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="cf51e-1898">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="cf51e-1899">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="cf51e-1899">Az.PolicyInsights</span></span>
* <span data-ttu-id="cf51e-1900">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1900">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1901">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1901">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1902">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1902">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="cf51e-1903">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1903">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="cf51e-1904">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="cf51e-1904">Az.ServiceBus</span></span>
* <span data-ttu-id="cf51e-1905">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1905">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="cf51e-1906">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="cf51e-1906">Az.ServiceFabric</span></span>
* <span data-ttu-id="cf51e-1907">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1907">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="cf51e-1908">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1908">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="cf51e-1909">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1909">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="cf51e-1910">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1910">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="cf51e-1911">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1911">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="cf51e-1912">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1912">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="cf51e-1913">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1913">Az.Profile</span></span>
* <span data-ttu-id="cf51e-1914">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1914">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="cf51e-1915">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1915">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1916">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1916">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1917">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1917">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="cf51e-1918">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1918">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="cf51e-1919">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="cf51e-1919">Az.DataLakeStore</span></span>
* <span data-ttu-id="cf51e-1920">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1920">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="cf51e-1921">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1921">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="cf51e-1922">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1922">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cf51e-1923">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1923">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="cf51e-1924">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1924">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1925">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1925">Az.Network</span></span>
* <span data-ttu-id="cf51e-1926">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1926">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="cf51e-1927">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1927">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1928">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1928">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1929">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1929">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="cf51e-1930">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1930">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="cf51e-1931">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1931">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="cf51e-1932">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1932">Azure.Storage</span></span>
* <span data-ttu-id="cf51e-1933">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1933">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="cf51e-1934">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1934">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="cf51e-1935">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="cf51e-1935">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="cf51e-1936">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1936">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="cf51e-1937">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="cf51e-1937">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="cf51e-1938">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="cf51e-1938">Az.CognitiveServices</span></span>
* <span data-ttu-id="cf51e-1939">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1939">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="cf51e-1940">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="cf51e-1940">Az.Compute</span></span>
* <span data-ttu-id="cf51e-1941">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1941">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="cf51e-1942">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1942">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="cf51e-1943">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1943">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="cf51e-1944">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="cf51e-1944">Az.DataFactoryV2</span></span>
* <span data-ttu-id="cf51e-1945">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1945">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="cf51e-1946">Az.Network</span><span class="sxs-lookup"><span data-stu-id="cf51e-1946">Az.Network</span></span>
* <span data-ttu-id="cf51e-1947">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1947">Added NetworkProfile functionality.</span></span> <span data-ttu-id="cf51e-1948">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="cf51e-1948">new cmdlets added</span></span>
    - <span data-ttu-id="cf51e-1949">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1949">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="cf51e-1950">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1950">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="cf51e-1951">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1951">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="cf51e-1952">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="cf51e-1952">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="cf51e-1953">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-1953">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="cf51e-1954">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="cf51e-1954">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="cf51e-1955">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1955">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="cf51e-1956">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1956">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="cf51e-1957">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1957">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="cf51e-1958">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="cf51e-1958">Az.RedisCache</span></span>
* <span data-ttu-id="cf51e-1959">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="cf51e-1959">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="cf51e-1960">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1960">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="cf51e-1961">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="cf51e-1961">Az.Resources</span></span>
* <span data-ttu-id="cf51e-1962">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1962">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="cf51e-1963">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1963">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="cf51e-1964">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="cf51e-1964">Az.Sql</span></span>
* <span data-ttu-id="cf51e-1965">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="cf51e-1965">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="cf51e-1966">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="cf51e-1966">Az.Websites</span></span>
* <span data-ttu-id="cf51e-1967">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1967">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="cf51e-1968">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="cf51e-1968">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="cf51e-1969">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="cf51e-1969">0.2.0 - September 2018</span></span>
 <span data-ttu-id="cf51e-1970">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="cf51e-1970">Initial Release</span></span>
