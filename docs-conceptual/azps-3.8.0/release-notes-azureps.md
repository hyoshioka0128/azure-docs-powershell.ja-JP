---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: bee24af99da4b36e89cff9852c77214e2e09a542
ms.sourcegitcommit: 6a91b4c545350d316d3cf8c62f384478e3f3ba24
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/21/2020
ms.locfileid: "81740543"
---
## <a name="380---april-2020"></a><span data-ttu-id="2b07e-103">3.8.0 - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-103">3.8.0 - April 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-104">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-104">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-105">'Resolve-AzError' の Azure PowerShell アンケートの URL を更新しました [#11507]</span><span class="sxs-lookup"><span data-stu-id="2b07e-105">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-106">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-106">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-107">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-107">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="2b07e-108">GroupId パラメーターの指定について 'Set-AzApiManagementGroup' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-108">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-109">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-109">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-110">ChinaCDN 関連の価格 SKU の表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-110">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-111">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-111">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-112">ID、暗号化、UserOwnedStorage をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-112">Supported Identity, Encryption, UserOwnedStorage</span></span> 

#### <a name="azcompute"></a><span data-ttu-id="2b07e-113">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-113">Az.Compute</span></span>
* <span data-ttu-id="2b07e-114">'Set-AzVmssOrchestrationServiceState' コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-114">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="2b07e-115">'Get-AzVmss' に -InstanceView を指定することで、OrchestrationService の状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-115">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-116">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-116">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-117">IoT デバイス ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-117">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-118">'Get-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="2b07e-118">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="2b07e-119">'Update-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="2b07e-119">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="2b07e-120">Iot Hub のデバイスでダイレクト メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-120">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="2b07e-121">IoT デバイス モジュール ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-121">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-122">'Get-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="2b07e-122">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="2b07e-123">'Update-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="2b07e-123">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="2b07e-124">IoT の自動デバイス管理構成を大規模に管理します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-124">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="2b07e-125">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-125">New cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-126">'Add-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="2b07e-126">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="2b07e-127">'Get-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="2b07e-127">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="2b07e-128">'Remove-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="2b07e-128">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="2b07e-129">'Set-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="2b07e-129">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="2b07e-130">Iot Hub で edge モジュール メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-130">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-131">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-131">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-132">コンテナーでの論理的な削除と消去保護を有効にできる新しいコマンドレット 'Update-AzKeyVault' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-132">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="2b07e-133">Microsoft.PowerShell.SecretManagement へのサポートを追加しました [#11178]</span><span class="sxs-lookup"><span data-stu-id="2b07e-133">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="2b07e-134">'Remove-AzKeyVaultManagedStorageSasDefinition' の例の誤りを修正しました [#11479]</span><span class="sxs-lookup"><span data-stu-id="2b07e-134">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="2b07e-135">プライベート エンドポイントへのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-135">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="2b07e-136">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="2b07e-136">Az.Maintenance</span></span>
* <span data-ttu-id="2b07e-137">GA 用のメンテナンス コマンドレットのリリース バージョンを公開しています</span><span class="sxs-lookup"><span data-stu-id="2b07e-137">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-138">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-138">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-139">プライベート リンク スコープのコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-139">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="2b07e-140">'Get-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="2b07e-140">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="2b07e-141">'Remove-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="2b07e-141">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="2b07e-142">'New-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="2b07e-142">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="2b07e-143">'Update-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="2b07e-143">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="2b07e-144">'Get-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="2b07e-144">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="2b07e-145">'New-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="2b07e-145">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="2b07e-146">'Remove-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="2b07e-146">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-147">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-147">Az.Network</span></span>
* <span data-ttu-id="2b07e-148">仮想ネットワーク ゲートウェイのプライベート IP での接続を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-148">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="2b07e-149">'New-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="2b07e-149">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="2b07e-150">'Set-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="2b07e-150">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="2b07e-151">'New-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="2b07e-151">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="2b07e-152">'Set-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="2b07e-152">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="2b07e-153">FQDN ベースの LocalNetworkGateways と VpnSites を有効にするコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-153">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="2b07e-154">'New-AzLocalNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="2b07e-154">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="2b07e-155">'New-AzVpnSiteLink'</span><span class="sxs-lookup"><span data-stu-id="2b07e-155">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="2b07e-156">ExpressRouteCircuitConnectionConfig (Global Reach) で IPv6 アドレス ファミリのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-156">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="2b07e-157">'Set-AzExpressRouteCircuitConnectionConfig' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-157">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="2b07e-158">IPv6CircuitConnectionProperties を含むすべての既存のプロパティを設定できます</span><span class="sxs-lookup"><span data-stu-id="2b07e-158">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="2b07e-159">'Add-AzExpressRouteCircuitConnectionConfig' を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-159">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="2b07e-160">アドレス プレフィックスのアドレス ファミリを指定する、別の省略可能なパラメーター AddressPrefixType を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-160">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="2b07e-161">仮想ネットワーク ゲートウェイ接続で DPD タイムアウトの設定を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-161">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="2b07e-162">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-162">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="2b07e-163">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-163">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-164">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-164">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-165">ポリシー コンプライアンス スキャンをトリガーするための 'Start-AzPolicyComplianceScan' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-165">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="2b07e-166">ポリシー定義、セット定義、および割り当てのバージョンを 'Get-AzPolicyState' 出力に追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-166">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-167">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-167">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-168">'New-AzServiceFabricCluster' サンプルのコードのフォーマットと使いやすさが向上しています</span><span class="sxs-lookup"><span data-stu-id="2b07e-168">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-169">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-169">Az.Sql</span></span>
* <span data-ttu-id="2b07e-170">コマンドレット 'Get-AzSqlInstanceOperation' および 'Stop-AzSqlInstanceOperation' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-170">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="2b07e-171">VNet のストレージ アカウントに対する監査をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-171">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-172">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-172">Az.Storage</span></span>
* <span data-ttu-id="2b07e-173">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-173">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="2b07e-174">ストレージ アカウントの作成/更新時に新しい SkuName StandardGZRS、StandardRAGZRS をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-174">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="2b07e-175">'New-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="2b07e-175">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="2b07e-176">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="2b07e-176">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="2b07e-177">Supported DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="2b07e-177">Supported DataLake Gen2</span></span> 
    - <span data-ttu-id="2b07e-178">'New-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="2b07e-178">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="2b07e-179">'Get-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="2b07e-179">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="2b07e-180">'Get-AzDataLakeGen2ChildItem'</span><span class="sxs-lookup"><span data-stu-id="2b07e-180">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="2b07e-181">'Move-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="2b07e-181">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="2b07e-182">'Set-AzDataLakeGen2ItemAclObject'</span><span class="sxs-lookup"><span data-stu-id="2b07e-182">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="2b07e-183">'Update-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="2b07e-183">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="2b07e-184">'Get-AzDataLakeGen2ItemContent'</span><span class="sxs-lookup"><span data-stu-id="2b07e-184">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="2b07e-185">'Remove-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="2b07e-185">'Remove-AzDataLakeGen2Item'</span></span>

# <a name="azure-powershell-release-notes"></a><span data-ttu-id="2b07e-186">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="2b07e-186">Azure PowerShell release notes</span></span>
## <a name="370---march-2020"></a><span data-ttu-id="2b07e-187">3.7.0 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-187">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-188">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-188">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-189">ログインしていない場合に、'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' が NullReferenceException をスローする問題を修正しました [#10292]</span><span class="sxs-lookup"><span data-stu-id="2b07e-189">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-190">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-190">Az.Compute</span></span>
* <span data-ttu-id="2b07e-191">'New-AzDiskConfig' コマンドレットに次のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-191">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span> 
    - <span data-ttu-id="2b07e-192">DiskIOPSReadOnly、DiskMBpsReadOnly、MaxSharesCount、GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="2b07e-192">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="2b07e-193">'New-AzGalleryImageVersion' コマンドレットの Target パラメーターで Encryption プロパティを使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-193">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="2b07e-194">'Set-AzVmss' の -Reimage と 'Invoke-AzVMReimage' コマンドレットの tempDisk の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-194">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="2b07e-195">[#11354]</span><span class="sxs-lookup"><span data-stu-id="2b07e-195">[#11354]</span></span>
* <span data-ttu-id="2b07e-196">新しい SAP 拡張機能の次のコマンドレットに対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-196">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="2b07e-197">'Set-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="2b07e-197">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="2b07e-198">'Get-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="2b07e-198">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="2b07e-199">'Remove-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="2b07e-199">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="2b07e-200">'Update-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="2b07e-200">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="2b07e-201">ヘルプ ドキュメントの例の誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-201">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="2b07e-202">VM PowerState の正確な文字列値をテーブル形式で示しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-202">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="2b07e-203">'New-AzVmssConfig': SinglePlacementGroup が無効な場合の AutomaticRepairs プロパティのシリアル化を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-203">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="2b07e-204">[#11257]</span><span class="sxs-lookup"><span data-stu-id="2b07e-204">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-205">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-205">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-206">ADF .Net SDK のバージョンを 4.8.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-206">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="2b07e-207">再実行をサポートするために、'Invoke-AzDataFactoryV2Pipeline' コマンドに省略可能なパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-207">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-208">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-208">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-209">'Export-AzDataLakeStoreItem' と 'Import-AzDataLakeStoreItem' に破壊的変更の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-209">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="2b07e-210">'New-AzDataLakeStoreItem'、'Add-AzDAtaLakeStoreItemContent'、および 'Get-AzDAtaLakeStoreItemContent' にバイト エンコードのオプションを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-210">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-211">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-211">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-212">クラスターの作成時に、最低限サポートされている TLS バージョンの指定をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-212">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-213">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-213">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-214">デバイスごとの分散設定の管理のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-214">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="2b07e-215">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-215">New Cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-216">'Get-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="2b07e-216">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="2b07e-217">'Set-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="2b07e-217">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-218">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-218">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-219">'New-AzKeyVault' に破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-219">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-220">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-220">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-221">'New-AzScheduledQueryRuleLogMetricTrigger' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-221">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-222">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-222">Az.Network</span></span>
* <span data-ttu-id="2b07e-223">テナント間の VirtualHubVnetConnections を許可するためにコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-223">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="2b07e-224">'New-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="2b07e-224">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="2b07e-225">'Update-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="2b07e-225">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="2b07e-226">'New-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="2b07e-226">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="2b07e-227">'Update-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="2b07e-227">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="2b07e-228">SQL 管理 SDK の依存関係を削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-228">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-229">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-229">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-230">エラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-230">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-231">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-231">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-232">Azure Site Recovery で再保護を行うためのサポートを追加し、Azure Disk Encryption を使用して暗号化されている Virtual Machines の vm プロパティを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-232">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="2b07e-233">Azure Site Recovery に VmwareToAzure プロパティの DR 監視を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-233">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="2b07e-234">Azure Backup に、失敗した項目の再試行ポリシー更新のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-234">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="2b07e-235">Azure Backup に、バックアップおよび復元中のディスク除外設定のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-235">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="2b07e-236">Azure Backup に、AzureFileShare で複数ファイル/フォルダーを復元するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-236">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="2b07e-237">Azure Backup に、IaasVM ポリシーの更新中にユーザーによって指定された Resourcegroup へのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-237">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-238">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-238">Az.Resources</span></span>
* <span data-ttu-id="2b07e-239">既定の apiVersion ではなく、リソースの実際の apiVersion を使用するように 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' を修正しました [#11267]</span><span class="sxs-lookup"><span data-stu-id="2b07e-239">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="2b07e-240">エラー シナリオでの correlationId のログ記録を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-240">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="2b07e-241">'Get-AzResourceLock' のドキュメントをわずかに変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-241">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="2b07e-242">例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-242">Added example.</span></span>
* <span data-ttu-id="2b07e-243">'Get-AzADUser' のパラメーター値の単一引用符をエスケープしました [#11317]</span><span class="sxs-lookup"><span data-stu-id="2b07e-243">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="2b07e-244">デプロイ スクリプト ('Get-AzDeploymentScript'、'Get-AzDeploymentScriptLog'、'Save-AzDeploymentScriptLog'、'Remove-AzDeploymentScript') に新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-244">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-245">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-245">Az.Sql</span></span>
* <span data-ttu-id="2b07e-246">'Invoke-AzSqlDatabaseFailover' に読み取り可能なセカンダリ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-246">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="2b07e-247">コマンドレット 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-247">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="2b07e-248">データベース内の列を分類するときの秘密度ランクを保存しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-248">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="2b07e-249">Az.Support</span><span class="sxs-lookup"><span data-stu-id="2b07e-249">Az.Support</span></span>
* <span data-ttu-id="2b07e-250">'Az.Support' モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="2b07e-250">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-251">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-251">Az.Websites</span></span>
* <span data-ttu-id="2b07e-252">次の新しいコマンドレットを使用して、webapp トラフィック ルーティング規則を処理するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-252">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="2b07e-253">'Get-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="2b07e-253">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="2b07e-254">'Update-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="2b07e-254">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="2b07e-255">'Add-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="2b07e-255">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="2b07e-256">'Remove-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="2b07e-256">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="2b07e-257">3.6.1 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-257">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-258">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-258">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-259">'Send-Feedback' で Azure PowerShell アンケート ページを開きます [#11020]</span><span class="sxs-lookup"><span data-stu-id="2b07e-259">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="2b07e-260">'Resolve-Error' に Azure PowerShell アンケートの URL を表示します [#11021]</span><span class="sxs-lookup"><span data-stu-id="2b07e-260">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="2b07e-261">UserAgent で Az バージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-261">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-262">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-262">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-263">DeveloperPortal エンドポイントでカスタム ドメインを取得および構成するためのサポートを追加しました [#11007]</span><span class="sxs-lookup"><span data-stu-id="2b07e-263">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="2b07e-264">'Export-AzApiManagementApi' で、JSON 形式で API 定義をダウンロードするためのサポートを追加しました [#9987]</span><span class="sxs-lookup"><span data-stu-id="2b07e-264">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="2b07e-265">'Import-AzApiManagementApi' で、JSON ドキュメントから OpenApi 3.0 定義をインポートするためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-265">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="2b07e-266">'New-AzApiManagementIdentityProvider' および 'Set-AzApiManagementIdentityProvider' で、AAD B2C プロバイダーの 'サインイン テナント' を構成するためのサポートを追加しました [#9784]</span><span class="sxs-lookup"><span data-stu-id="2b07e-266">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-267">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-267">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-268">csproj および psd1 で明示的に System.Buffers への参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-268">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-269">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-269">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-270">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-270">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="2b07e-271">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-271">New Cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-272">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-272">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="2b07e-273">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-273">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="2b07e-274">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-274">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="2b07e-275">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-275">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="2b07e-276">Iot Hub のターゲット Iot デバイスでモジュールを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-276">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="2b07e-277">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-277">New Cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-278">'Add-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="2b07e-278">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="2b07e-279">'Get-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="2b07e-279">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="2b07e-280">'Remove-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="2b07e-280">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="2b07e-281">'Set-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="2b07e-281">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="2b07e-282">Iot Hub 内のターゲット IoT デバイスの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-282">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="2b07e-283">Iot Hub 内のターゲット IoT デバイス上のモジュールの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-283">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="2b07e-284">IoT デバイスの親デバイスを取得/設定するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-284">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="2b07e-285">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-285">New Cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-286">'Get-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="2b07e-286">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="2b07e-287">'Set-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="2b07e-287">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="2b07e-288">デバイスの親子関係を管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-288">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-289">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-289">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-290">'Get-AzMetricDefinition' の出力値を修正しました [#9714]</span><span class="sxs-lookup"><span data-stu-id="2b07e-290">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-291">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-291">Az.Network</span></span>
* <span data-ttu-id="2b07e-292">SQL 管理 SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-292">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="2b07e-293">PrivateLinkServiceConnectionState クラスの naming-difference の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-293">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="2b07e-294">フィールド ActionRequired を ActionRequired にマップしています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-294">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="2b07e-295">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-295">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-296">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-296">Az.Resources</span></span>
* <span data-ttu-id="2b07e-297">'Get-AzRoleAssignment' で null 参照のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-297">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="2b07e-298">'Remove-AzADGroup' でスイッチ '-Force ' および '-PassThru ' に省略可能のマークを付けました [#10849]</span><span class="sxs-lookup"><span data-stu-id="2b07e-298">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="2b07e-299">'MailNickname' が 'Remove-AzADGroup' で返さない問題を修正しました [#11167]</span><span class="sxs-lookup"><span data-stu-id="2b07e-299">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="2b07e-300">'Remove-AzADGroup' パイプ操作が機能しない問題を修正しました [#11171]</span><span class="sxs-lookup"><span data-stu-id="2b07e-300">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="2b07e-301">GetAzureRoleAssignmentCommand の null 参照のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-301">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="2b07e-302">ポリシー コマンドレットの今後の変更について、破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-302">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="2b07e-303">サーバー側でリソース グループ タグのフィルター処理を実行するように 'Get-AzResourceGroup' を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-303">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="2b07e-304">タグ コマンドレットで -ResourceId を受け入れるように拡張しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-304">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="2b07e-305">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="2b07e-305">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="2b07e-306">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="2b07e-306">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="2b07e-307">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="2b07e-307">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="2b07e-308">新しいタグ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-308">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="2b07e-309">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="2b07e-309">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="2b07e-310">SDK 3.3.0 から ScopedDeployment を導入しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-310">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-311">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-311">Az.Sql</span></span>
* <span data-ttu-id="2b07e-312">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-312">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="2b07e-313">マネージド データベースの長期的な保有期間のバックアップ構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-313">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="2b07e-314">マネージド データベースで LTR ポリシーを取得/設定します</span><span class="sxs-lookup"><span data-stu-id="2b07e-314">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="2b07e-315">マネージド データベース、マネージド インスタンス、または場所で LTR バックアップを取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-315">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="2b07e-316">LTR バックアップを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-316">Remove an LTR backup</span></span>
    - <span data-ttu-id="2b07e-317">LTR バックアップを復元して新しいマネージド データベースを作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-317">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="2b07e-318">New-AzSqlServer と Set-AzSqlServer に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-318">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="2b07e-319">New-AzSqlInstance と Set-AzSqlInstance に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-319">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="2b07e-320">Az.Network の SQL SDK のバージョンを上げました</span><span class="sxs-lookup"><span data-stu-id="2b07e-320">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-321">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-321">Az.Storage</span></span>
* <span data-ttu-id="2b07e-322">ImmutabilityPolicy で AllowProtectedAppendWrite をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-322">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="2b07e-323">'Set-AzRmStorageContainerImmutabilityPolicy'</span><span class="sxs-lookup"><span data-stu-id="2b07e-323">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="2b07e-324">将来のリリースでの AzureStorageTable 型の変更に対する破壊的変更の警告メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-324">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="2b07e-325">'New-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="2b07e-325">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="2b07e-326">'Get-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="2b07e-326">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-327">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-327">Az.Websites</span></span>
* <span data-ttu-id="2b07e-328">'New-AzAppServicePlan' と 'Set-AzAppServicePlan' の Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-328">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="2b07e-329">Web サイトにカスタム ドメインを追加するときに例外がスローされた場合、コマンドレットの実行を停止します</span><span class="sxs-lookup"><span data-stu-id="2b07e-329">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="2b07e-330">App Service プランと同じリソース グループに含まれていない App Services の操作を実行するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-330">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="2b07e-331">異なるリソース グループ内の WebApp/Function へのアクセス制限を適用しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-331">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="2b07e-332">WebAppSlots のカスタム ホスト名を設定するための問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-332">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="2b07e-333">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-333">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="2b07e-334">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="2b07e-334">Highlights since the last major release</span></span>
* <span data-ttu-id="2b07e-335">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-335">Updated client side telemetry.</span></span>
* <span data-ttu-id="2b07e-336">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-336">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="2b07e-337">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-337">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-338">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-338">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-339">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-339">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-340">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-340">Az.Automation</span></span>
* <span data-ttu-id="2b07e-341">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-341">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-342">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-342">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-343">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-343">Updated SDK to 7.0</span></span>
* <span data-ttu-id="2b07e-344">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-344">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-345">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-345">Az.Compute</span></span>
* <span data-ttu-id="2b07e-346">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-346">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-347">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-347">Az.FrontDoor</span></span>
* <span data-ttu-id="2b07e-348">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-348">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-349">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-349">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-350">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-350">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="2b07e-351">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-351">New Cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-352">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-352">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="2b07e-353">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-353">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="2b07e-354">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-354">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="2b07e-355">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="2b07e-355">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-356">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-356">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-357">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-357">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-358">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-358">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-359">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-359">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="2b07e-360">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-360">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="2b07e-361">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-361">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-362">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-362">Az.Network</span></span>
* <span data-ttu-id="2b07e-363">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-363">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="2b07e-364">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-364">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="2b07e-365">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-365">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="2b07e-366">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-366">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="2b07e-367">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="2b07e-367">No new cmdlets are added.</span></span> <span data-ttu-id="2b07e-368">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="2b07e-368">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-369">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-369">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-370">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-370">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-371">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-371">Az.Resources</span></span>
* <span data-ttu-id="2b07e-372">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-372">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="2b07e-373">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="2b07e-373">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="2b07e-374">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="2b07e-374">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="2b07e-375">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-375">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="2b07e-376">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-376">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="2b07e-377">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-377">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="2b07e-378">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-378">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="2b07e-379">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-379">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-380">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-380">Az.Sql</span></span>
* <span data-ttu-id="2b07e-381">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-381">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="2b07e-382">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-382">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="2b07e-383">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="2b07e-383">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="2b07e-384">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="2b07e-384">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="2b07e-385">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-385">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="2b07e-386">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="2b07e-386">Az.StorageSync</span></span>
* <span data-ttu-id="2b07e-387">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-387">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="2b07e-388">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-388">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="2b07e-389">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="2b07e-389">Highlights since the last major release</span></span>
* <span data-ttu-id="2b07e-390">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-390">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="2b07e-391">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-391">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-392">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-392">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-393">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="2b07e-393">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="2b07e-394">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-394">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-395">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-395">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-396">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="2b07e-396">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="2b07e-397">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="2b07e-397">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="2b07e-398">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-398">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="2b07e-399">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-399">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-400">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-400">Az.Compute</span></span>
* <span data-ttu-id="2b07e-401">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-401">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="2b07e-402">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-402">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="2b07e-403">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-403">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="2b07e-404">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-404">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="2b07e-405">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-405">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-406">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-406">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-407">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-407">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="2b07e-408">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="2b07e-408">Az.DeploymentManager</span></span>
* <span data-ttu-id="2b07e-409">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-409">Adds LIST operations for resources</span></span>
* <span data-ttu-id="2b07e-410">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-410">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-411">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-411">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-412">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-412">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-413">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-413">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-414">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-414">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-415">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-415">Az.Network</span></span>
* <span data-ttu-id="2b07e-416">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-416">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="2b07e-417">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="2b07e-417">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="2b07e-418">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="2b07e-418">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="2b07e-419">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-419">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="2b07e-420">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="2b07e-420">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="2b07e-421">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-421">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="2b07e-422">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-422">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="2b07e-423">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-423">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="2b07e-424">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-424">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-425">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b07e-425">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="2b07e-426">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-426">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="2b07e-427">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-427">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="2b07e-428">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-428">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-429">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-429">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-430">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-430">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="2b07e-431">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-431">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="2b07e-432">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-432">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="2b07e-433">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-433">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-434">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-434">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-435">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-435">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="2b07e-436">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-436">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-437">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-437">Az.Resources</span></span>
* <span data-ttu-id="2b07e-438">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="2b07e-438">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="2b07e-439">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-439">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-440">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-440">Az.Sql</span></span>
<span data-ttu-id="2b07e-441">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-441">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-442">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-442">Az.Storage</span></span>
* <span data-ttu-id="2b07e-443">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-443">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="2b07e-444">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-444">New-AzStorageAccount</span></span>
* <span data-ttu-id="2b07e-445">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="2b07e-445">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="2b07e-446">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-446">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-447">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-447">Az.Websites</span></span>
* <span data-ttu-id="2b07e-448">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-448">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="2b07e-449">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-449">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="2b07e-450">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-450">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-451">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-451">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-452">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-452">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-453">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-453">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-454">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="2b07e-454">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-455">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-455">Az.Compute</span></span>
* <span data-ttu-id="2b07e-456">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-456">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="2b07e-457">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-457">Az.ContainerInstance</span></span>
* <span data-ttu-id="2b07e-458">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-458">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="2b07e-459">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="2b07e-459">Az.DataBoxEdge</span></span>
* <span data-ttu-id="2b07e-460">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-460">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="2b07e-461">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-461">Get the Edge Storage Container</span></span>
* <span data-ttu-id="2b07e-462">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-462">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="2b07e-463">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-463">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="2b07e-464">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-464">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="2b07e-465">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-465">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="2b07e-466">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-466">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="2b07e-467">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="2b07e-467">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="2b07e-468">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-468">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="2b07e-469">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-469">Get the Edge Storage Account</span></span>
* <span data-ttu-id="2b07e-470">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-470">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="2b07e-471">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-471">Create new Edge Storage Account</span></span>
* <span data-ttu-id="2b07e-472">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-472">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="2b07e-473">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-473">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="2b07e-474">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="2b07e-474">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="2b07e-475">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="2b07e-475">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="2b07e-476">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-476">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="2b07e-477">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="2b07e-477">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-478">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-478">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-479">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-479">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="2b07e-480">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-480">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="2b07e-481">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-481">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="2b07e-482">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="2b07e-482">Az.DevTestLabs</span></span>
* <span data-ttu-id="2b07e-483">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-483">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-484">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-484">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-485">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-485">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-486">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-486">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-487">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-487">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="2b07e-488">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="2b07e-488">Az.MachineLearning</span></span>
* <span data-ttu-id="2b07e-489">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-489">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="2b07e-490">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="2b07e-490">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="2b07e-491">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="2b07e-491">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="2b07e-492">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="2b07e-492">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="2b07e-493">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="2b07e-493">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="2b07e-494">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="2b07e-494">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="2b07e-495">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="2b07e-495">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="2b07e-496">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="2b07e-496">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-497">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-497">Az.Network</span></span>
* <span data-ttu-id="2b07e-498">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="2b07e-498">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-499">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-499">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-500">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-500">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="2b07e-501">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-501">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="2b07e-502">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-502">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="2b07e-503">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-503">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-504">Az.Resources</span></span>
* <span data-ttu-id="2b07e-505">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-505">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-506">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-506">Az.Sql</span></span>
* <span data-ttu-id="2b07e-507">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-507">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="2b07e-508">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-508">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="2b07e-509">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="2b07e-509">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="2b07e-510">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-510">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-511">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-511">Az.Storage</span></span>
* <span data-ttu-id="2b07e-512">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-512">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="2b07e-513">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-513">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="2b07e-514">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-514">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="2b07e-515">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-515">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="2b07e-516">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-516">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="2b07e-517">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-517">General</span></span>
* <span data-ttu-id="2b07e-518">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-518">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-519">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-519">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-520">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="2b07e-520">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="2b07e-521">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="2b07e-521">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="2b07e-522">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b07e-522">Az.Batch</span></span>
* <span data-ttu-id="2b07e-523">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-523">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-524">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-524">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-525">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-525">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-526">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-526">Az.FrontDoor</span></span>
* <span data-ttu-id="2b07e-527">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-527">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="2b07e-528">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-528">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="2b07e-529">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="2b07e-529">Az.HealthcareApis</span></span>
* <span data-ttu-id="2b07e-530">例外処理</span><span class="sxs-lookup"><span data-stu-id="2b07e-530">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-531">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-531">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-532">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-532">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="2b07e-533">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="2b07e-533">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="2b07e-534">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-534">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-535">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-535">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-536">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-536">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="2b07e-537">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="2b07e-537">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="2b07e-538">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="2b07e-538">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-539">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-539">Az.Network</span></span>
* <span data-ttu-id="2b07e-540">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-540">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-541">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-541">Az.Resources</span></span>
* <span data-ttu-id="2b07e-542">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-542">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="2b07e-543">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-543">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-544">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-544">Az.Sql</span></span>
* <span data-ttu-id="2b07e-545">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-545">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-546">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-546">Az.Storage</span></span>
* <span data-ttu-id="2b07e-547">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-547">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="2b07e-548">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="2b07e-548">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="2b07e-549">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="2b07e-549">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="2b07e-550">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="2b07e-550">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="2b07e-551">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="2b07e-551">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="2b07e-552">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-552">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="2b07e-553">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-553">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="2b07e-554">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="2b07e-554">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="2b07e-555">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="2b07e-555">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="2b07e-556">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-556">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="2b07e-557">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="2b07e-557">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="2b07e-558">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-558">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="2b07e-559">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="2b07e-559">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="2b07e-560">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-560">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="2b07e-561">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="2b07e-561">Highlights since the last major release</span></span>
* <span data-ttu-id="2b07e-562">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-562">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="2b07e-563">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-563">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-564">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-564">Az.Compute</span></span>
* <span data-ttu-id="2b07e-565">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="2b07e-565">VM Reapply feature</span></span>
    - <span data-ttu-id="2b07e-566">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-566">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="2b07e-567">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="2b07e-567">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="2b07e-568">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="2b07e-568">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="2b07e-569">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-569">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="2b07e-570">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-570">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="2b07e-571">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-571">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="2b07e-572">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="2b07e-572">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="2b07e-573">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-573">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="2b07e-574">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-574">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="2b07e-575">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-575">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="2b07e-576">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="2b07e-576">Az.DataBoxEdge</span></span>
* <span data-ttu-id="2b07e-577">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-577">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="2b07e-578">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-578">Get the Order</span></span>
* <span data-ttu-id="2b07e-579">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-579">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="2b07e-580">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-580">Create new Order</span></span>
* <span data-ttu-id="2b07e-581">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-581">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="2b07e-582">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-582">Remove the Order</span></span>
* <span data-ttu-id="2b07e-583">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="2b07e-583">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="2b07e-584">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="2b07e-584">Now creates Local Share</span></span>
* <span data-ttu-id="2b07e-585">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-585">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="2b07e-586">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-586">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="2b07e-587">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-587">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="2b07e-588">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="2b07e-588">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="2b07e-589">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-589">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="2b07e-590">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-590">Gets the information about Triggers</span></span>
* <span data-ttu-id="2b07e-591">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-591">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="2b07e-592">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-592">Create new Triggers</span></span>
* <span data-ttu-id="2b07e-593">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-593">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="2b07e-594">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-594">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-595">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-595">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-596">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-596">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="2b07e-597">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-597">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-598">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-598">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-599">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-599">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-600">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-600">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-601">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-601">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-602">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-602">Az.FrontDoor</span></span>
* <span data-ttu-id="2b07e-603">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-603">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="2b07e-604">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-604">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="2b07e-605">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-605">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="2b07e-606">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="2b07e-606">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-607">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-607">Az.Network</span></span>
* <span data-ttu-id="2b07e-608">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-608">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="2b07e-609">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="2b07e-609">Az.PrivateDns</span></span>
* <span data-ttu-id="2b07e-610">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-610">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-611">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-611">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-612">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-612">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="2b07e-613">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="2b07e-613">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="2b07e-614">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-614">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="2b07e-615">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2b07e-615">Az.RedisCache</span></span>
* <span data-ttu-id="2b07e-616">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-616">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="2b07e-617">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-617">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="2b07e-618">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-618">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-619">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-619">Az.Resources</span></span>
- <span data-ttu-id="2b07e-620">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-620">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="2b07e-621">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-621">Updated create policy definition help example</span></span>
- <span data-ttu-id="2b07e-622">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-622">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="2b07e-623">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-623">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="2b07e-624">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-624">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-625">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-625">Az.Sql</span></span>
* <span data-ttu-id="2b07e-626">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-626">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="2b07e-627">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-627">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="2b07e-628">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-628">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="2b07e-629">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-629">General</span></span>
* <span data-ttu-id="2b07e-630">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-630">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-631">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-631">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-632">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-632">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="2b07e-633">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="2b07e-633">Az.Advisor</span></span>
* <span data-ttu-id="2b07e-634">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-634">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="2b07e-635">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b07e-635">Az.Batch</span></span>
* <span data-ttu-id="2b07e-636">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-636">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="2b07e-637">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="2b07e-637">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="2b07e-638">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-638">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="2b07e-639">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-639">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="2b07e-640">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="2b07e-640">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="2b07e-641">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-641">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="2b07e-642">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-642">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="2b07e-643">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-643">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="2b07e-644">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-644">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="2b07e-645">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-645">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="2b07e-646">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-646">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="2b07e-647">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-647">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="2b07e-648">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-648">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="2b07e-649">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-649">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="2b07e-650">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-650">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="2b07e-651">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-651">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="2b07e-652">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-652">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="2b07e-653">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-653">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="2b07e-654">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-654">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="2b07e-655">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b07e-655">This operation is no longer supported.</span></span>
* <span data-ttu-id="2b07e-656">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-656">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="2b07e-657">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-657">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="2b07e-658">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-658">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="2b07e-659">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-659">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="2b07e-660">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-660">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="2b07e-661">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-661">New non-verified images are also now returned.</span></span> <span data-ttu-id="2b07e-662">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-662">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="2b07e-663">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-663">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="2b07e-664">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-664">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="2b07e-665">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-665">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="2b07e-666">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-666">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="2b07e-667">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-667">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="2b07e-668">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-668">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="2b07e-669">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-669">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="2b07e-670">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-670">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="2b07e-671">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-671">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-672">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-672">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-673">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-673">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="2b07e-674">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-674">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-675">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-675">Az.Compute</span></span>
* <span data-ttu-id="2b07e-676">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="2b07e-676">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="2b07e-677">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-677">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="2b07e-678">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。 Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile、Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="2b07e-678">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="2b07e-679">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-679">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="2b07e-680">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-680">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="2b07e-681">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="2b07e-681">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="2b07e-682">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-682">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="2b07e-683">重大な変更</span><span class="sxs-lookup"><span data-stu-id="2b07e-683">Breaking changes</span></span>
    - <span data-ttu-id="2b07e-684">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="2b07e-684">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="2b07e-685">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="2b07e-685">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-686">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-686">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-687">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-687">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-688">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-688">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-689">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="2b07e-689">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="2b07e-690">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-690">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="2b07e-691">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="2b07e-691">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="2b07e-692">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-692">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="2b07e-693">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-693">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="2b07e-694">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-694">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-695">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-695">Az.FrontDoor</span></span>
* <span data-ttu-id="2b07e-696">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-696">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-697">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-697">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-698">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-698">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="2b07e-699">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-699">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="2b07e-700">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-700">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="2b07e-701">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-701">Removed five cmdlets:</span></span>
    - <span data-ttu-id="2b07e-702">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="2b07e-702">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="2b07e-703">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="2b07e-703">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="2b07e-704">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="2b07e-704">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="2b07e-705">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="2b07e-705">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="2b07e-706">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="2b07e-706">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="2b07e-707">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-707">Added three cmdlets:</span></span>
    - <span data-ttu-id="2b07e-708">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-708">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="2b07e-709">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-709">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="2b07e-710">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-710">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="2b07e-711">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-711">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="2b07e-712">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-712">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="2b07e-713">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-713">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="2b07e-714">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="2b07e-714">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="2b07e-715">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-715">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="2b07e-716">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-716">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="2b07e-717">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-717">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="2b07e-718">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-718">Added some scenario test cases.</span></span>
* <span data-ttu-id="2b07e-719">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="2b07e-719">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-720">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-720">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-721">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="2b07e-721">Breaking changes:</span></span>
    - <span data-ttu-id="2b07e-722">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-722">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="2b07e-723">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-723">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="2b07e-724">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-724">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="2b07e-725">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-725">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="2b07e-726">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-726">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="2b07e-727">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-727">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="2b07e-728">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-728">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="2b07e-729">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-729">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="2b07e-730">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-730">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="2b07e-731">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-731">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="2b07e-732">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-732">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="2b07e-733">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-733">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-734">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-734">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-735">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-735">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-736">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-736">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="2b07e-737">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-737">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="2b07e-738">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-738">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-739">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-739">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-740">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-740">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-741">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-741">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-742">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-742">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-743">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-743">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-744">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-744">Az.Resources</span></span>
* <span data-ttu-id="2b07e-745">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-745">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-746">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-746">Az.Network</span></span>
* <span data-ttu-id="2b07e-747">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-747">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="2b07e-748">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-748">Updated cmdlet:</span></span>
        - <span data-ttu-id="2b07e-749">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-749">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-750">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-750">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-751">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-751">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-752">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-752">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-753">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-753">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="2b07e-754">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="2b07e-754">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="2b07e-755">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-755">New cmdlet:</span></span>
        - <span data-ttu-id="2b07e-756">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="2b07e-756">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="2b07e-757">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-757">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="2b07e-758">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-758">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="2b07e-759">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-759">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="2b07e-760">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-760">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="2b07e-761">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-761">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="2b07e-762">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-762">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="2b07e-763">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-763">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="2b07e-764">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-764">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-765">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="2b07e-765">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="2b07e-766">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-766">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="2b07e-767">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-767">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="2b07e-768">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-768">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="2b07e-769">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-769">Set-AzVirtualHub</span></span>
* <span data-ttu-id="2b07e-770">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-770">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="2b07e-771">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-771">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="2b07e-772">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-772">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="2b07e-773">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-773">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="2b07e-774">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-774">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="2b07e-775">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-775">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="2b07e-776">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-776">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="2b07e-777">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-777">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-778">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-778">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="2b07e-779">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-779">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="2b07e-780">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-780">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="2b07e-781">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-781">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="2b07e-782">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-782">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="2b07e-783">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-783">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="2b07e-784">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-784">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="2b07e-785">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-785">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="2b07e-786">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-786">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-787">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="2b07e-787">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="2b07e-788">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="2b07e-788">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="2b07e-789">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="2b07e-789">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="2b07e-790">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="2b07e-790">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="2b07e-791">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-791">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="2b07e-792">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-792">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="2b07e-793">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-793">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="2b07e-794">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-794">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="2b07e-795">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-795">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="2b07e-796">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-796">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="2b07e-797">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-797">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="2b07e-798">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-798">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="2b07e-799">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-799">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="2b07e-800">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-800">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="2b07e-801">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-801">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="2b07e-802">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-802">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="2b07e-803">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-803">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="2b07e-804">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-804">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-805">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="2b07e-805">New-AzIpGroup</span></span>
        - <span data-ttu-id="2b07e-806">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="2b07e-806">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="2b07e-807">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="2b07e-807">Get-AzIpGroup</span></span>
        - <span data-ttu-id="2b07e-808">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="2b07e-808">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-809">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-809">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-810">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-810">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-811">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-811">Az.Sql</span></span>
* <span data-ttu-id="2b07e-812">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-812">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="2b07e-813">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-813">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="2b07e-814">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-814">Removed deprecated aliases:</span></span>
* <span data-ttu-id="2b07e-815">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="2b07e-815">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="2b07e-816">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="2b07e-816">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="2b07e-817">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-817">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="2b07e-818">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-818">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="2b07e-819">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="2b07e-819">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="2b07e-820">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-820">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-821">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-821">Az.Storage</span></span>
* <span data-ttu-id="2b07e-822">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-822">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="2b07e-823">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-823">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="2b07e-824">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-824">Set-AzStorageAccount</span></span>
* <span data-ttu-id="2b07e-825">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="2b07e-825">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="2b07e-826">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="2b07e-826">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="2b07e-827">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="2b07e-827">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="2b07e-828">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-828">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="2b07e-829">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-829">General</span></span>
* <span data-ttu-id="2b07e-830">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-830">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-831">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-831">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-832">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-832">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-833">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-833">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-834">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-834">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="2b07e-835">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="2b07e-835">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-836">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-836">Az.Automation</span></span>
* <span data-ttu-id="2b07e-837">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-837">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="2b07e-838">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b07e-838">Az.Batch</span></span>
* <span data-ttu-id="2b07e-839">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-839">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-840">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-840">Az.Compute</span></span>
* <span data-ttu-id="2b07e-841">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-841">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="2b07e-842">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-842">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="2b07e-843">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-843">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="2b07e-844">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-844">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-845">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-845">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-846">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="2b07e-846">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="2b07e-847">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="2b07e-847">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="2b07e-848">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-848">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-849">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-849">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-850">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-850">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="2b07e-851">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="2b07e-851">Az.HealthcareApis</span></span>
* <span data-ttu-id="2b07e-852">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-852">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="2b07e-853">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-853">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="2b07e-854">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-854">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="2b07e-855">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-855">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-856">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-856">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-857">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="2b07e-857">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="2b07e-858">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="2b07e-858">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-859">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-859">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-860">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="2b07e-860">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="2b07e-861">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-861">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="2b07e-862">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="2b07e-862">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="2b07e-863">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-863">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-864">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-864">Az.Network</span></span>
* <span data-ttu-id="2b07e-865">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-865">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="2b07e-866">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-866">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="2b07e-867">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-867">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-868">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-868">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="2b07e-869">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-869">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="2b07e-870">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-870">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="2b07e-871">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-871">Updated cmdlets:</span></span>
        - <span data-ttu-id="2b07e-872">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-872">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="2b07e-873">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-873">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="2b07e-874">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-874">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="2b07e-875">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="2b07e-875">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="2b07e-876">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="2b07e-876">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="2b07e-877">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-877">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="2b07e-878">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-878">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="2b07e-879">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2b07e-879">Az.RedisCache</span></span>
* <span data-ttu-id="2b07e-880">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-880">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-881">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-881">Az.Sql</span></span>
* <span data-ttu-id="2b07e-882">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-882">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-883">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-883">Az.Storage</span></span>
* <span data-ttu-id="2b07e-884">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="2b07e-884">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="2b07e-885">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2b07e-885">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="2b07e-886">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="2b07e-886">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="2b07e-887">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2b07e-887">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="2b07e-888">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-888">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="2b07e-889">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="2b07e-889">Az.StorageSync</span></span>
* <span data-ttu-id="2b07e-890">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-890">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-891">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-891">Az.Websites</span></span>
* <span data-ttu-id="2b07e-892">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="2b07e-892">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="2b07e-893">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-893">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-894">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-894">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-895">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-895">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="2b07e-896">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-896">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="2b07e-897">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="2b07e-897">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-898">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-898">Az.Automation</span></span>
* <span data-ttu-id="2b07e-899">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-899">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="2b07e-900">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-900">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="2b07e-901">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-901">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-902">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-902">Az.Compute</span></span>
* <span data-ttu-id="2b07e-903">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-903">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="2b07e-904">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-904">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="2b07e-905">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-905">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="2b07e-906">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-906">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="2b07e-907">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-907">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="2b07e-908">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-908">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="2b07e-909">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-909">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="2b07e-910">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-910">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="2b07e-911">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-911">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-912">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-912">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-913">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-913">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="2b07e-914">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-914">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-915">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-915">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-916">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="2b07e-916">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-917">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-917">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-918">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-918">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="2b07e-919">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-919">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="2b07e-920">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2b07e-920">New cmdlets are:</span></span>
    - <span data-ttu-id="2b07e-921">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="2b07e-921">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="2b07e-922">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="2b07e-922">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="2b07e-923">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="2b07e-923">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="2b07e-924">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="2b07e-924">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-925">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-925">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-926">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="2b07e-926">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="2b07e-927">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-927">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="2b07e-928">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="2b07e-928">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="2b07e-929">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-929">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="2b07e-930">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-930">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="2b07e-931">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-931">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="2b07e-932">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-932">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="2b07e-933">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="2b07e-933">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="2b07e-934">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-934">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="2b07e-935">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-935">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="2b07e-936">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-936">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="2b07e-937">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="2b07e-937">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="2b07e-938">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-938">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="2b07e-939">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-939">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="2b07e-940">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-940">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="2b07e-941">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="2b07e-941">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="2b07e-942">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-942">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="2b07e-943">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-943">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="2b07e-944">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-944">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="2b07e-945">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-945">Overall improved help files</span></span>
* <span data-ttu-id="2b07e-946">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-946">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-947">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-947">Az.Network</span></span>
* <span data-ttu-id="2b07e-948">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-948">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="2b07e-949">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-949">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="2b07e-950">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-950">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="2b07e-951">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-951">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="2b07e-952">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-952">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="2b07e-953">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-953">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="2b07e-954">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-954">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="2b07e-955">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-955">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="2b07e-956">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-956">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="2b07e-957">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-957">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="2b07e-958">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-958">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="2b07e-959">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-959">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="2b07e-960">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-960">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-961">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="2b07e-961">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="2b07e-962">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-962">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="2b07e-963">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-963">Updated cmdlet:</span></span>
        - <span data-ttu-id="2b07e-964">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="2b07e-964">New-VpnSite</span></span>
        - <span data-ttu-id="2b07e-965">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="2b07e-965">Update-VpnSite</span></span>
        - <span data-ttu-id="2b07e-966">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-966">New-VpnConnection</span></span>
        - <span data-ttu-id="2b07e-967">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-967">Update-VpnConnection</span></span>
* <span data-ttu-id="2b07e-968">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-968">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-969">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-969">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-970">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-970">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="2b07e-971">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-971">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-972">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-972">Az.Resources</span></span>
* <span data-ttu-id="2b07e-973">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-973">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-974">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-974">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-975">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-975">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="2b07e-976">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-976">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="2b07e-977">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="2b07e-977">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="2b07e-978">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="2b07e-978">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="2b07e-979">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="2b07e-979">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="2b07e-980">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="2b07e-980">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="2b07e-981">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="2b07e-981">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="2b07e-982">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="2b07e-982">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="2b07e-983">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="2b07e-983">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="2b07e-984">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="2b07e-984">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="2b07e-985">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="2b07e-985">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="2b07e-986">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="2b07e-986">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="2b07e-987">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="2b07e-987">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="2b07e-988">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="2b07e-988">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="2b07e-989">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="2b07e-989">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="2b07e-990">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-990">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="2b07e-991">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="2b07e-991">Az.SignalR</span></span>
* <span data-ttu-id="2b07e-992">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="2b07e-992">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-993">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-993">Az.Sql</span></span>
* <span data-ttu-id="2b07e-994">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-994">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="2b07e-995">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-995">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="2b07e-996">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-996">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="2b07e-997">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-997">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="2b07e-998">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-998">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-999">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-999">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1000">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1000">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="2b07e-1001">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-1001">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="2b07e-1002">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1002">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="2b07e-1003">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1003">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="2b07e-1004">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1004">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="2b07e-1005">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1005">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="2b07e-1006">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-1006">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="2b07e-1007">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="2b07e-1007">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="2b07e-1008">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="2b07e-1008">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="2b07e-1009">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="2b07e-1009">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="2b07e-1010">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="2b07e-1010">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1011">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1011">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1012">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1012">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="2b07e-1013">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1013">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="2b07e-1014">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1014">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="2b07e-1015">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1015">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="2b07e-1016">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-1016">General</span></span>
* <span data-ttu-id="2b07e-1017">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1017">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1018">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1018">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1019">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="2b07e-1019">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="2b07e-1020">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="2b07e-1020">Az.Aks</span></span>
* <span data-ttu-id="2b07e-1021">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1021">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="2b07e-1022">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="2b07e-1022">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-1023">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-1023">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-1024">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="2b07e-1024">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="2b07e-1025">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1025">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="2b07e-1026">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1026">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="2b07e-1027">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="2b07e-1027">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="2b07e-1028">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1028">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="2b07e-1029">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b07e-1029">Az.Batch</span></span>
* <span data-ttu-id="2b07e-1030">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1030">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-1031">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-1031">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-1032">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1032">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1033">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1033">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1034">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1034">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="2b07e-1035">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1035">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="2b07e-1036">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1036">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="2b07e-1037">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1037">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="2b07e-1038">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="2b07e-1038">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="2b07e-1039">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1039">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="2b07e-1040">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1040">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="2b07e-1041">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1041">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1042">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1042">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1043">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1043">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="2b07e-1044">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1044">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="2b07e-1045">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1045">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="2b07e-1046">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1046">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-1047">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-1047">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-1048">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1048">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-1049">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1049">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-1050">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="2b07e-1050">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="2b07e-1051">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="2b07e-1051">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="2b07e-1052">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1052">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="2b07e-1053">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="2b07e-1053">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="2b07e-1054">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="2b07e-1054">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="2b07e-1055">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1055">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-1056">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1056">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-1057">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1057">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1058">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1058">Az.Network</span></span>
* <span data-ttu-id="2b07e-1059">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1059">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="2b07e-1060">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1060">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="2b07e-1061">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1061">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="2b07e-1062">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1062">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="2b07e-1063">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1063">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="2b07e-1064">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1064">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="2b07e-1065">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1065">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-1066">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1066">Az.OperationalInsights</span></span>
* <span data-ttu-id="2b07e-1067">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1067">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="2b07e-1068">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1068">Added example</span></span>
    - <span data-ttu-id="2b07e-1069">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1069">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="2b07e-1070">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1070">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="2b07e-1071">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1071">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1072">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1072">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1073">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1073">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1074">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1074">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1075">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1075">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="2b07e-1076">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1076">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="2b07e-1077">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="2b07e-1077">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="2b07e-1078">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1078">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2b07e-1079">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2b07e-1079">Az.ServiceBus</span></span>
* <span data-ttu-id="2b07e-1080">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="2b07e-1080">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="2b07e-1081">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="2b07e-1081">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="2b07e-1082">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1082">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-1083">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-1083">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-1084">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1084">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="2b07e-1085">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1085">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="2b07e-1086">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="2b07e-1086">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="2b07e-1087">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1087">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="2b07e-1088">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="2b07e-1088">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="2b07e-1089">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1089">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1090">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1090">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1091">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1091">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1092">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1092">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1093">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1093">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="2b07e-1094">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-1094">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="2b07e-1095">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1095">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="2b07e-1096">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1096">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="2b07e-1097">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-1097">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="2b07e-1098">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1098">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1099">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1099">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1100">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1100">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="2b07e-1101">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1101">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1102">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1102">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1103">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1103">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="2b07e-1104">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1104">Az.ApplicationInsights</span></span>
* <span data-ttu-id="2b07e-1105">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1105">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1106">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1106">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1107">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1107">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-1108">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1108">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-1109">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1109">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1110">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1110">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1111">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1111">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="2b07e-1112">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="2b07e-1112">Az.ContainerRegistry</span></span>
* <span data-ttu-id="2b07e-1113">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1113">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="2b07e-1114">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="2b07e-1114">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1115">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1115">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1116">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1116">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="2b07e-1117">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1117">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-1118">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1118">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-1119">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="2b07e-1119">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="2b07e-1120">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1120">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-1121">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-1121">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-1122">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1122">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="2b07e-1123">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="2b07e-1123">Az.LogicApp</span></span>
* <span data-ttu-id="2b07e-1124">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1124">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="2b07e-1125">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1125">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="2b07e-1126">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1126">Az.ManagedServices</span></span>
* <span data-ttu-id="2b07e-1127">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1127">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1128">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1128">Az.Network</span></span>
* <span data-ttu-id="2b07e-1129">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1129">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="2b07e-1130">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1130">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-1131">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="2b07e-1131">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="2b07e-1132">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="2b07e-1132">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="2b07e-1133">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1133">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-1134">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1134">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-1135">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1135">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-1136">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1136">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="2b07e-1137">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="2b07e-1137">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="2b07e-1138">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="2b07e-1138">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="2b07e-1139">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="2b07e-1139">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="2b07e-1140">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1140">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="2b07e-1141">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1141">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="2b07e-1142">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1142">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="2b07e-1143">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1143">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="2b07e-1144">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1144">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="2b07e-1145">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1145">Updated cmdlets</span></span>
        - <span data-ttu-id="2b07e-1146">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1146">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="2b07e-1147">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1147">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="2b07e-1148">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1148">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="2b07e-1149">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1149">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="2b07e-1150">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1150">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="2b07e-1151">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1151">Updated cmdlet:</span></span>
        - <span data-ttu-id="2b07e-1152">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1152">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="2b07e-1153">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1153">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="2b07e-1154">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1154">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="2b07e-1155">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1155">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="2b07e-1156">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1156">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="2b07e-1157">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1157">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-1158">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1158">Az.OperationalInsights</span></span>
* <span data-ttu-id="2b07e-1159">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1159">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="2b07e-1160">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1160">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1161">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1161">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1162">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1162">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="2b07e-1163">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1163">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="2b07e-1164">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1164">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="2b07e-1165">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1165">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="2b07e-1166">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1166">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="2b07e-1167">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1167">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="2b07e-1168">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1168">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="2b07e-1169">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1169">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="2b07e-1170">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1170">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="2b07e-1171">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1171">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1172">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1172">Az.Resources</span></span>
- <span data-ttu-id="2b07e-1173">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1173">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="2b07e-1174">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1174">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2b07e-1175">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2b07e-1175">Az.ServiceBus</span></span>
* <span data-ttu-id="2b07e-1176">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="2b07e-1176">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="2b07e-1177">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1177">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1178">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1178">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1179">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1179">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="2b07e-1180">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1180">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="2b07e-1181">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1181">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1182">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1182">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1183">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1183">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="2b07e-1184">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="2b07e-1184">Az.StorageSync</span></span>
* <span data-ttu-id="2b07e-1185">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1185">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="2b07e-1186">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1186">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1187">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1187">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1188">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1188">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="2b07e-1189">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1189">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="2b07e-1190">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1190">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="2b07e-1191">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1191">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1192">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1192">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1193">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1193">Add support for profile cmdlets</span></span>
* <span data-ttu-id="2b07e-1194">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1194">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="2b07e-1195">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1195">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="2b07e-1196">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1196">Az.Advisor</span></span>
* <span data-ttu-id="2b07e-1197">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-1197">GA release of Az.Advisor</span></span>
* <span data-ttu-id="2b07e-1198">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1198">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-1199">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-1199">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-1200">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="2b07e-1200">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="2b07e-1201">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="2b07e-1201">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="2b07e-1202">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1202">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="2b07e-1203">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1203">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="2b07e-1204">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1204">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="2b07e-1205">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="2b07e-1205">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="2b07e-1206">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1206">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1207">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1207">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1208">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1208">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1209">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1209">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1210">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1210">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1211">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1211">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1212">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1212">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="2b07e-1213">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="2b07e-1213">Az.EventGrid</span></span>
* <span data-ttu-id="2b07e-1214">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1214">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-1215">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1215">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-1216">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1216">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1217">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1217">Az.Network</span></span>
* <span data-ttu-id="2b07e-1218">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1218">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="2b07e-1219">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1219">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-1220">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1220">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-1221">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1221">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="2b07e-1222">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="2b07e-1222">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-1223">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1223">Az.OperationalInsights</span></span>
* <span data-ttu-id="2b07e-1224">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1224">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1225">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1225">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1226">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1226">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1227">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1227">Az.Resources</span></span>
    - <span data-ttu-id="2b07e-1228">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1228">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="2b07e-1229">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1229">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="2b07e-1230">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1230">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="2b07e-1231">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1231">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2b07e-1232">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2b07e-1232">Az.ServiceBus</span></span>
* <span data-ttu-id="2b07e-1233">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="2b07e-1233">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1234">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1234">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1235">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1235">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="2b07e-1236">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-1236">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="2b07e-1237">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="2b07e-1237">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="2b07e-1238">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="2b07e-1238">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="2b07e-1239">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="2b07e-1239">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="2b07e-1240">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="2b07e-1240">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="2b07e-1241">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="2b07e-1241">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="2b07e-1242">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="2b07e-1242">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="2b07e-1243">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1243">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1244">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1244">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1245">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1245">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="2b07e-1246">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="2b07e-1246">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="2b07e-1247">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1247">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="2b07e-1248">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="2b07e-1248">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="2b07e-1249">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-1249">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="2b07e-1250">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1250">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="2b07e-1251">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1251">Set-AzStorageAccount</span></span>
* <span data-ttu-id="2b07e-1252">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-1252">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="2b07e-1253">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="2b07e-1253">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="2b07e-1254">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="2b07e-1254">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="2b07e-1255">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="2b07e-1255">Az.StorageSync</span></span>
* <span data-ttu-id="2b07e-1256">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1256">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="2b07e-1257">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1257">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1258">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1258">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1259">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1259">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="2b07e-1260">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="2b07e-1260">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="2b07e-1261">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1261">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="2b07e-1262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="2b07e-1262">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="2b07e-1263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="2b07e-1263">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1264">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1264">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1265">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1265">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="2b07e-1266">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1266">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="2b07e-1267">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="2b07e-1267">Az.Dns</span></span>
* <span data-ttu-id="2b07e-1268">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1268">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="2b07e-1269">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="2b07e-1269">Az.EventGrid</span></span>
* <span data-ttu-id="2b07e-1270">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1270">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="2b07e-1271">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1271">New cmdlets:</span></span>
    - <span data-ttu-id="2b07e-1272">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="2b07e-1272">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="2b07e-1273">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1273">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="2b07e-1274">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="2b07e-1274">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="2b07e-1275">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1275">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="2b07e-1276">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="2b07e-1276">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="2b07e-1277">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1277">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="2b07e-1278">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="2b07e-1278">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="2b07e-1279">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1279">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="2b07e-1280">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="2b07e-1280">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="2b07e-1281">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1281">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="2b07e-1282">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1282">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="2b07e-1283">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1283">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="2b07e-1284">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="2b07e-1284">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="2b07e-1285">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1285">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="2b07e-1286">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1286">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="2b07e-1287">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1287">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="2b07e-1288">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1288">Updated cmdlets:</span></span>
    - <span data-ttu-id="2b07e-1289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1289">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="2b07e-1290">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1290">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="2b07e-1291">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1291">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="2b07e-1292">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1292">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="2b07e-1293">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1293">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="2b07e-1294">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="2b07e-1294">Event subscription expiration date,</span></span>
            - <span data-ttu-id="2b07e-1295">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="2b07e-1295">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="2b07e-1296">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1296">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="2b07e-1297">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1297">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="2b07e-1298">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1298">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="2b07e-1299">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1299">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="2b07e-1300">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="2b07e-1300">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="2b07e-1301">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1301">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="2b07e-1302">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1302">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-1303">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1303">Az.FrontDoor</span></span>
* <span data-ttu-id="2b07e-1304">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="2b07e-1304">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="2b07e-1305">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1305">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="2b07e-1306">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="2b07e-1306">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="2b07e-1307">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1307">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1308">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1308">Az.Network</span></span>
* <span data-ttu-id="2b07e-1309">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1309">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="2b07e-1310">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1310">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-1311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="2b07e-1311">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="2b07e-1312">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1312">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="2b07e-1313">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1313">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-1314">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="2b07e-1314">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="2b07e-1315">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1315">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="2b07e-1316">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1316">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-1317">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="2b07e-1317">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="2b07e-1318">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="2b07e-1318">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="2b07e-1319">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="2b07e-1319">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="2b07e-1320">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1320">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="2b07e-1321">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1321">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="2b07e-1322">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1322">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="2b07e-1323">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1323">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-1324">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="2b07e-1324">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="2b07e-1325">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="2b07e-1325">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="2b07e-1326">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="2b07e-1326">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="2b07e-1327">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1327">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="2b07e-1328">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="2b07e-1328">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="2b07e-1329">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1329">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="2b07e-1330">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1330">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="2b07e-1331">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1331">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="2b07e-1332">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1332">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="2b07e-1333">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1333">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="2b07e-1334">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1334">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="2b07e-1335">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1335">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="2b07e-1336">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1336">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="2b07e-1337">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1337">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="2b07e-1338">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1338">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="2b07e-1339">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1339">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="2b07e-1340">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1340">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="2b07e-1341">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1341">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="2b07e-1342">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1342">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="2b07e-1343">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1343">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="2b07e-1344">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1344">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="2b07e-1345">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="2b07e-1345">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="2b07e-1346">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1346">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="2b07e-1347">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1347">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="2b07e-1348">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1348">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="2b07e-1349">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1349">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="2b07e-1350">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1350">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-1351">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1351">Az.OperationalInsights</span></span>
* <span data-ttu-id="2b07e-1352">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1352">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1353">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1353">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1354">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1354">Support for additional Template Export options</span></span>
    - <span data-ttu-id="2b07e-1355">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1355">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="2b07e-1356">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1356">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="2b07e-1357">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1357">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-1358">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-1358">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-1359">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1359">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1360">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1360">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1361">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1361">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="2b07e-1362">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1362">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="2b07e-1363">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1363">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="2b07e-1364">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="2b07e-1364">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="2b07e-1365">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="2b07e-1365">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="2b07e-1366">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="2b07e-1366">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="2b07e-1367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="2b07e-1367">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="2b07e-1368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="2b07e-1368">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1369">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1369">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1370">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1370">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="2b07e-1371">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1371">New-AzStorageAccount</span></span>
* <span data-ttu-id="2b07e-1372">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1372">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="2b07e-1373">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1373">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1374">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1374">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1375">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1375">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="2b07e-1376">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1376">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="2b07e-1377">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1377">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="2b07e-1378">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-1378">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-1379">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1379">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1380">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1380">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1381">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1381">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="2b07e-1382">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="2b07e-1382">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-1383">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1383">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-1384">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1384">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="2b07e-1385">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1385">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1386">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1386">Az.Network</span></span>
* <span data-ttu-id="2b07e-1387">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1387">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="2b07e-1388">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1388">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-1389">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1389">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-1390">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1390">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1391">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1392">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1392">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2b07e-1393">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2b07e-1393">Az.ServiceBus</span></span>
* <span data-ttu-id="2b07e-1394">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1394">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-1395">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-1395">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-1396">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1396">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="2b07e-1397">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1397">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1398">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1398">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1399">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1399">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="2b07e-1400">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="2b07e-1400">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="2b07e-1401">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1401">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="2b07e-1402">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1402">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1403">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1403">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1404">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1404">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="2b07e-1405">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1405">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="2b07e-1406">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-1406">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-1407">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1407">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="2b07e-1408">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1408">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="2b07e-1409">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1409">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="2b07e-1410">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1410">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="2b07e-1411">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1411">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="2b07e-1412">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1412">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="2b07e-1413">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1413">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="2b07e-1414">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1414">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="2b07e-1415">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1415">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="2b07e-1416">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1416">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="2b07e-1417">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1417">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="2b07e-1418">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1418">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="2b07e-1419">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1419">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="2b07e-1420">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1420">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="2b07e-1421">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1421">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="2b07e-1422">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1422">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="2b07e-1423">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1423">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="2b07e-1424">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1424">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="2b07e-1425">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1425">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="2b07e-1426">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="2b07e-1426">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="2b07e-1427">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1427">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="2b07e-1428">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1428">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="2b07e-1429">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1429">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="2b07e-1430">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1430">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="2b07e-1431">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1431">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="2b07e-1432">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1432">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="2b07e-1433">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1433">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="2b07e-1434">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1434">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="2b07e-1435">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1435">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="2b07e-1436">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1436">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="2b07e-1437">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1437">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="2b07e-1438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="2b07e-1438">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="2b07e-1439">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1439">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="2b07e-1440">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1440">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="2b07e-1441">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="2b07e-1441">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="2b07e-1442">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1442">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="2b07e-1443">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1443">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="2b07e-1444">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1444">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="2b07e-1445">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1445">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="2b07e-1446">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1446">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="2b07e-1447">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1447">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="2b07e-1448">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1448">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="2b07e-1449">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1449">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="2b07e-1450">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1450">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="2b07e-1451">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1451">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="2b07e-1452">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1452">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="2b07e-1453">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1453">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="2b07e-1454">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1454">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="2b07e-1455">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1455">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="2b07e-1456">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1456">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="2b07e-1457">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1457">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="2b07e-1458">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1458">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="2b07e-1459">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1459">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="2b07e-1460">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1460">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="2b07e-1461">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1461">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="2b07e-1462">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1462">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="2b07e-1463">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1463">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="2b07e-1464">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1464">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="2b07e-1465">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1465">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="2b07e-1466">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1466">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="2b07e-1467">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1467">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="2b07e-1468">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1468">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="2b07e-1469">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="2b07e-1469">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="2b07e-1470">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1470">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="2b07e-1471">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1471">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="2b07e-1472">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1472">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="2b07e-1473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="2b07e-1473">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="2b07e-1474">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1474">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="2b07e-1475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="2b07e-1475">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="2b07e-1476">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1476">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="2b07e-1477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="2b07e-1477">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="2b07e-1478">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1478">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="2b07e-1479">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1479">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="2b07e-1480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-1480">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="2b07e-1481">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1481">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="2b07e-1482">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1482">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="2b07e-1483">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="2b07e-1483">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1484">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1484">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1485">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1485">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="2b07e-1486">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="2b07e-1486">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="2b07e-1487">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="2b07e-1487">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="2b07e-1488">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1488">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="2b07e-1489">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="2b07e-1489">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="2b07e-1490">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1490">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="2b07e-1491">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1491">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1492">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1492">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1493">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1493">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="2b07e-1494">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1494">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-1495">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-1495">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-1496">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1496">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-1497">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1497">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-1498">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1498">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1499">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1499">Az.Network</span></span>
* <span data-ttu-id="2b07e-1500">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1500">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="2b07e-1501">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1501">Updated cmdlet:</span></span>
        - <span data-ttu-id="2b07e-1502">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-1502">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="2b07e-1503">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1503">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1504">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1504">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1505">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1505">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1506">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1506">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1507">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1507">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="2b07e-1508">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1508">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1509">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1509">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1510">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1510">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-1511">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1511">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-1512">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1512">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="2b07e-1513">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1513">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1514">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1514">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1515">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1515">Proximity placement group feature.</span></span>
    - <span data-ttu-id="2b07e-1516">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="2b07e-1516">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="2b07e-1517">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-1517">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="2b07e-1518">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1518">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="2b07e-1519">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1519">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="2b07e-1520">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1520">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="2b07e-1521">重大な変更</span><span class="sxs-lookup"><span data-stu-id="2b07e-1521">Breaking changes</span></span>
    - <span data-ttu-id="2b07e-1522">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1522">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="2b07e-1523">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1523">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="2b07e-1524">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="2b07e-1524">Az.DeploymentManager</span></span>
* <span data-ttu-id="2b07e-1525">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-1525">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="2b07e-1526">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="2b07e-1526">Az.Dns</span></span>
* <span data-ttu-id="2b07e-1527">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="2b07e-1527">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="2b07e-1528">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1528">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="2b07e-1529">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1529">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-1530">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1530">Az.FrontDoor</span></span>
* <span data-ttu-id="2b07e-1531">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-1531">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="2b07e-1532">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1532">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-1533">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-1533">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-1534">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1534">Removed two cmdlets:</span></span>
    - <span data-ttu-id="2b07e-1535">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="2b07e-1535">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="2b07e-1536">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="2b07e-1536">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="2b07e-1537">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1537">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="2b07e-1538">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1538">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="2b07e-1539">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1539">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="2b07e-1540">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1540">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-1541">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1541">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-1542">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="2b07e-1542">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="2b07e-1543">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="2b07e-1543">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="2b07e-1544">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="2b07e-1544">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="2b07e-1545">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="2b07e-1545">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="2b07e-1546">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1546">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="2b07e-1547">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="2b07e-1547">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="2b07e-1548">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="2b07e-1548">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="2b07e-1549">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1549">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="2b07e-1550">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1550">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="2b07e-1551">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1551">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="2b07e-1552">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1552">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="2b07e-1553">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1553">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="2b07e-1554">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="2b07e-1554">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="2b07e-1555">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1555">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1556">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1556">Az.Network</span></span>
* <span data-ttu-id="2b07e-1557">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1557">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="2b07e-1558">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1558">New cmdlets</span></span>
        - <span data-ttu-id="2b07e-1559">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="2b07e-1559">New-AzNatGateway</span></span>
        - <span data-ttu-id="2b07e-1560">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="2b07e-1560">Get-AzNatGateway</span></span>
        - <span data-ttu-id="2b07e-1561">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="2b07e-1561">Set-AzNatGateway</span></span>
        - <span data-ttu-id="2b07e-1562">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="2b07e-1562">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="2b07e-1563">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1563">Updated cmdlets</span></span>
        - <span data-ttu-id="2b07e-1564">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="2b07e-1564">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="2b07e-1565">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="2b07e-1565">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="2b07e-1566">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1566">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="2b07e-1567">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1567">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="2b07e-1568">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1568">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-1569">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1569">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-1570">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1570">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="2b07e-1571">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1571">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="2b07e-1572">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1572">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1573">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1573">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1574">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1574">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="2b07e-1575">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1575">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="2b07e-1576">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1576">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="2b07e-1577">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1577">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="2b07e-1578">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1578">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="2b07e-1579">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1579">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="2b07e-1580">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="2b07e-1580">Az.Relay</span></span>
* <span data-ttu-id="2b07e-1581">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1581">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2b07e-1582">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2b07e-1582">Az.ServiceBus</span></span>
* <span data-ttu-id="2b07e-1583">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1583">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1584">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1584">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1585">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="2b07e-1585">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="2b07e-1586">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1586">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="2b07e-1587">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1587">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="2b07e-1588">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1588">New-AzStorageAccount</span></span>
* <span data-ttu-id="2b07e-1589">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="2b07e-1589">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="2b07e-1590">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1590">New-AzStorageAccount</span></span>
    - <span data-ttu-id="2b07e-1591">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1591">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="2b07e-1592">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="2b07e-1592">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1593">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1593">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1594">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="2b07e-1594">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="2b07e-1595">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1595">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="2b07e-1596">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1596">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="2b07e-1597">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="2b07e-1597">Highlights since the last major release</span></span>
* <span data-ttu-id="2b07e-1598">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="2b07e-1598">General availability of `Az` module</span></span>
* <span data-ttu-id="2b07e-1599">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="2b07e-1599">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="2b07e-1600">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="2b07e-1600">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="2b07e-1601">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1601">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="2b07e-1602">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1602">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="2b07e-1603">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1603">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="2b07e-1604">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1604">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1605">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1605">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1606">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1606">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="2b07e-1607">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b07e-1607">Az.Batch</span></span>
* <span data-ttu-id="2b07e-1608">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1608">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-1609">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-1609">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-1610">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1610">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-1611">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1611">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-1612">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1612">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1613">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1613">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1614">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1614">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="2b07e-1615">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1615">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="2b07e-1616">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1616">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1617">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1618">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1618">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-1619">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-1619">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-1620">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1620">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="2b07e-1621">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="2b07e-1621">Az.EventGrid</span></span>
* <span data-ttu-id="2b07e-1622">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1622">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-1623">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1623">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-1624">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1624">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="2b07e-1625">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="2b07e-1625">Az.HDInsight</span></span>
* <span data-ttu-id="2b07e-1626">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1626">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-1627">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1627">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-1628">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1628">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-1629">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-1629">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-1630">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1630">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="2b07e-1631">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1631">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="2b07e-1632">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="2b07e-1632">Az.MachineLearning</span></span>
* <span data-ttu-id="2b07e-1633">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1633">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="2b07e-1634">Az.Media</span><span class="sxs-lookup"><span data-stu-id="2b07e-1634">Az.Media</span></span>
* <span data-ttu-id="2b07e-1635">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1635">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-1636">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1636">Az.Monitor</span></span>
  * <span data-ttu-id="2b07e-1637">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1637">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="2b07e-1638">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="2b07e-1638">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="2b07e-1639">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="2b07e-1639">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="2b07e-1640">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="2b07e-1640">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="2b07e-1641">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="2b07e-1641">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="2b07e-1642">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="2b07e-1642">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="2b07e-1643">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1643">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1644">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1644">Az.Network</span></span>
* <span data-ttu-id="2b07e-1645">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1645">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="2b07e-1646">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1646">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="2b07e-1647">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="2b07e-1647">Az.NotificationHubs</span></span>
* <span data-ttu-id="2b07e-1648">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1648">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-1649">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1649">Az.OperationalInsights</span></span>
* <span data-ttu-id="2b07e-1650">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1650">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="2b07e-1651">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="2b07e-1651">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="2b07e-1652">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1652">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1653">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1653">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1654">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1654">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="2b07e-1655">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1655">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="2b07e-1656">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1656">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="2b07e-1657">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1657">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="2b07e-1658">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2b07e-1658">Az.RedisCache</span></span>
* <span data-ttu-id="2b07e-1659">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1659">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1660">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1660">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1661">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1661">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1662">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1662">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1663">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="2b07e-1663">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="2b07e-1664">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1664">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="2b07e-1665">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1665">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="2b07e-1666">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1666">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="2b07e-1667">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1667">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="2b07e-1668">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1668">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="2b07e-1669">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1669">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1670">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1670">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1671">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1671">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="2b07e-1672">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1672">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="2b07e-1673">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1673">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="2b07e-1674">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1674">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="2b07e-1675">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1675">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="2b07e-1676">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="2b07e-1676">Highlights since the last major release</span></span>
* <span data-ttu-id="2b07e-1677">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="2b07e-1677">General availability of `Az` module</span></span>
* <span data-ttu-id="2b07e-1678">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="2b07e-1678">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="2b07e-1679">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="2b07e-1679">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="2b07e-1680">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1680">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="2b07e-1681">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1681">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="2b07e-1682">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1682">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="2b07e-1683">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1683">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1684">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1684">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1685">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1685">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="2b07e-1686">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1686">Az.AnalysisServices</span></span>
* <span data-ttu-id="2b07e-1687">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="2b07e-1687">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="2b07e-1688">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1688">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1689">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1689">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1690">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1690">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="2b07e-1691">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1691">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="2b07e-1692">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1692">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1693">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1693">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1694">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1694">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="2b07e-1695">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1695">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="2b07e-1696">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-1696">Az.ContainerInstance</span></span>
* <span data-ttu-id="2b07e-1697">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1697">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1698">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1698">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1699">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1699">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="2b07e-1700">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1700">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1701">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1701">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1702">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1702">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="2b07e-1703">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1703">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="2b07e-1704">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1704">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="2b07e-1705">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="2b07e-1705">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="2b07e-1706">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1706">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="2b07e-1707">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="2b07e-1707">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1708">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1708">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1709">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1709">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1710">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1710">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1711">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="2b07e-1711">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="2b07e-1712">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="2b07e-1712">New-AzStorageContext</span></span>
* <span data-ttu-id="2b07e-1713">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1713">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="2b07e-1714">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="2b07e-1714">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="2b07e-1715">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="2b07e-1715">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="2b07e-1716">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1716">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="2b07e-1717">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1717">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="2b07e-1718">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1718">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="2b07e-1719">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1719">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="2b07e-1720">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1720">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="2b07e-1721">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1721">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="2b07e-1722">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="2b07e-1722">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="2b07e-1723">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1723">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="2b07e-1724">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="2b07e-1724">Highlights since the last major release</span></span>
* <span data-ttu-id="2b07e-1725">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="2b07e-1725">General availability of `Az` module</span></span>
* <span data-ttu-id="2b07e-1726">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="2b07e-1726">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="2b07e-1727">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="2b07e-1727">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="2b07e-1728">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1728">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="2b07e-1729">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1729">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="2b07e-1730">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1730">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="2b07e-1731">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1731">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1732">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1732">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1733">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1733">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="2b07e-1734">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="2b07e-1734">Dynamic grouping</span></span>
    * <span data-ttu-id="2b07e-1735">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="2b07e-1735">Pre-Post script</span></span>
    * <span data-ttu-id="2b07e-1736">再起動設定</span><span class="sxs-lookup"><span data-stu-id="2b07e-1736">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1737">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1737">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1738">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1738">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="2b07e-1739">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1739">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-1740">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-1740">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-1741">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1741">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1742">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1742">Az.Network</span></span>
* <span data-ttu-id="2b07e-1743">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1743">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="2b07e-1744">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1744">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1745">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1745">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1746">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1746">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="2b07e-1747">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1747">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1748">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1748">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1749">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1749">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="2b07e-1750">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1750">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1751">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1751">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1752">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1752">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1753">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1753">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1754">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-1754">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="2b07e-1755">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1755">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="2b07e-1756">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1756">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="2b07e-1757">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="2b07e-1757">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="2b07e-1758">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="2b07e-1758">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="2b07e-1759">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="2b07e-1759">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="2b07e-1760">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-1760">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1761">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1761">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1762">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1762">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="2b07e-1763">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1763">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1764">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1764">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1765">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1765">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="2b07e-1766">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1766">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1767">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1767">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1768">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1768">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="2b07e-1769">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1769">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="2b07e-1770">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1770">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-1771">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-1771">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-1772">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1772">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1773">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1773">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1774">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1774">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1775">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1775">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1776">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1776">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="2b07e-1777">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="2b07e-1777">Az.LogicApp</span></span>
* <span data-ttu-id="2b07e-1778">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1778">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1779">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1779">Az.Network</span></span>
* <span data-ttu-id="2b07e-1780">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1780">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1781">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1781">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1782">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1782">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="2b07e-1783">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1783">SDK Update</span></span>
* <span data-ttu-id="2b07e-1784">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1784">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="2b07e-1785">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1785">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1786">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1786">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1787">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1787">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="2b07e-1788">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="2b07e-1788">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="2b07e-1789">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1789">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="2b07e-1790">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="2b07e-1790">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="2b07e-1791">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1791">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="2b07e-1792">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="2b07e-1792">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1793">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1793">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1794">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1794">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="2b07e-1795">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1795">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1796">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1796">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1797">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1797">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="2b07e-1798">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1798">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="2b07e-1799">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1799">Az.AnalysisServices</span></span>
* <span data-ttu-id="2b07e-1800">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1800">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1801">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1801">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1802">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1802">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="2b07e-1803">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1803">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="2b07e-1804">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1804">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-1805">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1805">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-1806">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1806">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1807">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1807">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1808">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1808">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="2b07e-1809">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1809">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="2b07e-1810">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1810">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="2b07e-1811">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1811">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-1812">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-1812">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-1813">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1813">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="2b07e-1814">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1814">Az.EventHub</span></span>
* <span data-ttu-id="2b07e-1815">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1815">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-1816">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-1816">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-1817">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1817">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="2b07e-1818">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="2b07e-1818">Az.LogicApp</span></span>
* <span data-ttu-id="2b07e-1819">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1819">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="2b07e-1820">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1820">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="2b07e-1821">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1821">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="2b07e-1822">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="2b07e-1822">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="2b07e-1823">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="2b07e-1823">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="2b07e-1824">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="2b07e-1824">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="2b07e-1825">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="2b07e-1825">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="2b07e-1826">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-1826">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="2b07e-1827">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b07e-1827">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="2b07e-1828">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b07e-1828">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="2b07e-1829">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b07e-1829">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="2b07e-1830">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b07e-1830">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="2b07e-1831">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1831">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="2b07e-1832">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-1832">Az.Monitor</span></span>
* <span data-ttu-id="2b07e-1833">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1833">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1834">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1834">Az.Network</span></span>
* <span data-ttu-id="2b07e-1835">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1835">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-1836">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-1836">Az.OperationalInsights</span></span>
* <span data-ttu-id="2b07e-1837">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1837">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="2b07e-1838">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1838">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="2b07e-1839">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1839">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1840">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1840">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1841">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="2b07e-1841">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="2b07e-1842">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="2b07e-1842">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="2b07e-1843">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="2b07e-1843">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="2b07e-1844">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1844">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1845">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1845">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1846">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1846">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="2b07e-1847">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1847">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1848">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1848">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1849">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1849">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="2b07e-1850">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1850">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1851">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1851">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1852">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1852">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="2b07e-1853">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1853">Az.AnalysisServices</span></span>
<span data-ttu-id="2b07e-1854">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="2b07e-1854">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1855">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1855">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1856">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1856">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="2b07e-1857">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1857">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="2b07e-1858">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1858">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1859">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1859">Az.RecoveryServices</span></span>
<span data-ttu-id="2b07e-1860">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="2b07e-1860">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1861">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1861">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1862">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1862">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="2b07e-1863">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="2b07e-1863">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="2b07e-1864">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1864">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="2b07e-1865">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="2b07e-1865">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1866">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1866">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1867">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1867">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="2b07e-1868">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1868">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="2b07e-1869">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1869">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="2b07e-1870">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1870">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1871">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1871">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1872">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-1872">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="2b07e-1873">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1873">Az.AnalysisServices</span></span>
* <span data-ttu-id="2b07e-1874">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-1874">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-1875">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-1875">Az.RecoveryServices</span></span>
* <span data-ttu-id="2b07e-1876">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-1876">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="2b07e-1877">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1877">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1878">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1878">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1879">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1879">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="2b07e-1880">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1880">Update incorrect online help URLs</span></span>
* <span data-ttu-id="2b07e-1881">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1881">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="2b07e-1882">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="2b07e-1882">Az.Aks</span></span>
* <span data-ttu-id="2b07e-1883">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1883">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="2b07e-1884">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-1884">Az.Automation</span></span>
* <span data-ttu-id="2b07e-1885">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1885">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="2b07e-1886">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1886">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="2b07e-1887">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="2b07e-1887">Az.Cdn</span></span>
* <span data-ttu-id="2b07e-1888">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1888">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1889">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1889">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1890">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1890">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="2b07e-1891">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1891">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="2b07e-1892">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1892">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="2b07e-1893">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="2b07e-1893">Az.ContainerRegistry</span></span>
* <span data-ttu-id="2b07e-1894">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1894">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="2b07e-1895">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="2b07e-1895">Az.DataFactory</span></span>
* <span data-ttu-id="2b07e-1896">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1896">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-1897">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-1897">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-1898">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="2b07e-1898">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="2b07e-1899">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="2b07e-1899">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="2b07e-1900">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1900">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-1901">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1901">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-1902">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1902">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="2b07e-1903">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-1903">Az.KeyVault</span></span>
* <span data-ttu-id="2b07e-1904">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1904">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-1905">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-1905">Az.Network</span></span>
* <span data-ttu-id="2b07e-1906">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1906">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1907">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1907">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1908">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1908">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="2b07e-1909">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1909">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="2b07e-1910">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1910">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="2b07e-1911">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="2b07e-1911">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="2b07e-1912">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="2b07e-1912">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="2b07e-1913">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1913">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="2b07e-1914">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="2b07e-1914">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-1915">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-1915">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-1916">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="2b07e-1916">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="2b07e-1917">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1917">Fix some error messages.</span></span>
* <span data-ttu-id="2b07e-1918">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1918">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="2b07e-1919">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1919">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="2b07e-1920">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="2b07e-1920">Az.SignalR</span></span>
* <span data-ttu-id="2b07e-1921">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1921">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1922">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1922">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1923">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1923">Update incorrect online help URLs</span></span>
* <span data-ttu-id="2b07e-1924">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1924">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="2b07e-1925">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1925">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="2b07e-1926">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-1926">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1927">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1927">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1928">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1928">Update incorrect online help URLs</span></span>
* <span data-ttu-id="2b07e-1929">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="2b07e-1929">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="2b07e-1930">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="2b07e-1930">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="2b07e-1931">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="2b07e-1931">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="2b07e-1932">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="2b07e-1932">Az.TrafficManager</span></span>
* <span data-ttu-id="2b07e-1933">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1933">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1934">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1934">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1935">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1935">Update incorrect online help URLs</span></span>
* <span data-ttu-id="2b07e-1936">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1936">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="2b07e-1937">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="2b07e-1937">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="2b07e-1938">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1938">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="2b07e-1939">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1939">Az.Accounts</span></span>
* <span data-ttu-id="2b07e-1940">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="2b07e-1940">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-1941">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-1941">Az.Compute</span></span>
* <span data-ttu-id="2b07e-1942">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1942">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="2b07e-1943">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1943">Updated the description of ID in help files</span></span>
* <span data-ttu-id="2b07e-1944">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1944">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-1945">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-1945">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-1946">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1946">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="2b07e-1947">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1947">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="2b07e-1948">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="2b07e-1948">Az.EventGrid</span></span>
* <span data-ttu-id="2b07e-1949">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1949">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="2b07e-1950">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="2b07e-1950">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="2b07e-1951">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1951">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="2b07e-1952">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="2b07e-1952">Event Time-To-Live,</span></span>
        - <span data-ttu-id="2b07e-1953">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="2b07e-1953">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="2b07e-1954">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="2b07e-1954">Dead letter endpoint.</span></span>
    - <span data-ttu-id="2b07e-1955">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="2b07e-1955">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="2b07e-1956">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="2b07e-1956">Event Time-To-Live,</span></span>
        - <span data-ttu-id="2b07e-1957">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="2b07e-1957">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="2b07e-1958">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="2b07e-1958">Dead letter endpoint.</span></span>
* <span data-ttu-id="2b07e-1959">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1959">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="2b07e-1960">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1960">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="2b07e-1961">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="2b07e-1961">Az.IotHub</span></span>
* <span data-ttu-id="2b07e-1962">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1962">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="2b07e-1963">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="2b07e-1963">Az.LogicApp</span></span>
* <span data-ttu-id="2b07e-1964">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="2b07e-1964">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-1965">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-1965">Az.Resources</span></span>
* <span data-ttu-id="2b07e-1966">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1966">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="2b07e-1967">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="2b07e-1967">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="2b07e-1968">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1968">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="2b07e-1969">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1969">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="2b07e-1970">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1970">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="2b07e-1971">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="2b07e-1971">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="2b07e-1972">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="2b07e-1972">Az.SignalR</span></span>
* <span data-ttu-id="2b07e-1973">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1973">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-1974">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-1974">Az.Sql</span></span>
* <span data-ttu-id="2b07e-1975">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1975">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="2b07e-1976">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-1976">Az.Storage</span></span>
* <span data-ttu-id="2b07e-1977">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="2b07e-1977">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="2b07e-1978">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="2b07e-1978">New-AzStorageContext</span></span>
* <span data-ttu-id="2b07e-1979">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1979">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="2b07e-1980">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="2b07e-1980">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-1981">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-1981">Az.Websites</span></span>
* <span data-ttu-id="2b07e-1982">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1982">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="2b07e-1983">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1983">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="2b07e-1984">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-1984">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="2b07e-1985">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-1985">General</span></span>

- <span data-ttu-id="2b07e-1986">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="2b07e-1986">General Availability of Az Module</span></span>
- <span data-ttu-id="2b07e-1987">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="2b07e-1987">Online help for each module</span></span>
- <span data-ttu-id="2b07e-1988">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-1988">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="2b07e-1989">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-1989">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="2b07e-1990">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="2b07e-1990">Az.Accounts</span></span>
- <span data-ttu-id="2b07e-1991">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1991">Changed from Az.Profile</span></span>
- <span data-ttu-id="2b07e-1992">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-1992">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="2b07e-1993">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-1993">Az.ApiManagement</span></span>
- <span data-ttu-id="2b07e-1994">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="2b07e-1994">Fixes for #7002</span></span>
- <span data-ttu-id="2b07e-1995">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-1995">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="2b07e-1996">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="2b07e-1996">Az.Batch</span></span>
- <span data-ttu-id="2b07e-1997">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1997">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="2b07e-1998">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-1998">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="2b07e-1999">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-1999">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="2b07e-2000">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="2b07e-2000">Az.Billing</span></span>
- <span data-ttu-id="2b07e-2001">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2001">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="2b07e-2002">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-2002">Az.CognitivServices</span></span>
- <span data-ttu-id="2b07e-2003">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2003">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="2b07e-2004">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2004">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="2b07e-2005">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-2005">Az.ContainerInstance</span></span>
- <span data-ttu-id="2b07e-2006">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2006">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="2b07e-2007">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="2b07e-2007">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="2b07e-2008">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2008">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-2009">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-2009">Az.DataLakeStore</span></span>
- <span data-ttu-id="2b07e-2010">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2010">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="2b07e-2011">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="2b07e-2011">Az.Monitor</span></span>
- <span data-ttu-id="2b07e-2012">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2012">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="2b07e-2013">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="2b07e-2013">Az.KeyVault</span></span>
- <span data-ttu-id="2b07e-2014">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2014">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="2b07e-2015">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="2b07e-2015">Az.MachineLearning</span></span>
- <span data-ttu-id="2b07e-2016">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2016">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="2b07e-2017">Az.Media</span><span class="sxs-lookup"><span data-stu-id="2b07e-2017">Az.Media</span></span>
- <span data-ttu-id="2b07e-2018">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2018">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="2b07e-2019">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-2019">Az.Network</span></span>
<span data-ttu-id="2b07e-2020">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2020">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="2b07e-2021">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-2021">New cmdlets added:</span></span>
        - <span data-ttu-id="2b07e-2022">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-2022">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2b07e-2023">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-2023">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2b07e-2024">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-2024">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2b07e-2025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-2025">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2b07e-2026">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-2026">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="2b07e-2027">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-2027">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="2b07e-2028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="2b07e-2028">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="2b07e-2029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b07e-2029">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="2b07e-2030">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-2030">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="2b07e-2031">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="2b07e-2031">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="2b07e-2032">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-2032">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="2b07e-2033">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="2b07e-2033">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="2b07e-2034">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-2034">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="2b07e-2035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-2035">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="2b07e-2036">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2036">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="2b07e-2037">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-2037">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="2b07e-2038">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="2b07e-2038">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="2b07e-2039">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="2b07e-2039">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="2b07e-2040">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="2b07e-2040">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="2b07e-2041">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-2041">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="2b07e-2042">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2042">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="2b07e-2043">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-2043">Az.OperationalInsights</span></span>
- <span data-ttu-id="2b07e-2044">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2044">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="2b07e-2045">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2045">Az.Profile</span></span>
- <span data-ttu-id="2b07e-2046">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2046">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-2047">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-2047">Az.RecoveryServices</span></span>
- <span data-ttu-id="2b07e-2048">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2048">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="2b07e-2049">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-2049">Az.Resources</span></span>
- <span data-ttu-id="2b07e-2050">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2050">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="2b07e-2051">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-2051">Az.ServiceFabric</span></span>
- <span data-ttu-id="2b07e-2052">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="2b07e-2052">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="2b07e-2053">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2053">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="2b07e-2054">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="2b07e-2054">Az.SIgnalR</span></span>
- <span data-ttu-id="2b07e-2055">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="2b07e-2055">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="2b07e-2056">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-2056">Az.Sql</span></span>
- <span data-ttu-id="2b07e-2057">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2057">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="2b07e-2058">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2058">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="2b07e-2059">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2059">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="2b07e-2060">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-2060">Az.Storage</span></span>
- <span data-ttu-id="2b07e-2061">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2061">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="2b07e-2062">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-2062">Az.Websites</span></span>
- <span data-ttu-id="2b07e-2063">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="2b07e-2063">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="2b07e-2064">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-2064">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="2b07e-2065">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-2065">General</span></span>

* <span data-ttu-id="2b07e-2066">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="2b07e-2066">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="2b07e-2067">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-2067">Az.Compute</span></span>

* <span data-ttu-id="2b07e-2068">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2068">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-2069">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-2069">Az.DataLakeStore</span></span>

* <span data-ttu-id="2b07e-2070">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2070">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="2b07e-2071">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="2b07e-2071">Az.FrontDoor</span></span>

* <span data-ttu-id="2b07e-2072">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2072">Fixed some broken links</span></span>
    - <span data-ttu-id="2b07e-2073">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2073">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="2b07e-2074">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2074">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="2b07e-2075">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-2075">Az.RecoveryServices</span></span>

* <span data-ttu-id="2b07e-2076">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2076">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="2b07e-2077">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2077">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="2b07e-2078">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-2078">Az.Resources</span></span>

* <span data-ttu-id="2b07e-2079">https://github.com/Azure/azure-powershell/issues/7679 を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2079">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="2b07e-2080">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2080">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="2b07e-2081">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-2081">Az.Sql</span></span>

* <span data-ttu-id="2b07e-2082">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="2b07e-2082">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="2b07e-2083">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2083">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="2b07e-2084">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2084">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="2b07e-2085">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-2085">Az.Storage</span></span>

* <span data-ttu-id="2b07e-2086">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2086">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="2b07e-2087">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2087">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="2b07e-2088">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="2b07e-2088">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="2b07e-2089">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="2b07e-2089">Support Static Website configuration</span></span>
    - <span data-ttu-id="2b07e-2090">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="2b07e-2090">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="2b07e-2091">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="2b07e-2091">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="2b07e-2092">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-2092">Az.Websites</span></span>

* <span data-ttu-id="2b07e-2093">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="2b07e-2093">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="2b07e-2094">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2094">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="2b07e-2095">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="2b07e-2095">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="2b07e-2096">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-2096">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="2b07e-2097">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="2b07e-2097">Az.ApiManagement</span></span>
* <span data-ttu-id="2b07e-2098">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2098">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="2b07e-2099">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="2b07e-2099">Az.Automation</span></span>
* <span data-ttu-id="2b07e-2100">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="2b07e-2100">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="2b07e-2101">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2101">Added Update Management cmdlets</span></span>
* <span data-ttu-id="2b07e-2102">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2102">Added Source Control cmdlets</span></span>
* <span data-ttu-id="2b07e-2103">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2103">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="2b07e-2104">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2104">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="2b07e-2105">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-2105">Az.Compute</span></span>
* <span data-ttu-id="2b07e-2106">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2106">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="2b07e-2107">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2107">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="2b07e-2108">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-2108">Az.ContainerInstance</span></span>
* <span data-ttu-id="2b07e-2109">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2109">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="2b07e-2110">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="2b07e-2110">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="2b07e-2111">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2111">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="2b07e-2112">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-2112">Az.Network</span></span>
* <span data-ttu-id="2b07e-2113">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2113">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="2b07e-2114">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2114">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="2b07e-2115">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2115">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="2b07e-2116">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2116">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="2b07e-2117">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="2b07e-2117">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="2b07e-2118">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2118">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="2b07e-2119">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2119">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="2b07e-2120">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="2b07e-2120">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="2b07e-2121">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2121">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="2b07e-2122">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2122">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="2b07e-2123">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="2b07e-2123">Az.Relay</span></span>
* <span data-ttu-id="2b07e-2124">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="2b07e-2124">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="2b07e-2125">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-2125">Az.Resources</span></span>
* <span data-ttu-id="2b07e-2126">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2126">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="2b07e-2127">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2127">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="2b07e-2128">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="2b07e-2128">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="2b07e-2129">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-2129">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-2130">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2130">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="2b07e-2131">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-2131">Az.Sql</span></span>
* <span data-ttu-id="2b07e-2132">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2132">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="2b07e-2133">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-2133">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2b07e-2134">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-2134">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2b07e-2135">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-2135">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2b07e-2136">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="2b07e-2136">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="2b07e-2137">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2b07e-2137">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="2b07e-2138">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2b07e-2138">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="2b07e-2139">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2b07e-2139">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="2b07e-2140">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="2b07e-2140">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="2b07e-2141">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2141">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="2b07e-2142">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2142">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="2b07e-2143">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2143">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="2b07e-2144">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="2b07e-2144">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="2b07e-2145">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="2b07e-2145">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="2b07e-2146">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="2b07e-2146">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="2b07e-2147">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="2b07e-2147">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="2b07e-2148">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2148">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="2b07e-2149">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-2149">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="2b07e-2150">全般</span><span class="sxs-lookup"><span data-stu-id="2b07e-2150">General</span></span>
* <span data-ttu-id="2b07e-2151">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="2b07e-2151">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="2b07e-2152">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2152">Az.Profile</span></span>
* <span data-ttu-id="2b07e-2153">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2153">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="2b07e-2154">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2154">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="2b07e-2155">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2155">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="2b07e-2156">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2156">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="2b07e-2157">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2157">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="2b07e-2158">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2158">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="2b07e-2159">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2159">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-2160">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-2160">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-2161">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2161">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-2162">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-2162">Az.Compute</span></span>
* <span data-ttu-id="2b07e-2163">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2163">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="2b07e-2164">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="2b07e-2164">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="2b07e-2165">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2165">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-2166">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-2166">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-2167">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2167">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="2b07e-2168">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2168">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="2b07e-2169">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="2b07e-2169">Az.Insights</span></span>
* <span data-ttu-id="2b07e-2170">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2170">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="2b07e-2171">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2171">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="2b07e-2172">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2172">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="2b07e-2173">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="2b07e-2173">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-2174">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-2174">Az.Network</span></span>
* <span data-ttu-id="2b07e-2175">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="2b07e-2175">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="2b07e-2176">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-2176">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="2b07e-2177">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-2177">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="2b07e-2178">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="2b07e-2178">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="2b07e-2179">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-2179">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="2b07e-2180">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="2b07e-2180">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="2b07e-2181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="2b07e-2181">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="2b07e-2182">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="2b07e-2182">Az.PolicyInsights</span></span>
* <span data-ttu-id="2b07e-2183">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2183">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-2184">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-2184">Az.Resources</span></span>
* <span data-ttu-id="2b07e-2185">https://github.com/Azure/azure-powershell/issues/7402 を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2185">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="2b07e-2186">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2186">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="2b07e-2187">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="2b07e-2187">Az.ServiceBus</span></span>
* <span data-ttu-id="2b07e-2188">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2188">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="2b07e-2189">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="2b07e-2189">Az.ServiceFabric</span></span>
* <span data-ttu-id="2b07e-2190">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2190">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="2b07e-2191">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2191">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="2b07e-2192">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2192">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="2b07e-2193">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2193">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="2b07e-2194">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2194">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="2b07e-2195">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-2195">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="2b07e-2196">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2196">Az.Profile</span></span>
* <span data-ttu-id="2b07e-2197">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2197">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="2b07e-2198">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2198">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-2199">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-2199">Az.Compute</span></span>
* <span data-ttu-id="2b07e-2200">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2200">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="2b07e-2201">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2201">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="2b07e-2202">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="2b07e-2202">Az.DataLakeStore</span></span>
* <span data-ttu-id="2b07e-2203">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2203">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="2b07e-2204">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2204">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="2b07e-2205">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2205">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="2b07e-2206">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2206">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="2b07e-2207">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2207">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-2208">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-2208">Az.Network</span></span>
* <span data-ttu-id="2b07e-2209">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2209">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="2b07e-2210">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2210">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-2211">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-2211">Az.Resources</span></span>
* <span data-ttu-id="2b07e-2212">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2212">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="2b07e-2213">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2213">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="2b07e-2214">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-2214">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="2b07e-2215">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="2b07e-2215">Azure.Storage</span></span>
* <span data-ttu-id="2b07e-2216">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2216">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="2b07e-2217">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="2b07e-2217">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="2b07e-2218">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="2b07e-2218">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="2b07e-2219">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2219">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="2b07e-2220">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="2b07e-2220">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="2b07e-2221">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="2b07e-2221">Az.CognitiveServices</span></span>
* <span data-ttu-id="2b07e-2222">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2222">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="2b07e-2223">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="2b07e-2223">Az.Compute</span></span>
* <span data-ttu-id="2b07e-2224">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2224">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="2b07e-2225">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2225">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="2b07e-2226">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2226">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="2b07e-2227">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="2b07e-2227">Az.DataFactoryV2</span></span>
* <span data-ttu-id="2b07e-2228">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2228">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="2b07e-2229">Az.Network</span><span class="sxs-lookup"><span data-stu-id="2b07e-2229">Az.Network</span></span>
* <span data-ttu-id="2b07e-2230">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2230">Added NetworkProfile functionality.</span></span> <span data-ttu-id="2b07e-2231">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="2b07e-2231">new cmdlets added</span></span>
    - <span data-ttu-id="2b07e-2232">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2232">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="2b07e-2233">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2233">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="2b07e-2234">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2234">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="2b07e-2235">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="2b07e-2235">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="2b07e-2236">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-2236">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="2b07e-2237">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="2b07e-2237">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="2b07e-2238">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2238">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="2b07e-2239">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2239">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="2b07e-2240">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2240">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="2b07e-2241">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="2b07e-2241">Az.RedisCache</span></span>
* <span data-ttu-id="2b07e-2242">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="2b07e-2242">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="2b07e-2243">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2243">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="2b07e-2244">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="2b07e-2244">Az.Resources</span></span>
* <span data-ttu-id="2b07e-2245">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2245">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="2b07e-2246">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2246">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="2b07e-2247">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="2b07e-2247">Az.Sql</span></span>
* <span data-ttu-id="2b07e-2248">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="2b07e-2248">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="2b07e-2249">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="2b07e-2249">Az.Websites</span></span>
* <span data-ttu-id="2b07e-2250">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="2b07e-2250">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="2b07e-2251">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="2b07e-2251">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="2b07e-2252">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="2b07e-2252">0.2.0 - September 2018</span></span>
 <span data-ttu-id="2b07e-2253">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="2b07e-2253">Initial Release</span></span>
