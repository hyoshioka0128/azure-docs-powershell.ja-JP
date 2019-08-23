---
ms.openlocfilehash: 77cb28e47d8dddcf3936edff23f794de3b78442b
ms.sourcegitcommit: b02cbcd00748a4a9a4790a5fba229ce53c3bf973
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/09/2019
ms.locfileid: "68861186"
---
## <a name="250---july-2019"></a><span data-ttu-id="8d934-101">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8d934-101">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-102">Az.Accounts</span></span>
* <span data-ttu-id="8d934-103">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-103">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="8d934-104">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-104">Az.ApplicationInsights</span></span>
* <span data-ttu-id="8d934-105">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-105">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span> 

#### <a name="azautomation"></a><span data-ttu-id="8d934-106">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-106">Az.Automation</span></span>
* <span data-ttu-id="8d934-107">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-107">Fix typo in resource string</span></span> 

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d934-108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d934-108">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d934-109">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-109">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-110">Az.Compute</span></span>
* <span data-ttu-id="8d934-111">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-111">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8d934-112">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8d934-112">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8d934-113">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-113">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="8d934-114">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="8d934-114">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d934-115">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d934-115">Az.DataFactory</span></span>
* <span data-ttu-id="8d934-116">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-116">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="8d934-117">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-117">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d934-118">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d934-118">Az.EventHub</span></span>
* <span data-ttu-id="8d934-119">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8d934-119">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8d934-120">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-120">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d934-121">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d934-121">Az.KeyVault</span></span>
* <span data-ttu-id="8d934-122">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-122">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d934-123">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d934-123">Az.LogicApp</span></span>
* <span data-ttu-id="8d934-124">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-124">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="8d934-125">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-125">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="8d934-126">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="8d934-126">Az.ManagedServices</span></span>
* <span data-ttu-id="8d934-127">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-127">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-128">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-128">Az.Network</span></span>
* <span data-ttu-id="8d934-129">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-129">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="8d934-130">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-130">New cmdlets</span></span>
        - <span data-ttu-id="8d934-131">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d934-131">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d934-132">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d934-132">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d934-133">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d934-133">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d934-134">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d934-134">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d934-135">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d934-135">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d934-136">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d934-136">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="8d934-137">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="8d934-137">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="8d934-138">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d934-138">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="8d934-139">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="8d934-139">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="8d934-140">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-140">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="8d934-141">このサブネット内のプライベート エンドポイントでネットワーク ポリシーの適用を有効または無効にすることを示す省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-141">Added optional parameter -PrivateEndpointNetworkPoliciesFlag to indicate that enable or disable apply network policies on pivate endpoint in this subnet.</span></span>
        - <span data-ttu-id="8d934-142">このサブネット内のプライベート リンク サービスでネットワーク ポリシーの適用を有効または無効にすることを示す省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-142">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag to indicate that enable or disable apply network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="8d934-143">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="8d934-143">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="8d934-144">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="8d934-144">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="8d934-145">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-145">Updated cmdlets</span></span>
        - <span data-ttu-id="8d934-146">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-146">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8d934-147">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-147">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="8d934-148">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-148">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="8d934-149">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-149">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="8d934-150">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-150">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="8d934-151">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d934-151">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d934-152">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-152">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8d934-153">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-153">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="8d934-154">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-154">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="8d934-155">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="8d934-155">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="8d934-156">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-156">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="8d934-157">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="8d934-157">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d934-158">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-158">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d934-159">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-159">Updated default version for saved searches to be 1.</span></span> 
* <span data-ttu-id="8d934-160">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-160">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-161">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-162">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-162">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8d934-163">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-163">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="8d934-164">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-164">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="8d934-165">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-165">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="8d934-166">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-166">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="8d934-167">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-167">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8d934-168">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-168">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="8d934-169">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-169">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="8d934-170">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-170">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="8d934-171">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-171">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-172">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-172">Az.Resources</span></span>
- <span data-ttu-id="8d934-173">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d934-173">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="8d934-174">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-174">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d934-175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d934-175">Az.ServiceBus</span></span>
* <span data-ttu-id="8d934-176">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="8d934-176">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="8d934-177">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-177">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-178">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-178">Az.Sql</span></span>
* <span data-ttu-id="8d934-179">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-179">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="8d934-180">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-180">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="8d934-181">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-181">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-182">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-182">Az.Storage</span></span>
* <span data-ttu-id="8d934-183">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-183">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d934-184">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d934-184">Az.StorageSync</span></span>
* <span data-ttu-id="8d934-185">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-185">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="8d934-186">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-186">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-187">Az.Websites</span></span>
* <span data-ttu-id="8d934-188">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-188">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="8d934-189">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-189">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="8d934-190">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-190">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="8d934-191">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="8d934-191">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-192">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-192">Az.Accounts</span></span>
* <span data-ttu-id="8d934-193">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8d934-193">Add support for profile cmdlets</span></span>
* <span data-ttu-id="8d934-194">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="8d934-194">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="8d934-195">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="8d934-195">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="8d934-196">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="8d934-196">Az.Advisor</span></span>
* <span data-ttu-id="8d934-197">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="8d934-197">GA release of Az.Advisor</span></span>
* <span data-ttu-id="8d934-198">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8d934-198">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="8d934-199">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d934-199">Az.ApiManagement</span></span>
* <span data-ttu-id="8d934-200">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="8d934-200">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="8d934-201">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="8d934-201">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="8d934-202">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-202">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="8d934-203">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-203">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="8d934-204">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-204">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="8d934-205">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="8d934-205">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="8d934-206">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-206">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-207">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-207">Az.Automation</span></span>
* <span data-ttu-id="8d934-208">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-208">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-209">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-209">Az.Compute</span></span>
* <span data-ttu-id="8d934-210">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="8d934-210">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d934-211">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d934-211">Az.DataFactory</span></span>
* <span data-ttu-id="8d934-212">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="8d934-212">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d934-213">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d934-213">Az.EventGrid</span></span>
* <span data-ttu-id="8d934-214">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-214">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d934-215">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d934-215">Az.IotHub</span></span>
* <span data-ttu-id="8d934-216">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-216">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-217">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-217">Az.Network</span></span>
* <span data-ttu-id="8d934-218">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-218">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="8d934-219">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d934-219">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d934-220">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-220">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d934-221">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-221">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="8d934-222">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="8d934-222">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d934-223">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-223">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d934-224">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-224">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-225">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-225">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-226">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-226">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-227">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-227">Az.Resources</span></span>
    - <span data-ttu-id="8d934-228">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-228">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="8d934-229">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-229">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="8d934-230">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-230">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="8d934-231">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-231">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d934-232">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d934-232">Az.ServiceBus</span></span>
* <span data-ttu-id="8d934-233">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="8d934-233">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-234">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-234">Az.Sql</span></span>
* <span data-ttu-id="8d934-235">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-235">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="8d934-236">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="8d934-236">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="8d934-237">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d934-237">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d934-238">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d934-238">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d934-239">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="8d934-239">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="8d934-240">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d934-240">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8d934-241">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d934-241">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="8d934-242">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="8d934-242">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="8d934-243">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="8d934-243">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-244">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-244">Az.Storage</span></span>
* <span data-ttu-id="8d934-245">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-245">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="8d934-246">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d934-246">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="8d934-247">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-247">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="8d934-248">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="8d934-248">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="8d934-249">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="8d934-249">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="8d934-250">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-250">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="8d934-251">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-251">Set-AzStorageAccount</span></span>
* <span data-ttu-id="8d934-252">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="8d934-252">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="8d934-253">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d934-253">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="8d934-254">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="8d934-254">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="8d934-255">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="8d934-255">Az.StorageSync</span></span>
* <span data-ttu-id="8d934-256">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="8d934-256">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="8d934-257">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8d934-257">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-258">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-258">Az.Accounts</span></span>
* <span data-ttu-id="8d934-259">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-259">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="8d934-260">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="8d934-260">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="8d934-261">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-261">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="8d934-262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="8d934-262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="8d934-263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="8d934-263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-264">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-264">Az.Compute</span></span>
* <span data-ttu-id="8d934-265">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-265">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="8d934-266">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-266">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="8d934-267">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8d934-267">Az.Dns</span></span>
* <span data-ttu-id="8d934-268">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-268">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d934-269">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d934-269">Az.EventGrid</span></span>
* <span data-ttu-id="8d934-270">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-270">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="8d934-271">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d934-271">New cmdlets:</span></span>
    - <span data-ttu-id="8d934-272">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d934-272">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d934-273">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d934-273">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d934-274">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d934-274">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d934-275">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d934-275">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="8d934-276">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="8d934-276">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="8d934-277">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d934-277">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d934-278">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8d934-278">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8d934-279">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="8d934-279">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="8d934-280">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="8d934-280">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="8d934-281">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="8d934-281">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="8d934-282">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8d934-282">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8d934-283">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d934-283">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="8d934-284">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="8d934-284">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="8d934-285">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d934-285">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span> 
    - <span data-ttu-id="8d934-286">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="8d934-286">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="8d934-287">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d934-287">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="8d934-288">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d934-288">Updated cmdlets:</span></span>
    - <span data-ttu-id="8d934-289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8d934-289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="8d934-290">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-290">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8d934-291">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-291">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="8d934-292">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="8d934-292">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="8d934-293">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8d934-293">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="8d934-294">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="8d934-294">Event subscription expiration date,</span></span>
            - <span data-ttu-id="8d934-295">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="8d934-295">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="8d934-296">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-296">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="8d934-297">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="8d934-297">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span> 
    - <span data-ttu-id="8d934-298">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="8d934-298">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="8d934-299">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-299">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="8d934-300">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="8d934-300">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="8d934-301">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-301">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="8d934-302">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-302">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d934-303">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d934-303">Az.FrontDoor</span></span>
* <span data-ttu-id="8d934-304">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="8d934-304">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="8d934-305">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-305">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="8d934-306">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="8d934-306">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="8d934-307">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-307">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-308">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-308">Az.Network</span></span>
* <span data-ttu-id="8d934-309">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-309">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="8d934-310">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-310">New cmdlets</span></span>
        - <span data-ttu-id="8d934-311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="8d934-311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="8d934-312">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-312">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="8d934-313">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-313">New cmdlets</span></span> 
        - <span data-ttu-id="8d934-314">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="8d934-314">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="8d934-315">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-315">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="8d934-316">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-316">New cmdlets</span></span> 
        - <span data-ttu-id="8d934-317">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d934-317">Get-AzPrivateLinkService</span></span> 
        - <span data-ttu-id="8d934-318">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d934-318">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d934-319">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="8d934-319">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="8d934-320">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-320">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="8d934-321">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="8d934-321">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="8d934-322">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-322">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="8d934-323">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-323">New cmdlets</span></span>
        - <span data-ttu-id="8d934-324">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d934-324">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d934-325">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d934-325">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d934-326">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="8d934-326">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="8d934-327">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="8d934-327">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="8d934-328">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="8d934-328">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="8d934-329">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-329">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="8d934-330">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-330">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="8d934-331">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-331">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="8d934-332">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-332">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="8d934-333">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-333">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="8d934-334">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-334">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="8d934-335">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-335">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="8d934-336">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-336">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="8d934-337">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-337">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="8d934-338">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-338">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="8d934-339">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-339">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="8d934-340">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-340">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="8d934-341">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-341">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="8d934-342">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="8d934-342">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="8d934-343">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-343">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="8d934-344">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-344">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="8d934-345">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="8d934-345">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="8d934-346">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="8d934-346">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span> 
* <span data-ttu-id="8d934-347">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-347">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span> 
    - <span data-ttu-id="8d934-348">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-348">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8d934-349">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-349">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="8d934-350">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-350">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d934-351">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-351">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d934-352">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="8d934-352">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-353">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-353">Az.Resources</span></span>
* <span data-ttu-id="8d934-354">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d934-354">Support for additional Template Export options</span></span>
    - <span data-ttu-id="8d934-355">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-355">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8d934-356">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-356">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="8d934-357">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-357">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d934-358">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d934-358">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d934-359">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-359">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-360">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-360">Az.Sql</span></span>
* <span data-ttu-id="8d934-361">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-361">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="8d934-362">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-362">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="8d934-363">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="8d934-363">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="8d934-364">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d934-364">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d934-365">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d934-365">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d934-366">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="8d934-366">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="8d934-367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8d934-367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="8d934-368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="8d934-368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-369">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-369">Az.Storage</span></span>
* <span data-ttu-id="8d934-370">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-370">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="8d934-371">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-371">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d934-372">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="8d934-372">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="8d934-373">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="8d934-373">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-374">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-374">Az.Websites</span></span>
* <span data-ttu-id="8d934-375">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="8d934-375">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="8d934-376">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-376">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="8d934-377">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="8d934-377">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="8d934-378">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d934-378">Az.Cdn</span></span>
* <span data-ttu-id="8d934-379">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-379">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-380">Az.Compute</span></span>
* <span data-ttu-id="8d934-381">操作を開始し、操作が完了する前にすぐに返す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-381">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="8d934-382">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="8d934-382">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d934-383">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d934-383">Az.EventHub</span></span>
* <span data-ttu-id="8d934-384">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-384">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="8d934-385">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-385">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-386">Az.Network</span></span>
* <span data-ttu-id="8d934-387">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-387">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="8d934-388">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-388">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d934-389">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-389">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d934-390">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-390">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-391">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-392">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-392">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d934-393">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d934-393">Az.ServiceBus</span></span>
* <span data-ttu-id="8d934-394">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-394">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d934-395">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d934-395">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d934-396">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-396">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="8d934-397">Service Fabric のコマンドラインの文字の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-397">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-398">Az.Sql</span></span>
* <span data-ttu-id="8d934-399">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-399">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="8d934-400">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="8d934-400">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="8d934-401">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-401">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="8d934-402">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-402">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-403">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-403">Az.Websites</span></span>
* <span data-ttu-id="8d934-404">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-404">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="8d934-405">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8d934-405">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="8d934-406">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d934-406">Az.ApiManagement</span></span>
* <span data-ttu-id="8d934-407">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8d934-407">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="8d934-408">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="8d934-408">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="8d934-409">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="8d934-409">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="8d934-410">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8d934-410">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="8d934-411">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="8d934-411">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="8d934-412">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="8d934-412">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="8d934-413">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="8d934-413">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="8d934-414">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="8d934-414">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="8d934-415">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8d934-415">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="8d934-416">**Get-AzApiManagementCache** -識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="8d934-416">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="8d934-417">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="8d934-417">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="8d934-418">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="8d934-418">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="8d934-419">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="8d934-419">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="8d934-420">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-420">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="8d934-421">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="8d934-421">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="8d934-422">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="8d934-422">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="8d934-423">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="8d934-423">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="8d934-424">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="8d934-424">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="8d934-425">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-425">Created new Cmdlet for generating a User Token.</span></span> 
    - <span data-ttu-id="8d934-426">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="8d934-426">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="8d934-427">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="8d934-427">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="8d934-428">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="8d934-428">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="8d934-429">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="8d934-429">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="8d934-430">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-430">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span> 
    - <span data-ttu-id="8d934-431">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-431">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="8d934-432">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-432">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="8d934-433">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="8d934-433">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="8d934-434">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="8d934-434">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="8d934-435">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-435">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="8d934-436">'PsApiManagement' オブジェクトを入力として取得するためにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-436">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="8d934-437">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-437">Updated the cmdlet to display Error Messages inline</span></span> 
     > <span data-ttu-id="8d934-438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="8d934-438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="8d934-439">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-439">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="8d934-440">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-440">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d934-441">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="8d934-441">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="8d934-442">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8d934-442">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="8d934-443">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8d934-443">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="8d934-444">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-444">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="8d934-445">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-445">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="8d934-446">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-446">Updated cmdlet **New-AzApiManagementApi**</span></span> 
    - <span data-ttu-id="8d934-447">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8d934-447">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8d934-448">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="8d934-448">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="8d934-449">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="8d934-449">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="8d934-450">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-450">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8d934-451">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-451">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="8d934-452">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="8d934-452">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="8d934-453">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="8d934-453">To updated an API into an 'ApiVersionSet'</span></span>    
    - <span data-ttu-id="8d934-454">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-454">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span> 
* <span data-ttu-id="8d934-455">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-455">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="8d934-456">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="8d934-456">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="8d934-457">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="8d934-457">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="8d934-458">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="8d934-458">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="8d934-459">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="8d934-459">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="8d934-460">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-460">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="8d934-461">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="8d934-461">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="8d934-462">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="8d934-462">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="8d934-463">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-463">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8d934-464">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8d934-464">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8d934-465">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8d934-465">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8d934-466">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-466">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8d934-467">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-467">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="8d934-468">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="8d934-468">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="8d934-469">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="8d934-469">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="8d934-470">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-470">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="8d934-471">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-471">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="8d934-472">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="8d934-472">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="8d934-473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="8d934-473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="8d934-474">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="8d934-474">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="8d934-475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="8d934-475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="8d934-476">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8d934-476">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="8d934-477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="8d934-477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="8d934-478">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="8d934-478">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="8d934-479">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="8d934-479">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="8d934-480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="8d934-480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="8d934-481">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="8d934-481">'Get-AzApiManagementCertificate'</span></span> 
    - <span data-ttu-id="8d934-482">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="8d934-482">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="8d934-483">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="8d934-483">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-484">Az.Automation</span></span>
* <span data-ttu-id="8d934-485">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-485">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="8d934-486">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="8d934-486">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="8d934-487">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="8d934-487">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="8d934-488">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-488">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="8d934-489">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="8d934-489">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="8d934-490">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-490">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="8d934-491">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-491">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-492">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-492">Az.Compute</span></span>
* <span data-ttu-id="8d934-493">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-493">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="8d934-494">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="8d934-494">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-495">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-496">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-496">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d934-497">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d934-497">Az.Monitor</span></span>
* <span data-ttu-id="8d934-498">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-498">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-499">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-499">Az.Network</span></span>
* <span data-ttu-id="8d934-500">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-500">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="8d934-501">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="8d934-501">Updated cmdlet:</span></span>
        - <span data-ttu-id="8d934-502">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d934-502">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="8d934-503">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-503">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-504">Az.Resources</span></span>
* <span data-ttu-id="8d934-505">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-505">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-506">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-506">Az.Sql</span></span>
* <span data-ttu-id="8d934-507">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8d934-507">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="8d934-508">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="8d934-508">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-509">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-509">Az.Accounts</span></span>
* <span data-ttu-id="8d934-510">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-510">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d934-511">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d934-511">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d934-512">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="8d934-512">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="8d934-513">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-513">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-514">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-514">Az.Compute</span></span>
* <span data-ttu-id="8d934-515">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="8d934-515">Proximity placement group feature.</span></span>
    - <span data-ttu-id="8d934-516">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="8d934-516">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="8d934-517">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-517">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="8d934-518">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-518">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="8d934-519">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-519">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="8d934-520">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-520">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>       
* <span data-ttu-id="8d934-521">重大な変更</span><span class="sxs-lookup"><span data-stu-id="8d934-521">Breaking changes</span></span>
    - <span data-ttu-id="8d934-522">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8d934-522">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="8d934-523">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="8d934-523">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="8d934-524">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="8d934-524">Az.DeploymentManager</span></span>
* <span data-ttu-id="8d934-525">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8d934-525">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="8d934-526">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="8d934-526">Az.Dns</span></span>
* <span data-ttu-id="8d934-527">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="8d934-527">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="8d934-528">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="8d934-528">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="8d934-529">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-529">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="8d934-530">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d934-530">Az.FrontDoor</span></span>
* <span data-ttu-id="8d934-531">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="8d934-531">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="8d934-532">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="8d934-532">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="8d934-533">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d934-533">Az.HDInsight</span></span>
* <span data-ttu-id="8d934-534">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-534">Removed two cmdlets:</span></span>
    - <span data-ttu-id="8d934-535">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d934-535">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="8d934-536">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="8d934-536">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8d934-537">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-537">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="8d934-538">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-538">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="8d934-539">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="8d934-539">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="8d934-540">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="8d934-540">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d934-541">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d934-541">Az.Monitor</span></span>
* <span data-ttu-id="8d934-542">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="8d934-542">New cmdlets for SQR API (Scheduled Query Rule)</span></span>  
    - <span data-ttu-id="8d934-543">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="8d934-543">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="8d934-544">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="8d934-544">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="8d934-545">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="8d934-545">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="8d934-546">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="8d934-546">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="8d934-547">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="8d934-547">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="8d934-548">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="8d934-548">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="8d934-549">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d934-549">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d934-550">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d934-550">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d934-551">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d934-551">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d934-552">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d934-552">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d934-553">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="8d934-553">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="8d934-554">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="8d934-554">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="8d934-555">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-555">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-556">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-556">Az.Network</span></span>
* <span data-ttu-id="8d934-557">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-557">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="8d934-558">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-558">New cmdlets</span></span>
        - <span data-ttu-id="8d934-559">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d934-559">New-AzNatGateway</span></span>
        - <span data-ttu-id="8d934-560">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d934-560">Get-AzNatGateway</span></span>
        - <span data-ttu-id="8d934-561">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d934-561">Set-AzNatGateway</span></span>
        - <span data-ttu-id="8d934-562">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="8d934-562">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="8d934-563">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-563">Updated cmdlets</span></span>
        - <span data-ttu-id="8d934-564">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8d934-564">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="8d934-565">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="8d934-565">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="8d934-566">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="8d934-566">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="8d934-567">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-567">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="8d934-568">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-568">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d934-569">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-569">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d934-570">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="8d934-570">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="8d934-571">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-571">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="8d934-572">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="8d934-572">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-573">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-573">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-574">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="8d934-574">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="8d934-575">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="8d934-575">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="8d934-576">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="8d934-576">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="8d934-577">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8d934-577">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="8d934-578">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="8d934-578">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="8d934-579">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="8d934-579">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="8d934-580">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8d934-580">Az.Relay</span></span>
* <span data-ttu-id="8d934-581">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-581">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d934-582">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d934-582">Az.ServiceBus</span></span>
* <span data-ttu-id="8d934-583">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-583">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-584">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-584">Az.Storage</span></span>
* <span data-ttu-id="8d934-585">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="8d934-585">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="8d934-586">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="8d934-586">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="8d934-587">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-587">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="8d934-588">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-588">New-AzStorageAccount</span></span>
* <span data-ttu-id="8d934-589">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="8d934-589">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="8d934-590">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-590">New-AzStorageAccount</span></span>
    - <span data-ttu-id="8d934-591">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-591">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="8d934-592">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="8d934-592">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-593">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-593">Az.Websites</span></span>
* <span data-ttu-id="8d934-594">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8d934-594">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="8d934-595">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="8d934-595">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="8d934-596">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8d934-596">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d934-597">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8d934-597">Highlights since the last major release</span></span>
* <span data-ttu-id="8d934-598">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8d934-598">General availability of `Az` module</span></span>
* <span data-ttu-id="8d934-599">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d934-599">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d934-600">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d934-600">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d934-601">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-601">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d934-602">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d934-602">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d934-603">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-603">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d934-604">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-604">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d934-605">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-605">Az.Accounts</span></span>
* <span data-ttu-id="8d934-606">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-606">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="8d934-607">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d934-607">Az.Batch</span></span>
* <span data-ttu-id="8d934-608">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-608">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d934-609">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d934-609">Az.Cdn</span></span>
* <span data-ttu-id="8d934-610">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-610">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d934-611">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d934-611">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d934-612">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-612">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-613">Az.Compute</span></span>
* <span data-ttu-id="8d934-614">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-614">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="8d934-615">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-615">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d934-616">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-616">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d934-617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d934-617">Az.DataFactory</span></span>
* <span data-ttu-id="8d934-618">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-618">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-619">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-619">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-620">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-620">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d934-621">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d934-621">Az.EventGrid</span></span>
* <span data-ttu-id="8d934-622">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-622">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d934-623">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d934-623">Az.EventHub</span></span>
* <span data-ttu-id="8d934-624">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-624">Added new cmdlets for NetworkRuleSet of Namespace</span></span> 

#### <a name="azhdinsight"></a><span data-ttu-id="8d934-625">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="8d934-625">Az.HDInsight</span></span>
* <span data-ttu-id="8d934-626">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-626">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d934-627">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d934-627">Az.IotHub</span></span>
* <span data-ttu-id="8d934-628">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-628">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d934-629">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d934-629">Az.KeyVault</span></span>
* <span data-ttu-id="8d934-630">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-630">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d934-631">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-631">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="8d934-632">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d934-632">Az.MachineLearning</span></span>
* <span data-ttu-id="8d934-633">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-633">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="8d934-634">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8d934-634">Az.Media</span></span>
* <span data-ttu-id="8d934-635">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-635">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d934-636">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d934-636">Az.Monitor</span></span>
  * <span data-ttu-id="8d934-637">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-637">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="8d934-638">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="8d934-638">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="8d934-639">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="8d934-639">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="8d934-640">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d934-640">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8d934-641">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d934-641">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="8d934-642">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="8d934-642">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="8d934-643">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-643">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-644">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-644">Az.Network</span></span>
* <span data-ttu-id="8d934-645">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-645">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d934-646">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-646">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="8d934-647">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="8d934-647">Az.NotificationHubs</span></span>
* <span data-ttu-id="8d934-648">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-648">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d934-649">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-649">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d934-650">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-650">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="8d934-651">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="8d934-651">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="8d934-652">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-652">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-653">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-653">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-654">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-654">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d934-655">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-655">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="8d934-656">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-656">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="8d934-657">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-657">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d934-658">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d934-658">Az.RedisCache</span></span>
* <span data-ttu-id="8d934-659">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-659">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-660">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-660">Az.Resources</span></span>
* <span data-ttu-id="8d934-661">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-661">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-662">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-662">Az.Sql</span></span>
* <span data-ttu-id="8d934-663">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="8d934-663">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="8d934-664">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-664">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d934-665">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-665">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="8d934-666">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="8d934-666">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="8d934-667">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="8d934-667">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="8d934-668">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="8d934-668">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="8d934-669">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-669">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-670">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-670">Az.Websites</span></span>
* <span data-ttu-id="8d934-671">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-671">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="8d934-672">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-672">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="8d934-673">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-673">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="8d934-674">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-674">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="8d934-675">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="8d934-675">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d934-676">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8d934-676">Highlights since the last major release</span></span>
* <span data-ttu-id="8d934-677">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8d934-677">General availability of `Az` module</span></span>
* <span data-ttu-id="8d934-678">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d934-678">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d934-679">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d934-679">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d934-680">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-680">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d934-681">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d934-681">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d934-682">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-682">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d934-683">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-683">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="8d934-684">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-684">Az.Accounts</span></span>
* <span data-ttu-id="8d934-685">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-685">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d934-686">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d934-686">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d934-687">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="8d934-687">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="8d934-688">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="8d934-688">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-689">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-689">Az.Automation</span></span>
* <span data-ttu-id="8d934-690">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-690">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="8d934-691">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-691">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="8d934-692">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-692">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-693">Az.Compute</span></span>
* <span data-ttu-id="8d934-694">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-694">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="8d934-695">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-695">Allow VM creation with galley image from other tenants.</span></span> 

#### <a name="azcontainerinstance"></a><span data-ttu-id="8d934-696">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-696">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d934-697">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-697">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d934-698">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d934-698">Az.DataFactory</span></span>
* <span data-ttu-id="8d934-699">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-699">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="8d934-700">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-700">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-701">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-701">Az.Resources</span></span>
* <span data-ttu-id="8d934-702">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d934-702">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="8d934-703">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d934-703">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="8d934-704">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="8d934-704">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="8d934-705">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8d934-705">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="8d934-706">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-706">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="8d934-707">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="8d934-707">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-708">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-708">Az.Sql</span></span>
* <span data-ttu-id="8d934-709">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="8d934-709">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-710">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-710">Az.Storage</span></span>
* <span data-ttu-id="8d934-711">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="8d934-711">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="8d934-712">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8d934-712">New-AzStorageContext</span></span>
* <span data-ttu-id="8d934-713">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d934-713">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="8d934-714">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8d934-714">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8d934-715">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="8d934-715">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="8d934-716">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d934-716">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="8d934-717">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="8d934-717">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="8d934-718">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d934-718">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="8d934-719">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d934-719">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8d934-720">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="8d934-720">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="8d934-721">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d934-721">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="8d934-722">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="8d934-722">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="8d934-723">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8d934-723">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="8d934-724">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="8d934-724">Highlights since the last major release</span></span>
* <span data-ttu-id="8d934-725">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="8d934-725">General availability of `Az` module</span></span>
* <span data-ttu-id="8d934-726">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="8d934-726">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="8d934-727">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="8d934-727">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="8d934-728">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-728">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="8d934-729">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d934-729">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d934-730">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-730">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="8d934-731">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-731">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-732">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-732">Az.Automation</span></span>
* <span data-ttu-id="8d934-733">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="8d934-733">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="8d934-734">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="8d934-734">Dynamic grouping</span></span>
    * <span data-ttu-id="8d934-735">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="8d934-735">Pre-Post script</span></span>
    * <span data-ttu-id="8d934-736">再起動設定</span><span class="sxs-lookup"><span data-stu-id="8d934-736">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-737">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-737">Az.Compute</span></span>
* <span data-ttu-id="8d934-738">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-738">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="8d934-739">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-739">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d934-740">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d934-740">Az.KeyVault</span></span>
* <span data-ttu-id="8d934-741">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-741">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-742">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-742">Az.Network</span></span>
* <span data-ttu-id="8d934-743">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-743">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="8d934-744">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-744">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-745">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-745">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-746">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-746">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="8d934-747">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-747">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-748">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-748">Az.Resources</span></span>
* <span data-ttu-id="8d934-749">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="8d934-749">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="8d934-750">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-750">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-751">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-751">Az.Sql</span></span>
* <span data-ttu-id="8d934-752">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-752">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-753">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-753">Az.Storage</span></span>
* <span data-ttu-id="8d934-754">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="8d934-754">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="8d934-755">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d934-755">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d934-756">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d934-756">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d934-757">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="8d934-757">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="8d934-758">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="8d934-758">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="8d934-759">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="8d934-759">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="8d934-760">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="8d934-760">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-761">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-761">Az.Websites</span></span>
* <span data-ttu-id="8d934-762">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-762">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span> 

## <a name="150---march-2019"></a><span data-ttu-id="8d934-763">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="8d934-763">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-764">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-764">Az.Accounts</span></span>
* <span data-ttu-id="8d934-765">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-765">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="8d934-766">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-766">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-767">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-767">Az.Automation</span></span>
* <span data-ttu-id="8d934-768">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-768">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="8d934-769">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-769">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="8d934-770">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="8d934-770">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d934-771">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d934-771">Az.Cdn</span></span>
* <span data-ttu-id="8d934-772">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8d934-772">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-773">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-773">Az.Compute</span></span>
* <span data-ttu-id="8d934-774">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-774">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d934-775">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d934-775">Az.DataFactory</span></span>
* <span data-ttu-id="8d934-776">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-776">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d934-777">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d934-777">Az.LogicApp</span></span>
* <span data-ttu-id="8d934-778">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-778">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-779">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-779">Az.Network</span></span>
* <span data-ttu-id="8d934-780">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-780">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-781">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-781">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-782">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-782">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="8d934-783">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="8d934-783">SDK Update</span></span>
* <span data-ttu-id="8d934-784">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d934-784">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="8d934-785">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-785">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-786">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-786">Az.Resources</span></span>
* <span data-ttu-id="8d934-787">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-787">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="8d934-788">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="8d934-788">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="8d934-789">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-789">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="8d934-790">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="8d934-790">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="8d934-791">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-791">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="8d934-792">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="8d934-792">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-793">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-793">Az.Sql</span></span>
* <span data-ttu-id="8d934-794">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-794">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="8d934-795">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-795">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-796">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-796">Az.Storage</span></span>
* <span data-ttu-id="8d934-797">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="8d934-797">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="8d934-798">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8d934-798">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="8d934-799">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d934-799">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d934-800">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="8d934-800">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-801">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-801">Az.Automation</span></span>
* <span data-ttu-id="8d934-802">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-802">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="8d934-803">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-803">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="8d934-804">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="8d934-804">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d934-805">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d934-805">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d934-806">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="8d934-806">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-807">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-807">Az.Compute</span></span>
* <span data-ttu-id="8d934-808">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-808">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="8d934-809">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-809">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="8d934-810">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-810">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="8d934-811">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="8d934-811">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-812">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-812">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-813">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-813">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="8d934-814">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="8d934-814">Az.EventHub</span></span>
* <span data-ttu-id="8d934-815">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-815">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span> 

#### <a name="azkeyvault"></a><span data-ttu-id="8d934-816">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d934-816">Az.KeyVault</span></span>
* <span data-ttu-id="8d934-817">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-817">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d934-818">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d934-818">Az.LogicApp</span></span>
* <span data-ttu-id="8d934-819">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-819">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="8d934-820">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-820">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="8d934-821">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-821">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="8d934-822">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d934-822">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d934-823">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d934-823">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d934-824">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d934-824">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="8d934-825">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="8d934-825">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="8d934-826">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-826">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="8d934-827">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d934-827">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d934-828">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d934-828">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d934-829">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d934-829">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="8d934-830">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d934-830">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="8d934-831">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-831">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="8d934-832">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d934-832">Az.Monitor</span></span>
* <span data-ttu-id="8d934-833">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-833">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-834">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-834">Az.Network</span></span>
* <span data-ttu-id="8d934-835">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-835">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="8d934-836">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-836">Az.OperationalInsights</span></span>
* <span data-ttu-id="8d934-837">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-837">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="8d934-838">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-838">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span> 
    - <span data-ttu-id="8d934-839">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-839">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span> 

#### <a name="azresources"></a><span data-ttu-id="8d934-840">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-840">Az.Resources</span></span>
* <span data-ttu-id="8d934-841">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8d934-841">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8d934-842">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8d934-842">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="8d934-843">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="8d934-843">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="8d934-844">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-844">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-845">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-845">Az.Sql</span></span>
* <span data-ttu-id="8d934-846">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-846">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="8d934-847">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-847">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-848">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-848">Az.Websites</span></span>
* <span data-ttu-id="8d934-849">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-849">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="8d934-850">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="8d934-850">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-851">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-851">Az.Accounts</span></span>
* <span data-ttu-id="8d934-852">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="8d934-852">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d934-853">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d934-853">Az.AnalysisServices</span></span>
<span data-ttu-id="8d934-854">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8d934-854">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-855">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-855">Az.Compute</span></span>
* <span data-ttu-id="8d934-856">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-856">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="8d934-857">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-857">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="8d934-858">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-858">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-859">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-859">Az.RecoveryServices</span></span>
<span data-ttu-id="8d934-860">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="8d934-860">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-861">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-861">Az.Resources</span></span>
* <span data-ttu-id="8d934-862">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-862">Fix tagging for resource groups</span></span> 
    - <span data-ttu-id="8d934-863">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="8d934-863">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="8d934-864">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-864">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span> 
    - <span data-ttu-id="8d934-865">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="8d934-865">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-866">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-866">Az.Sql</span></span>
* <span data-ttu-id="8d934-867">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="8d934-867">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="8d934-868">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-868">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="8d934-869">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-869">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="8d934-870">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8d934-870">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-871">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-871">Az.Accounts</span></span>
* <span data-ttu-id="8d934-872">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="8d934-872">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="8d934-873">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="8d934-873">Az.AnalysisServices</span></span>
* <span data-ttu-id="8d934-874">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8d934-874">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-875">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-875">Az.RecoveryServices</span></span>
* <span data-ttu-id="8d934-876">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="8d934-876">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="8d934-877">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8d934-877">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-878">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-878">Az.Accounts</span></span>
* <span data-ttu-id="8d934-879">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="8d934-879">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="8d934-880">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-880">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d934-881">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-881">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="8d934-882">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="8d934-882">Az.Aks</span></span>
* <span data-ttu-id="8d934-883">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-883">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="8d934-884">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-884">Az.Automation</span></span>
* <span data-ttu-id="8d934-885">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-885">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="8d934-886">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-886">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="8d934-887">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="8d934-887">Az.Cdn</span></span>
* <span data-ttu-id="8d934-888">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-888">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-889">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-889">Az.Compute</span></span>
* <span data-ttu-id="8d934-890">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="8d934-890">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="8d934-891">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="8d934-891">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="8d934-892">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-892">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="8d934-893">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="8d934-893">Az.ContainerRegistry</span></span>
* <span data-ttu-id="8d934-894">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-894">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="8d934-895">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="8d934-895">Az.DataFactory</span></span>
* <span data-ttu-id="8d934-896">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="8d934-896">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-897">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-897">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-898">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="8d934-898">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="8d934-899">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="8d934-899">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="8d934-900">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-900">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d934-901">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d934-901">Az.IotHub</span></span>
* <span data-ttu-id="8d934-902">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="8d934-902">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="8d934-903">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d934-903">Az.KeyVault</span></span>
* <span data-ttu-id="8d934-904">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-904">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-905">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-905">Az.Network</span></span>
* <span data-ttu-id="8d934-906">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-906">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-907">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-907">Az.Resources</span></span>
* <span data-ttu-id="8d934-908">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-908">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="8d934-909">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-909">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="8d934-910">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-910">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="8d934-911">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="8d934-911">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="8d934-912">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="8d934-912">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="8d934-913">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-913">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="8d934-914">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="8d934-914">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d934-915">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d934-915">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d934-916">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="8d934-916">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="8d934-917">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="8d934-917">Fix some error messages.</span></span>
* <span data-ttu-id="8d934-918">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-918">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="8d934-919">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-919">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d934-920">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d934-920">Az.SignalR</span></span>
* <span data-ttu-id="8d934-921">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-921">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-922">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-922">Az.Sql</span></span>
* <span data-ttu-id="8d934-923">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-923">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d934-924">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-924">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="8d934-925">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-925">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="8d934-926">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="8d934-926">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-927">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-927">Az.Storage</span></span>
* <span data-ttu-id="8d934-928">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-928">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d934-929">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="8d934-929">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="8d934-930">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="8d934-930">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="8d934-931">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="8d934-931">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="8d934-932">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="8d934-932">Az.TrafficManager</span></span>
* <span data-ttu-id="8d934-933">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-933">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-934">Az.Websites</span></span>
* <span data-ttu-id="8d934-935">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="8d934-935">Update incorrect online help URLs</span></span>
* <span data-ttu-id="8d934-936">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-936">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="8d934-937">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="8d934-937">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="8d934-938">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="8d934-938">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="8d934-939">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-939">Az.Accounts</span></span>
* <span data-ttu-id="8d934-940">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="8d934-940">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-941">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-941">Az.Compute</span></span>
* <span data-ttu-id="8d934-942">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-942">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="8d934-943">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="8d934-943">Updated the description of ID in help files</span></span>
* <span data-ttu-id="8d934-944">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-944">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-945">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-945">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-946">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-946">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="8d934-947">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-947">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="8d934-948">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="8d934-948">Az.EventGrid</span></span>
* <span data-ttu-id="8d934-949">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-949">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="8d934-950">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="8d934-950">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="8d934-951">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8d934-951">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8d934-952">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8d934-952">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8d934-953">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8d934-953">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8d934-954">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8d934-954">Dead letter endpoint.</span></span>
    - <span data-ttu-id="8d934-955">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="8d934-955">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="8d934-956">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="8d934-956">Event Time-To-Live,</span></span>
        - <span data-ttu-id="8d934-957">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="8d934-957">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="8d934-958">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="8d934-958">Dead letter endpoint.</span></span>
* <span data-ttu-id="8d934-959">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-959">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="8d934-960">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="8d934-960">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="8d934-961">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="8d934-961">Az.IotHub</span></span>
* <span data-ttu-id="8d934-962">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-962">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="8d934-963">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="8d934-963">Az.LogicApp</span></span>
* <span data-ttu-id="8d934-964">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="8d934-964">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-965">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-965">Az.Resources</span></span>
* <span data-ttu-id="8d934-966">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-966">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="8d934-967">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="8d934-967">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="8d934-968">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-968">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8d934-969">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-969">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="8d934-970">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="8d934-970">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="8d934-971">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="8d934-971">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="8d934-972">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="8d934-972">Az.SignalR</span></span>
* <span data-ttu-id="8d934-973">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-973">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-974">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-974">Az.Sql</span></span>
* <span data-ttu-id="8d934-975">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="8d934-975">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="8d934-976">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-976">Az.Storage</span></span>
* <span data-ttu-id="8d934-977">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="8d934-977">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="8d934-978">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="8d934-978">New-AzStorageContext</span></span>
* <span data-ttu-id="8d934-979">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-979">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="8d934-980">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="8d934-980">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-981">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-981">Az.Websites</span></span>
* <span data-ttu-id="8d934-982">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-982">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="8d934-983">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-983">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="8d934-984">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8d934-984">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="8d934-985">全般</span><span class="sxs-lookup"><span data-stu-id="8d934-985">General</span></span>

- <span data-ttu-id="8d934-986">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="8d934-986">General Availability of Az Module</span></span>
- <span data-ttu-id="8d934-987">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="8d934-987">Online help for each module</span></span>
- <span data-ttu-id="8d934-988">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-988">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="8d934-989">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-989">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="8d934-990">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="8d934-990">Az.Accounts</span></span>
- <span data-ttu-id="8d934-991">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-991">Changed from Az.Profile</span></span>
- <span data-ttu-id="8d934-992">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-992">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8d934-993">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d934-993">Az.ApiManagement</span></span>
- <span data-ttu-id="8d934-994">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="8d934-994">Fixes for #7002</span></span>
- <span data-ttu-id="8d934-995">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-995">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="8d934-996">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="8d934-996">Az.Batch</span></span>
- <span data-ttu-id="8d934-997">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-997">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="8d934-998">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-998">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="8d934-999">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-999">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="8d934-1000">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="8d934-1000">Az.Billing</span></span>
- <span data-ttu-id="8d934-1001">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1001">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="8d934-1002">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="8d934-1002">Az.CognitivServices</span></span>
- <span data-ttu-id="8d934-1003">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1003">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="8d934-1004">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1004">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8d934-1005">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-1005">Az.ContainerInstance</span></span>
- <span data-ttu-id="8d934-1006">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1006">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="8d934-1007">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="8d934-1007">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="8d934-1008">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1008">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8d934-1009">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-1009">Az.DataLakeStore</span></span>
- <span data-ttu-id="8d934-1010">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1010">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="8d934-1011">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="8d934-1011">Az.Monitor</span></span>
- <span data-ttu-id="8d934-1012">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1012">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="8d934-1013">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="8d934-1013">Az.KeyVault</span></span>
- <span data-ttu-id="8d934-1014">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1014">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="8d934-1015">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="8d934-1015">Az.MachineLearning</span></span>
- <span data-ttu-id="8d934-1016">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="8d934-1016">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="8d934-1017">Az.Media</span><span class="sxs-lookup"><span data-stu-id="8d934-1017">Az.Media</span></span>
- <span data-ttu-id="8d934-1018">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1018">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8d934-1019">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-1019">Az.Network</span></span>
<span data-ttu-id="8d934-1020">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1020">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="8d934-1021">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8d934-1021">New cmdlets added:</span></span>
        - <span data-ttu-id="8d934-1022">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d934-1022">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d934-1023">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d934-1023">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d934-1024">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d934-1024">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d934-1025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d934-1025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d934-1026">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="8d934-1026">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="8d934-1027">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="8d934-1027">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="8d934-1028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="8d934-1028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="8d934-1029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d934-1029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="8d934-1030">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-1030">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="8d934-1031">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="8d934-1031">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="8d934-1032">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8d934-1032">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8d934-1033">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="8d934-1033">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="8d934-1034">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-1034">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="8d934-1035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-1035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="8d934-1036">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1036">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="8d934-1037">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-1037">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="8d934-1038">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d934-1038">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8d934-1039">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d934-1039">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="8d934-1040">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="8d934-1040">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="8d934-1041">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-1041">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="8d934-1042">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1042">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="8d934-1043">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-1043">Az.OperationalInsights</span></span>
- <span data-ttu-id="8d934-1044">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1044">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="8d934-1045">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d934-1045">Az.Profile</span></span>
- <span data-ttu-id="8d934-1046">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1046">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-1047">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-1047">Az.RecoveryServices</span></span>
- <span data-ttu-id="8d934-1048">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1048">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="8d934-1049">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-1049">Az.Resources</span></span>
- <span data-ttu-id="8d934-1050">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1050">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8d934-1051">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d934-1051">Az.ServiceFabric</span></span>
- <span data-ttu-id="8d934-1052">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="8d934-1052">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="8d934-1053">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1053">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="8d934-1054">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="8d934-1054">Az.SIgnalR</span></span>
- <span data-ttu-id="8d934-1055">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="8d934-1055">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="8d934-1056">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-1056">Az.Sql</span></span>
- <span data-ttu-id="8d934-1057">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1057">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="8d934-1058">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1058">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="8d934-1059">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1059">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="8d934-1060">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-1060">Az.Storage</span></span>
- <span data-ttu-id="8d934-1061">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1061">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8d934-1062">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-1062">Az.Websites</span></span>
- <span data-ttu-id="8d934-1063">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="8d934-1063">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="8d934-1064">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="8d934-1064">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="8d934-1065">全般</span><span class="sxs-lookup"><span data-stu-id="8d934-1065">General</span></span>

* <span data-ttu-id="8d934-1066">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8d934-1066">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="8d934-1067">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-1067">Az.Compute</span></span>

* <span data-ttu-id="8d934-1068">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1068">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="8d934-1069">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-1069">Az.DataLakeStore</span></span>

* <span data-ttu-id="8d934-1070">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1070">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="8d934-1071">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="8d934-1071">Az.FrontDoor</span></span>

* <span data-ttu-id="8d934-1072">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1072">Fixed some broken links</span></span>
    - <span data-ttu-id="8d934-1073">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1073">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="8d934-1074">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1074">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="8d934-1075">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="8d934-1075">Az.RecoveryServices</span></span>

* <span data-ttu-id="8d934-1076">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1076">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="8d934-1077">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1077">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="8d934-1078">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-1078">Az.Resources</span></span>

* <span data-ttu-id="8d934-1079">[https://github.com/Azure/azure-powershell/issues/7679](https://github.com/Azure/azure-powershell/issues/7679 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1079">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="8d934-1080">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1080">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="8d934-1081">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-1081">Az.Sql</span></span>

* <span data-ttu-id="8d934-1082">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="8d934-1082">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="8d934-1083">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1083">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="8d934-1084">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1084">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="8d934-1085">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-1085">Az.Storage</span></span>

* <span data-ttu-id="8d934-1086">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1086">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="8d934-1087">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1087">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="8d934-1088">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8d934-1088">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8d934-1089">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="8d934-1089">Support Static Website configuration</span></span>
    - <span data-ttu-id="8d934-1090">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d934-1090">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="8d934-1091">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="8d934-1091">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="8d934-1092">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-1092">Az.Websites</span></span>

* <span data-ttu-id="8d934-1093">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="8d934-1093">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span> 
    - <span data-ttu-id="8d934-1094">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1094">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="8d934-1095">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="8d934-1095">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="8d934-1096">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8d934-1096">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="8d934-1097">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="8d934-1097">Az.ApiManagement</span></span>
* <span data-ttu-id="8d934-1098">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1098">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="8d934-1099">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="8d934-1099">Az.Automation</span></span>
* <span data-ttu-id="8d934-1100">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="8d934-1100">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="8d934-1101">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1101">Added Update Management cmdlets</span></span>
* <span data-ttu-id="8d934-1102">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1102">Added Source Control cmdlets</span></span>
* <span data-ttu-id="8d934-1103">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1103">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="8d934-1104">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1104">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="8d934-1105">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-1105">Az.Compute</span></span>
* <span data-ttu-id="8d934-1106">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1106">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="8d934-1107">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1107">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="8d934-1108">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-1108">Az.ContainerInstance</span></span>
* <span data-ttu-id="8d934-1109">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1109">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="8d934-1110">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="8d934-1110">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="8d934-1111">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1111">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="8d934-1112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-1112">Az.Network</span></span>
* <span data-ttu-id="8d934-1113">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1113">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="8d934-1114">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1114">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="8d934-1115">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1115">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span> 
* <span data-ttu-id="8d934-1116">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1116">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="8d934-1117">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="8d934-1117">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="8d934-1118">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1118">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="8d934-1119">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1119">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="8d934-1120">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="8d934-1120">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="8d934-1121">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1121">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="8d934-1122">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1122">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="8d934-1123">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="8d934-1123">Az.Relay</span></span>
* <span data-ttu-id="8d934-1124">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="8d934-1124">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="8d934-1125">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-1125">Az.Resources</span></span>
* <span data-ttu-id="8d934-1126">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1126">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="8d934-1127">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1127">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="8d934-1128">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="8d934-1128">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="8d934-1129">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d934-1129">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d934-1130">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1130">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="8d934-1131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-1131">Az.Sql</span></span>
* <span data-ttu-id="8d934-1132">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1132">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="8d934-1133">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-1133">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d934-1134">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-1134">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d934-1135">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-1135">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d934-1136">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="8d934-1136">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="8d934-1137">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d934-1137">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d934-1138">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d934-1138">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d934-1139">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d934-1139">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="8d934-1140">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="8d934-1140">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="8d934-1141">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="8d934-1141">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="8d934-1142">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1142">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="8d934-1143">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1143">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="8d934-1144">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8d934-1144">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8d934-1145">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="8d934-1145">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="8d934-1146">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8d934-1146">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="8d934-1147">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="8d934-1147">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="8d934-1148">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1148">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="8d934-1149">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="8d934-1149">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="8d934-1150">全般</span><span class="sxs-lookup"><span data-stu-id="8d934-1150">General</span></span>
* <span data-ttu-id="8d934-1151">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="8d934-1151">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="8d934-1152">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d934-1152">Az.Profile</span></span>
* <span data-ttu-id="8d934-1153">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1153">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="8d934-1154">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1154">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="8d934-1155">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1155">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="8d934-1156">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1156">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="8d934-1157">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1157">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="8d934-1158">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1158">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="8d934-1159">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1159">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="8d934-1160">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d934-1160">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d934-1161">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1161">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-1162">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-1162">Az.Compute</span></span>
* <span data-ttu-id="8d934-1163">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1163">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="8d934-1164">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="8d934-1164">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="8d934-1165">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1165">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-1166">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-1166">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-1167">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1167">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="8d934-1168">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1168">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="8d934-1169">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="8d934-1169">Az.Insights</span></span>
* <span data-ttu-id="8d934-1170">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1170">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="8d934-1171">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="8d934-1171">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="8d934-1172">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1172">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="8d934-1173">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="8d934-1173">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-1174">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-1174">Az.Network</span></span>
* <span data-ttu-id="8d934-1175">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="8d934-1175">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="8d934-1176">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d934-1176">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="8d934-1177">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="8d934-1177">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="8d934-1178">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8d934-1178">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="8d934-1179">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="8d934-1179">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="8d934-1180">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="8d934-1180">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="8d934-1181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="8d934-1181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="8d934-1182">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="8d934-1182">Az.PolicyInsights</span></span>
* <span data-ttu-id="8d934-1183">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1183">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-1184">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-1184">Az.Resources</span></span>
* <span data-ttu-id="8d934-1185">[https://github.com/Azure/azure-powershell/issues/7402](https://github.com/Azure/azure-powershell/issues/7402 ) を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1185">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="8d934-1186">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1186">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="8d934-1187">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="8d934-1187">Az.ServiceBus</span></span>
* <span data-ttu-id="8d934-1188">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1188">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="8d934-1189">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="8d934-1189">Az.ServiceFabric</span></span>
* <span data-ttu-id="8d934-1190">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1190">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="8d934-1191">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1191">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="8d934-1192">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="8d934-1192">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="8d934-1193">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="8d934-1193">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="8d934-1194">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1194">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="8d934-1195">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8d934-1195">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="8d934-1196">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="8d934-1196">Az.Profile</span></span>
* <span data-ttu-id="8d934-1197">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1197">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="8d934-1198">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1198">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-1199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-1199">Az.Compute</span></span>
* <span data-ttu-id="8d934-1200">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1200">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="8d934-1201">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1201">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="8d934-1202">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="8d934-1202">Az.DataLakeStore</span></span>
* <span data-ttu-id="8d934-1203">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1203">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="8d934-1204">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="8d934-1204">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="8d934-1205">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="8d934-1205">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8d934-1206">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="8d934-1206">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="8d934-1207">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="8d934-1207">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-1208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-1208">Az.Network</span></span>
* <span data-ttu-id="8d934-1209">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1209">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="8d934-1210">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1210">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-1211">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-1211">Az.Resources</span></span>
* <span data-ttu-id="8d934-1212">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1212">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="8d934-1213">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1213">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="8d934-1214">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="8d934-1214">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="8d934-1215">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="8d934-1215">Azure.Storage</span></span>
* <span data-ttu-id="8d934-1216">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1216">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="8d934-1217">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="8d934-1217">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="8d934-1218">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="8d934-1218">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="8d934-1219">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1219">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="8d934-1220">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="8d934-1220">Get-AzStorageUsage</span></span>
    
#### <a name="azcognitiveservices"></a><span data-ttu-id="8d934-1221">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="8d934-1221">Az.CognitiveServices</span></span>
* <span data-ttu-id="8d934-1222">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1222">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="8d934-1223">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="8d934-1223">Az.Compute</span></span>
* <span data-ttu-id="8d934-1224">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1224">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="8d934-1225">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1225">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="8d934-1226">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1226">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="8d934-1227">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="8d934-1227">Az.DataFactoryV2</span></span>
* <span data-ttu-id="8d934-1228">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1228">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="8d934-1229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="8d934-1229">Az.Network</span></span>
* <span data-ttu-id="8d934-1230">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="8d934-1230">Added NetworkProfile functionality.</span></span> <span data-ttu-id="8d934-1231">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="8d934-1231">new cmdlets added</span></span>
    - <span data-ttu-id="8d934-1232">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d934-1232">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d934-1233">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d934-1233">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d934-1234">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d934-1234">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d934-1235">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="8d934-1235">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="8d934-1236">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-1236">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="8d934-1237">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="8d934-1237">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="8d934-1238">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1238">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="8d934-1239">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1239">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="8d934-1240">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1240">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="8d934-1241">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="8d934-1241">Az.RedisCache</span></span>
* <span data-ttu-id="8d934-1242">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="8d934-1242">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="8d934-1243">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1243">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="8d934-1244">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="8d934-1244">Az.Resources</span></span>
* <span data-ttu-id="8d934-1245">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1245">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="8d934-1246">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1246">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="8d934-1247">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="8d934-1247">Az.Sql</span></span>
* <span data-ttu-id="8d934-1248">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="8d934-1248">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="8d934-1249">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="8d934-1249">Az.Websites</span></span>
* <span data-ttu-id="8d934-1250">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="8d934-1250">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="8d934-1251">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="8d934-1251">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="8d934-1252">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="8d934-1252">0.2.0 - September 2018</span></span>
 <span data-ttu-id="8d934-1253">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="8d934-1253">Initial Release</span></span>