---
title: Azure PowerShell リリース ノート
description: Azure PowerShell モジュールの最新の更新プログラムについて説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: a9c5394a5fac8a8a3de96925b3563776783ea9fe
ms.sourcegitcommit: de813e8a4e3629a6fee6e87a0208c1f0362a16ca
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2020
ms.locfileid: "82080200"
---
# <a name="azure-powershell-release-notes"></a><span data-ttu-id="77eee-103">Azure PowerShell リリース ノート</span><span class="sxs-lookup"><span data-stu-id="77eee-103">Azure PowerShell release notes</span></span>

## <a name="380---april-2020"></a><span data-ttu-id="77eee-104">3.8.0 - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="77eee-104">3.8.0 - April 2020</span></span>
### <a name="highlights-since-the-last-release"></a><span data-ttu-id="77eee-105">前回のリリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-105">Highlights since the last release</span></span>
* <span data-ttu-id="77eee-106">Az.Storage でサポートされる PowerShell のバージョンは次のとおりです。Windows PowerShell 5.1、PowerShell Core 6.2.4+、PowerShell 7</span><span class="sxs-lookup"><span data-stu-id="77eee-106">PowerShell versions that Az.Storage supports: Windows PowerShell 5.1, PowerShell Core 6.2.4+, PowerShell 7</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-107">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-107">Az.Accounts</span></span>
* <span data-ttu-id="77eee-108">'Resolve-AzError' の Azure PowerShell アンケートの URL を更新しました [#11507]</span><span class="sxs-lookup"><span data-stu-id="77eee-108">Updated Azure PowerShell survey URL in 'Resolve-AzError' [#11507]</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="77eee-109">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-109">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-110">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-110">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="77eee-111">GroupId パラメーターの指定について 'Set-AzApiManagementGroup' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-111">'Set-AzApiManagementGroup' Updated documentation to specify the GroupId parameter</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-112">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-112">Az.Cdn</span></span>
* <span data-ttu-id="77eee-113">ChinaCDN 関連の価格 SKU の表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-113">Fixed ChinaCDN related pricing SKU display</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-114">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-114">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-115">ID、暗号化、UserOwnedStorage をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-115">Supported Identity, Encryption, UserOwnedStorage</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-116">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-116">Az.Compute</span></span>
* <span data-ttu-id="77eee-117">'Set-AzVmssOrchestrationServiceState' コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-117">Added 'Set-AzVmssOrchestrationServiceState' cmdlet.</span></span>
* <span data-ttu-id="77eee-118">'Get-AzVmss' に -InstanceView を指定することで、OrchestrationService の状態が表示されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-118">'Get-AzVmss' with -InstanceView shows OrchestrationService states.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-119">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-119">Az.IotHub</span></span>
* <span data-ttu-id="77eee-120">IoT デバイス ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-120">Manage IoT device twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="77eee-121">'Get-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="77eee-121">'Get-AzIotHubDeviceTwin'</span></span>
    - <span data-ttu-id="77eee-122">'Update-AzIotHubDeviceTwin'</span><span class="sxs-lookup"><span data-stu-id="77eee-122">'Update-AzIotHubDeviceTwin'</span></span>
* <span data-ttu-id="77eee-123">Iot Hub のデバイスでダイレクト メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-123">Added cmdlet to invoke direct method on a device in an Iot Hub.</span></span>
* <span data-ttu-id="77eee-124">IoT デバイス モジュール ツインの構成を管理します。新しいコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-124">Manage IoT device module twin configuration, New cmdlets are:</span></span>
    - <span data-ttu-id="77eee-125">'Get-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="77eee-125">'Get-AzIotHubModuleTwin'</span></span>
    - <span data-ttu-id="77eee-126">'Update-AzIotHubModuleTwin'</span><span class="sxs-lookup"><span data-stu-id="77eee-126">'Update-AzIotHubModuleTwin'</span></span>
* <span data-ttu-id="77eee-127">IoT の自動デバイス管理構成を大規模に管理します。</span><span class="sxs-lookup"><span data-stu-id="77eee-127">Manage IoT automatic device management configuration at scale.</span></span> <span data-ttu-id="77eee-128">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-128">New cmdlets are:</span></span>
    - <span data-ttu-id="77eee-129">'Add-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="77eee-129">'Add-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="77eee-130">'Get-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="77eee-130">'Get-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="77eee-131">'Remove-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="77eee-131">'Remove-AzIotHubConfiguration'</span></span>
    - <span data-ttu-id="77eee-132">'Set-AzIotHubConfiguration'</span><span class="sxs-lookup"><span data-stu-id="77eee-132">'Set-AzIotHubConfiguration'</span></span>
* <span data-ttu-id="77eee-133">Iot Hub で edge モジュール メソッドを呼び出すコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-133">Added cmdlet to invoke an edge module method in an Iot Hub.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-134">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-134">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-135">コンテナーでの論理的な削除と消去保護を有効にできる新しいコマンドレット 'Update-AzKeyVault' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-135">Added a new cmdlet 'Update-AzKeyVault' that can enable soft delete and purge protection on a vault</span></span>
* <span data-ttu-id="77eee-136">Microsoft.PowerShell.SecretManagement へのサポートを追加しました [#11178]</span><span class="sxs-lookup"><span data-stu-id="77eee-136">Added support to Microsoft.PowerShell.SecretManagement [#11178]</span></span>
* <span data-ttu-id="77eee-137">'Remove-AzKeyVaultManagedStorageSasDefinition' の例の誤りを修正しました [#11479]</span><span class="sxs-lookup"><span data-stu-id="77eee-137">Fixed error in the examples of 'Remove-AzKeyVaultManagedStorageSasDefinition' [#11479]</span></span>
* <span data-ttu-id="77eee-138">プライベート エンドポイントへのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-138">Added support to private endpoint</span></span>

#### <a name="azmaintenance"></a><span data-ttu-id="77eee-139">Az.Maintenance</span><span class="sxs-lookup"><span data-stu-id="77eee-139">Az.Maintenance</span></span>
* <span data-ttu-id="77eee-140">GA 用のメンテナンス コマンドレットのリリース バージョンを公開しています</span><span class="sxs-lookup"><span data-stu-id="77eee-140">Publishing release version of Maintenance cmdlets for GA</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-141">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-141">Az.Monitor</span></span>
* <span data-ttu-id="77eee-142">プライベート リンク スコープのコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-142">Added cmdlets for private link scope</span></span>
    - <span data-ttu-id="77eee-143">'Get-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="77eee-143">'Get-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="77eee-144">'Remove-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="77eee-144">'Remove-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="77eee-145">'New-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="77eee-145">'New-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="77eee-146">'Update-AzInsightsPrivateLinkScope'</span><span class="sxs-lookup"><span data-stu-id="77eee-146">'Update-AzInsightsPrivateLinkScope'</span></span>
    - <span data-ttu-id="77eee-147">'Get-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="77eee-147">'Get-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="77eee-148">'New-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="77eee-148">'New-AzInsightsPrivateLinkScopedResource'</span></span>
    - <span data-ttu-id="77eee-149">'Remove-AzInsightsPrivateLinkScopedResource'</span><span class="sxs-lookup"><span data-stu-id="77eee-149">'Remove-AzInsightsPrivateLinkScopedResource'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-150">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-150">Az.Network</span></span>
* <span data-ttu-id="77eee-151">仮想ネットワーク ゲートウェイのプライベート IP での接続を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-151">Updated cmdlets to enable connection on private IP for Virtual Network Gateway.</span></span>
    - <span data-ttu-id="77eee-152">'New-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="77eee-152">'New-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="77eee-153">'Set-AzVirtualNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="77eee-153">'Set-AzVirtualNetworkGateway'</span></span>
    - <span data-ttu-id="77eee-154">'New-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="77eee-154">'New-AzVirtualNetworkGatewayConnection'</span></span>
    - <span data-ttu-id="77eee-155">'Set-AzVirtualNetworkGatewayConnection'</span><span class="sxs-lookup"><span data-stu-id="77eee-155">'Set-AzVirtualNetworkGatewayConnection'</span></span>
* <span data-ttu-id="77eee-156">FQDN ベースの LocalNetworkGateways と VpnSites を有効にするコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-156">Updated cmdlets to enable FQDN based LocalNetworkGateways and VpnSites</span></span>
    - <span data-ttu-id="77eee-157">'New-AzLocalNetworkGateway'</span><span class="sxs-lookup"><span data-stu-id="77eee-157">'New-AzLocalNetworkGateway'</span></span>
    - <span data-ttu-id="77eee-158">'New-AzVpnSiteLink'</span><span class="sxs-lookup"><span data-stu-id="77eee-158">'New-AzVpnSiteLink'</span></span>
* <span data-ttu-id="77eee-159">ExpressRouteCircuitConnectionConfig (Global Reach) で IPv6 アドレス ファミリのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-159">Added support for IPv6 address family in ExpressRouteCircuitConnectionConfig (Global Reach)</span></span>
    - <span data-ttu-id="77eee-160">'Set-AzExpressRouteCircuitConnectionConfig' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-160">Added 'Set-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="77eee-161">IPv6CircuitConnectionProperties を含むすべての既存のプロパティを設定できます</span><span class="sxs-lookup"><span data-stu-id="77eee-161">allows setting of all the existing properties including the IPv6CircuitConnectionProperties</span></span>
    - <span data-ttu-id="77eee-162">'Add-AzExpressRouteCircuitConnectionConfig' を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-162">Updated 'Add-AzExpressRouteCircuitConnectionConfig'</span></span>
        - <span data-ttu-id="77eee-163">アドレス プレフィックスのアドレス ファミリを指定する、別の省略可能なパラメーター AddressPrefixType を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-163">Added another optional parameter AddressPrefixType to specify the address family of address prefix</span></span>
* <span data-ttu-id="77eee-164">仮想ネットワーク ゲートウェイ接続で DPD タイムアウトの設定を有効にするコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-164">Updated cmdlets to enable setting of DPD Timeout on Virtual Network Gateway Connections.</span></span>
    - <span data-ttu-id="77eee-165">New-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-165">New-AzVirtualNetworkGatewayConnection</span></span>
    - <span data-ttu-id="77eee-166">Set-AzVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-166">Set-AzVirtualNetworkGatewayConnection</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-167">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-167">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-168">ポリシー コンプライアンス スキャンをトリガーするための 'Start-AzPolicyComplianceScan' コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-168">Added 'Start-AzPolicyComplianceScan' cmdlet for triggering policy compliance scans</span></span>
* <span data-ttu-id="77eee-169">ポリシー定義、セット定義、および割り当てのバージョンを 'Get-AzPolicyState' 出力に追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-169">Added policy definition, set definition, and assignment versions to 'Get-AzPolicyState' output</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-170">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-170">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-171">'New-AzServiceFabricCluster' サンプルのコードのフォーマットと使いやすさが向上しています</span><span class="sxs-lookup"><span data-stu-id="77eee-171">Improved code formatting and usability of 'New-AzServiceFabricCluster' examples</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-172">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-172">Az.Sql</span></span>
* <span data-ttu-id="77eee-173">コマンドレット 'Get-AzSqlInstanceOperation' および 'Stop-AzSqlInstanceOperation' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-173">Added cmdlets 'Get-AzSqlInstanceOperation' and 'Stop-AzSqlInstanceOperation'</span></span>
* <span data-ttu-id="77eee-174">VNet のストレージ アカウントに対する監査をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-174">Supported auditing to a storage account in VNet.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-175">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-175">Az.Storage</span></span>
* <span data-ttu-id="77eee-176">将来のリリースでの Azure File コマンドレット出力の変更に対する破壊的変更の通知を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-176">Added breaking change notice for Azure File cmdlets output change in a future release</span></span>
* <span data-ttu-id="77eee-177">ストレージ アカウントの作成/更新時に新しい SkuName StandardGZRS、StandardRAGZRS をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-177">Supported new SkuName StandardGZRS, StandardRAGZRS when create/update Storage account</span></span>
    - <span data-ttu-id="77eee-178">'New-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="77eee-178">'New-AzStorageAccount'</span></span>
    - <span data-ttu-id="77eee-179">'Set-AzStorageAccount'</span><span class="sxs-lookup"><span data-stu-id="77eee-179">'Set-AzStorageAccount'</span></span>
* <span data-ttu-id="77eee-180">Supported DataLake Gen2</span><span class="sxs-lookup"><span data-stu-id="77eee-180">Supported DataLake Gen2</span></span>
    - <span data-ttu-id="77eee-181">'New-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="77eee-181">'New-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="77eee-182">'Get-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="77eee-182">'Get-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="77eee-183">'Get-AzDataLakeGen2ChildItem'</span><span class="sxs-lookup"><span data-stu-id="77eee-183">'Get-AzDataLakeGen2ChildItem'</span></span>
    - <span data-ttu-id="77eee-184">'Move-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="77eee-184">'Move-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="77eee-185">'Set-AzDataLakeGen2ItemAclObject'</span><span class="sxs-lookup"><span data-stu-id="77eee-185">'Set-AzDataLakeGen2ItemAclObject'</span></span>
    - <span data-ttu-id="77eee-186">'Update-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="77eee-186">'Update-AzDataLakeGen2Item'</span></span>
    - <span data-ttu-id="77eee-187">'Get-AzDataLakeGen2ItemContent'</span><span class="sxs-lookup"><span data-stu-id="77eee-187">'Get-AzDataLakeGen2ItemContent'</span></span>
    - <span data-ttu-id="77eee-188">'Remove-AzDataLakeGen2Item'</span><span class="sxs-lookup"><span data-stu-id="77eee-188">'Remove-AzDataLakeGen2Item'</span></span>

## <a name="0100-preview---april-2020"></a><span data-ttu-id="77eee-189">0.10.0-preview - 2020 年 4 月</span><span class="sxs-lookup"><span data-stu-id="77eee-189">0.10.0-preview - April 2020</span></span>
### <a name="general"></a><span data-ttu-id="77eee-190">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-190">General</span></span>
* <span data-ttu-id="77eee-191">Az モジュールが Azure Stack Hub のプレビューで使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-191">Az modules is now available in preview on Azure Stack Hub.</span></span> <span data-ttu-id="77eee-192">これにより、Linux および macOS とのクロスプラットフォームの互換性が確保されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-192">This allows for cross-platform compatibility with Linux and macOs.</span></span> <span data-ttu-id="77eee-193">Azure Stack Hub で、Az モジュールを使用した PowerShell Core がサポートされるようになりました。詳細については、[こちら](https://aka.ms/az4AzureStack)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-193">Azure Stack Hub now supports PowerShell core with the Az modules, more information [here](https://aka.ms/az4AzureStack)</span></span>
* <span data-ttu-id="77eee-194">Az モジュールでプロファイル 2019-03-01-hybrid がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="77eee-194">Az modules support profile 2019-03-01-hybrid:</span></span>
  - <span data-ttu-id="77eee-195">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="77eee-195">Az.Billing</span></span>
  - <span data-ttu-id="77eee-196">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-196">Az.Compute</span></span>
  - <span data-ttu-id="77eee-197">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="77eee-197">Az.DataBoxEdge</span></span>
  - <span data-ttu-id="77eee-198">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-198">Az.EventHub</span></span>
  - <span data-ttu-id="77eee-199">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-199">Az.IotHub</span></span>
  - <span data-ttu-id="77eee-200">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-200">Az.KeyVault</span></span>
  - <span data-ttu-id="77eee-201">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-201">Az.Monitor</span></span>
  - <span data-ttu-id="77eee-202">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-202">Az.Network</span></span>
  - <span data-ttu-id="77eee-203">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-203">Az.Resources</span></span>
  - <span data-ttu-id="77eee-204">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-204">Az.Storage</span></span>
  - <span data-ttu-id="77eee-205">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-205">Az.Websites</span></span>
* <span data-ttu-id="77eee-206">Azure Stack Hubで動作する、Az 用の 3 つの新しい PowerShell モジュール (Az.Databox、Az.IotHub、Az.EventHu) が導入されました</span><span class="sxs-lookup"><span data-stu-id="77eee-206">Three new PowerShell modules for az have been introduced that work with Azure Stack Hub, which are Az.Databox, Az.IotHub, and Az.EventHub</span></span>
* <span data-ttu-id="77eee-207">コマンドは比較的同じままですが、AzureRM を Az に変更するなどの軽微な変更が加えられています</span><span class="sxs-lookup"><span data-stu-id="77eee-207">Commands remain relatively the same, with minor changes such as changing AzureRM to Az</span></span>
* <span data-ttu-id="77eee-208">Azure Stack Hub の PowerShell ドキュメントへのリンクを更新しました。[こちら](https://aka.ms/InstallASHPowerShell)で確認できます</span><span class="sxs-lookup"><span data-stu-id="77eee-208">Updated link to PowerShell documentation for Azure Stack Hub can be found [here](https://aka.ms/InstallASHPowerShell)</span></span>

## <a name="370---march-2020"></a><span data-ttu-id="77eee-209">3.7.0 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="77eee-209">3.7.0 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-210">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-210">Az.Accounts</span></span>
* <span data-ttu-id="77eee-211">ログインしていない場合に、'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' が NullReferenceException をスローする問題を修正しました [#10292]</span><span class="sxs-lookup"><span data-stu-id="77eee-211">Fixed 'Get-AzTenant'/'Get-AzDefault'/'Set-AzDefault' throw NullReferenceException when not login [#10292]</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-212">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-212">Az.Compute</span></span>
* <span data-ttu-id="77eee-213">'New-AzDiskConfig' コマンドレットに次のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-213">Added the following parameters to 'New-AzDiskConfig' cmdlet:</span></span>
    - <span data-ttu-id="77eee-214">DiskIOPSReadOnly、DiskMBpsReadOnly、MaxSharesCount、GalleryImageReference</span><span class="sxs-lookup"><span data-stu-id="77eee-214">DiskIOPSReadOnly, DiskMBpsReadOnly, MaxSharesCount, GalleryImageReference</span></span>
* <span data-ttu-id="77eee-215">'New-AzGalleryImageVersion' コマンドレットの Target パラメーターで Encryption プロパティを使用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-215">Allowed Encryption property to Target parameter of 'New-AzGalleryImageVersion' cmdlet.</span></span>
* <span data-ttu-id="77eee-216">'Set-AzVmss' の -Reimage と 'Invoke-AzVMReimage' コマンドレットの tempDisk の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-216">Fixed tempDisk issue for 'Set-AzVmss' -Reimage and 'Invoke-AzVMReimage' cmdlets.</span></span> <span data-ttu-id="77eee-217">[#11354]</span><span class="sxs-lookup"><span data-stu-id="77eee-217">[#11354]</span></span>
* <span data-ttu-id="77eee-218">新しい SAP 拡張機能の次のコマンドレットに対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-218">Added support to below cmdlets for new SAP Extension</span></span>
    - <span data-ttu-id="77eee-219">'Set-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="77eee-219">'Set-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="77eee-220">'Get-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="77eee-220">'Get-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="77eee-221">'Remove-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="77eee-221">'Remove-AzVMAEMExtension'</span></span>
    - <span data-ttu-id="77eee-222">'Update-AzVMAEMExtension'</span><span class="sxs-lookup"><span data-stu-id="77eee-222">'Update-AzVMAEMExtension'</span></span>
* <span data-ttu-id="77eee-223">ヘルプ ドキュメントの例の誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-223">Fixed errors in examples of help document</span></span>
* <span data-ttu-id="77eee-224">VM PowerState の正確な文字列値をテーブル形式で示しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-224">Showed the exact string value for VM PowerState in the table format.</span></span>
* <span data-ttu-id="77eee-225">'New-AzVmssConfig': SinglePlacementGroup が無効な場合の AutomaticRepairs プロパティのシリアル化を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-225">'New-AzVmssConfig': fixed serialization of AutomaticRepairs property when SinglePlacementGroup is disabled.</span></span> <span data-ttu-id="77eee-226">[#11257]</span><span class="sxs-lookup"><span data-stu-id="77eee-226">[#11257]</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-227">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-227">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-228">ADF .Net SDK のバージョンを 4.8.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-228">Updated ADF .Net SDK version to 4.8.0</span></span>
* <span data-ttu-id="77eee-229">再実行をサポートするために、'Invoke-AzDataFactoryV2Pipeline' コマンドに省略可能なパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-229">Added optional parameters to 'Invoke-AzDataFactoryV2Pipeline' command to support rerun</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-230">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-230">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-231">'Export-AzDataLakeStoreItem' と 'Import-AzDataLakeStoreItem' に破壊的変更の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-231">Added breaking change description for 'Export-AzDataLakeStoreItem' and 'Import-AzDataLakeStoreItem'</span></span>
* <span data-ttu-id="77eee-232">'New-AzDataLakeStoreItem'、'Add-AzDAtaLakeStoreItemContent'、および 'Get-AzDAtaLakeStoreItemContent' にバイト エンコードのオプションを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-232">Added option of Byte encoding for 'New-AzDataLakeStoreItem', 'Add-AzDAtaLakeStoreItemContent', and 'Get-AzDAtaLakeStoreItemContent'</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="77eee-233">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-233">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-234">クラスターの作成時に、最低限サポートされている TLS バージョンの指定をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-234">Supported specifying minimal supported TLS version when creating cluster.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-235">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-235">Az.IotHub</span></span>
* <span data-ttu-id="77eee-236">デバイスごとの分散設定の管理のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-236">Added support to manage distributed settings per-device.</span></span> <span data-ttu-id="77eee-237">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-237">New Cmdlets are:</span></span>
    - <span data-ttu-id="77eee-238">'Get-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="77eee-238">'Get-AzIotHubDistributedTracing'</span></span>
    - <span data-ttu-id="77eee-239">'Set-AzIotHubDistributedTracing'</span><span class="sxs-lookup"><span data-stu-id="77eee-239">'Set-AzIotHubDistributedTracing'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-240">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-240">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-241">'New-AzKeyVault' に破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-241">Added breaking change attributes to 'New-AzKeyVault'</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-242">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-242">Az.Monitor</span></span>
* <span data-ttu-id="77eee-243">'New-AzScheduledQueryRuleLogMetricTrigger' のドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-243">Updated documentation for 'New-AzScheduledQueryRuleLogMetricTrigger'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-244">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-244">Az.Network</span></span>
* <span data-ttu-id="77eee-245">テナント間の VirtualHubVnetConnections を許可するためにコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-245">Updated cmdlets to allow cross-tenant VirtualHubVnetConnections</span></span>
    - <span data-ttu-id="77eee-246">'New-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="77eee-246">'New-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="77eee-247">'Update-AzVirtualHubVnetConnection'</span><span class="sxs-lookup"><span data-stu-id="77eee-247">'Update-AzVirtualHubVnetConnection'</span></span>
    - <span data-ttu-id="77eee-248">'New-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="77eee-248">'New-AzVirtualHub'</span></span>
    - <span data-ttu-id="77eee-249">'Update-AzVirtualHub'</span><span class="sxs-lookup"><span data-stu-id="77eee-249">'Update-AzVirtualHub'</span></span>
* <span data-ttu-id="77eee-250">SQL 管理 SDK の依存関係を削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-250">Removed Sql Management SDK dependency</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-251">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-251">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-252">エラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-252">Improved error messages</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-253">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-253">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-254">Azure Site Recovery で再保護を行うためのサポートを追加し、Azure Disk Encryption を使用して暗号化されている Virtual Machines の vm プロパティを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-254">Azure Site Recovery added support for doing reprotect and updated vm properties for Azure disk encrypted Virtual Machines.</span></span>
* <span data-ttu-id="77eee-255">Azure Site Recovery に VmwareToAzure プロパティの DR 監視を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-255">Added Azure Site Recovery VmwareToAzure properties DR monitoring</span></span>
* <span data-ttu-id="77eee-256">Azure Backup に、失敗した項目の再試行ポリシー更新のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-256">Azure Backup added support for retrying policy update for failed items.</span></span>
* <span data-ttu-id="77eee-257">Azure Backup に、バックアップおよび復元中のディスク除外設定のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-257">Azure Backup Added support for disk exclusion settings during backup and restore.</span></span>
* <span data-ttu-id="77eee-258">Azure Backup に、AzureFileShare で複数ファイル/フォルダーを復元するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-258">Azure Backup Added Support for Restoring Multiple files/folders in AzureFileShare</span></span>
* <span data-ttu-id="77eee-259">Azure Backup に、IaasVM ポリシーの更新中にユーザーによって指定された Resourcegroup へのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-259">Azure Backup Added support for User-specified Resourcegroup support while updating IaasVM Policy</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-260">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-260">Az.Resources</span></span>
* <span data-ttu-id="77eee-261">既定の apiVersion ではなく、リソースの実際の apiVersion を使用するように 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' を修正しました [#11267]</span><span class="sxs-lookup"><span data-stu-id="77eee-261">Fixed 'Get-AzResource -ResourceGroupName -Name -ExpandProperties -ResourceType' to use actual apiVersion of resources instead of default apiVersion [#11267]</span></span>
* <span data-ttu-id="77eee-262">エラー シナリオでの correlationId のログ記録を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-262">Added correlationId logging for error scenarios</span></span>
* <span data-ttu-id="77eee-263">'Get-AzResourceLock' のドキュメントをわずかに変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-263">Small documentation change to 'Get-AzResourceLock'.</span></span> <span data-ttu-id="77eee-264">例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-264">Added example.</span></span>
* <span data-ttu-id="77eee-265">'Get-AzADUser' のパラメーター値の単一引用符をエスケープしました [#11317]</span><span class="sxs-lookup"><span data-stu-id="77eee-265">Escaped single quote in parameter value of 'Get-AzADUser' [#11317]</span></span>
* <span data-ttu-id="77eee-266">デプロイ スクリプト ('Get-AzDeploymentScript'、'Get-AzDeploymentScriptLog'、'Save-AzDeploymentScriptLog'、'Remove-AzDeploymentScript') に新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-266">Added new cmdlets for Deployment Scripts ('Get-AzDeploymentScript', 'Get-AzDeploymentScriptLog', 'Save-AzDeploymentScriptLog', 'Remove-AzDeploymentScript')</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-267">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-267">Az.Sql</span></span>
* <span data-ttu-id="77eee-268">'Invoke-AzSqlDatabaseFailover' に読み取り可能なセカンダリ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-268">Added readable secondary parameter to 'Invoke-AzSqlDatabaseFailover'</span></span>
* <span data-ttu-id="77eee-269">コマンドレット 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-269">Added cmdlet 'Disable-AzSqlServerActiveDirectoryOnlyAuthentication'</span></span>
* <span data-ttu-id="77eee-270">データベース内の列を分類するときの秘密度ランクを保存しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-270">Saved sensitivity rank when classifying columns in the database.</span></span>

#### <a name="azsupport"></a><span data-ttu-id="77eee-271">Az.Support</span><span class="sxs-lookup"><span data-stu-id="77eee-271">Az.Support</span></span>
* <span data-ttu-id="77eee-272">'Az.Support' モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="77eee-272">General availability of 'Az.Support' module</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-273">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-273">Az.Websites</span></span>
* <span data-ttu-id="77eee-274">次の新しいコマンドレットを使用して、webapp トラフィック ルーティング規則を処理するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-274">Added support for working with webapp Traffic Routing Rules via below new cmdlets</span></span>
    - <span data-ttu-id="77eee-275">'Get-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="77eee-275">'Get-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="77eee-276">'Update-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="77eee-276">'Update-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="77eee-277">'Add-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="77eee-277">'Add-AzWebAppTrafficRouting'</span></span>
    - <span data-ttu-id="77eee-278">'Remove-AzWebAppTrafficRouting'</span><span class="sxs-lookup"><span data-stu-id="77eee-278">'Remove-AzWebAppTrafficRouting'</span></span>

## <a name="361---march-2020"></a><span data-ttu-id="77eee-279">3.6.1 - 2020 年 3 月</span><span class="sxs-lookup"><span data-stu-id="77eee-279">3.6.1 - March 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-280">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-280">Az.Accounts</span></span>
* <span data-ttu-id="77eee-281">'Send-Feedback' で Azure PowerShell アンケート ページを開きます [#11020]</span><span class="sxs-lookup"><span data-stu-id="77eee-281">Open Azure PowerShell survey page in 'Send-Feedback' [#11020]</span></span>
* <span data-ttu-id="77eee-282">'Resolve-Error' に Azure PowerShell アンケートの URL を表示します [#11021]</span><span class="sxs-lookup"><span data-stu-id="77eee-282">Display Azure PowerShell survey URL in 'Resolve-Error' [#11021]</span></span>
* <span data-ttu-id="77eee-283">UserAgent で Az バージョンを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-283">Added Az version in UserAgent</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="77eee-284">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-284">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-285">DeveloperPortal エンドポイントでカスタム ドメインを取得および構成するためのサポートを追加しました [#11007]</span><span class="sxs-lookup"><span data-stu-id="77eee-285">Added support for retrieving and configuring Custom Domain on the DeveloperPortal Endpoint [#11007]</span></span>
* <span data-ttu-id="77eee-286">'Export-AzApiManagementApi' で、JSON 形式で API 定義をダウンロードするためのサポートを追加しました [#9987]</span><span class="sxs-lookup"><span data-stu-id="77eee-286">'Export-AzApiManagementApi' Added support for downloading Api Definition in Json format [#9987]</span></span>
* <span data-ttu-id="77eee-287">'Import-AzApiManagementApi' で、JSON ドキュメントから OpenApi 3.0 定義をインポートするためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-287">'Import-AzApiManagementApi' Added support for importing OpenApi 3.0 definition from Json document</span></span>
* <span data-ttu-id="77eee-288">'New-AzApiManagementIdentityProvider' および 'Set-AzApiManagementIdentityProvider' で、AAD B2C プロバイダーの 'サインイン テナント' を構成するためのサポートを追加しました [#9784]</span><span class="sxs-lookup"><span data-stu-id="77eee-288">'New-AzApiManagementIdentityProvider' and 'Set-AzApiManagementIdentityProvider' Added support for configuring 'Signin Tenant' for AAD B2C Provider [#9784]</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-289">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-289">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-290">csproj および psd1 で明示的に System.Buffers への参照を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-290">Added reference to System.Buffers explicitly in csproj and psd1.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-291">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-291">Az.IotHub</span></span>
* <span data-ttu-id="77eee-292">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-292">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="77eee-293">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-293">New Cmdlets are:</span></span>
    - <span data-ttu-id="77eee-294">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-294">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="77eee-295">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-295">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="77eee-296">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-296">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="77eee-297">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-297">'Set-AzIotHubDevice'</span></span>
* <span data-ttu-id="77eee-298">Iot Hub のターゲット Iot デバイスでモジュールを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-298">Added support to manage modules on a target Iot device in an Iot Hub.</span></span> <span data-ttu-id="77eee-299">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-299">New Cmdlets are:</span></span>
    - <span data-ttu-id="77eee-300">'Add-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="77eee-300">'Add-AzIotHubModule'</span></span>
    - <span data-ttu-id="77eee-301">'Get-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="77eee-301">'Get-AzIotHubModule'</span></span>
    - <span data-ttu-id="77eee-302">'Remove-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="77eee-302">'Remove-AzIotHubModule'</span></span>
    - <span data-ttu-id="77eee-303">'Set-AzIotHubModule'</span><span class="sxs-lookup"><span data-stu-id="77eee-303">'Set-AzIotHubModule'</span></span>
* <span data-ttu-id="77eee-304">Iot Hub 内のターゲット IoT デバイスの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-304">Added cmdlet to get the connection string of a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="77eee-305">Iot Hub 内のターゲット IoT デバイス上のモジュールの接続文字列を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-305">Added cmdlet to get the connection string of a module on a target IoT device in an Iot Hub.</span></span>
* <span data-ttu-id="77eee-306">IoT デバイスの親デバイスを取得/設定するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-306">Added support to get/set parent device of an IoT device.</span></span> <span data-ttu-id="77eee-307">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-307">New Cmdlets are:</span></span>
    - <span data-ttu-id="77eee-308">'Get-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="77eee-308">'Get-AzIotHubDeviceParent'</span></span>
    - <span data-ttu-id="77eee-309">'Set-AzIotHubDeviceParent'</span><span class="sxs-lookup"><span data-stu-id="77eee-309">'Set-AzIotHubDeviceParent'</span></span>
* <span data-ttu-id="77eee-310">デバイスの親子関係を管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-310">Added support to manage device parent-child relationship.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-311">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-311">Az.Monitor</span></span>
* <span data-ttu-id="77eee-312">'Get-AzMetricDefinition' の出力値を修正しました [#9714]</span><span class="sxs-lookup"><span data-stu-id="77eee-312">Fixed output value for 'Get-AzMetricDefinition' [#9714]</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-313">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-313">Az.Network</span></span>
* <span data-ttu-id="77eee-314">SQL 管理 SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-314">Updated Sql Management SDK.</span></span>
* <span data-ttu-id="77eee-315">PrivateLinkServiceConnectionState クラスの naming-difference の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-315">Fixed a naming-difference issue in PrivateLinkServiceConnectionState class.</span></span>
    - <span data-ttu-id="77eee-316">フィールド ActionRequired を ActionRequired にマップしています。</span><span class="sxs-lookup"><span data-stu-id="77eee-316">Mapping the field ActionsRequired to ActionRequired.</span></span>
* <span data-ttu-id="77eee-317">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-317">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-318">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-318">Az.Resources</span></span>
* <span data-ttu-id="77eee-319">'Get-AzRoleAssignment' で null 参照のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-319">Fixed for null reference bug in 'Get-AzRoleAssignment'</span></span>
* <span data-ttu-id="77eee-320">'Remove-AzADGroup' でスイッチ '-Force ' および '-PassThru ' に省略可能のマークを付けました [#10849]</span><span class="sxs-lookup"><span data-stu-id="77eee-320">Marked switch '-Force' and '-PassThru' optional in 'Remove-AzADGroup' [#10849]</span></span>
* <span data-ttu-id="77eee-321">'MailNickname' が 'Remove-AzADGroup' で返さない問題を修正しました [#11167]</span><span class="sxs-lookup"><span data-stu-id="77eee-321">Fixed issue that 'MailNickname' doesn't return in 'Remove-AzADGroup' [#11167]</span></span>
* <span data-ttu-id="77eee-322">'Remove-AzADGroup' パイプ操作が機能しない問題を修正しました [#11171]</span><span class="sxs-lookup"><span data-stu-id="77eee-322">Fixed issue that 'Remove-AzADGroup' pipe operation doesn't work [#11171]</span></span>
* <span data-ttu-id="77eee-323">GetAzureRoleAssignmentCommand の null 参照のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-323">Fixed for null reference bug in GetAzureRoleAssignmentCommand</span></span>
* <span data-ttu-id="77eee-324">ポリシー コマンドレットの今後の変更について、破壊的変更の属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-324">Added breaking change attributes for upcoming changes to policy cmdlets</span></span>
* <span data-ttu-id="77eee-325">サーバー側でリソース グループ タグのフィルター処理を実行するように 'Get-AzResourceGroup' を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-325">Updated 'Get-AzResourceGroup' to perform resource group tag filtering on server-side</span></span>
* <span data-ttu-id="77eee-326">タグ コマンドレットで -ResourceId を受け入れるように拡張しました</span><span class="sxs-lookup"><span data-stu-id="77eee-326">Extended Tag cmdlets to accept -ResourceId</span></span>
    - <span data-ttu-id="77eee-327">Get-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="77eee-327">Get-AzTag -ResourceId</span></span>
    - <span data-ttu-id="77eee-328">New-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="77eee-328">New-AzTag -ResourceId</span></span>
    - <span data-ttu-id="77eee-329">Remove-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="77eee-329">Remove-AzTag -ResourceId</span></span>
* <span data-ttu-id="77eee-330">新しいタグ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-330">Added new Tag cmdlet</span></span>
    - <span data-ttu-id="77eee-331">Update-AzTag -ResourceId</span><span class="sxs-lookup"><span data-stu-id="77eee-331">Update-AzTag -ResourceId</span></span>
* <span data-ttu-id="77eee-332">SDK 3.3.0 から ScopedDeployment を導入しました</span><span class="sxs-lookup"><span data-stu-id="77eee-332">Brought ScopedDeployment from SDK 3.3.0</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-333">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-333">Az.Sql</span></span>
* <span data-ttu-id="77eee-334">'New-AzSqlServer' と 'Set-AzSqlServer' に PublicNetworkAccess を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-334">Added PublicNetworkAccess to 'New-AzSqlServer' and 'Set-AzSqlServer'</span></span>
* <span data-ttu-id="77eee-335">マネージド データベースの長期的な保有期間のバックアップ構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-335">Added support for Long Term Retention backup configuration for Managed Databases</span></span>
    - <span data-ttu-id="77eee-336">マネージド データベースで LTR ポリシーを取得/設定します</span><span class="sxs-lookup"><span data-stu-id="77eee-336">Get/Set LTR policy on a managed database</span></span>
    - <span data-ttu-id="77eee-337">マネージド データベース、マネージド インスタンス、または場所で LTR バックアップを取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-337">Get LTR backup(s) by managed database, managed instance, or by location</span></span>
    - <span data-ttu-id="77eee-338">LTR バックアップを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-338">Remove an LTR backup</span></span>
    - <span data-ttu-id="77eee-339">LTR バックアップを復元して新しいマネージド データベースを作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-339">Restore an LTR backup to create a new managed database</span></span>
* <span data-ttu-id="77eee-340">New-AzSqlServer と Set-AzSqlServer に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-340">Added MinimalTlsVersion to New-AzSqlServer and Set-AzSqlServer</span></span>
* <span data-ttu-id="77eee-341">New-AzSqlInstance と Set-AzSqlInstance に MinimalTlsVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-341">Added MinimalTlsVersion to New-AzSqlInstance and Set-AzSqlInstance</span></span>
* <span data-ttu-id="77eee-342">Az.Network の SQL SDK のバージョンを上げました</span><span class="sxs-lookup"><span data-stu-id="77eee-342">Bumped SQL SDK version for Az.Network</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-343">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-343">Az.Storage</span></span>
* <span data-ttu-id="77eee-344">ImmutabilityPolicy で AllowProtectedAppendWrite をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-344">Supported AllowProtectedAppendWrite in ImmutabilityPolicy</span></span>
    - <span data-ttu-id="77eee-345">'Set-AzRmStorageContainerImmutabilityPolicy'</span><span class="sxs-lookup"><span data-stu-id="77eee-345">'Set-AzRmStorageContainerImmutabilityPolicy'</span></span>
* <span data-ttu-id="77eee-346">将来のリリースでの AzureStorageTable 型の変更に対する破壊的変更の警告メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-346">Added breaking change warning message for AzureStorageTable type change in a future release</span></span>
    - <span data-ttu-id="77eee-347">'New-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="77eee-347">'New-AzStorageTable'</span></span>
    - <span data-ttu-id="77eee-348">'Get-AzStorageTable'</span><span class="sxs-lookup"><span data-stu-id="77eee-348">'Get-AzStorageTable'</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-349">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-349">Az.Websites</span></span>
* <span data-ttu-id="77eee-350">'New-AzAppServicePlan' と 'Set-AzAppServicePlan' の Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-350">Added Tag parameter for 'New-AzAppServicePlan' and 'Set-AzAppServicePlan'</span></span>
* <span data-ttu-id="77eee-351">Web サイトにカスタム ドメインを追加するときに例外がスローされた場合、コマンドレットの実行を停止します</span><span class="sxs-lookup"><span data-stu-id="77eee-351">Stop cmdlet execution if an exception is thrown when adding a custom domain to a website</span></span>
* <span data-ttu-id="77eee-352">App Service プランと同じリソース グループに含まれていない App Services の操作を実行するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-352">Added support to perform operations for App Services not in the same resource group as the App Service Plan</span></span>
* <span data-ttu-id="77eee-353">異なるリソース グループ内の WebApp/Function へのアクセス制限を適用しました</span><span class="sxs-lookup"><span data-stu-id="77eee-353">Applied access restriction to WebApp/Function in different resource groups</span></span>
* <span data-ttu-id="77eee-354">WebAppSlots のカスタム ホスト名を設定するための問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-354">Fixed issue to set custom hostnames for WebAppSlots</span></span>

## <a name="350---february-2020"></a><span data-ttu-id="77eee-355">3.5.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="77eee-355">3.5.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="77eee-356">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-356">Highlights since the last major release</span></span>
* <span data-ttu-id="77eee-357">クライアント側のテレメトリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-357">Updated client side telemetry.</span></span>
* <span data-ttu-id="77eee-358">Az.IotHub に、デバイスの管理をサポートするコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-358">Az.IotHub added cmdlets to support to manage devices.</span></span>
* <span data-ttu-id="77eee-359">Az.SqlVirtualMachine に、可用性グループ リスナー用のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-359">Az.SqlVirtualMachine added cmdlets for Availability Group Listener.</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-360">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-360">Az.Accounts</span></span>
* <span data-ttu-id="77eee-361">クライアント側テレメトリのデータに SubscriptionId、TenantId および実行時間を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-361">Added SubscriptionId, TenantId, and execution time into data of client side telemetry</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-362">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-362">Az.Automation</span></span>
* <span data-ttu-id="77eee-363">'New-AzAutomationSoftwareUpdateConfiguration' のリファレンス ドキュメントの例 1 で、タイプミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-363">Fixed typo in Example 1 in reference documentation for 'New-AzAutomationSoftwareUpdateConfiguration'</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-364">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-364">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-365">SDK を 7.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-365">Updated SDK to 7.0</span></span>
* <span data-ttu-id="77eee-366">サーバーが空の本文を応答する場合のエラー メッセージを改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-366">Improved error message when server responses empty body</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-367">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-367">Az.Compute</span></span>
* <span data-ttu-id="77eee-368">更新中に ProximityPlacementGroupId で空の値を許可するようにしました</span><span class="sxs-lookup"><span data-stu-id="77eee-368">Allowed empty value for ProximityPlacementGroupId during update</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="77eee-369">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-369">Az.FrontDoor</span></span>
* <span data-ttu-id="77eee-370">WAF で使用できるマネージド ルールの定義を取得するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-370">Added cmdlet to get managed rule definitions that can be used in WAF</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-371">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-371">Az.IotHub</span></span>
* <span data-ttu-id="77eee-372">Iot Hub でデバイスを管理するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-372">Added support to manage devices in an Iot Hub.</span></span> <span data-ttu-id="77eee-373">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-373">New Cmdlets are:</span></span>
    - <span data-ttu-id="77eee-374">'Add-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-374">'Add-AzIotHubDevice'</span></span>
    - <span data-ttu-id="77eee-375">'Get-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-375">'Get-AzIotHubDevice'</span></span>
    - <span data-ttu-id="77eee-376">'Remove-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-376">'Remove-AzIotHubDevice'</span></span>
    - <span data-ttu-id="77eee-377">'Set-AzIotHubDevice'</span><span class="sxs-lookup"><span data-stu-id="77eee-377">'Set-AzIotHubDevice'</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-378">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-378">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-379">Add-AzKeyVaultKey.md の重複するテキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-379">Fixed duplicated text for Add-AzKeyVaultKey.md</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-380">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-380">Az.Monitor</span></span>
* <span data-ttu-id="77eee-381">Get-AzLog コマンドレットの説明を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-381">Fixed description of the Get-AzLog cmdlet.</span></span>
* <span data-ttu-id="77eee-382">ActionGroupId という名前の新しいパラメーターが、'New-AzMetricAlertRuleV2' コマンドに追加されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-382">A new parameter called ActionGroupId was added to 'New-AzMetricAlertRuleV2' command.</span></span>
    - <span data-ttu-id="77eee-383">ユーザーは、ActionGroupId(string) または ActionGorup(ActivityLogAlertActionGroup) のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-383">The user can provide either ActionGroupId(string) or ActionGorup(ActivityLogAlertActionGroup).</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-384">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-384">Az.Network</span></span>
* <span data-ttu-id="77eee-385">'New-AzPrivateLinkService' コマンドレットのパラメーター '-EnableProxyProtocol' にパラメーターのノートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-385">Added one extra parameter note for parameter '-EnableProxyProtocol' for 'New-AzPrivateLinkService' cmdlet.</span></span>
* <span data-ttu-id="77eee-386">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md の FilterData 例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-386">Fixed FilterData example in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="77eee-387">Start-AzVirtualNetworkGatewayConnectionPacketCapture.md と Start-AzVirtualnetworkGatewayPacketCapture.md ですべての内部および外部パケットをキャプチャするパケット キャプチャの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-387">Added Packet Capture example for capture all inner and outer packets in Start-AzVirtualNetworkGatewayConnectionPacketCapture.md and Start-AzVirtualnetworkGatewayPacketCapture.md.</span></span>
* <span data-ttu-id="77eee-388">VNet ファイアウォールで Azure Firewall ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-388">Supported Azure Firewall Policy on VNet Firewalls</span></span>
    - <span data-ttu-id="77eee-389">新たに追加されたコマンドレットはありません。</span><span class="sxs-lookup"><span data-stu-id="77eee-389">No new cmdlets are added.</span></span> <span data-ttu-id="77eee-390">VNet ファイアウォールでのファイアウォール ポリシーの制限を緩和します</span><span class="sxs-lookup"><span data-stu-id="77eee-390">Relaxing the restriction for firewall policy on VNet firewalls</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-391">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-391">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-392">SQL Database でファイルとして復元のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-392">Added Support for Restore-as-files for SQL Databases.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-393">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-393">Az.Resources</span></span>
* <span data-ttu-id="77eee-394">テンプレート デプロイのコマンドレットをリファクターしました</span><span class="sxs-lookup"><span data-stu-id="77eee-394">Refactored template deployment cmdlets</span></span>
    - <span data-ttu-id="77eee-395">管理グループでデプロイを管理するための新しいコマンドレットを追加しました: \*-AzManagementGroupDeployment</span><span class="sxs-lookup"><span data-stu-id="77eee-395">Added new cmdlets for managing deployments at management group: \*-AzManagementGroupDeployment</span></span>
    - <span data-ttu-id="77eee-396">テナントの範囲でデプロイを管理するための新しいコマンドレットを追加しました: \*-AzTenantDeployment</span><span class="sxs-lookup"><span data-stu-id="77eee-396">Added new cmdlets for managing deployments at tenant scope: \*-AzTenantDeployment</span></span>
    - <span data-ttu-id="77eee-397">\*-AzDeployment コマンドレットをリファクターしてサブスクリプションの範囲で動作するようにしました</span><span class="sxs-lookup"><span data-stu-id="77eee-397">Refactored \*-AzDeployment cmdlets to work specifically at subscription scope</span></span>
    - <span data-ttu-id="77eee-398">\*-AzDeployment コマンドレット用の別名 \*-AzSubscriptionDeployment を作成しました</span><span class="sxs-lookup"><span data-stu-id="77eee-398">Created aliases \*-AzSubscriptionDeployment for \*-AzDeployment cmdlets</span></span>
* <span data-ttu-id="77eee-399">パラメーター 'AvailableToOtherTenants' が設定されていない場合の 'Update-AzADApplication' を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-399">Fixed 'Update-AzADApplication' when parameter 'AvailableToOtherTenants' is not set</span></span>
* <span data-ttu-id="77eee-400">AmbiguousParameterSetException を回避するために ApplicationObjectWithoutCredentialParameterSet を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-400">Removed ApplicationObjectWithoutCredentialParameterSet to avoid AmbiguousParameterSetException.</span></span>
* <span data-ttu-id="77eee-401">ヘルプ ファイルを再生成しました</span><span class="sxs-lookup"><span data-stu-id="77eee-401">Regenerated help files</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-402">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-402">Az.Sql</span></span>
* <span data-ttu-id="77eee-403">Managed Instance でのクロス サブスクリプションのポイントインタイム リストアのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-403">Added support for cross subscription point in time restore on Managed Instances.</span></span>
* <span data-ttu-id="77eee-404">既存の SQL Managed Instance ハードウェアの世代変更のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-404">Added support for changing existing Sql Managed Instance hardware generation</span></span>
* <span data-ttu-id="77eee-405">'Update-AzSqlServerVulnerabilityAssessmentSetting' のヘルプの例を修正しました: パラメーター/プロパティの出力 - EmailAdmins</span><span class="sxs-lookup"><span data-stu-id="77eee-405">Fixed 'Update-AzSqlServerVulnerabilityAssessmentSetting' help examples: parameter/property output - EmailAdmins</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="77eee-406">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="77eee-406">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="77eee-407">可用性グループ リスナー用のコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-407">Added cmdlets for Availability Group Listener</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="77eee-408">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="77eee-408">Az.StorageSync</span></span>
* <span data-ttu-id="77eee-409">'Invoke-AzStorageSyncCompatibilityCheck' でサポートされている文字セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-409">Updated supported character sets in 'Invoke-AzStorageSyncCompatibilityCheck'.</span></span>

## <a name="340---february-2020"></a><span data-ttu-id="77eee-410">3.4.0 - 2020 年 2 月</span><span class="sxs-lookup"><span data-stu-id="77eee-410">3.4.0 - February 2020</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="77eee-411">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-411">Highlights since the last major release</span></span>
* <span data-ttu-id="77eee-412">Az.CosmosDB 初期バージョン 0.1.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="77eee-412">Az.CosmosDB initial version 0.1.0 released</span></span>
* <span data-ttu-id="77eee-413">Az.Network ConnectionMonitor V2 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-413">Az.Network ConnectionMonitor V2 support added</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-414">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-414">Az.Accounts</span></span>
* <span data-ttu-id="77eee-415">AzureRmContext.json が使用できないときにコンテキストの自動保存を無効にします</span><span class="sxs-lookup"><span data-stu-id="77eee-415">Disable context auto saving when AzureRmContext.json not available</span></span>
* <span data-ttu-id="77eee-416">Azure Powershell Common の参照を 1.3.5-preview に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-416">Update the reference to Azure Powershell Common to 1.3.5-preview</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="77eee-417">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-417">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-418">**Get-AzApiManagementApiSchema** API に関連付けられたOpen-Api スキーマの取得を修正しました https://github.com/Azure/azure-powershell/issues/10626</span><span class="sxs-lookup"><span data-stu-id="77eee-418">**Get-AzApiManagementApiSchema** Fixed getting Open-Api Schema associated with an API   https://github.com/Azure/azure-powershell/issues/10626</span></span>
* <span data-ttu-id="77eee-419">**New-AzApiManagementProduct**\* および **Set-AzApiManagementProduct**</span><span class="sxs-lookup"><span data-stu-id="77eee-419">**New-AzApiManagementProduct**\* and **Set-AzApiManagementProduct**</span></span>
  - <span data-ttu-id="77eee-420">https://github.com/Azure/azure-powershell/issues/10472 のドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-420">Fix documentation for https://github.com/Azure/azure-powershell/issues/10472</span></span>
* <span data-ttu-id="77eee-421">**Set-AzApiManagementApi** コマンドレットを使用して ServiceUrl を更新する方法を示す例を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-421">**Set-AzApiManagementApi** Added example to show how to update the ServiceUrl using the cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-422">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-422">Az.Compute</span></span>
* <span data-ttu-id="77eee-423">Get-AzVM -Status がVM 名なしで実行される場合にスロットルを回避するために、VM 状態の数を 100 に制限します。</span><span class="sxs-lookup"><span data-stu-id="77eee-423">Limit the number of VM status to 100 to avoid throttling when Get-AzVM -Status is performed without VM name.</span></span>
* <span data-ttu-id="77eee-424">Update-AzDiskEncryptionSet コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-424">Add Update-AzDiskEncryptionSet cmdlet</span></span>
* <span data-ttu-id="77eee-425">EncryptionType と DiskEncryptionSetId パラメーターを次のコマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-425">Add EncryptionType and DiskEncryptionSetId parameters to the following cmdlets:</span></span>
    - <span data-ttu-id="77eee-426">New-AzDiskUpdateConfig、New-AzSnapshotUpdateConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-426">New-AzDiskUpdateConfig, New-AzSnapshotUpdateConfig</span></span>
* <span data-ttu-id="77eee-427">ColocationStatus パラメーターを Get-AzProximityPlacementGroup コマンドレットに追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-427">Add ColocationStatus parameter to Get-AzProximityPlacementGroup cmdlet.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-428">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-428">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-429">ADF .Net SDK のバージョンを 4.7.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-429">Update ADF .Net SDK version to 4.7.0</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="77eee-430">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="77eee-430">Az.DeploymentManager</span></span>
* <span data-ttu-id="77eee-431">リソースの LIST 操作を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-431">Adds LIST operations for resources</span></span>
* <span data-ttu-id="77eee-432">正常性チェック ステップで操作を実行するための機能を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-432">Adds capability for performing operations on Health Check steps</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="77eee-433">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-433">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-434">New-AzHDInsightCluster のドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-434">Fix document error of New-AzHDInsightCluster.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-435">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-435">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-436">名前エイリアスを VaultName 属性に追加して、Remove-AzureKeyVault を New-AzureKeyVault と一致させます。</span><span class="sxs-lookup"><span data-stu-id="77eee-436">Add Name alias to VaultName attribute to make Remove-AzureKeyVault consistent with New-AzureKeyVault.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-437">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-437">Az.Network</span></span>
* <span data-ttu-id="77eee-438">Traffic Analytics が無効なシナリオを示すために、Set-AzNetworkWatcherConfigFlowLog.md に新しい例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-438">New example added to Set-AzNetworkWatcherConfigFlowLog.md to demonstrate Traffic Analytics disable scenario.</span></span>
* <span data-ttu-id="77eee-439">管理 IP 構成を Azure Firewall に割り当てるサポートを追加します: ファイアウォールが管理トラフィックに使用する専用サブネットとパブリック IP</span><span class="sxs-lookup"><span data-stu-id="77eee-439">Add support for assigning management IP configuration to Azure Firewall - a dedicated subnet and Public IP that the firewall will use for its management traffic</span></span>
    - <span data-ttu-id="77eee-440">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="77eee-440">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="77eee-441">パブリック IP アドレス オブジェクトを受け入れるパラメーター -ManagementPublicIpAddress (必須でない) を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-441">Added parameter -ManagementPublicIpAddress (not mandatory) which accepts a Public IP Address object</span></span>
        - <span data-ttu-id="77eee-442">ファイアウォール オブジェクトにメソッド SetManagementIpConfiguration を追加しました。サブネットとパブリック IP アドレスが入力として必要です。サブネット名は 'AzureFirewallManagementSubnet' でなければなりません</span><span class="sxs-lookup"><span data-stu-id="77eee-442">Added method SetManagementIpConfiguration on firewall object - requires a subnet and a Public IP address as input - subnet name must be 'AzureFirewallManagementSubnet'</span></span>
* <span data-ttu-id="77eee-443">ネットワーク インターフェイスではなく NSG の例を示すために、Get-AzNetworkSecurityGroup の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-443">Corrected Get-AzNetworkSecurityGroup examples to show examples for NSG's instead of network interfaces.</span></span>
* <span data-ttu-id="77eee-444">New-AzVpnSite コマンドで、リソース ID 補完機能がパラメーターを完了できない入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-444">Fixed typo in New-AzVpnSite command that was preventing resource id completer from completing a parameter.</span></span>
* <span data-ttu-id="77eee-445">Application Gateway での Rewrite Rules Action Set の URL 構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-445">Added support for Url Confiugration in Rewrite Rules Action Set in the Application Gateway</span></span>
    - <span data-ttu-id="77eee-446">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-446">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-447">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span><span class="sxs-lookup"><span data-stu-id="77eee-447">New-AzApplicationGatewayRewriteRuleUrlConfiguration</span></span>
    - <span data-ttu-id="77eee-448">省略可能なパラメーター - UrlConfiguration を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-448">Cmdlets updated with optional parameter - UrlConfiguration</span></span>
        - <span data-ttu-id="77eee-449">New-AzApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="77eee-449">New-AzApplicationGatewayRewriteRuleActionSet</span></span>
* <span data-ttu-id="77eee-450">NetworkWatcher ConnectionMonitor バージョン 2 リソースのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-450">Add suppport for NetworkWatcher ConnectionMonitor version 2 resources</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-451">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-451">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-452">修復するリソースを決定する前にコンプライアンスを評価することをサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-452">Support evaluating compliance prior to determining what resource to remediate</span></span>
    - <span data-ttu-id="77eee-453">'-ResourceDiscoverMode' パラメーターを Start-AzPolicyRemediation に追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-453">Add '-ResourceDiscoverMode' parameter to Start-AzPolicyRemediation</span></span>
* <span data-ttu-id="77eee-454">ポリシー メタデータ リソースを取得するための Get-AzPolicyMetadata コマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-454">Add Get-AzPolicyMetadata cmdlet for getting policy metadata resources</span></span>
* <span data-ttu-id="77eee-455">API バージョン 2019-10-01 の Get-AzPolicyState および Get-AzPolicyStateSummary を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-455">Updated Get-AzPolicyState and Get-AzPolicyStateSummary for API version 2019-10-01</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-456">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-456">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-457">レプリケートされたディスクを削除するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-457">Azure Site Recovery support for removing a replicated disk.</span></span>
* <span data-ttu-id="77eee-458">Recovery Services コンテナー の作成中にタグを追加するサポートが Azure Backup で追加されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-458">Azure Backup added support for adding tags while creating a Recovery Services Vault.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-459">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-459">Az.Resources</span></span>
* <span data-ttu-id="77eee-460">\*-AzPolicyAssignment コマンドレットで -Scope を任意指定にし、コンテキスト サブスクリプションを既定にします</span><span class="sxs-lookup"><span data-stu-id="77eee-460">Make -Scope optional in \*-AzPolicyAssignment cmdlets with default to context subscription</span></span>
* <span data-ttu-id="77eee-461">パスワードとキー資格情報を使用した ADServicePrincipal の作成例を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-461">Add examples of creating ADServicePrincipal with password and key credential</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-462">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-462">Az.Sql</span></span>
<span data-ttu-id="77eee-463">DatabaseName の存在の代わりに PartnerDatabaseName の存在を確認するように New-AzSqlDatabaseSecondary コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-463">Fix New-AzSqlDatabaseSecondary cmdlet to check for PartnerDatabaseName existence instead of DatabaseName existence.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-464">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-464">Az.Storage</span></span>
* <span data-ttu-id="77eee-465">[ストレージ アカウントの作成] でテーブル/キュー暗号化キーの種類の設定をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-465">Support set Table/Queue Encryption Keytype in Create Storage Account</span></span>
    - <span data-ttu-id="77eee-466">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-466">New-AzStorageAccount</span></span>
* <span data-ttu-id="77eee-467">StorageException で ExtendedErrorInformation がない場合に RequestId を表示します</span><span class="sxs-lookup"><span data-stu-id="77eee-467">Show RequestId when StorageException don't have ExtendedErrorInformation</span></span>
* <span data-ttu-id="77eee-468">コマンドレット Start-AzStorageBlobCopy の例 6 を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-468">Fix the Example 6 of cmdlet Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-469">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-469">Az.Websites</span></span>
* <span data-ttu-id="77eee-470">Set-AzWebapp および Set-AzWebappSlot で AlwaysOn、MinTls、および FtpsState プロパティをサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-470">Set-AzWebapp and Set-AzWebappSlot supports AlwaysOn, MinTls and FtpsState properties</span></span>
* <span data-ttu-id="77eee-471">単一の Set-AzWebApp コマンドを使用して、AppservicePlan の変更と同時に HttpsOnly を設定すると、HttpsOnly が既定値にリセットされる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-471">Fixing issue where setting HttpsOnly along with changing AppservicePlan at the same time using the single Set-AzWebApp Command, was resetting HttpsOnly to default value</span></span>

## <a name="330---january-2020"></a><span data-ttu-id="77eee-472">3.3.0 - 2020 年 1 月</span><span class="sxs-lookup"><span data-stu-id="77eee-472">3.3.0 - January 2020</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-473">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-473">Az.Accounts</span></span>
* <span data-ttu-id="77eee-474">AzureAttestationServiceEndpointResourceId および AzureAttestationServiceEndpointSuffix パラメーターを受け入れるように、Add-AzEnvironment と Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-474">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameters AzureAttestationServiceEndpointResourceId and AzureAttestationServiceEndpointSuffix</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-475">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-475">Az.Cdn</span></span>
* <span data-ttu-id="77eee-476">New-AzCdnEndpoint コマンドレットのエラー応答の詳細を表示します</span><span class="sxs-lookup"><span data-stu-id="77eee-476">Display error response detail in New-AzCdnEndpoint cmdlet</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-477">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-477">Az.Compute</span></span>
* <span data-ttu-id="77eee-478">OS プロファイルのないマネージド OD ディスクを使用する VM 用の Set-AzVMCustomScriptExtension コマンドレットを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-478">Fix Set-AzVMCustomScriptExtension cmdlet for a VM with managed OD disk which does not have OS profile.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="77eee-479">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-479">Az.ContainerInstance</span></span>
* <span data-ttu-id="77eee-480">New-AzContainerGroup の例で使用されるパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-480">Fixed parameter names used by example of New-AzContainerGroup</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="77eee-481">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="77eee-481">Az.DataBoxEdge</span></span>
* <span data-ttu-id="77eee-482">コマンドレット 'Get-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-482">Added cmdlet 'Get-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="77eee-483">Edge ストレージ コンテナーを取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-483">Get the Edge Storage Container</span></span>
* <span data-ttu-id="77eee-484">コマンドレット 'New-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-484">Added cmdlet 'New-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="77eee-485">新しい Edge ストレージ コンテナーを作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-485">Create new Edge Strorage Container</span></span>
* <span data-ttu-id="77eee-486">コマンドレット 'Remove-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-486">Added cmdlet 'Remove-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="77eee-487">Edge ストレージ コンテナーを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-487">Remove the Edge Storage Container</span></span>
* <span data-ttu-id="77eee-488">コマンドレット 'Invoke-AzDataBoxEdgeStorageContainer' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-488">Added cmdlet 'Invoke-AzDataBoxEdgeStorageContainer'</span></span>
  - <span data-ttu-id="77eee-489">Edge ストレージ コンテナーのデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="77eee-489">Invoke action to refresh data on Edge Storage Container</span></span>
* <span data-ttu-id="77eee-490">コマンドレット 'Get-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-490">Added cmdlet 'Get-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="77eee-491">Edge ストレージ アカウントを取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-491">Get the Edge Storage Account</span></span>
* <span data-ttu-id="77eee-492">コマンドレット 'New-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-492">Added cmdlet 'New-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="77eee-493">新しい Edge ストレージ アカウントを作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-493">Create new Edge Storage Account</span></span>
* <span data-ttu-id="77eee-494">コマンドレット 'Remove-AzDataBoxEdgeStorageAccount' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-494">Added cmdlet 'Remove-AzDataBoxEdgeStorageAccount'</span></span>
  - <span data-ttu-id="77eee-495">Edge ストレージ アカウントを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-495">Remove the Edge Storage Account</span></span>
* <span data-ttu-id="77eee-496">コマンドレット 'Invoke-AzDataBoxEdgeShare' を呼び出します</span><span class="sxs-lookup"><span data-stu-id="77eee-496">Invoke cmdlet 'Invoke-AzDataBoxEdgeShare'</span></span>
  - <span data-ttu-id="77eee-497">共有のデータを更新するアクションを呼び出します</span><span class="sxs-lookup"><span data-stu-id="77eee-497">Invoke action to refresh data on share</span></span>
* <span data-ttu-id="77eee-498">コマンドレット 'Set-AzDataBoxEdgeStorageAccountCredential' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-498">Added cmdlet 'Set-AzDataBoxEdgeStorageAccountCredential'</span></span>
  - <span data-ttu-id="77eee-499">az databoxedge ストレージ アカウント資格情報を設定します</span><span class="sxs-lookup"><span data-stu-id="77eee-499">Set the az databoxedge storage account credential</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-500">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-500">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-501">Get-AzDataFactoryV2IntegrationRuntime コマンドに AutoUpdateETA、LatestVersion、PushedVersion、TaskQueueId、VersionStatus の各プロパティを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-501">Add AutoUpdateETA, LatestVersion, PushedVersion, TaskQueueId and VersionStatus properties for Get-AzDataFactoryV2IntegrationRuntime cmd</span></span>
* <span data-ttu-id="77eee-502">ADF .Net SDK のバージョンを 4.6.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-502">Update ADF .Net SDK version to 4.6.0</span></span>
* <span data-ttu-id="77eee-503">'Set-AzureRmDataFactoryV2IntegrationRuntime' コマンドにパラメーター 'PublicIPs' を追加し、静的パブリック IP アドレスを持つ Azure-SSIS IR の作成を有効にします。</span><span class="sxs-lookup"><span data-stu-id="77eee-503">Add parameter 'PublicIPs' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable create Azure-SSIS IR with static public IP addresses.</span></span>

#### <a name="azdevtestlabs"></a><span data-ttu-id="77eee-504">Az.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="77eee-504">Az.DevTestLabs</span></span>
* <span data-ttu-id="77eee-505">Get-AzDtlAllowedVMSizesPolicy.md の壊れたリンクを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-505">Remove the broken link in Get-AzDtlAllowedVMSizesPolicy.md</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-506">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-506">Az.EventHub</span></span>
* <span data-ttu-id="77eee-507">問題 10634 を修正:remove eventhubnamespace の null オブジェクト参照を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-507">Fix for issue 10634 : Fix the null Object reference for remove eventhubnamespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="77eee-508">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-508">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-509">Invoke-AzHDInsightHiveJob.md エラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-509">Fix Invoke-AzHDInsightHiveJob.md error.</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="77eee-510">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="77eee-510">Az.MachineLearning</span></span>
* <span data-ttu-id="77eee-511">MachineLearningCompute が使用できなくなったため、以下のコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-511">Removed below cmdlets because MachineLearningCompute is not available any longer</span></span>
  - <span data-ttu-id="77eee-512">Get-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="77eee-512">Get-AzMlOpCluster</span></span>
  - <span data-ttu-id="77eee-513">Get-AzMlOpClusterKey</span><span class="sxs-lookup"><span data-stu-id="77eee-513">Get-AzMlOpClusterKey</span></span>
  - <span data-ttu-id="77eee-514">New-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="77eee-514">New-AzMlOpCluster</span></span>
  - <span data-ttu-id="77eee-515">Remove-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="77eee-515">Remove-AzMlOpCluster</span></span>
  - <span data-ttu-id="77eee-516">Set-AzMlOpCluster</span><span class="sxs-lookup"><span data-stu-id="77eee-516">Set-AzMlOpCluster</span></span>
  - <span data-ttu-id="77eee-517">Test-AzMlOpClusterSystemServicesUpdateAvailability</span><span class="sxs-lookup"><span data-stu-id="77eee-517">Test-AzMlOpClusterSystemServicesUpdateAvailability</span></span>
  - <span data-ttu-id="77eee-518">Update-AzMlOpClusterSystemService</span><span class="sxs-lookup"><span data-stu-id="77eee-518">Update-AzMlOpClusterSystemService</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-519">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-519">Az.Network</span></span>
* <span data-ttu-id="77eee-520">Microsoft.Azure.Management.Sql の依存関係を 1.36-preview から 1.37-preview にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="77eee-520">Upgrade dependency of Microsoft.Azure.Management.Sql from 1.36-preview to 1.37-preview</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-521">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-521">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-522">Azure Site Recovery は、Azure から Azure へのプロバイダー向けの、カスタマー マネージド キーを使用して保存時に暗号化されたマネージド ディスク VM のサポートを変更します。</span><span class="sxs-lookup"><span data-stu-id="77eee-522">Azure Site Recovery change support for managed disk vms encrypted at rest with customer managed keys for Azure to Azure provider.</span></span>
* <span data-ttu-id="77eee-523">Azure Site Recovery は、Vmware から Azure への保護を有効にするときに、オプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-523">Azure Site Recovery support to input disk encryption Set Id as optional input at enabling protection for Vmware to Azure.</span></span>
* <span data-ttu-id="77eee-524">Azure Site Recovery は、Vmware から Azure への保護を有効にするために、ディスク レベルでのオプションの入力として、ディスク暗号化セット ID の入力をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-524">Azure Site Recovery support to input disk encryption Set Id as optional input at disk level to enable protection for Vmware to Azure.</span></span>
* <span data-ttu-id="77eee-525">Azure Site Recovery は、HyperV から Azure へのディスク暗号化セット マップを使用して、レプリケーション保護された項目の更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-525">Azure Site Recovery support to update replication protected item with disk encryption set Map for HyperV to Azure.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-526">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-526">Az.Resources</span></span>
* <span data-ttu-id="77eee-527">'Remove-AzTag' のヘルプ ドキュメントのエラーを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-527">Fix an error in help document of 'Remove-AzTag'.</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-528">Az.Sql</span></span>
* <span data-ttu-id="77eee-529">脆弱性評価のベースラインの設定のコマンドレット機能が Azure データベースのマスター DB で動作し、マネージド インスタンス システム データベース上に限定されるように修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-529">Fix vulnerability assessment set baseline cmdlets functionality to work on master db for azure database and limit it on managed instance system databases.</span></span>
* <span data-ttu-id="77eee-530">SQL インスタンスのフェールオーバー グループの作成時のエラーを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-530">Fix an error when creating SQL instance failover group</span></span>

#### <a name="azsqlvirtualmachine"></a><span data-ttu-id="77eee-531">Az.SqlVirtualMachine</span><span class="sxs-lookup"><span data-stu-id="77eee-531">Az.SqlVirtualMachine</span></span>
* <span data-ttu-id="77eee-532">新しい有効なライセンスの種類として DR を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-532">Add DR as a new valid License type</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-533">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-533">Az.Storage</span></span>
* <span data-ttu-id="77eee-534">将来のリリースでの DefaultAction 値の変更に対する破壊的変更の警告メッセージを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-534">Add breaking change warning message for DefaultAction Value change in a future release</span></span>
    - <span data-ttu-id="77eee-535">Update-AzStorageAccountNetworkRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-535">Update-AzStorageAccountNetworkRuleSet</span></span>
* <span data-ttu-id="77eee-536">パラメーター -IncludeGeoReplicationStats を指定して get-AzureRMStorageAccount を実行することで、ストレージ アカウントの最終同期時刻の取得をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-536">Support Get last sync time of Storage account by run get-AzureRMStorageAccount with parameter -IncludeGeoReplicationStats</span></span>
    - <span data-ttu-id="77eee-537">Get-AzureRMStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-537">Get-AzureRMStorageAccount</span></span>

## <a name="320---december-2019"></a><span data-ttu-id="77eee-538">3.2.0 - 2019 年 12 月</span><span class="sxs-lookup"><span data-stu-id="77eee-538">3.2.0 - December 2019</span></span>

### <a name="general"></a><span data-ttu-id="77eee-539">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-539">General</span></span>
* <span data-ttu-id="77eee-540">すべてのモジュールで相対パスを使用するように、.psd1 の参照を更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-540">Update references in .psd1 to use relative path for all modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-541">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-541">Az.Accounts</span></span>
* <span data-ttu-id="77eee-542">Az 4.0 プレビューのクライアント側テレメトリに適切な UserAgent を設定します</span><span class="sxs-lookup"><span data-stu-id="77eee-542">Set correct UserAgent for client-side telemetry for Az 4.0 preview</span></span>
* <span data-ttu-id="77eee-543">Az 4.0 プレビューでコンテキストが null の場合にユーザー フレンドリなエラー メッセージを表示します</span><span class="sxs-lookup"><span data-stu-id="77eee-543">Display user friendly error message when context is null in Az 4.0 preview</span></span>

#### <a name="azbatch"></a><span data-ttu-id="77eee-544">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="77eee-544">Az.Batch</span></span>
* <span data-ttu-id="77eee-545">問題 [#10602](https://github.com/Azure/azure-powershell/issues/10602) を修正します。これは、**New-AzBatchPool** で 'VirtualMachineConfiguration.ContainerConfiguration' または 'VirtualMachineConfiguration.DataDisks' が適切にサーバーに送信されていなかったというものです。</span><span class="sxs-lookup"><span data-stu-id="77eee-545">Fix issue [#10602](https://github.com/Azure/azure-powershell/issues/10602), where **New-AzBatchPool** did not properly send 'VirtualMachineConfiguration.ContainerConfiguration' or 'VirtualMachineConfiguration.DataDisks' to the server.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-546">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-546">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-547">ADF .Net SDK のバージョンを 4.5.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-547">Update ADF .Net SDK version to 4.5.0</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="77eee-548">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-548">Az.FrontDoor</span></span>
* <span data-ttu-id="77eee-549">WAF マネージド規則の除外サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-549">Added WAF managed rules exclusion support</span></span>
* <span data-ttu-id="77eee-550">SocketAddr をオートコンプリートに追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-550">Add SocketAddr to auto-complete</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="77eee-551">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="77eee-551">Az.HealthcareApis</span></span>
* <span data-ttu-id="77eee-552">例外処理</span><span class="sxs-lookup"><span data-stu-id="77eee-552">Exception Handling</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-553">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-553">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-554">設定されていない可能性のある値へのアクセス エラーを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-554">Fixed error accessing value that is potentially not set</span></span>
* <span data-ttu-id="77eee-555">楕円曲線暗号証明書の管理</span><span class="sxs-lookup"><span data-stu-id="77eee-555">Elliptic Curve Cryptography Certificate Managment</span></span>
    - <span data-ttu-id="77eee-556">証明書ポリシーの曲線を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-556">Added support to specify the Curve for Certificate Policies</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-557">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-557">Az.Monitor</span></span>
* <span data-ttu-id="77eee-558">[診断設定を追加する] コマンドに省略可能な引数を追加しています。</span><span class="sxs-lookup"><span data-stu-id="77eee-558">Adding optional argument to the Add Diagnostic Settings command.</span></span> <span data-ttu-id="77eee-559">存在する場合は Log Analytics へのエクスポートが固定スキーマ (</span><span class="sxs-lookup"><span data-stu-id="77eee-559">A switch argument that if present indicates that the export to Log Analytics must be to a fixed schema (a.k.a.</span></span> <span data-ttu-id="77eee-560">専用、データ型) 宛でなければならないことを示す切り替え引数</span><span class="sxs-lookup"><span data-stu-id="77eee-560">dedicated, data type)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-561">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-561">Az.Network</span></span>
* <span data-ttu-id="77eee-562">AzureFirewall アプリケーション、NAT、およびネットワーク規則での IpGroups のサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-562">Support for IpGroups in AzureFirewall Application,Nat & Network Rules.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-563">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-563">Az.Resources</span></span>
* <span data-ttu-id="77eee-564">テンプレートの名前が組み込みパラメーター名と競合している場合、テンプレートのデプロイでテンプレート パラメーターの読み取りに失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-564">Fix an issue where template deployment fails to read a template parameter if its name conflicts with some built-in parameter name.</span></span>
* <span data-ttu-id="77eee-565">ポリシー セット定義内でのグループ化サポートを導入する新しい API バージョン 2019-09-01 を使用するようにポリシーのコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-565">Updated policy cmdlets to use new api version 2019-09-01 that introduces grouping support within policy set definitions.</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-566">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-566">Az.Sql</span></span>
* <span data-ttu-id="77eee-567">脆弱性評価の自動有効化でのストレージ作成を StorageV2 にアップグレードしました</span><span class="sxs-lookup"><span data-stu-id="77eee-567">Upgraded storage creation in Vulnerability Assessment auto enablement to StorageV2</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-568">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-568">Az.Storage</span></span>
* <span data-ttu-id="77eee-569">OAuth 認証に基づくストレージ コンテキストでの BLOB/コンテナー ID ベースの SAS トークン生成をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-569">Support generate Blob/Constainer Idenity based SAS token with Storage Context based on Oauth authentication</span></span>
    - <span data-ttu-id="77eee-570">New-AzStorageContainerSASToken</span><span class="sxs-lookup"><span data-stu-id="77eee-570">New-AzStorageContainerSASToken</span></span>
    - <span data-ttu-id="77eee-571">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="77eee-571">New-AzStorageBlobSASToken</span></span>
* <span data-ttu-id="77eee-572">ストレージ アカウントのユーザー委任キーの取り消しをサポートします。これにより、すべての ID SAS トークンが取り消されます</span><span class="sxs-lookup"><span data-stu-id="77eee-572">Support revoke Storage Account User Delegation Keys, so all Idenity SAS tokens are revoked</span></span>
    - <span data-ttu-id="77eee-573">Revoke-AzStorageAccountUserDelegationKeys</span><span class="sxs-lookup"><span data-stu-id="77eee-573">Revoke-AzStorageAccountUserDelegationKeys</span></span>
* <span data-ttu-id="77eee-574">新しい API バージョン 2019-06-01 をサポートするために、Microsoft.Azure.Management.Storage 14.2.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-574">Upgrade to Microsoft.Azure.Management.Storage 14.2.0, to support new API version 2019-06-01.</span></span>
* <span data-ttu-id="77eee-575">ファイル共有コマンドレットの管理プレーンで 5120 を超える値の QuotaGiB (ギビバイト単位の共有クォータ) をサポートし、'QuotaGiB' パラメーターにパラメーター エイリアス 'Quota' を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-575">Support of QuotaGiB (Share Quota in Gibibye) for values of more than 5120 in the Management plane of File Share cmdlets and added the 'Quota' parameter alias to the 'QuotaGiB' parameter.</span></span>
    - <span data-ttu-id="77eee-576">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="77eee-576">New-AzRmStorageShare</span></span>
    - <span data-ttu-id="77eee-577">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="77eee-577">Update-AzRmStorageShare</span></span>
* <span data-ttu-id="77eee-578">パラメーター別名 'QuotaGiB' をパラメーター 'Quota' に追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-578">Add parameter alias 'QuotaGiB' to parameter 'Quota'</span></span>
    - <span data-ttu-id="77eee-579">Set-AzStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="77eee-579">Set-AzStorageShareQuota</span></span>
* <span data-ttu-id="77eee-580">Set-AzStorageContainerAcl で保存されているアクセス ポリシーをクリーンアップできる問題を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-580">Fix the issue that Set-AzStorageContainerAcl can clean up the stored Access Policy</span></span>
    - <span data-ttu-id="77eee-581">Set-AzStorageContainerAcl</span><span class="sxs-lookup"><span data-stu-id="77eee-581">Set-AzStorageContainerAcl</span></span>

## <a name="310---november-2019"></a><span data-ttu-id="77eee-582">3.1.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="77eee-582">3.1.0 - November 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="77eee-583">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-583">Highlights since the last major release</span></span>
* <span data-ttu-id="77eee-584">Az.DataBoxEdge 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="77eee-584">Az.DataBoxEdge 1.0.0 released</span></span>
* <span data-ttu-id="77eee-585">Az.SqlVirtualMachine 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="77eee-585">Az.SqlVirtualMachine 1.0.0 released</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-586">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-586">Az.Compute</span></span>
* <span data-ttu-id="77eee-587">VM の再適用機能</span><span class="sxs-lookup"><span data-stu-id="77eee-587">VM Reapply feature</span></span>
    - <span data-ttu-id="77eee-588">Set-AzVM コマンドレットに Reapply パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-588">Add Reapply parameter to Set-AzVM cmdlet</span></span>
* <span data-ttu-id="77eee-589">VM スケール セットの AutomaticRepairs 機能:</span><span class="sxs-lookup"><span data-stu-id="77eee-589">VM Scale Set AutomaticRepairs feature:</span></span>
    - <span data-ttu-id="77eee-590">次のコマンドレットに、EnableAutomaticRepair、AutomaticRepairGracePeriod、および AutomaticRepairMaxInstanceRepairsPercent パラメーターを追加します。 New-AzVmssConfig   Update-AzVmss</span><span class="sxs-lookup"><span data-stu-id="77eee-590">Add EnableAutomaticRepair, AutomaticRepairGracePeriod, and AutomaticRepairMaxInstanceRepairsPercent parameters to the following cmdlets:   New-AzVmssConfig   Update-AzVmss</span></span>
* <span data-ttu-id="77eee-591">New-AzVM でのテナント間のギャラリー イメージ サポート</span><span class="sxs-lookup"><span data-stu-id="77eee-591">Cross tenant gallery image support for New-AzVM</span></span>
* <span data-ttu-id="77eee-592">New-AzVM、New-AzVMConfig、および New-AzVmss コマンドレットの Priority パラメーターの引数の入力候補に "Spot" を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-592">Add 'Spot' to the argument completer of Priority parameter in New-AzVM, New-AzVMConfig and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="77eee-593">Add-AzVmssDataDisk コマンドレットに DiskIOPSReadWrite および DiskMBpsReadWrite パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-593">Add DiskIOPSReadWrite and DiskMBpsReadWrite parameters to Add-AzVmssDataDisk cmdlet</span></span>
* <span data-ttu-id="77eee-594">New-AzGalleryImageVersion コマンドレットの SourceImageId パラメーターを省略可能に変更します</span><span class="sxs-lookup"><span data-stu-id="77eee-594">Change SourceImageId parameter of New-AzGalleryImageVersion cmdlet to optional</span></span>
* <span data-ttu-id="77eee-595">New-AzGalleryImageVersion コマンドレットに OSDiskImage および DataDiskImage パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-595">Add OSDiskImage and DataDiskImage parameters to New-AzGalleryImageVersion cmdlet</span></span>
* <span data-ttu-id="77eee-596">New-AzGalleryImageDefinition コマンドレットに HyperVGeneration パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-596">Add HyperVGeneration parameter to New-AzGalleryImageDefinition cmdlet</span></span>
* <span data-ttu-id="77eee-597">New-AzVmss、New-AzVmssConfi および Update-AzVmss コマンドレットに SkipExtensionsOnOverprovisionedVMs パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-597">Add SkipExtensionsOnOverprovisionedVMs parameters to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>

#### <a name="azdataboxedge"></a><span data-ttu-id="77eee-598">Az.DataBoxEdge</span><span class="sxs-lookup"><span data-stu-id="77eee-598">Az.DataBoxEdge</span></span>
* <span data-ttu-id="77eee-599">コマンドレット `Get-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-599">Added cmdlet `Get-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="77eee-600">注文を取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-600">Get the Order</span></span>
* <span data-ttu-id="77eee-601">コマンドレット `New-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-601">Added cmdlet `New-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="77eee-602">新しい注文を作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-602">Create new Order</span></span>
* <span data-ttu-id="77eee-603">コマンドレット `Remove-AzDataBoxEdgeOrder` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-603">Added cmdlet `Remove-AzDataBoxEdgeOrder`</span></span>
    - <span data-ttu-id="77eee-604">注文を削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-604">Remove the Order</span></span>
* <span data-ttu-id="77eee-605">コマンドレット `New-AzDataBoxEdgeShare` の変更</span><span class="sxs-lookup"><span data-stu-id="77eee-605">Change in cmdlet `New-AzDataBoxEdgeShare`</span></span>
    - <span data-ttu-id="77eee-606">ローカル共有を作成するようになります</span><span class="sxs-lookup"><span data-stu-id="77eee-606">Now creates Local Share</span></span>
* <span data-ttu-id="77eee-607">コマンドレット `Set-AzDataBoxEdgeRole` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-607">Added cmdlet `Set-AzDataBoxEdgeRole`</span></span>
    - <span data-ttu-id="77eee-608">IotRole を共有にマップできるようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-608">Now IotRole can be mapped to Share</span></span>
* <span data-ttu-id="77eee-609">コマンドレット `Invoke-AzDataBoxEdgeDevice` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-609">Added cmdlet `Invoke-AzDataBoxEdgeDevice`</span></span>
    - <span data-ttu-id="77eee-610">デバイスで更新プログラムのスキャン、更新プログラムのダウンロード、更新プログラムのインストールを呼び出します</span><span class="sxs-lookup"><span data-stu-id="77eee-610">Invoke scan update, download update, install updates on the device</span></span>
* <span data-ttu-id="77eee-611">コマンドレット `Get-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-611">Added cmdlet `Get-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="77eee-612">トリガーに関する情報を取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-612">Gets the information about Triggers</span></span>
* <span data-ttu-id="77eee-613">コマンドレット `New-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-613">Added cmdlet `New-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="77eee-614">新しいトリガーを作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-614">Create new Triggers</span></span>
* <span data-ttu-id="77eee-615">コマンドレット `Remove-AzDataBoxEdgeTrigger` を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-615">Added cmdlet `Remove-AzDataBoxEdgeTrigger`</span></span>
    - <span data-ttu-id="77eee-616">トリガーを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-616">Remove the Triggers</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-617">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-617">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-618">ADF .Net SDK のバージョンを 4.4.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-618">Update ADF .Net SDK version to 4.4.0</span></span>
* <span data-ttu-id="77eee-619">カスタム セットアップ スクリプトなしでセットアップ構成およびサードパーティ コンポーネントを有効にするために、"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドにパラメーター "ExpressCustomSetup" を追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-619">Add parameter 'ExpressCustomSetup' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable setup configurations and 3rd party components without custom setup script.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-620">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-620">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-621">Get-AzDataLakeStoreDeletedItem および Restore-AzDataLakeStoreDeletedItem のドキュメントを更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-621">Update documentation of Get-AzDataLakeStoreDeletedItem and Restore-AzDataLakeStoreDeletedItem</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-622">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-622">Az.EventHub</span></span>
* <span data-ttu-id="77eee-623">問題 10301 を修正:SAS トークンの日付形式を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-623">Fix for issue 10301 : Fix the SAS Token date format</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="77eee-624">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-624">Az.FrontDoor</span></span>
* <span data-ttu-id="77eee-625">Enable-AzFrontDoorCustomDomainHttps および New-AzFrontDoorFrontendEndpointObject に MinimumTlsVersion パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-625">Add MinimumTlsVersion parameter to Enable-AzFrontDoorCustomDomainHttps and New-AzFrontDoorFrontendEndpointObject</span></span>
* <span data-ttu-id="77eee-626">New-AzFrontDoorHealthProbeSettingObject に HealthProbeMethod および EnabledState パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-626">Add HealthProbeMethod and EnabledState parameters to New-AzFrontDoorHealthProbeSettingObject</span></span>
* <span data-ttu-id="77eee-627">Front Door の作成/更新に渡される BackendPoolsSettings オブジェクトを作成するための新しいコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-627">Add new cmdlet to create BackendPoolsSettings objec to pass into creation/update of Front Door</span></span>
    - <span data-ttu-id="77eee-628">New-AzFrontDoorBackendPoolsSettingObject</span><span class="sxs-lookup"><span data-stu-id="77eee-628">New-AzFrontDoorBackendPoolsSettingObject</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-629">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-629">Az.Network</span></span>
* <span data-ttu-id="77eee-630">"Start-AzVirtualNetworkGatewayConnectionPacketCapture.md" と "Start-AzVirtualnetworkGatewayPacketCapture.md" の FilterData オプションの例を変更します。</span><span class="sxs-lookup"><span data-stu-id="77eee-630">Change 'Start-AzVirtualNetworkGatewayConnectionPacketCapture.md' and 'Start-AzVirtualnetworkGatewayPacketCapture.md' FilterData option examples.</span></span>

#### <a name="azprivatedns"></a><span data-ttu-id="77eee-631">Az.PrivateDns</span><span class="sxs-lookup"><span data-stu-id="77eee-631">Az.PrivateDns</span></span>
* <span data-ttu-id="77eee-632">PrivateDns .net sdk をバージョン 1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-632">Updated PrivateDns .net sdk to version 1.0.0</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-633">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-633">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-634">保護の有効時にディスクの種類を選択するための Azure Site Recovery のサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-634">Azure Site Recovery support to select disk type at enabling protection.</span></span>
* <span data-ttu-id="77eee-635">復旧計画アクション編集のための Azure Site Recovery のバグ修正。</span><span class="sxs-lookup"><span data-stu-id="77eee-635">Azure Site Recovery bug fix for recovery plan action edit.</span></span>
* <span data-ttu-id="77eee-636">filestream DB を受け入れるための Azure Backup での SQL 復元のサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-636">Azure Backup SQL Restore support to accept filestream DBs.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="77eee-637">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="77eee-637">Az.RedisCache</span></span>
* <span data-ttu-id="77eee-638">"New-AzRedisCache" および "Set-AzRedisCache" コマンドレットに "MinimumTlsVersion" パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-638">Added 'MinimumTlsVersion' parameter in 'New-AzRedisCache' and 'Set-AzRedisCache' cmdlets.</span></span> <span data-ttu-id="77eee-639">また、"Get-AzRedisCache" コマンドレットの出力に "MinimumTlsVersion" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-639">Also, added 'MinimumTlsVersion' in the output of 'Get-AzRedisCache' cmdlet.</span></span>
* <span data-ttu-id="77eee-640">"Set-AzRedisCache" および "New-AzRedisCache" コマンドレットの "-Size" パラメーターに対する検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-640">Added validation on '-Size' parameter for 'Set-AzRedisCache' and 'New-AzRedisCache' cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-641">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-641">Az.Resources</span></span>
- <span data-ttu-id="77eee-642">ポリシー割り当てに新しい EnforcementMode プロパティを持つ新しい API バージョン 2019-06-01 を使用するように、ポリシー コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-642">Updated policy cmdlets to use new api version 2019-06-01 that has new EnforcementMode property in policy assignment.</span></span>
- <span data-ttu-id="77eee-643">ポリシー定義作成のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-643">Updated create policy definition help example</span></span>
- <span data-ttu-id="77eee-644">サービス プリンシパル名が見つからない場合に Remove-AZADServicePrincipal -ServicePrincipalName が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-644">Fix bug Remove-AZADServicePrincipal -ServicePrincipalName, throw null reference when service principal name not found.</span></span>
- <span data-ttu-id="77eee-645">テナントにサブスクリプションがない場合に New-AZADServicePrincipal が null 参照をスローするバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-645">Fix bug New-AZADServicePrincipal, throw null reference when tenant doesn't have any subscription.</span></span>
- <span data-ttu-id="77eee-646">関連付けられたアプリケーションのみに資格情報を追加するように New-AzAdServicePrincipal を変更します。</span><span class="sxs-lookup"><span data-stu-id="77eee-646">Change New-AzAdServicePrincipal to add credentials only to associated application.</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-647">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-647">Az.Sql</span></span>
* <span data-ttu-id="77eee-648">データベース ReadReplicaCount のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-648">Added support for database ReadReplicaCount.</span></span>
* <span data-ttu-id="77eee-649">ゾーン冗長性が設定されていない場合の Set-AzSqlDatabase を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-649">Fixed Set-AzSqlDatabase when zone redundancy not set</span></span>

## <a name="300---november-2019"></a><span data-ttu-id="77eee-650">3.0.0 - 2019 年 11 月</span><span class="sxs-lookup"><span data-stu-id="77eee-650">3.0.0 - November 2019</span></span>
### <a name="general"></a><span data-ttu-id="77eee-651">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-651">General</span></span>
* <span data-ttu-id="77eee-652">Az.PrivateDns 1.0.0 がリリースされました</span><span class="sxs-lookup"><span data-stu-id="77eee-652">Az.PrivateDns 1.0.0 released</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-653">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-653">Az.Accounts</span></span>
* <span data-ttu-id="77eee-654">'Resolve-Error' エイリアスの非推奨メッセージを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-654">Add a deprecation message for 'Resolve-Error' alias.</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="77eee-655">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="77eee-655">Az.Advisor</span></span>
* <span data-ttu-id="77eee-656">Get-AzAdvisorRecommendation コマンドレットに新しいカテゴリ 'Operational Excellence' が追加されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-656">Added new category 'Operational Excellence' to Get-AzAdvisorRecommendation cmdlet.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="77eee-657">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="77eee-657">Az.Batch</span></span>
* <span data-ttu-id="77eee-658">`BatchAccountContext` の `CoreQuota` を `DedicatedCoreQuota` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-658">Renamed `CoreQuota` on `BatchAccountContext` to `DedicatedCoreQuota`.</span></span> <span data-ttu-id="77eee-659">新しい `LowPriorityCoreQuota` もあります。</span><span class="sxs-lookup"><span data-stu-id="77eee-659">There is also a new `LowPriorityCoreQuota`.</span></span>
  - <span data-ttu-id="77eee-660">これにより、**Get-AzBatchAccount** が影響をうけます。</span><span class="sxs-lookup"><span data-stu-id="77eee-660">This impacts **Get-AzBatchAccount**.</span></span>
* <span data-ttu-id="77eee-661">**New-AzBatchTask** の `-ResourceFile` パラメーターは `PSResourceFile` オブジェクトのコレクションを受け取るようになりました。これは新しい **New-AzBatchResourceFile** コマンドレットを使用して作成できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-661">**New-AzBatchTask** `-ResourceFile` parameter now takes a collection of `PSResourceFile` objects, which can be constructed using the new **New-AzBatchResourceFile** cmdlet.</span></span>
* <span data-ttu-id="77eee-662">新しい **New-AzBatchResourceFile** コマンドレットにより `PSResourceFile` オブジェクトの作成が簡単になります。</span><span class="sxs-lookup"><span data-stu-id="77eee-662">New **New-AzBatchResourceFile** cmdlet to help create `PSResourceFile` objects.</span></span> <span data-ttu-id="77eee-663">これらは、`-ResourceFile` パラメーターで **New-AzBatchTask** に指定できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-663">These can be supplied to **New-AzBatchTask** on the `-ResourceFile` parameter.</span></span>
  - <span data-ttu-id="77eee-664">これにより、既存の `HttpUrl` の方法に加えて、2 つの新しい種類のリソース ファイルがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="77eee-664">This supports two new kinds of resource file in addition to the existing `HttpUrl` way:</span></span>
    - <span data-ttu-id="77eee-665">`AutoStorageContainerName` ベースのリソース ファイルでは、自動ストレージ コンテナー全体が Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="77eee-665">`AutoStorageContainerName` based resource files download an entire auto-storage container to the Batch node.</span></span>
    - <span data-ttu-id="77eee-666">`StorageContainerUrl` ベースのリソース ファイルでは、URL で指定されたコンテナーが Batch ノードにダウンロードされます。</span><span class="sxs-lookup"><span data-stu-id="77eee-666">`StorageContainerUrl` based resource files download the container specified in the URL to the Batch node.</span></span>
* <span data-ttu-id="77eee-667">**Get-AzBatchApplication** によって返される `PSApplication` の `ApplicationPackages` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-667">Removed `ApplicationPackages` property of `PSApplication` returned by **Get-AzBatchApplication**.</span></span>
  - <span data-ttu-id="77eee-668">アプリケーション内の特定のパッケージは **Get-AzBatchApplicationPackage** を使用して取得できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-668">The specific packages inside of an application now can be retrieved using **Get-AzBatchApplicationPackage**.</span></span> <span data-ttu-id="77eee-669">(例: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`)。</span><span class="sxs-lookup"><span data-stu-id="77eee-669">For example: `Get-AzBatchApplication -AccountName myaccount -ResourceGroupName myresourcegroup -ApplicationId myapplication`.</span></span>
* <span data-ttu-id="77eee-670">**Get-AzBatchApplicationPackage**、**New-AzBatchApplicationPackage**、**Remove-AzBatchApplicationPackage**、**Get-AzBatchApplication**、**New-AzBatchApplication**、**Remove-AzBatchApplication**、および **Set-AzBatchApplication** の `ApplicationId` を `ApplicationName` に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-670">Renamed `ApplicationId` to `ApplicationName` on **Get-AzBatchApplicationPackage**, **New-AzBatchApplicationPackage**, **Remove-AzBatchApplicationPackage**, **Get-AzBatchApplication**, **New-AzBatchApplication**, **Remove-AzBatchApplication**, and **Set-AzBatchApplication**.</span></span>
  - <span data-ttu-id="77eee-671">`ApplicationId` は `ApplicationName` の別名になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-671">`ApplicationId` now is an alias of `ApplicationName`.</span></span>
* <span data-ttu-id="77eee-672">新しい `PSWindowsUserConfiguration` プロパティが `PSUserAccount` に追加されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-672">Added new `PSWindowsUserConfiguration` property to `PSUserAccount`.</span></span>
* <span data-ttu-id="77eee-673">`PSApplicationPackage` の `Version` が `Name` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-673">Renamed `Version` to `Name` on `PSApplicationPackage`.</span></span>
* <span data-ttu-id="77eee-674">`PSResourceFile` の `BlobSource` が `HttpUrl` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-674">Renamed `BlobSource` to `HttpUrl` on `PSResourceFile`.</span></span>
* <span data-ttu-id="77eee-675">`PSVirtualMachineConfiguration` から `OSDisk` プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-675">Removed `OSDisk` property from `PSVirtualMachineConfiguration`.</span></span>
* <span data-ttu-id="77eee-676">**Set-AzBatchPoolOSVersion** を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-676">Removed **Set-AzBatchPoolOSVersion**.</span></span> <span data-ttu-id="77eee-677">この操作は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="77eee-677">This operation is no longer supported.</span></span>
* <span data-ttu-id="77eee-678">`PSCloudServiceConfiguration` から `TargetOSVersion` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-678">Removed `TargetOSVersion` from `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="77eee-679">`PSCloudServiceConfiguration` の `CurrentOSVersion` が `OSVersion` に変更されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-679">Renamed `CurrentOSVersion` to `OSVersion` on `PSCloudServiceConfiguration`.</span></span>
* <span data-ttu-id="77eee-680">`PSPoolUsageMetrics` から `DataEgressGiB` および `DataIngressGiB` を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-680">Removed `DataEgressGiB` and `DataIngressGiB` from `PSPoolUsageMetrics`.</span></span>
* <span data-ttu-id="77eee-681">**Get-AzBatchNodeAgentSku** を削除し、**Get-AzBatchSupportedImage** に置き換えました。</span><span class="sxs-lookup"><span data-stu-id="77eee-681">Removed **Get-AzBatchNodeAgentSku** and replaced it with  **Get-AzBatchSupportedImage**.</span></span>
  - <span data-ttu-id="77eee-682">**Get-AzBatchSupportedImage** は、**Get-AzBatchNodeAgentSku** と同じデータを返しますが、よりわかりやすい形式で返します。</span><span class="sxs-lookup"><span data-stu-id="77eee-682">**Get-AzBatchSupportedImage** returns the same data as **Get-AzBatchNodeAgentSku** but in a more friendly format.</span></span>
  - <span data-ttu-id="77eee-683">新しく検証されていないイメージも返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-683">New non-verified images are also now returned.</span></span> <span data-ttu-id="77eee-684">各イメージの `Capabilities` と `BatchSupportEndOfLife` に関する追加情報も含まれています。</span><span class="sxs-lookup"><span data-stu-id="77eee-684">Additional information about `Capabilities` and `BatchSupportEndOfLife` for each image is also included.</span></span>
* <span data-ttu-id="77eee-685">**New-AzBatchPool** の新しい `MountConfiguration` パラメーターを使用して、プールの各ノードにリモート ファイル システムをマウントする機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-685">Added ability to mount remote file-systems on each node of a pool via the new `MountConfiguration` parameter of **New-AzBatchPool**.</span></span>
* <span data-ttu-id="77eee-686">トラフィックのソース ポートに基づいてプールへのネットワーク アクセスをブロックするネットワーク セキュリティ規則がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-686">Now support network security rules blocking network access to a pool based on the source port of the traffic.</span></span> <span data-ttu-id="77eee-687">これを行うには、`PSNetworkSecurityGroupRule` の `SourcePortRanges` プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="77eee-687">This is done via the `SourcePortRanges` property on `PSNetworkSecurityGroupRule`.</span></span>
* <span data-ttu-id="77eee-688">コンテナーを実行するときに、Batch でコンテナーの作業ディレクトリまたは Batch タスクの作業ディレクトリでのタスクの実行がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-688">When running a container, Batch now supports executing the task in the container working directory or in the Batch task working directory.</span></span> <span data-ttu-id="77eee-689">これは `PSTaskContainerSettings` の `WorkingDirectory` プロパティで制御されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-689">This is controlled by the `WorkingDirectory` property on `PSTaskContainerSettings`.</span></span>
* <span data-ttu-id="77eee-690">新しい `PublicIPs` プロパティを使用して `PSNetworkConfiguration` でパブリック IP のコレクションを指定する機能が追加されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-690">Added ability to specify a collection of public IPs on `PSNetworkConfiguration` via the new `PublicIPs` property.</span></span> <span data-ttu-id="77eee-691">これにより、プール内のノードは、ユーザーが指定した IP アドレスの一覧から IP を持つことが保証されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-691">This guarantees nodes in the Pool will have an IP from the list user provided IPs.</span></span>
* <span data-ttu-id="77eee-692">指定しない場合、`PSSTartTask` の `WaitForSuccess` の既定値は `$True` になります (以前は `$False` でした)。</span><span class="sxs-lookup"><span data-stu-id="77eee-692">When not specified, the default value of `WaitForSuccess` on `PSSTartTask` is now `$True` (was `$False`).</span></span>
* <span data-ttu-id="77eee-693">指定しない場合、`PSAutoUserSpecification` の `Scope` の既定値は `Pool` になります (以前は Windows では `Task`、Linux では `Pool` でした)。</span><span class="sxs-lookup"><span data-stu-id="77eee-693">When not specified, the default value of `Scope` on `PSAutoUserSpecification` is now `Pool` (was `Task` on Windows and `Pool` on Linux).</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-694">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-694">Az.Cdn</span></span>
* <span data-ttu-id="77eee-695">UrlRewriteAction と CacheKeyQueryStringAction を RulesEngine に導入しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-695">Introduced UrlRewriteAction and CacheKeyQueryStringAction to RulesEngine.</span></span>
* <span data-ttu-id="77eee-696">New-AzDeliveryRuleCondition コマンドレットで 'Selector' 入力が見つからないなどのいくつかのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-696">Fixed several bugs like missing 'Selector' Input in New-AzDeliveryRuleCondition cmdlet.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-697">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-697">Az.Compute</span></span>
* <span data-ttu-id="77eee-698">ディスク暗号化の設定機能</span><span class="sxs-lookup"><span data-stu-id="77eee-698">Disk Encryption Set feature</span></span>
    - <span data-ttu-id="77eee-699">新しいコマンドレット: New-AzDiskEncryptionSetConfig、New-AzDiskEncryptionSet、Get-AzDiskEncryptionSet、Remove-AzDiskEncryptionSet</span><span class="sxs-lookup"><span data-stu-id="77eee-699">New cmdlets:   New-AzDiskEncryptionSetConfig   New-AzDiskEncryptionSet   Get-AzDiskEncryptionSet   Remove-AzDiskEncryptionSet</span></span>
    - <span data-ttu-id="77eee-700">DiskEncryptionSetId パラメーターが、次のコマンドレットに追加されます。 Set-AzImageOSDisk、Set-AzVMOSDisk、Set-AzVmssStorageProfile、Add-AzImageDataDisk、New-AzVMDataDisk、Set-AzVMDataDisk、Add-AzVMDataDisk、Add-AzVmssDataDisk、Add-AzVmssVMDataDisk</span><span class="sxs-lookup"><span data-stu-id="77eee-700">DiskEncryptionSetId parameter is added to the following cmdlets:   Set-AzImageOSDisk   Set-AzVMOSDisk   Set-AzVmssStorageProfile   Add-AzImageDataDisk   New-AzVMDataDisk   Set-AzVMDataDisk   Add-AzVMDataDisk   Add-AzVmssDataDisk   Add-AzVmssVMDataDisk</span></span>
    - <span data-ttu-id="77eee-701">DiskEncryptionSetId と EncryptionType パラメーターが、次のコマンドレットに追加されます。 New-AzDiskConfig、New-AzSnapshotConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-701">DiskEncryptionSetId and EncryptionType parameters are added to the following cmdlets:   New-AzDiskConfig   New-AzSnapshotConfig</span></span>
* <span data-ttu-id="77eee-702">PublicIPAddressVersion パラメーターを New-AzVmssIPConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-702">Add PublicIPAddressVersion parameter to New-AzVmssIPConfig</span></span>
* <span data-ttu-id="77eee-703">カスタム スクリプト拡張機能の FileUris をパブリック設定から保護された設定に移動します</span><span class="sxs-lookup"><span data-stu-id="77eee-703">Move FileUris of custom script extension from public setting to protected setting</span></span>
* <span data-ttu-id="77eee-704">ScaleInPolicy を New-AzVmss、New-AzVmssConfig、および Update-AzVmss コマンドレットに追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-704">Add ScaleInPolicy to New-AzVmss, New-AzVmssConfig and Update-AzVmss cmdlets</span></span>
* <span data-ttu-id="77eee-705">重大な変更</span><span class="sxs-lookup"><span data-stu-id="77eee-705">Breaking changes</span></span>
    - <span data-ttu-id="77eee-706">CreateOption が Upload のときに、New-AzDiskConfig に対して DiskSizeGB ではなく UploadSizeInBytes パラメーターが使用されます</span><span class="sxs-lookup"><span data-stu-id="77eee-706">UploadSizeInBytes parameter is used instead of DiskSizeGB for New-AzDiskConfig when CreateOption is Upload</span></span>
    - <span data-ttu-id="77eee-707">PublishingProfile.Source.ManagedImage.Id は、GalleryImageVersion オブジェクトの StorageProfile.Source.Id に置き換えられます</span><span class="sxs-lookup"><span data-stu-id="77eee-707">PublishingProfile.Source.ManagedImage.Id is replaced with StorageProfile.Source.Id in GalleryImageVersion object</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-708">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-708">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-709">ADF .Net SDK のバージョンを 4.3.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-709">Update ADF .Net SDK version to 4.3.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-710">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-710">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-711">ADLS SDK バージョン (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha) を更新し、次の修正を行います。</span><span class="sxs-lookup"><span data-stu-id="77eee-711">Update ADLS SDK version (https://github.com/Azure/azure-data-lake-store-net/blob/preview-alpha/CHANGELOG.md#version-123-alpha), brings following fixes</span></span>
* <span data-ttu-id="77eee-712">ごみ箱またはディレクトリ エントリの creationtime を逆シリアル化できない場合に例外をスローしないようにします。</span><span class="sxs-lookup"><span data-stu-id="77eee-712">Avoid throwing exception while unable to deserialize the creationtime of the trash or directory entry.</span></span>
* <span data-ttu-id="77eee-713">adlsclient で要求タイムアウトごとに設定を公開します</span><span class="sxs-lookup"><span data-stu-id="77eee-713">Expose setting per request timeout in adlsclient</span></span>
* <span data-ttu-id="77eee-714">badoffset 復旧のための元の syncflag の受け渡しを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-714">Fix passing the original syncflag for badoffset recovery</span></span>
* <span data-ttu-id="77eee-715">応答が確認された後に継続トークンを取得するように EnumerateDirectory を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-715">Fix EnumerateDirectory to retrieve continuation token once response is checked</span></span>
* <span data-ttu-id="77eee-716">Concat のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-716">Fix Concat Bug</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="77eee-717">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-717">Az.FrontDoor</span></span>
* <span data-ttu-id="77eee-718">モジュール全体でさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-718">Fixed miscellaneous typos across module</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="77eee-719">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-719">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-720">Get-AzHDInsightCluster を使用して ADLSGen1 ストレージのクラスターを取得するときに、ユーザーが「有効な Base-64 文字列ではありません」というエラーを受け取るバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-720">Fixed the bug that customer will get 'Not a valid Base-64 string' error when using Get-AzHDInsightCluster to get the cluster with ADLSGen1 storage.</span></span>
* <span data-ttu-id="77eee-721">AzHDInsightClusterIdentity、AzHDInsightClusterConfig、AzHDInsightCluster の 3 つのコマンドレットに 'ApplicationId' という名前のパラメーターを追加して、顧客が Azure Data Lake にアクセスするためのサービス プリンシパル アプリケーション ID を指定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="77eee-721">Add a parameter named 'ApplicationId' to three cmdlets Add-AzHDInsightClusterIdentity, New-AzHDInsightClusterConfig and New-AzHDInsightCluster so that customer can provide the service principal application id for accessing Azure Data Lake.</span></span>
* <span data-ttu-id="77eee-722">Microsoft.Azure.Management.HDInsight を 2.1.0 から 5.1.0 に変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-722">Changed Microsoft.Azure.Management.HDInsight from 2.1.0 to 5.1.0</span></span>
* <span data-ttu-id="77eee-723">5 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-723">Removed five cmdlets:</span></span>
    - <span data-ttu-id="77eee-724">Get-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="77eee-724">Get-AzHDInsightOMS</span></span>
    - <span data-ttu-id="77eee-725">Enable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="77eee-725">Enable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="77eee-726">Disable-AzHDInsightOMS</span><span class="sxs-lookup"><span data-stu-id="77eee-726">Disable-AzHDInsightOMS</span></span>
    - <span data-ttu-id="77eee-727">Grant-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="77eee-727">Grant-AzHDInsightRdpServicesAccess</span></span>
    - <span data-ttu-id="77eee-728">Revoke-AzHDInsightRdpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="77eee-728">Revoke-AzHDInsightRdpServicesAccess</span></span>
* <span data-ttu-id="77eee-729">3 つのコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-729">Added three cmdlets:</span></span>
    - <span data-ttu-id="77eee-730">Get-AzHDInsightOMS を Get-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="77eee-730">Get-AzHDInsightMonitoring to replace Get-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="77eee-731">Enable-AzHDInsightOMS を Enable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="77eee-731">Enable-AzHDInsightMonitoring to replace Enable-AzHDInsightOMS.</span></span>
    - <span data-ttu-id="77eee-732">Disable-AzHDInsightOMS を Disable-AzHDInsightMonitoring に置き換えます。</span><span class="sxs-lookup"><span data-stu-id="77eee-732">Disable-AzHDInsightMonitoring to replace Disable-AzHDInsightOMS.</span></span>
* <span data-ttu-id="77eee-733">特定の場所からの機能情報の取得をサポートするために、コマンドレット Get-AzHDInsightProperties を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-733">Fixed cmdlet Get-AzHDInsightProperties to support get capabilities information from a specific location.</span></span>
* <span data-ttu-id="77eee-734">Add-AzHDInsightConfigValue からパラメーターセット ('Spark1'、'Spark2') を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-734">Removed parameter sets('Spark1', 'Spark2') from Add-AzHDInsightConfigValue.</span></span>
* <span data-ttu-id="77eee-735">コマンドレット Add-AzHDInsightSecurityProfile のヘルプ ドキュメントに例を追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-735">Add examples to the help documents of cmdlet Add-AzHDInsightSecurityProfile.</span></span>
* <span data-ttu-id="77eee-736">次のコマンドレットの出力の型を変更しました:</span><span class="sxs-lookup"><span data-stu-id="77eee-736">Changed output type of the following cmdlets:</span></span>
*  - <span data-ttu-id="77eee-737">Get-AzHDInsightProperties の出力の型を CapabilitiesResponse から AzureHDInsightCapabilities に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-737">Changed the output type of Get-AzHDInsightProperties from  CapabilitiesResponse to AzureHDInsightCapabilities.</span></span>
*  - <span data-ttu-id="77eee-738">Remove-AzHDInsightCluster の出力の型を ClusterGetResponse からブール値に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-738">Changed the output type of Remove-AzHDInsightCluster from ClusterGetResponse to bool.</span></span>
*  - <span data-ttu-id="77eee-739">Set-AzHDInsightGatewaySettings HttpConnectivitySettings の出力の型を GatewaySettings に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-739">Changed the output type of Set-AzHDInsightGatewaySettings HttpConnectivitySettings to GatewaySettings.</span></span>
* <span data-ttu-id="77eee-740">いくつかのシナリオ テスト ケースを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-740">Added some scenario test cases.</span></span>
* <span data-ttu-id="77eee-741">次の別名を削除します。'Add-AzHDInsightConfigValues'、'Get-AzHDInsightProperties'。</span><span class="sxs-lookup"><span data-stu-id="77eee-741">Remove some alias: 'Add-AzHDInsightConfigValues', 'Get-AzHDInsightProperties'.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-742">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-742">Az.IotHub</span></span>
* <span data-ttu-id="77eee-743">破壊的変更:</span><span class="sxs-lookup"><span data-stu-id="77eee-743">Breaking changes:</span></span>
    - <span data-ttu-id="77eee-744">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="77eee-744">The cmdlet 'Add-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="77eee-745">コマンドレット 'Add-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-745">The parameter set '__AllParameterSets' for cmdlet 'Add-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="77eee-746">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="77eee-746">The cmdlet 'Get-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="77eee-747">コマンドレット 'Get-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-747">The parameter set '__AllParameterSets' for cmdlet 'Get-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="77eee-748">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-748">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubProperties' has been removed.</span></span>
    - <span data-ttu-id="77eee-749">'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' 型のプロパティ 'OperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-749">The property 'OperationsMonitoringProperties' of type 'Microsoft.Azure.Commands.Management.IotHub.Models.PSIotHubInputProperties' has been removed.</span></span>
    - <span data-ttu-id="77eee-750">コマンドレット 'New-AzIotHubExportDevice' では、別名 'New-AzIotHubExportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-750">The cmdlet 'New-AzIotHubExportDevice' no longer supports the alias 'New-AzIotHubExportDevices'.</span></span>
    - <span data-ttu-id="77eee-751">コマンドレット 'New-AzIotHubImportDevice' では、別名 'New-AzIotHubImportDevices' がサポートされなくなりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-751">The cmdlet 'New-AzIotHubImportDevice' no longer supports the alias 'New-AzIotHubImportDevices'.</span></span>
    - <span data-ttu-id="77eee-752">コマンドレット 'Removet-AzIotHubEventHubConsumerGroup' でパラメーター 'EventHubEndpointName' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="77eee-752">The cmdlet 'Remove-AzIotHubEventHubConsumerGroup' no longer supports the parameter 'EventHubEndpointName' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="77eee-753">コマンドレット 'Remove-AzIotHubEventHubConsumerGroup' のパラメーター セット '__AllParameterSets' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-753">The parameter set '__AllParameterSets' for cmdlet 'Remove-AzIotHubEventHubConsumerGroup' has been removed.</span></span>
    - <span data-ttu-id="77eee-754">コマンドレット 'Set-AzIotHub' でパラメーター 'OperationsMonitoringProperties' がサポートされなくなり、元のパラメーター名の別名は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="77eee-754">The cmdlet 'Set-AzIotHub' no longer supports the parameter 'OperationsMonitoringProperties' and no alias was found for the original parameter name.</span></span>
    - <span data-ttu-id="77eee-755">コマンドレット 'Set-AzIotHub' のパラメーター セット 'UpdateOperationsMonitoringProperties' が削除されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-755">The parameter set 'UpdateOperationsMonitoringProperties' for cmdlet 'Set-AzIotHub' has been removed.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-756">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-756">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-757">Azure Site Recovery は、Azure から Azure での NSG、パブリック IP、内部ロード バランサーなどのネットワーク リソースの構成をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-757">Azure Site Recovery support to configure networking resources like NSG, public IP and internal load balancers for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-758">Azure Site Recovery は VMWare から Azure でのマネージド ディスクへの書き込みをサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-758">Azure Site Recovery Support to write to managed disk for vMWare to Azure.</span></span>
* <span data-ttu-id="77eee-759">Azure Site Recovery は VMWare から Azure での NIC 削減をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-759">Azure Site Recovery Support to NIC reduction for vMWare to Azure.</span></span>
* <span data-ttu-id="77eee-760">Azure Site Recovery は Azure から Azure での高速ネットワークをサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-760">Azure Site Recovery Support to accelerated networking for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-761">Azure Site Recovery は Azure から Azure でのエージェント自動更新をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-761">Azure Site Recovery Support to agent auto update for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-762">Azure Site Recovery は Azure から Azure での Standard SSD をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-762">Azure Site Recovery Support to Standard SSD for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-763">Azure Site Recovery は Azure から Azure での Azure Disk Encryption の 2 パスをサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-763">Azure Site Recovery Support to Azure Disk Encryption two pass for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-764">Azure Site Recovery は Azure から Azure で新しく追加されたディスクの保護をサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-764">Azure Site Recovery Support to protect newly added disk for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-765">VM の SoftDelete 機能を追加し、softdelete のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-765">Added SoftDelete feature for VM and added tests for softdelete</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-766">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-766">Az.Resources</span></span>
* <span data-ttu-id="77eee-767">依存関係アセンブリ Microsoft.Extensions.Caching.Memory を 1.1.1 から 2.2 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-767">Update dependency assembly Microsoft.Extensions.Caching.Memory from 1.1.1 to 2.2</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-768">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-768">Az.Network</span></span>
* <span data-ttu-id="77eee-769">汎用サービス プロバイダーをサポートするために、PrivateEndpointConnection のすべてのコマンドレットを変更します。</span><span class="sxs-lookup"><span data-stu-id="77eee-769">Change all cmdlets for PrivateEndpointConnection to support generic service provider.</span></span>
    - <span data-ttu-id="77eee-770">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-770">Updated cmdlet:</span></span>
        - <span data-ttu-id="77eee-771">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-771">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-772">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-772">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-773">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-773">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-774">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-774">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-775">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-775">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="77eee-776">PrivateLinkResource の新しいコマンドレットを追加し、これも汎用サービス プロバイダーをサポートします。</span><span class="sxs-lookup"><span data-stu-id="77eee-776">Add new cmdlet for PrivateLinkResource and it also support generic service provider.</span></span>
    - <span data-ttu-id="77eee-777">新しいコマンドレット: </span><span class="sxs-lookup"><span data-stu-id="77eee-777">New cmdlet:</span></span>
        - <span data-ttu-id="77eee-778">Get-AzPrivateLinkResource</span><span class="sxs-lookup"><span data-stu-id="77eee-778">Get-AzPrivateLinkResource</span></span>
* <span data-ttu-id="77eee-779">機能 Proxy Protocol V2 の新しいフィールドとパラメーターを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-779">Add new fields and parameter for the feature Proxy Protocol V2.</span></span>
    - <span data-ttu-id="77eee-780">PrivateLinkService にプロパティ EnableProxyProtocol を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-780">Add property EnableProxyProtocol in PrivateLinkService</span></span>
    - <span data-ttu-id="77eee-781">PrivateEndpointConnection にプロパティ LinkIdentifier を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-781">Add property LinkIdentifier in PrivateEndpointConnection</span></span>
    - <span data-ttu-id="77eee-782">新しい省略可能なパラメーター EnableProxyProtocol を追加するように New-AzPrivateLinkService を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-782">Updated New-AzPrivateLinkService to add a new optional parameter EnableProxyProtocol.</span></span>
* <span data-ttu-id="77eee-783">'New-AzApplicationGatewaySku' のリファレンス ドキュメントで間違ったパラメーターの説明を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-783">Fix incorrect parameter description in 'New-AzApplicationGatewaySku' reference documentation</span></span>
* <span data-ttu-id="77eee-784">Azure ファイアウォール ポリシーをサポートするための新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-784">New cmdlets to support the azure firewall policy</span></span>
* <span data-ttu-id="77eee-785">VirtualHub の子リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-785">Add support for child resource RouteTables of VirtualHub</span></span>
    - <span data-ttu-id="77eee-786">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-786">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-787">Add-AzVirtualHubRoute</span><span class="sxs-lookup"><span data-stu-id="77eee-787">Add-AzVirtualHubRoute</span></span>
        - <span data-ttu-id="77eee-788">Add-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="77eee-788">Add-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="77eee-789">Get-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="77eee-789">Get-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="77eee-790">Remove-AzVirtualHubRouteTable</span><span class="sxs-lookup"><span data-stu-id="77eee-790">Remove-AzVirtualHubRouteTable</span></span>
        - <span data-ttu-id="77eee-791">Set-AzVirtualHub</span><span class="sxs-lookup"><span data-stu-id="77eee-791">Set-AzVirtualHub</span></span>
* <span data-ttu-id="77eee-792">VirtualHub の Sku と VirtualWANType の VirtualHub という新しいプロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-792">Add support for new properties Sku of VirtualHub and VirtualWANType of VirtualWan</span></span>
    - <span data-ttu-id="77eee-793">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-793">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="77eee-794">New-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-794">New-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="77eee-795">Update-AzVirtualHub: パラメーター Sku を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-795">Update-AzVirtualHub : added parameter Sku</span></span>
        - <span data-ttu-id="77eee-796">New-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-796">New-AzVirtualWan : added parameter VirtualWANType</span></span>
        - <span data-ttu-id="77eee-797">Update-AzVirtualWan: パラメーター VirtualWANType を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-797">Update-AzVirtualWan : added parameter VirtualWANType</span></span>
* <span data-ttu-id="77eee-798">HubVnetConnection、VpnConnection、および ExpressRouteConnection の EnableInternetSecurity プロパティのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-798">Add support for EnableInternetSecurity property for HubVnetConnection, VpnConnection and ExpressRouteConnection</span></span>
    - <span data-ttu-id="77eee-799">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-799">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-800">Update-AzureRmVirtualHubVnetConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-800">Update-AzureRmVirtualHubVnetConnection</span></span>
    - <span data-ttu-id="77eee-801">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-801">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="77eee-802">New-AzureRmVirtualHubVnetConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-802">New-AzureRmVirtualHubVnetConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="77eee-803">New-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-803">New-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="77eee-804">Update-AzureRmVpnConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-804">Update-AzureRmVpnConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="77eee-805">New-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-805">New-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
        - <span data-ttu-id="77eee-806">Set-AzureRmExpressRouteConnection: パラメーター EnableInternetSecurity を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-806">Set-AzureRmExpressRouteConnection : added parameter EnableInternetSecurity</span></span>
* <span data-ttu-id="77eee-807">TopLevel WebApplicationFirewall ポリシーを構成するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-807">Add support for Configuring TopLevel WebApplicationFirewall Policy</span></span>
    - <span data-ttu-id="77eee-808">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-808">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-809">New-AzApplicationGatewayFirewallPolicySetting</span><span class="sxs-lookup"><span data-stu-id="77eee-809">New-AzApplicationGatewayFirewallPolicySetting</span></span>
        - <span data-ttu-id="77eee-810">New-AzApplicationGatewayFirewallPolicyExclusion</span><span class="sxs-lookup"><span data-stu-id="77eee-810">New-AzApplicationGatewayFirewallPolicyExclusion</span></span>
        - <span data-ttu-id="77eee-811">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span><span class="sxs-lookup"><span data-stu-id="77eee-811">New-AzApplicationGatewayFirewallPolicyManagedRuleGroupOverride</span></span>
        - <span data-ttu-id="77eee-812">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span><span class="sxs-lookup"><span data-stu-id="77eee-812">New-AzApplicationGatewayFirewallPolicyManagedRuleOverride</span></span>
        - <span data-ttu-id="77eee-813">New-AzApplicationGatewayFirewallPolicyManagedRule</span><span class="sxs-lookup"><span data-stu-id="77eee-813">New-AzApplicationGatewayFirewallPolicyManagedRule</span></span>
        - <span data-ttu-id="77eee-814">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-814">New-AzApplicationGatewayFirewallPolicyManagedRuleSet</span></span>
    - <span data-ttu-id="77eee-815">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-815">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="77eee-816">New-AzApplicationGatewayFirewallPolicy: パラメーター PolicySetting、ManagedRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-816">New-AzApplicationGatewayFirewallPolicy : added parameter PolicySetting, ManagedRule</span></span>
* <span data-ttu-id="77eee-817">CustomRule での Geo-Match 演算子のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-817">Added support for Geo-Match operator on CustomRule</span></span>
    - <span data-ttu-id="77eee-818">FirewallCondition の演算子に GeoMatch を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-818">Added GeoMatch to the operator on the FirewallCondition</span></span>
* <span data-ttu-id="77eee-819">perListener および perSite ファイアウォール ポリシーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-819">Added support for perListener and perSite Firewall policy</span></span>
    - <span data-ttu-id="77eee-820">省略可能なパラメーターを持つように更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-820">Cmdlets updated with optional parameters:</span></span>
        - <span data-ttu-id="77eee-821">New-AzApplicationGatewayHttpListener: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-821">New-AzApplicationGatewayHttpListener : added parameter FirewallPolicy, FirewallPolicyId</span></span>
        - <span data-ttu-id="77eee-822">New-AzApplicationGatewayPathRuleConfig: パラメーター FirewallPolicy、FirewallPolicyId を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-822">New-AzApplicationGatewayPathRuleConfig : added parameter FirewallPolicy, FirewallPolicyId</span></span>
* <span data-ttu-id="77eee-823">'PSBastion' で AzureBastionSubnet という名前の必須サブネットの大文字と小文字が区別されないように修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-823">Fix required subnet with name AzureBastionSubnet in 'PSBastion' can be case insensitive</span></span>
* <span data-ttu-id="77eee-824">Azure Firewall のネットワーク規則における宛先 FQDN と NAT 規則における変換された FQDN のサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-824">Support for Destination FQDNs in Network Rules and Translated FQDN in NAT Rules for Azure Firewall</span></span>
* <span data-ttu-id="77eee-825">IpGroup の最上位リソース RouteTables のサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-825">Add support for top level resource RouteTables of IpGroup</span></span>
    - <span data-ttu-id="77eee-826">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-826">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-827">New-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="77eee-827">New-AzIpGroup</span></span>
        - <span data-ttu-id="77eee-828">Remove-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="77eee-828">Remove-AzIpGroup</span></span>
        - <span data-ttu-id="77eee-829">Get-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="77eee-829">Get-AzIpGroup</span></span>
        - <span data-ttu-id="77eee-830">Set-AzIpGroup</span><span class="sxs-lookup"><span data-stu-id="77eee-830">Set-AzIpGroup</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-831">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-831">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-832">Add-AzServiceFabricApplicationCertificate コマンドレットを削除します。このシナリオは、Add-AzVmssSecret のよってカバーされています。</span><span class="sxs-lookup"><span data-stu-id="77eee-832">Remove Add-AzServiceFabricApplicationCertificate cmdlet as this scenario is covered by Add-AzVmssSecret.</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-833">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-833">Az.Sql</span></span>
* <span data-ttu-id="77eee-834">Managed Instance での削除されたデータベースの復元のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-834">Added support for restore of dropped databases on Managed Instances.</span></span>
* <span data-ttu-id="77eee-835">古い監査コマンドレットをコードから非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-835">Deprecated from code old auditing cmdlets.</span></span>
* <span data-ttu-id="77eee-836">非推奨の別名を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-836">Removed deprecated aliases:</span></span>
* <span data-ttu-id="77eee-837">Get-AzSqlDatabaseIndexRecommendations (代わりに Get-AzSqlDatabaseIndexRecommendation を使用します)</span><span class="sxs-lookup"><span data-stu-id="77eee-837">Get-AzSqlDatabaseIndexRecommendations (use Get-AzSqlDatabaseIndexRecommendation instead)</span></span>
* <span data-ttu-id="77eee-838">Get-AzSqlDatabaseRestorePoints (代わりに Get-AzSqlDatabaseRestorePoint を使用します)</span><span class="sxs-lookup"><span data-stu-id="77eee-838">Get-AzSqlDatabaseRestorePoints (use Get-AzSqlDatabaseRestorePoint instead)</span></span>
* <span data-ttu-id="77eee-839">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-839">Remove Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="77eee-840">非推奨の脆弱性評価の設定コマンドレットの別名を削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-840">Remove aliases for deprecated Vulnerability Assessment Settings cmdlets</span></span>
* <span data-ttu-id="77eee-841">高度な脅威検出の設定コマンドレットを非推奨にします</span><span class="sxs-lookup"><span data-stu-id="77eee-841">Deprecate Advanced Threat Detection Settings cmdlets</span></span>
* <span data-ttu-id="77eee-842">データベースの列に対する機密性の推奨を無効および有効にするコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-842">Adding cmdlets to Disable and enable sensitivity recommendations on columns in a database.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-843">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-843">Az.Storage</span></span>
* <span data-ttu-id="77eee-844">Storage アカウントの作成または更新時に大容量ファイル共有の有効化をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-844">Support enable Large File share when create or update Storage account</span></span>
    -  <span data-ttu-id="77eee-845">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-845">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="77eee-846">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-846">Set-AzStorageAccount</span></span>
* <span data-ttu-id="77eee-847">ファイル ハンドルを閉じる/取得するときに、入力パスがファイル ディレクトリまたはファイルであることの確認をスキップして、DeletePending ステータスのオブジェクトでのエラーを回避します</span><span class="sxs-lookup"><span data-stu-id="77eee-847">When close/get File handle, skip check the input path is File directory or File, to avoid failure with object in DeletePending status</span></span>
    -  <span data-ttu-id="77eee-848">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="77eee-848">Get-AzStorageFileHandle</span></span>
    -  <span data-ttu-id="77eee-849">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="77eee-849">Close-AzStorageFileHandle</span></span>

## <a name="280---october-2019"></a><span data-ttu-id="77eee-850">2.8.0 - 2019 年 10 月</span><span class="sxs-lookup"><span data-stu-id="77eee-850">2.8.0 - October 2019</span></span>
### <a name="general"></a><span data-ttu-id="77eee-851">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-851">General</span></span>
* <span data-ttu-id="77eee-852">Az. HealthcareApis 1.0.0 リリース</span><span class="sxs-lookup"><span data-stu-id="77eee-852">Az.HealthcareApis 1.0.0 release</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-853">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-853">Az.Accounts</span></span>
* <span data-ttu-id="77eee-854">生成されるモジュールのテレメトリと URL 書き換えを更新し、Windows 単体テストを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-854">Update telemetry and url rewriting for generated modules, fix windows unit tests.</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="77eee-855">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-855">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-856">**Set-AzApiManagementApi** - Api を ApiVersionSet に更新するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-856">**Set-AzApiManagementApi** - Added support for Updating Api into ApiVersionSet</span></span>
    - <span data-ttu-id="77eee-857">次の問題を修正: https://github.com/Azure/azure-powershell/issues/10068</span><span class="sxs-lookup"><span data-stu-id="77eee-857">Fix for issue https://github.com/Azure/azure-powershell/issues/10068</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-858">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-858">Az.Automation</span></span>
* <span data-ttu-id="77eee-859">Linux リブート設定パラメーターの New-AzureAutomationSoftwareUpdateConfiguration コマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-859">Fixed New-AzureAutomationSoftwareUpdateConfiguration cmdlet for Linux reboot setting parameter.</span></span>

#### <a name="azbatch"></a><span data-ttu-id="77eee-860">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="77eee-860">Az.Batch</span></span>
* <span data-ttu-id="77eee-861">**Get-AzBatchNodeAgentSku** は非推奨となり、バージョン 2.0.0 で **Get-AzBatchSupportImage** に置き換えられます。</span><span class="sxs-lookup"><span data-stu-id="77eee-861">**Get-AzBatchNodeAgentSku** is deprecated and will be replaced by **Get-AzBatchSupportImage** in version 2.0.0.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-862">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-862">Az.Compute</span></span>
* <span data-ttu-id="77eee-863">New-AzVM と New-AzVmss コマンドレットに Priority、EvictionPolicy、および MaxPrice パラメーターを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-863">Add Priority, EvictionPolicy, and MaxPrice parameters to New-AzVM and New-AzVmss cmdlets</span></span>
* <span data-ttu-id="77eee-864">Add-AzVMAdditionalUnattendContent および Add-AzVMSshPublicKey コマンドレットの警告メッセージとヘルプ ドキュメントを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-864">Fix warning message and help document for Add-AzVMAdditionalUnattendContent and Add-AzVMSshPublicKey cmdlets</span></span>
* <span data-ttu-id="77eee-865">Set-AzVMDiskEncryptionExtension のマネージド ディスクを使用する Linux VM の -skipVmBackup 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-865">Fix -skipVmBackup exception for Linux VMs with managed disks for Set-AzVMDiskEncryptionExtension.</span></span>
* <span data-ttu-id="77eee-866">Set-AzVMDiskEncryptionExtension の 2つのパス シナリオでの暗号化設定の更新のバグを修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-866">Fix bug in update encryption settings in Set-AzVMDiskEncryptionExtension, two pass scenario.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-867">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-867">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-868">ADF V2 データ フロー用の次の CRUD コマンドを追加します:Set-AzDataFactoryV2DataFlow、Remove-AzDataFactoryV2DataFlow、Get-AzDataFactoryV2DataFlow。</span><span class="sxs-lookup"><span data-stu-id="77eee-868">Adding CRUD commands for ADF V2 data flow: Set-AzDataFactoryV2DataFlow, Remove-AzDataFactoryV2DataFlow, and Get-AzDataFactoryV2DataFlow.</span></span>
* <span data-ttu-id="77eee-869">ADF V2 データ フローのデバッグ セッション用のアクション コマンドを追加します:Start-AzDataFactoryV2DataFlowDebugSession、Get-AzDataFactoryV2DataFlowDebugSession、Add-AzDataFactoryV2DataFlowDebugSessionPackage、Invoke-AzDataFactoryV2DataFlowDebugSessionCommand、Stop-AzDataFactoryV2DataFlowDebugSession。</span><span class="sxs-lookup"><span data-stu-id="77eee-869">Adding action commands for ADF V2 data flow debug Session: Start-AzDataFactoryV2DataFlowDebugSession, Get-AzDataFactoryV2DataFlowDebugSession, Add-AzDataFactoryV2DataFlowDebugSessionPackage, Invoke-AzDataFactoryV2DataFlowDebugSessionCommand and Stop-AzDataFactoryV2DataFlowDebugSession.</span></span>
* <span data-ttu-id="77eee-870">ADF .Net SDK のバージョンを 4.2.0 に更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-870">Update ADF .Net SDK version to 4.2.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-871">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-871">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-872">ドメインを使用せずに '-' を含むアカウントを渡すことができるように、アカウントの検証を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-872">Fix account validation so that accounts with '-' can be passed without domain</span></span>

#### <a name="azhealthcareapis"></a><span data-ttu-id="77eee-873">Az.HealthcareApis</span><span class="sxs-lookup"><span data-stu-id="77eee-873">Az.HealthcareApis</span></span>
* <span data-ttu-id="77eee-874">PowerShell のバージョンを1.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-874">Updated the powershell version to 1.0.0</span></span>
* <span data-ttu-id="77eee-875">SDK のバージョンを1.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-875">Updated the SDK version to 1.0.2</span></span>
* <span data-ttu-id="77eee-876">新しい SDK バージョンを参照するようにテストを更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-876">Update in tests to refer to new SDK version</span></span>
* <span data-ttu-id="77eee-877">出力構造を入れ子からフラット化に更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-877">Updated the output structure from nested to flattened.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-878">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-878">Az.IotHub</span></span>
* <span data-ttu-id="77eee-879">新しいルーティング ソースの追加:DigitalTwinChangeEvents</span><span class="sxs-lookup"><span data-stu-id="77eee-879">Add new routing source: DigitalTwinChangeEvents</span></span>
* <span data-ttu-id="77eee-880">軽微なバグの修正:Get-AzIothub が subscriptionId を返さない</span><span class="sxs-lookup"><span data-stu-id="77eee-880">Minor bug fix: Get-AzIothub not returning subscriptionId</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-881">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-881">Az.Monitor</span></span>
* <span data-ttu-id="77eee-882">アクション グループに追加された新しいアクション グループ受信者: -ItsmReceiver、-VoiceReceiver、-ArmRoleReceiver、-AzureFunctionReceiver、-LogicAppReceiver、-AutomationRunbookReceiver、-AzureAppPushReceiver</span><span class="sxs-lookup"><span data-stu-id="77eee-882">New action group receivers added for action group   -ItsmReceiver   -VoiceReceiver   -ArmRoleReceiver   -AzureFunctionReceiver   -LogicAppReceiver   -AutomationRunbookReceiver   -AzureAppPushReceiver</span></span>
* <span data-ttu-id="77eee-883">受信側で有効になっている共通のアラート スキーマを使用します。</span><span class="sxs-lookup"><span data-stu-id="77eee-883">Use common alert schema enabled for the receivers.</span></span> <span data-ttu-id="77eee-884">これは、SMS、Azure アプリのプッシュ、ITSM、および音声の受信側には適用されません</span><span class="sxs-lookup"><span data-stu-id="77eee-884">This is not applicable for SMS, Azure App push , ITSM and Voice recievers</span></span>
* <span data-ttu-id="77eee-885">Webhook で Azure Active Directory 認証をサポートするようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-885">Webhooks now supports Azure active directory authentication .</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-886">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-886">Az.Network</span></span>
* <span data-ttu-id="77eee-887">サービス エンドポイント ポリシーに使用できる別名を取得するために呼び出すことができる新しいコマンドレット Get-AzAvailableServiceAlias を追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-887">Add new cmdlet Get-AzAvailableServiceAlias which can be called to get the aliases that can be used for Service Endpoint Policies.</span></span>
* <span data-ttu-id="77eee-888">Virtual Network ゲートウェイ接続にトラフィック セレクターを追加するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-888">Added support for the adding traffic selectors to Virtual Network Gateway Connections</span></span>
    - <span data-ttu-id="77eee-889">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-889">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-890">New-AzureRmTrafficSelectorPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-890">New-AzureRmTrafficSelectorPolicy</span></span>
    - <span data-ttu-id="77eee-891">省略可能なパラメーターでコマンドレットが更新されました: -TrafficSelectorPolicies、-New-AzureRmVirtualNetworkGatewayConnection、-Set-AzureRmVirtualNetworkGatewayConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-891">Cmdlets updated with optional parameter -TrafficSelectorPolicies   -New-AzureRmVirtualNetworkGatewayConnection   -Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="77eee-892">ネットワーク セキュリティ規則の構成で ESP および AH プロトコルのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-892">Add support for ESP and AH protocols in network security rule configurations</span></span>
    - <span data-ttu-id="77eee-893">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-893">Updated cmdlets:</span></span>
        - <span data-ttu-id="77eee-894">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-894">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="77eee-895">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-895">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="77eee-896">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-896">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="77eee-897">Cortex コマンドレットでの例外処理を改善します</span><span class="sxs-lookup"><span data-stu-id="77eee-897">Improve handling of exceptions in Cortex cmdlets</span></span>
* <span data-ttu-id="77eee-898">VirtualNetworkGateways の新しい世代と SKU</span><span class="sxs-lookup"><span data-stu-id="77eee-898">New Generations and SKUs for VirtualNetworkGateways</span></span>
  - <span data-ttu-id="77eee-899">VirtualNetworkGateways の新しい世代を導入します。</span><span class="sxs-lookup"><span data-stu-id="77eee-899">Introduce new Generations for VirtualNetworkGateways.</span></span>
  - <span data-ttu-id="77eee-900">VirtualNetworkGateways の新しい高スループット SKU を導入します。</span><span class="sxs-lookup"><span data-stu-id="77eee-900">Introduce new high throughput SKUs for VirtualNetworkGateways.</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="77eee-901">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="77eee-901">Az.RedisCache</span></span>
* <span data-ttu-id="77eee-902">'-Size' パラメーターの欠損値を含むように 'Set-AzRedisCache' 参照ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-902">Updated 'Set-AzRedisCache' reference documentation to include missing values for '-Size' parameter</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-903">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-903">Az.Sql</span></span>
* <span data-ttu-id="77eee-904">Managed Instance に Active Directory 管理者を設定するためのサポートを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-904">Add support for setting Active Directory Administrator on Managed Instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-905">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-905">Az.Storage</span></span>
* <span data-ttu-id="77eee-906">Storage クライアント ライブラリを 11.1.0 にアップグレードします</span><span class="sxs-lookup"><span data-stu-id="77eee-906">Upgrade Storage Client Library to 11.1.0</span></span>
* <span data-ttu-id="77eee-907">管理プレーン API を使用してコンテナーを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="77eee-907">List containers with Management plane API, will list with NextPageLink</span></span>
    -  <span data-ttu-id="77eee-908">Get-AzRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="77eee-908">Get-AzRmStorageContainer</span></span>
* <span data-ttu-id="77eee-909">サブスクリプションから Storage アカウントを一覧表示する場合に、NextPageLink で一覧表示する</span><span class="sxs-lookup"><span data-stu-id="77eee-909">List Storage accounts from subscription, will list with NextPageLink</span></span>
    -  <span data-ttu-id="77eee-910">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-910">Get-AzStorageAccount</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="77eee-911">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="77eee-911">Az.StorageSync</span></span>
* <span data-ttu-id="77eee-912">Reset-AzStorageSyncServerCertificate の問題 9810 を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-912">Fix Issue 9810 in Reset-AzStorageSyncServerCertificate.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-913">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-913">Az.Websites</span></span>
* <span data-ttu-id="77eee-914">Set-AzWebApp でアプリの ASP の更新が失敗していました</span><span class="sxs-lookup"><span data-stu-id="77eee-914">Set-AzWebApp updating ASP of an app was failing</span></span>

## <a name="270---september-2019"></a><span data-ttu-id="77eee-915">2.7.0 - 2019 年 9 月</span><span class="sxs-lookup"><span data-stu-id="77eee-915">2.7.0 - September 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="77eee-916">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-916">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-917">'Set-AzApiManagementPolicy' リファレンス ドキュメントで '-Format' パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-917">Update '-Format' parameter description in 'Set-AzApiManagementPolicy' reference documentation</span></span>
* <span data-ttu-id="77eee-918">リファレンス ドキュメントから、非推奨のコマンドレット 'Update-AzApiManagementDeployment' の参照を削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-918">Removed references of deprecated cmdlet 'Update-AzApiManagementDeployment' from reference documentation.</span></span> <span data-ttu-id="77eee-919">代わりに 'Set-AzApiManagement' を使用してください。</span><span class="sxs-lookup"><span data-stu-id="77eee-919">Use 'Set-AzApiManagement' instead.</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-920">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-920">Az.Automation</span></span>
* <span data-ttu-id="77eee-921">'Register-AzAutomationDscNode' のリファレンス ドキュメントで例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-921">Fixed example typo in reference documentation for 'Register-AzAutomationDscNode'</span></span>
* <span data-ttu-id="77eee-922">Register-AzAutomationDSCNode に OS 制限の説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-922">Added clarification on OS restriction to Register-AzAutomationDSCNode</span></span>
* <span data-ttu-id="77eee-923">AzAutomationRunbook コマンドレットの -Wait オプションにおける null 参照の例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-923">Fixed Start-AzAutomationRunbook cmdlet Null reference exception for -Wait option.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-924">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-924">Az.Compute</span></span>
* <span data-ttu-id="77eee-925">UploadSizeInBytes パラメーターを New-AzDiskConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-925">Add UploadSizeInBytes parameter tp New-AzDiskConfig</span></span>
* <span data-ttu-id="77eee-926">Incremental パラメーターを New-AzSnapshotConfig に追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-926">Add Incremental parameter to New-AzSnapshotConfig</span></span>
* <span data-ttu-id="77eee-927">低優先度の仮想マシン機能を追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-927">Add a low priority virtual machine feature:</span></span>
    - <span data-ttu-id="77eee-928">MaxPrice、EvictionPolicy、および Priority パラメーターが New-AzVMConfig に追加されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-928">MaxPrice, EvictionPolicy and Priority parameters are added to New-AzVMConfig.</span></span>
    - <span data-ttu-id="77eee-929">MaxPrice パラメーターが New-AzVmssConfig、Update-AzVM、Update-AzVmssAzVmss コマンドレットに追加されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-929">MaxPrice parameter is added to New-AzVmssConfig, Update-AzVM and Update-AzVmss cmdlets.</span></span>
* <span data-ttu-id="77eee-930">サブスクリプション内のすべての可用性セットを一覧表示するときの Get-AzAvailabilitySet コマンドレットの VM 参照の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-930">Fix VM reference issue for Get-AzAvailabilitySet cmdlet when it lists all availability sets in the subscription.</span></span>
* <span data-ttu-id="77eee-931">Get-AzRemoteDesktopFile の null 例外を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-931">Fix the null exception for Get-AzRemoteDesktopFile.</span></span>
* <span data-ttu-id="77eee-932">VHD Seek メソッドの終了相対位置を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-932">Fix VHD Seek method for end-relative position.</span></span>
* <span data-ttu-id="77eee-933">New-AzVM と Update-AzVM の UltraSSD の問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-933">Fix UltraSSD issue for New-AzVM and Update-AzVM.</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-934">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-934">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-935">ADF V2 の新しい 3 つのコマンド (AzDataFactoryV2TriggerSubscription、Remove-AzDataFactoryV2TriggerSubscription、Get-AzDataFactoryV2TriggerSubscriptionStatus) を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-935">Adding 3 new commands for ADF V2 - Add-AzDataFactoryV2TriggerSubscription, Remove-AzDataFactoryV2TriggerSubscription, and Get-AzDataFactoryV2TriggerSubscriptionStatus</span></span>
* <span data-ttu-id="77eee-936">ADF .Net SDK のバージョンを 4.1.3 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-936">Updated ADF .Net SDK version to 4.1.3</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="77eee-937">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-937">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-938">破壊的変更についてお知らせします</span><span class="sxs-lookup"><span data-stu-id="77eee-938">Call out breaking changes</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-939">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-939">Az.IotHub</span></span>
* <span data-ttu-id="77eee-940">geo ペアのディザスター リカバリー リージョンへの IotHub のフェールオーバーを呼び出すためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-940">Add support to invoke failover for an IotHub to the geo-paired disaster recovery region.</span></span>
* <span data-ttu-id="77eee-941">IotHub のメッセージ詳細化を管理するためのサポートを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-941">Add support to manage message enrichment for an IotHub.</span></span> <span data-ttu-id="77eee-942">新たに追加されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="77eee-942">New cmdlets are:</span></span>
    - <span data-ttu-id="77eee-943">Add-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="77eee-943">Add-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="77eee-944">Get-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="77eee-944">Get-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="77eee-945">Remove-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="77eee-945">Remove-AzIotHubMessageEnrichment</span></span>
    - <span data-ttu-id="77eee-946">Set-AzIotHubMessageEnrichment</span><span class="sxs-lookup"><span data-stu-id="77eee-946">Set-AzIotHubMessageEnrichment</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-947">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-947">Az.Monitor</span></span>
* <span data-ttu-id="77eee-948">最新の Monitor SDK (0.24.1-preview) を指しています</span><span class="sxs-lookup"><span data-stu-id="77eee-948">Pointing to the most recent Monitor SDK, i.e. 0.24.1-preview</span></span>
   - <span data-ttu-id="77eee-949">Metrics のコマンドレットに破壊的でない変更を追加します。Unit の列挙型でいくつかの新しい値がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="77eee-949">Adds non-braking changes to the Metrics cmdlets, i.e. the Unit enumeration supports several new values.</span></span> <span data-ttu-id="77eee-950">これらは読み取り専用のコマンドレットのため、コマンドレットの入力に変更はありません。</span><span class="sxs-lookup"><span data-stu-id="77eee-950">These are read-only cmdlets, so there would be no change in the input of the cmdlets.</span></span>
   - <span data-ttu-id="77eee-951">**ActionGroups** 要求の api-version が **2019-06-01** になりました。以前は **2018-03-01** でした。</span><span class="sxs-lookup"><span data-stu-id="77eee-951">The api-version of the **ActionGroups** requests is now **2019-06-01**, before it was **2018-03-01**.</span></span> <span data-ttu-id="77eee-952">この変更に対応するために、シナリオ テストが更新されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-952">The scenario tests have been updated to accommodate for this change.</span></span>
   - <span data-ttu-id="77eee-953">クラス **EmailReceiver** と **WebhookReceiver** のコンストラクターに、**useCommonAlertSchema** というブール値が新しく必須の引数として追加されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-953">The constructors for the classes **EmailReceiver** and **WebhookReceiver** added one new mandatory argument, i.e. a Boolean value called **useCommonAlertSchema**.</span></span> <span data-ttu-id="77eee-954">現時点では、この値は **false** に固定されており、この破壊的変更がコマンドレットに影響しないようになっています。</span><span class="sxs-lookup"><span data-stu-id="77eee-954">Currently, the value is fixed to **false** to hide this breaking change from the cmdlets.</span></span> <span data-ttu-id="77eee-955">**注**: これは、アラート チームによって検証する必要がある一時的な変更です。</span><span class="sxs-lookup"><span data-stu-id="77eee-955">**NOTE**: this is a temporary change that must be validated by the Alerts team.</span></span>
   - <span data-ttu-id="77eee-956">クラス **Source** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-956">The order of the arguments for the constructor of the class **Source** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="77eee-957">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="77eee-957">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
   - <span data-ttu-id="77eee-958">クラス **AlertingAction** のコンストラクターの引数の順序 (**ScheduledQueryRuleSource** クラスに関連) が、前の SDK から変更されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-958">The order of the arguments for the constructor of the class **AlertingAction** (related to the **ScheduledQueryRuleSource** class) changed from the previous SDK.</span></span> <span data-ttu-id="77eee-959">この変更により、2 つの単体テストを修正する必要が生じました。コンパイルはされますが、テストに合格しませんでした。</span><span class="sxs-lookup"><span data-stu-id="77eee-959">This change required two unit tests to the be fixed: they compiled, but failed to pass the tests.</span></span>
* <span data-ttu-id="77eee-960">メトリック アラート V2 の動的しきい値条件のサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-960">Support Dynamic Threshold criteria for metric alert V2</span></span>
    - <span data-ttu-id="77eee-961">New-AzMetricAlertRuleV2Criteria: 動的しきい値の条件も作成するようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-961">New-AzMetricAlertRuleV2Criteria: now creats dynamic threshold criteria also</span></span>
    - <span data-ttu-id="77eee-962">Add-AzMetricAlertRuleV2: 動的しきい値の条件も受け入れるようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-962">Add-AzMetricAlertRuleV2: now accept dynamic threshold criteria also</span></span>
* <span data-ttu-id="77eee-963">スケジュールされたクエリ ルール コマンドレット (SQR) の機能強化</span><span class="sxs-lookup"><span data-stu-id="77eee-963">Improvements in Scheduled Query Rule cmdlets (SQR)</span></span>
 - <span data-ttu-id="77eee-964">コマンドレットは、'Location' パラメーターを両方の形式 (場所 (例: eastus) または場所の表示名 (例: 米国東部)) で受け入れます。</span><span class="sxs-lookup"><span data-stu-id="77eee-964">Cmdlets will accept 'Location' paramater in both formats, either the location (e.g. eastus) or the location display name (e.g. East US)</span></span>
 - <span data-ttu-id="77eee-965">ヘルプ ファイルで 'Enabled' パラメーターを正しく示しました</span><span class="sxs-lookup"><span data-stu-id="77eee-965">Illustrated 'Enabled' parameter in help files properly</span></span>
 - <span data-ttu-id="77eee-966">省略可能なパラメーター 'ActionGroup' の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-966">Added examples for 'ActionGroup' optional parameter</span></span>
 - <span data-ttu-id="77eee-967">ヘルプ ファイルを全体的に改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-967">Overall improved help files</span></span>
* <span data-ttu-id="77eee-968">'Set-AzActionRule' のスコープの種類を決定する際のバグを修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-968">Fix bug in determining scope type for 'Set-AzActionRule'</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-969">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-969">Az.Network</span></span>
* <span data-ttu-id="77eee-970">'New-AzApplicationGateway' リファレンス ドキュメントの間違った例を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-970">Fix incorrect example in 'New-AzApplicationGateway' reference documentation</span></span>
* <span data-ttu-id="77eee-971">'Get-AzNetworkWatcherPacketCapture' のリファレンス ドキュメントに、パケット キャプチャのすべてのプロパティの取得に関する注を追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-971">Add note in 'Get-AzNetworkWatcherPacketCapture' reference documentation about retrieving all properties for a packet capture</span></span>
* <span data-ttu-id="77eee-972">'Test-AzNetworkWatcherIPFlow' リファレンス ドキュメントの例を修正し、NIC を正しく列挙しました</span><span class="sxs-lookup"><span data-stu-id="77eee-972">Fixed example in 'Test-AzNetworkWatcherIPFlow' reference documentation to correctly enumerate NICs</span></span>
* <span data-ttu-id="77eee-973">クラウド例外の解析を改善し、追加の詳細が存在する場合は表示するようにしました</span><span class="sxs-lookup"><span data-stu-id="77eee-973">Improved cloud exception parsing to display additional details if they are present</span></span>
* <span data-ttu-id="77eee-974">クラウド例外の解析を改善し、SDK 例外の追加の種類を処理するようにしました</span><span class="sxs-lookup"><span data-stu-id="77eee-974">Improved cloud exception parsing to handle additional type of SDK exception</span></span>
* <span data-ttu-id="77eee-975">セキュリティ規則モデルの不適切なマッピングを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-975">Fixed incorrect mapping of Security Rule models</span></span>
* <span data-ttu-id="77eee-976">プライベート IP 機能用のプロパティをネットワーク インターフェイスに追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-976">Added properties to network interface for private ip feature</span></span>
    - <span data-ttu-id="77eee-977">PSNetworkInterface に PSResourceId の型としてプロパティ 'PrivateEndpoint' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-977">Added property 'PrivateEndpoint' as type of PSResourceId to PSNetworkInterface</span></span>
    - <span data-ttu-id="77eee-978">PSNetworkInterfaceIPConfiguration に PSIpConfigurationConnectivityInformation の型としてプロパティ 'PrivateLinkConnectionProperties' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-978">Added property 'PrivateLinkConnectionProperties' as type of PSIpConfigurationConnectivityInformation to PSNetworkInterfaceIPConfiguration</span></span>
    - <span data-ttu-id="77eee-979">新しいモデル クラス PSIpConfigurationConnectivityInformation を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-979">Added new model class PSIpConfigurationConnectivityInformation</span></span>
* <span data-ttu-id="77eee-980">Azure Firewall リソースの新しい ApplicationRuleProtocolType 'mssql' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-980">Added new ApplicationRuleProtocolType 'mssql' for Azure Firewall resource</span></span>
* <span data-ttu-id="77eee-981">Virtual WAN でのマルチリンクのサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-981">MultiLink support in Virtual WAN</span></span>
    - <span data-ttu-id="77eee-982">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-982">New cmdlets</span></span>
        - <span data-ttu-id="77eee-983">New-AzVpnSiteLink</span><span class="sxs-lookup"><span data-stu-id="77eee-983">New-AzVpnSiteLink</span></span>
        - <span data-ttu-id="77eee-984">New-AzVpnSiteLinkConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-984">New-AzVpnSiteLinkConnection</span></span>
    - <span data-ttu-id="77eee-985">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-985">Updated cmdlet:</span></span>
        - <span data-ttu-id="77eee-986">New-VpnSite</span><span class="sxs-lookup"><span data-stu-id="77eee-986">New-VpnSite</span></span>
        - <span data-ttu-id="77eee-987">Update-VpnSite</span><span class="sxs-lookup"><span data-stu-id="77eee-987">Update-VpnSite</span></span>
        - <span data-ttu-id="77eee-988">New-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-988">New-VpnConnection</span></span>
        - <span data-ttu-id="77eee-989">Update-VpnConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-989">Update-VpnConnection</span></span>
* <span data-ttu-id="77eee-990">AzureRM コマンドレットの代わりに Az コマンドレットを使用するようにいくつかの PowerShell の例のドキュメントを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-990">Fixed documents for some PowerShell examples to use Az cmdlets instead of AzureRM cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-991">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-991">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-992">ProtectedItemsCount 属性を使用して AzureVMpolicy オブジェクトを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-992">Update AzureVMpolicy Object with ProtectedItemsCount Attribute</span></span>
* <span data-ttu-id="77eee-993">VM ポリシーと元のストレージ アカウントの復元のテストを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-993">Added Tests for VM policy and Original Storage Account Restore</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-994">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-994">Az.Resources</span></span>
* <span data-ttu-id="77eee-995">New-AzRoleAssignment をパラメーター Scope なしで呼び出せないバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-995">Fix bug where New-AzRoleAssignment could not be called without parameter Scope.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-996">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-996">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-997">'Update-AzServiceFabricReliability' リファレンス ドキュメントの例のスペルミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-997">Fixed typo in example for 'Update-AzServiceFabricReliability' reference documentation</span></span>
* <span data-ttu-id="77eee-998">アプリケーションとサービスを管理する以下の新しいコマンドレットを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-998">Adding new cmdlets to manage appliaction and services:</span></span>
    - <span data-ttu-id="77eee-999">New-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="77eee-999">New-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="77eee-1000">New-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="77eee-1000">New-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="77eee-1001">New-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="77eee-1001">New-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="77eee-1002">New-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="77eee-1002">New-AzServiceFabricService</span></span>
    - <span data-ttu-id="77eee-1003">Update-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="77eee-1003">Update-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="77eee-1004">Get-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="77eee-1004">Get-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="77eee-1005">Get-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="77eee-1005">Get-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="77eee-1006">Get-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="77eee-1006">Get-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="77eee-1007">Get-AzServiceFabricService</span><span class="sxs-lookup"><span data-stu-id="77eee-1007">Get-AzServiceFabricService</span></span>
    - <span data-ttu-id="77eee-1008">Remove-AzServiceFabricApplication</span><span class="sxs-lookup"><span data-stu-id="77eee-1008">Remove-AzServiceFabricApplication</span></span>
    - <span data-ttu-id="77eee-1009">Remove-AzServiceFabricApplicationType</span><span class="sxs-lookup"><span data-stu-id="77eee-1009">Remove-AzServiceFabricApplicationType</span></span>
    - <span data-ttu-id="77eee-1010">Remove-AzServiceFabricApplicationTypeVersion</span><span class="sxs-lookup"><span data-stu-id="77eee-1010">Remove-AzServiceFabricApplicationTypeVersion</span></span>
    - <span data-ttu-id="77eee-1011">Remove-AzServiceFabricServic</span><span class="sxs-lookup"><span data-stu-id="77eee-1011">Remove-AzServiceFabricServic</span></span>
* <span data-ttu-id="77eee-1012">Service Fabric SDK をバージョン 1.2.0 にアップグレードしました。これはサービス ファブリックのリソース プロバイダー api-version 2019-03-01 を使用します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1012">Upgraded Service Fabric SDK to version 1.2.0 which uses service fabric resource provider api-version 2019-03-01.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="77eee-1013">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="77eee-1013">Az.SignalR</span></span>
* <span data-ttu-id="77eee-1014">Update、Restart、CheckNameAvailability、GetUsage のコマンドレットを追加します</span><span class="sxs-lookup"><span data-stu-id="77eee-1014">Add Update, Restart, CheckNameAvailability, GetUsage Cmdlets</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1015">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1015">Az.Sql</span></span>
* <span data-ttu-id="77eee-1016">'Get-AzSqlElasticPool' のリファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-1016">Update example in reference documentation for 'Get-AzSqlElasticPool'</span></span>
* <span data-ttu-id="77eee-1017">エラスティック プールの作成 (New-AzSqlElasticPool) に仮想コアの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1017">Added vCore example to creating an elastic pool (New-AzSqlElasticPool).</span></span>
* <span data-ttu-id="77eee-1018">Set-AzSqlServerAdvancedThreatProtectionPolicy および Set-AzSqlDatabaseAdvancedThreatProtectionPolicy で EmailAddresses が空の場合、EmailAddresses の検証と EmailAdmins が false でないことの検査を削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-1018">Remove the validation of EmailAddresses and the check that EmailAdmins is not false in case EmailAddresses is empty in Set-AzSqlServerAdvancedThreatProtectionPolicy and Set-AzSqlDatabaseAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="77eee-1019">監査カテゴリを有効にする複数の診断設定が存在する場合に、サーバーとデータベースの監査設定が削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1019">Enabled removal of server/database auditing settings when multiple diagnostic settings that enable audit category exist.</span></span>
* <span data-ttu-id="77eee-1020">複数の SQL 脆弱性評価コマンドレットで、メール アドレスの検証を修正します (Update-AzSqlDatabaseVulnerabilityAssessmentSetting、Update-AzSqlServerVulnerabilityAssessmentSetting、Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting、Update-AzSqlInstanceVulnerabilityAssessmentSetting)。</span><span class="sxs-lookup"><span data-stu-id="77eee-1020">Fix email addresses validation in multiple Sql Vulnerability Assessment cmdlets (Update-AzSqlDatabaseVulnerabilityAssessmentSetting, Update-AzSqlServerVulnerabilityAssessmentSetting, Update-AzSqlInstanceDatabaseVulnerabilityAssessmentSetting and Update-AzSqlInstanceVulnerabilityAssessmentSetting).</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1021">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1021">Az.Storage</span></span>
* <span data-ttu-id="77eee-1022">'Get-AzStorageAccountKey' のリファレンス ドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1022">Updated example in reference documentation for 'Get-AzStorageAccountKey'</span></span>
* <span data-ttu-id="77eee-1023">Azure ファイルのアップロード/ダウンロードで、ソース ファイルの SMB プロパティ (ファイルの属性、ファイルの作成時刻、ファイルの最終書き込み時刻) をコピー先のファイルで維持することをサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-1023">In upload/Downalod Azure File,support perserve the source File SMB properties (File Attributtes, File Creation Time, File Last Write Time) in the destination file</span></span>
    -  <span data-ttu-id="77eee-1024">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1024">Set-AzStorageFileContent</span></span>
    -  <span data-ttu-id="77eee-1025">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1025">Get-AzStorageFileContent</span></span>
* <span data-ttu-id="77eee-1026">コンテナーが有効になっている ImmutabilityPolicy で、プロパティ/メタデータを使用するアップロード ブロック BLOB が失敗する問題を修正します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1026">Fix Upload block blob with properties/metadate fail on container enabled ImmutabilityPolicy.</span></span>
    -  <span data-ttu-id="77eee-1027">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1027">Set-AzStorageBlobContent</span></span>
* <span data-ttu-id="77eee-1028">管理プレーン API を使用した Azure ファイル共有の管理をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-1028">Support manage Azure File shares with Management plane API</span></span>
    -  <span data-ttu-id="77eee-1029">New-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="77eee-1029">New-AzRmStorageShare</span></span>
    -  <span data-ttu-id="77eee-1030">Get-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="77eee-1030">Get-AzRmStorageShare</span></span>
    -  <span data-ttu-id="77eee-1031">Update-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="77eee-1031">Update-AzRmStorageShare</span></span>
    -  <span data-ttu-id="77eee-1032">Remove-AzRmStorageShare</span><span class="sxs-lookup"><span data-stu-id="77eee-1032">Remove-AzRmStorageShare</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1033">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1033">Az.Websites</span></span>
* <span data-ttu-id="77eee-1034">アプリを新しい ASP に移行するときに webapp タグが削除される問題を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-1034">Fixing issue where webapp Tags were getting deleted when migrating App to new ASPwhere webapp Tags were getting deleted when migrating App to new ASP</span></span>
* <span data-ttu-id="77eee-1035">Linux と Windows にまたがって動作するように Publish-AzureWebapp を修正します</span><span class="sxs-lookup"><span data-stu-id="77eee-1035">Fixing the Publish-AzureWebapp to work across Linux and windows</span></span>
* <span data-ttu-id="77eee-1036">'Get-AzWebAppPublishingProfile' リファレンス ドキュメントの例を更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-1036">Update example in 'Get-AzWebAppPublishingProfile' reference documentation</span></span>

## <a name="260---august-2019"></a><span data-ttu-id="77eee-1037">2.6.0 - 2019 年 8 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1037">2.6.0 - August 2019</span></span>
#### <a name="general"></a><span data-ttu-id="77eee-1038">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-1038">General</span></span>
* <span data-ttu-id="77eee-1039">多数のモジュールでさまざまな入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1039">Fixed miscellaneous typos across numerous modules</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-1040">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1040">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1041">Azure 関数の認証でユーザー割り当て MSI をサポート (#9479)</span><span class="sxs-lookup"><span data-stu-id="77eee-1041">Support user-assigned MSI in Azure Functiosn Authentication (#9479)</span></span>

#### <a name="azaks"></a><span data-ttu-id="77eee-1042">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="77eee-1042">Az.Aks</span></span>
* <span data-ttu-id="77eee-1043">"Get-AzAks" の出力に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1043">Fix issue with output for 'Get-AzAks'</span></span>
    * <span data-ttu-id="77eee-1044">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9847</span><span class="sxs-lookup"><span data-stu-id="77eee-1044">More information here: https://github.com/Azure/azure-powershell/issues/9847</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="77eee-1045">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-1045">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-1046">次の問題を修正: https://github.com/Azure/azure-powershell/issues/9351</span><span class="sxs-lookup"><span data-stu-id="77eee-1046">Fix for issue https://github.com/Azure/azure-powershell/issues/9351</span></span>
    - <span data-ttu-id="77eee-1047">.NET NuGet バージョンを更新しました。これにより、productId、apiId、groupId、userId に対する制限は適用されません。</span><span class="sxs-lookup"><span data-stu-id="77eee-1047">Update .net nuget version, which does not enforce restrictions on productId, apiId, groupId and userId</span></span>
* <span data-ttu-id="77eee-1048">**Get-AzApiManagementProduct** - API を使用した製品の照会のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1048">**Get-AzApiManagementProduct** - Added support for querying products using Api.</span></span>
  https://github.com/Azure/azure-powershell/issues/9482
* <span data-ttu-id="77eee-1049">**New-AzApiManagementApiRevision** - 新しい API リビジョンの作成時に ApiRevisionDescription が設定されていない問題を修正しました。 https://github.com/Azure/azure-powershell/issues/9752</span><span class="sxs-lookup"><span data-stu-id="77eee-1049">**New-AzApiManagementApiRevision** - Fix for issue where ApiRevisionDescription was not being set when creating new api revision https://github.com/Azure/azure-powershell/issues/9752</span></span>
* <span data-ttu-id="77eee-1050">モデル "PsApiManagementOAuth2AuthrozationServer" のスペルミスを "PsApiManagementOAuth2AuthorizationServer" に修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1050">Fixed typo in model 'PsApiManagementOAuth2AuthrozationServer' to 'PsApiManagementOAuth2AuthorizationServer'</span></span>

#### <a name="azbatch"></a><span data-ttu-id="77eee-1051">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="77eee-1051">Az.Batch</span></span>
* <span data-ttu-id="77eee-1052">ヘルプ メッセージとドキュメントの入力ミスを修正して Windows の先頭文字を大文字にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1052">Fixed typo in help message and documentation to capitalize Windows</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-1053">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-1053">Az.Cdn</span></span>
* <span data-ttu-id="77eee-1054">CDN モジュール変換ヘルパーの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1054">Fixed a typo in CDN module conversion helper</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1055">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1055">Az.Compute</span></span>
* <span data-ttu-id="77eee-1056">New-AzVMConfig コマンドレットに VmssId を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1056">Add VmssId to New-AzVMConfig cmdlet</span></span>
* <span data-ttu-id="77eee-1057">New-AzVmssConfig と Update-AzVmss に TerminateScheduledEvents および TerminateScheduledEventNotBeforeTimeoutInMinutes パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1057">Add TerminateScheduledEvents and TerminateScheduledEventNotBeforeTimeoutInMinutes parameters to New-AzVmssConfig and Update-AzVmss</span></span>
* <span data-ttu-id="77eee-1058">VM イメージ オブジェクトに HyperVGeneration プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1058">Add HyperVGeneration property to VM image object</span></span>
* <span data-ttu-id="77eee-1059">Host と HostGroup の機能を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1059">Add Host and HostGroup features</span></span>
    - <span data-ttu-id="77eee-1060">新しいコマンドレット: New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span><span class="sxs-lookup"><span data-stu-id="77eee-1060">New cmdlets:   New-AzHostGroup   New-AzHost   Get-AzHostGroup   Get-AzHost   Remove-AzHostGroup   Remove-AzHost</span></span>
    - <span data-ttu-id="77eee-1061">HostId パラメーターが New-AzVMConfig と New-AzVM に追加されました</span><span class="sxs-lookup"><span data-stu-id="77eee-1061">HostId parameter is added to New-AzVMConfig and New-AzVM</span></span>
* <span data-ttu-id="77eee-1062">"Invoke-AzVMRunCommand" のドキュメントの例を、適切なパラメーター名を使用するよう更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1062">Update example in 'Invoke-AzVMRunCommand' documentation to use correct parameter name</span></span>
* <span data-ttu-id="77eee-1063">"Set-AzVMDiskEncryptionExtension" と "Set-AzVmssDiskEncryptionExtension" の参照ドキュメントの "-VolumeType" の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1063">Update '-VolumeType' description in 'Set-AzVMDiskEncryptionExtension' and 'Set-AzVmssDiskEncryptionExtension' reference documentation</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1064">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1064">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1065">"New-AzDataFactoryEncryptValue" のドキュメントで "Windows" の先頭文字が大文字になるように入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1065">Fix typo to capitalize 'Windows' in 'New-AzDataFactoryEncryptValue' documentation</span></span>
* <span data-ttu-id="77eee-1066">ADF .Net SDK のバージョンを 4.1.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1066">Updated ADF .Net SDK version to 4.1.2</span></span>
* <span data-ttu-id="77eee-1067">"Set-AzureRmDataFactoryV2IntegrationRuntime" コマンドのパラメーター "DataProxyIntegrationRuntimeName"、"DataProxyStagingLinkedServiceName"、"DataProxyStagingPath" を追加して、SSIS Integration Runtime のプロキシとしてセルフホステッド統合ランタイムを設定できるようにしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1067">Add parameter 'DataProxyIntegrationRuntimeName', 'DataProxyStagingLinkedServiceName' and 'DataProxyStagingPath' for 'Set-AzureRmDataFactoryV2IntegrationRuntime' cmd to enable set up Self-Hosted Integration Runtime as a proxy for SSIS Integration Runtime</span></span>
* <span data-ttu-id="77eee-1068">トリガーされたパイプライン、メッセージ、プロパティを表示するよう PSTriggerRun を更新し、アクティビティの種類を表示するよう PSActivityRun を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1068">Updated PSTriggerRun to show the triggered pipelines, message and properties, and PSActivityRun to show the activity type</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-1069">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-1069">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-1070">任意のエラーやリモート例外での Get-DataLakeStoreDeletedItem のハングを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1070">Fix hanging of Get-DataLakeStoreDeletedItem for any errors or remote exceptions.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-1071">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1071">Az.EventHub</span></span>
* <span data-ttu-id="77eee-1072">問題 #9658 を修正しました: Set-AzEventHubNetworkRuleSet の VirtualNteworkRule パラメーターのスペルミス</span><span class="sxs-lookup"><span data-stu-id="77eee-1072">Fix for issue #9658 : Typo VirtualNteworkRule parameter in Set-AzEventHubNetworkRuleSet</span></span>
* <span data-ttu-id="77eee-1073">問題 #9558 を修正しました: Set-AzEventHubNamespace では PUT ではなく PATCH が使用されています</span><span class="sxs-lookup"><span data-stu-id="77eee-1073">Fix for issue #9558 : Set-AzEventHubNamespace is using PATCH instead of PUT</span></span>
* <span data-ttu-id="77eee-1074">Set-AzEventHubNamespace コマンドレットに EnableKafka パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1074">added EnableKafka parameter to Set-AzEventHubNamespace cmdlet</span></span>
* <span data-ttu-id="77eee-1075">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="77eee-1075">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>

#### <a name="azmarketplaceordering"></a><span data-ttu-id="77eee-1076">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="77eee-1076">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="77eee-1077">"Azure" がすべて小文字であるドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1077">Fixed documentation typo where 'Azure' was all lowercase letters</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-1078">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-1078">Az.Monitor</span></span>
* <span data-ttu-id="77eee-1079">ヘルプ ドキュメントで正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1079">Fixed incorrect parameter name in help documentation</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1080">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1080">Az.Network</span></span>
* <span data-ttu-id="77eee-1081">New-AzPrivateLinkServiceIpConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1081">Updated New-AzPrivateLinkServiceIpConfig</span></span>
    - <span data-ttu-id="77eee-1082">"PublicIpAddress" パラメーターはサーバー側で使用されないため、非推奨にしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1082">Deprecated the paramster 'PublicIpAddress' since this is never used in the server side.</span></span>
    - <span data-ttu-id="77eee-1083">現在の IP 構成がプライパリかどうかを示す省略可能なパラメーター "Primary" を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1083">Added one optional parameter 'Primary' that indicate the current ip configuration is primary one or not.</span></span>
* <span data-ttu-id="77eee-1084">SDK からの要求エラーの例外の処理を改良しました - 以前の SDK の例外が正しく処理されず、主なエラーの詳細が表示されないという問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1084">Improved handling of request error exception from SDK   -Fixes the issue that previously SDK exceptions aren't handled correctly which results in key error details not being displayed</span></span>
* <span data-ttu-id="77eee-1085">適切な IPv6 のプレフィックス長に合わせて IPv6 の IP プレフィックスの検証ロジックを調整しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1085">Adjusted validation logic for Ipv6 IP Prefix to check for correct IPv6 prefix length.</span></span>
* <span data-ttu-id="77eee-1086">Get-AzVirtualNetworkSubnetConfig を更新しました: サブネット リソース ID によって取得するように設定されたパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1086">Updated Get-AzVirtualNetworkSubnetConfig: Added parameter set to get by subnet resource id.</span></span>
* <span data-ttu-id="77eee-1087">AzNetworkServiceTag の Location パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1087">Updated description of Location parameter for AzNetworkServiceTag</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-1088">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1088">Az.OperationalInsights</span></span>
* <span data-ttu-id="77eee-1089">"New-AzOperationalInsightsLinuxSyslogDataSource" に関するドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1089">Updated documentation for 'New-AzOperationalInsightsLinuxSyslogDataSource'</span></span>
    - <span data-ttu-id="77eee-1090">例を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1090">Added example</span></span>
    - <span data-ttu-id="77eee-1091">"-Name" パラメーターの説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1091">Updated description for '-Name' parameter</span></span>
* <span data-ttu-id="77eee-1092">New-AzOperationalInsightsWindowsEventDataSource に関する例を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1092">Added an example for New-AzOperationalInsightsWindowsEventDataSource</span></span>
* <span data-ttu-id="77eee-1093">New-AzOperationalInsightsWindowsEventDataSource の -Name パラメーターの説明を変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1093">Changed the description of the -Name parameter for New-AzOperationalInsightsWindowsEventDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1094">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1094">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1095">"Get-AzRecoveryServicesBackupJobDetail.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1095">Update 'Get-AzRecoveryServicesBackupJobDetail.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1096">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1096">Az.Resources</span></span>
* <span data-ttu-id="77eee-1097">Microsoft.Resource の新しい API バージョン 2019-05-10 のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1097">Add support for new api version 2019-05-10 for Microsoft.Resource</span></span>
    - <span data-ttu-id="77eee-1098">変数、リソース、プロパティに対して "copy.count = 0" のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1098">Add support for 'copy.count = 0' for variables, resources and properties</span></span>
    - <span data-ttu-id="77eee-1099">"condition = false" または "copy.count = 0" が設定されたリソースは完全モードで削除されます</span><span class="sxs-lookup"><span data-stu-id="77eee-1099">Resources with 'condition = false' or 'copy.count = 0' will be deleted in complete mode</span></span>
* <span data-ttu-id="77eee-1100">サブスクリプション レベルでのポリシーの割り当ての例をヘルプ ドキュメントに追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1100">Add an example of assigning policy at subscription level to help doc</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="77eee-1101">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="77eee-1101">Az.ServiceBus</span></span>
* <span data-ttu-id="77eee-1102">問題 #9658 を修正しました: Set-AzServiceBusNetworkRuleSet の VirtualNetworkRule パラメーターのタイプミス</span><span class="sxs-lookup"><span data-stu-id="77eee-1102">Fix for issue #9658 : Typo VirtualNetworkRule parameter in Set-AzServiceBusNetworkRuleSet</span></span>
* <span data-ttu-id="77eee-1103">問題 #9786 を修正しました: リッスンのみの権限を持つルールを作成できません</span><span class="sxs-lookup"><span data-stu-id="77eee-1103">Fix for issue #9786 : cannot create a rule with Listen only rights</span></span>
* <span data-ttu-id="77eee-1104">キューとトピックに名前を使用できるかどうかを確認するために新しいコマンド "Test-AzServiceBusNameAvailability" を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1104">Added new command 'Test-AzServiceBusNameAvailability' to check the name availability for queue and topic</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-1105">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-1105">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-1106">ノード タイプの追加のコマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1106">Fix add node type cmdlet bugs:</span></span>
    - <span data-ttu-id="77eee-1107">リソース グループの他の VMSS がサービス ファブリック クラスターに関連していない場合の NullReferenceException のバグ。</span><span class="sxs-lookup"><span data-stu-id="77eee-1107">NullReferenceException bug when resource group had other vmss not related to the service fabric cluster.</span></span> <span data-ttu-id="77eee-1108">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8681</span><span class="sxs-lookup"><span data-stu-id="77eee-1108">Fixes issue: https://github.com/Azure/azure-powershell/issues/8681</span></span>
    - <span data-ttu-id="77eee-1109">virtualNetwork がクラスターとは別のリソース グループに存在する場合にコマンドレットが失敗するというバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1109">Fix bug where cmdlet failed if virtualNetwork was in a different resource group that the cluster.</span></span> <span data-ttu-id="77eee-1110">問題を修正しました: https://github.com/Azure/azure-powershell/issues/8407</span><span class="sxs-lookup"><span data-stu-id="77eee-1110">fixes issue: https://github.com/Azure/azure-powershell/issues/8407</span></span>
    - <span data-ttu-id="77eee-1111">Add-AzServiceFabricApplicationCertificate コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1111">Deprecating Add-AzServiceFabricApplicationCertificate cmdlet</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1112">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1112">Az.Sql</span></span>
* <span data-ttu-id="77eee-1113">古い監査コマンドレットのドキュメントを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1113">Update documentation of old Auditing cmdlets.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1114">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1114">Az.Storage</span></span>
* <span data-ttu-id="77eee-1115">コマンドレットの例にシナリオをさらに追加し、パラメーターの説明を更新することで、Get/Close-AzStorageFileHandle のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1115">Update help for Get/Close-AzStorageFileHandle, by add more scenarios to cmdlet examples and update parameter descriptions</span></span>
* <span data-ttu-id="77eee-1116">BLOB のアップロードと BLOB のコピーで StandardBlobTier をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-1116">Support StandardBlobTier in upload blob and copy blob</span></span>
    -  <span data-ttu-id="77eee-1117">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1117">Set-AzStorageBlobContent</span></span>
    -  <span data-ttu-id="77eee-1118">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="77eee-1118">Start-AzStorageBlobCopy</span></span>
* <span data-ttu-id="77eee-1119">BLOB のコピーでリハイドレート優先度をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-1119">Support Rehydrate Priority in copy blob</span></span>
    -  <span data-ttu-id="77eee-1120">Start-AzStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="77eee-1120">Start-AzStorageBlobCopy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1121">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1121">Az.Websites</span></span>
* <span data-ttu-id="77eee-1122">Set-AzWebApp と Set-AzWebAppSlot の -AppSettings パラメーターの説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1122">Add clarification around -AppSettings parameter in Set-AzWebApp and Set-AzWebAppSlot</span></span>

## <a name="250---july-2019"></a><span data-ttu-id="77eee-1123">2.5.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1123">2.5.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1124">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1124">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1125">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1125">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azapplicationinsights"></a><span data-ttu-id="77eee-1126">Az.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1126">Az.ApplicationInsights</span></span>
* <span data-ttu-id="77eee-1127">「Remove-AzApplicationInsightsApiKey」ドキュメントの例の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1127">Fix example typo in 'Remove-AzApplicationInsightsApiKey' documentation</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1128">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1128">Az.Automation</span></span>
* <span data-ttu-id="77eee-1129">リソース文字列の入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1129">Fix typo in resource string</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-1130">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1130">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-1131">NetworkRuleSet のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1131">Added NetworkRuleSet support.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1132">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1132">Az.Compute</span></span>
* <span data-ttu-id="77eee-1133">VM インスタンス ビュー オブジェクトの不足していたプロパティ (ComputerName、OsName、OsVersion、HyperVGeneration) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1133">Add missing properties (ComputerName, OsName, OsVersion and HyperVGeneration) of VM instance view object.</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="77eee-1134">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="77eee-1134">Az.ContainerRegistry</span></span>
* <span data-ttu-id="77eee-1135">Remove-AzContainerRegistryReplication の Replication パラメーターの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1135">Fix typo in Remove-AzContainerRegistryReplication for Replication parameter</span></span>
    - <span data-ttu-id="77eee-1136">詳細については、こちらを参照してください: https://github.com/Azure/azure-powershell/issues/9633</span><span class="sxs-lookup"><span data-stu-id="77eee-1136">More information here https://github.com/Azure/azure-powershell/issues/9633</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1137">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1137">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1138">ADF .Net SDK のバージョンを 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1138">Updated ADF .Net SDK version to 4.1.0</span></span>
* <span data-ttu-id="77eee-1139">「Get-AzDataFactoryV2PipelineRun」ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1139">Fix typo in documentation for 'Get-AzDataFactoryV2PipelineRun'</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-1140">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1140">Az.EventHub</span></span>
* <span data-ttu-id="77eee-1141">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzEventHubAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="77eee-1141">Added new cmmdlet added for generating SAS token : New-AzEventHubAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="77eee-1142">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1142">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-1143">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-1143">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-1144">証明書ポリシーの KeySize を指定するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1144">Added support to specify the KeySize for Certificate Policies</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="77eee-1145">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="77eee-1145">Az.LogicApp</span></span>
* <span data-ttu-id="77eee-1146">Get-AzIntegrationAccountMap ですべてのマップの種類を一覧表示するように修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1146">Fix for Get-AzIntegrationAccountMap to list all map types</span></span>
    - <span data-ttu-id="77eee-1147">フィルター処理用に新しい MapType パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1147">Added new MapType parameter for filtering</span></span>

#### <a name="azmanagedservices"></a><span data-ttu-id="77eee-1148">Az.ManagedServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1148">Az.ManagedServices</span></span>
* <span data-ttu-id="77eee-1149">API バージョン 2019-06-01 (GA) のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1149">Added support for api version 2019-06-01 (GA)</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1150">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1150">Az.Network</span></span>
* <span data-ttu-id="77eee-1151">プライベート エンドポイントとプライベート リンク サービスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1151">Add support for private endpoint and private link service</span></span>
    - <span data-ttu-id="77eee-1152">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1152">New cmdlets</span></span>
        - <span data-ttu-id="77eee-1153">Set-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="77eee-1153">Set-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="77eee-1154">Set-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="77eee-1154">Set-AzPrivateLinkService</span></span>
        - <span data-ttu-id="77eee-1155">Approve-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-1155">Approve-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-1156">Deny-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-1156">Deny-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-1157">Get-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-1157">Get-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-1158">Remove-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-1158">Remove-AzPrivateEndpointConnection</span></span>
        - <span data-ttu-id="77eee-1159">Test-AzPrivateLinkServiceVisibility</span><span class="sxs-lookup"><span data-stu-id="77eee-1159">Test-AzPrivateLinkServiceVisibility</span></span>
        - <span data-ttu-id="77eee-1160">Get-AzAutoApprovedPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="77eee-1160">Get-AzAutoApprovedPrivateLinkService</span></span>
* <span data-ttu-id="77eee-1161">次の機能のために以下のコマンドを更新しました。Virtualnetwork 内のサブネット上の PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies フラグ</span><span class="sxs-lookup"><span data-stu-id="77eee-1161">Updated below commands for feature: PrivateEndpointNetworkPolicies/PrivateLinkServiceNetworkPolicies flag on Subnet in Virtualnetwork</span></span>
    - <span data-ttu-id="77eee-1162">New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1162">Updated New-AzVirtualNetworkSubnetConfig/Set-AzVirtualNetworkSubnetConfig/Add-AzVirtualNetworkSubnetConfig</span></span>
        - <span data-ttu-id="77eee-1163">このサブネット内のプライベート エンドポイントでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateEndpointNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1163">Added optional parameter -PrivateEndpointNetworkPoliciesFlag that configures whether to apply network policies on private endpoint in this subnet.</span></span>
        - <span data-ttu-id="77eee-1164">このサブネット内のプライベート リンク サービスでネットワーク ポリシーを適用するかどうかを構成する、省略可能なパラメーター -PrivateLinkServiceNetworkPoliciesFlag を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1164">Added optional parameter -PrivateLinkServiceNetworkPoliciesFlag that configures whether to apply network policies network policies on private link service in this subnet.</span></span>
* <span data-ttu-id="77eee-1165">AzPrivateLinkService のコマンドレット パラメーター "ServiceName" の名前が、下位互換性のために別名 "ServiceName" 付きで "Name" に変更されました</span><span class="sxs-lookup"><span data-stu-id="77eee-1165">AzPrivateLinkService's cmdlet parameter 'ServiceName' was renamed to 'Name' with an alias 'ServiceName' for backward compatibility</span></span>
* <span data-ttu-id="77eee-1166">ネットワークのセキュリティ規則の構成に対して ICMP プロトコルを有効にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1166">Enable ICMP protocol for network security rule configurations</span></span>
    - <span data-ttu-id="77eee-1167">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1167">Updated cmdlets</span></span>
        - <span data-ttu-id="77eee-1168">Add-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1168">Add-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="77eee-1169">New-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1169">New-AzNetworkSecurityRuleConfig</span></span>
        - <span data-ttu-id="77eee-1170">Set-AzNetworkSecurityRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1170">Set-AzNetworkSecurityRuleConfig</span></span>
* <span data-ttu-id="77eee-1171">ConnectionProtocolType (Ikev1/Ikev2) を New-AzVirtualNetworkGatewayConnection の構成可能なパラメーターとして追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1171">Add ConnectionProtocolType (Ikev1/Ikev2) as a configurable parameter for New-AzVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="77eee-1172">LoadBalancerFrontendIpConfiguration に PrivateIpAddressVersion を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1172">Add PrivateIpAddressVersion in LoadBalancerFrontendIpConfiguration</span></span>
    - <span data-ttu-id="77eee-1173">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-1173">Updated cmdlet:</span></span>
        - <span data-ttu-id="77eee-1174">New-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1174">New-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="77eee-1175">Add-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1175">Add-AzLoadBalancerFrontendIpConfig</span></span>
        - <span data-ttu-id="77eee-1176">Set-AzLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1176">Set-AzLoadBalancerFrontendIpConfig</span></span>
* <span data-ttu-id="77eee-1177">プローブ内のカスタム ポートをサポートするための Application Gateway の New-AzApplicationGatewayProbeConfig コマンドの更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1177">Application Gateway New-AzApplicationGatewayProbeConfig command update for supporting custom port in Probe</span></span>
    - <span data-ttu-id="77eee-1178">New-AzApplicationGatewayProbeConfig を更新しました。バックエンドサーバーのプローブに使用される省略可能なパラメーター Port を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1178">Updated New-AzApplicationGatewayProbeConfig: Added optional parameter Port which is used for probing backend server.</span></span> <span data-ttu-id="77eee-1179">このパラメーターは、Standard_V2 および WAF_V2 SKU に適用されます。</span><span class="sxs-lookup"><span data-stu-id="77eee-1179">This parameter is applicable for Standard_V2 and WAF_V2 SKU.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-1180">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1180">Az.OperationalInsights</span></span>
* <span data-ttu-id="77eee-1181">保存された検索条件の既定のバージョンを 1 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1181">Updated default version for saved searches to be 1.</span></span>
* <span data-ttu-id="77eee-1182">カスタム ログの null 正規表現の扱いを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1182">Fixed custom log null regex handling</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1183">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1183">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1184">"Get-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1184">Update 'Get-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="77eee-1185">"Get-AzRecoveryServicesBackupContainer.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1185">Update 'Get-AzRecoveryServicesBackupContainer.md'</span></span>
* <span data-ttu-id="77eee-1186">"Get-AzRecoveryServicesVault.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1186">Update 'Get-AzRecoveryServicesVault.md'</span></span>
* <span data-ttu-id="77eee-1187">"Wait-AzRecoveryServicesBackupJob.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1187">Update 'Wait-AzRecoveryServicesBackupJob.md'</span></span>
* <span data-ttu-id="77eee-1188">"Set-AzRecoveryServicesVaultContext.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1188">Update 'Set-AzRecoveryServicesVaultContext.md'</span></span>
* <span data-ttu-id="77eee-1189">"Get-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1189">Update 'Get-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="77eee-1190">"Get-AzRecoveryServicesBackupRecoveryPoint.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1190">Update 'Get-AzRecoveryServicesBackupRecoveryPoint.md'</span></span>
* <span data-ttu-id="77eee-1191">"Restore-AzRecoveryServicesBackupItem.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1191">Update 'Restore-AzRecoveryServicesBackupItem.md'</span></span>
* <span data-ttu-id="77eee-1192">Azure ファイル共有のコンテナーの登録を解除するためのサービスの呼び出しを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1192">Updated service call for Unregistering container for Azure File Share</span></span>
* <span data-ttu-id="77eee-1193">"Set-AzRecoveryServicesAsrAlertSetting.md" を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1193">Update 'Set-AzRecoveryServicesAsrAlertSetting.md'</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1194">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1194">Az.Resources</span></span>
- <span data-ttu-id="77eee-1195">「New-AzResourceGroupDeployment」ドキュメントで参照されていた存在しないコマンドレットを削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1195">Remove missing cmdlet referenced in 'New-AzResourceGroupDeployment' documentation</span></span>
- <span data-ttu-id="77eee-1196">新しい API バージョン 2019-01-01 を使用するようにポリシー コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1196">Updated policy cmdlets to use new api version 2019-01-01</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="77eee-1197">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="77eee-1197">Az.ServiceBus</span></span>
* <span data-ttu-id="77eee-1198">SAS トークンを生成するために次の新しいコマンドレットを追加しました。New-AzServiceBusAuthorizationRuleSASToken</span><span class="sxs-lookup"><span data-stu-id="77eee-1198">Added new cmmdlet added for generating SAS token : New-AzServiceBusAuthorizationRuleSASToken</span></span>
* <span data-ttu-id="77eee-1199">authorizationrule 権限について、"Manage" のみが割り当てられているかどうかの検証とエラー メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1199">added verification and error message for authorizationrules rights if only 'Manage' is assigned</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1200">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1200">Az.Sql</span></span>
* <span data-ttu-id="77eee-1201">Set-AzSqlDatabaseSecondary コマンドレットの例の不足を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1201">Fix missing examples for Set-AzSqlDatabaseSecondary cmdlet</span></span>
* <span data-ttu-id="77eee-1202">メール アドレスの指定なしでの脆弱性評価の反復スキャンの設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1202">Fix set Vulnerability Assessment recurring scans without providing any email addresses</span></span>
* <span data-ttu-id="77eee-1203">警告メッセージの軽微な入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1203">Fix a small typo in a warining message.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1204">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1204">Az.Storage</span></span>
* <span data-ttu-id="77eee-1205">正しいパラメーター名が使用されるようにリファレンス ドキュメント「Get-AzStorageAccount」内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1205">Update example in reference documentation for 'Get-AzStorageAccount' to use correct parameter name</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="77eee-1206">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="77eee-1206">Az.StorageSync</span></span>
* <span data-ttu-id="77eee-1207">Invoke-AzStorageSyncChangeDetection コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1207">Adding Invoke-AzStorageSyncChangeDetection cmdlet.</span></span>
* <span data-ttu-id="77eee-1208">TierFilesOlderThanDays に従うように問題 9551 を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1208">Fix Issue 9551 for honoring TierFilesOlderThanDays</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1209">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1209">Az.Websites</span></span>
* <span data-ttu-id="77eee-1210">Get-AzWebApp および Set-AzWebApp によって一部の SiteConfig プロパティが返されなかったバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1210">Fixing a bug where some SiteConfig properties were not returned by Get-AzWebApp and Set-AzWebApp</span></span>
* <span data-ttu-id="77eee-1211">Get-AzDeletedWebApp と Restore-AzDeletedWebApp に新しい Location パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1211">Adds a new Location parameter to Get-AzDeletedWebApp and Restore-AzDeletedWebApp</span></span>
* <span data-ttu-id="77eee-1212">New-AzWebApp -IncludeSourceWebAppSlots を使用した Web アプリ スロットの複製におけるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1212">Fixes a bug with cloning web app slots using New-AzWebApp -IncludeSourceWebAppSlots</span></span>

## <a name="240---july-2019"></a><span data-ttu-id="77eee-1213">2.4.0 - 2019 年 7 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1213">2.4.0 - July 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1214">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1214">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1215">プロファイル コマンドレットのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1215">Add support for profile cmdlets</span></span>
* <span data-ttu-id="77eee-1216">生成されたコマンドレットにおける環境とデータ プレーンのサポートの追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1216">Add support for environments and data planes in generated cmdlets</span></span>
* <span data-ttu-id="77eee-1217">Windows PowerShell でのデータ プレーン コマンドレットの一部のケースで不適切なエンドポイントが使用されていたバグの修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1217">Fix bug where incorrect endpoint was being used in some cases for data plane cmdlets in Windows PowerShell</span></span>

#### <a name="azadvisor"></a><span data-ttu-id="77eee-1218">Az.Advisor</span><span class="sxs-lookup"><span data-stu-id="77eee-1218">Az.Advisor</span></span>
* <span data-ttu-id="77eee-1219">Az.Advisor の GA リリース</span><span class="sxs-lookup"><span data-stu-id="77eee-1219">GA release of Az.Advisor</span></span>
* <span data-ttu-id="77eee-1220">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1220">This module is now included as a part of the roll-up `Az` module</span></span>

#### <a name="azapimanagement"></a><span data-ttu-id="77eee-1221">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-1221">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-1222">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8671</span><span class="sxs-lookup"><span data-stu-id="77eee-1222">Fix for issue https://github.com/Azure/azure-powershell/issues/8671</span></span>
    - <span data-ttu-id="77eee-1223">**Get-AzApiManagementSubscription**</span><span class="sxs-lookup"><span data-stu-id="77eee-1223">**Get-AzApiManagementSubscription**</span></span>
        - <span data-ttu-id="77eee-1224">ユーザーおよび製品別のサブスクリプションへのクエリの実行のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1224">Added support for querying subscriptions by User and Product</span></span>
        - <span data-ttu-id="77eee-1225">スコープ '/', '/apis', '/apis/echo-api' を使用したクエリのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1225">Added support for querying using Scope '/', '/apis', '/apis/echo-api'</span></span>
* <span data-ttu-id="77eee-1226">[https://github.com/Azure/azure-powershell/issues/9307](https://github.com/Azure/azure-powershell/issues/9307 ) と https://github.com/Azure/azure-powershell/issues/8432 の問題を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1226">Fix for issue https://github.com/Azure/azure-powershell/issues/9307 and https://github.com/Azure/azure-powershell/issues/8432</span></span>
    - <span data-ttu-id="77eee-1227">**Import-AzApiManagementApi**</span><span class="sxs-lookup"><span data-stu-id="77eee-1227">**Import-AzApiManagementApi**</span></span>
        - <span data-ttu-id="77eee-1228">Api をインポートするときに 'ApiVersion' と 'ApiVersionSetId' を指定するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1228">Added support for specifying 'ApiVersion' and 'ApiVersionSetId' when importing Apis</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1229">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1229">Az.Automation</span></span>
* <span data-ttu-id="77eee-1230">文字列値を処理するように Set-AzAutomationConnectionFieldValue コマンドレットのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1230">Fixed Set-AzAutomationConnectionFieldValue cmdlet bug to handle string value.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1231">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1231">Az.Compute</span></span>
* <span data-ttu-id="77eee-1232">New-AzImageConfig への HyperVGeneration パラメーターの追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1232">Add HyperVGeneration parameter to New-AzImageConfig</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1233">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1233">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1234">アクティビティ実行の取得、パイプライン実行の取得、トリガー実行取得の ADF コマンドレットの出力を Select-Object パイプをサポートするように更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1234">Updating the output of get activity runs, get pipeline runs, and get trigger runs ADF cmdlets to support Select-Object pipe.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="77eee-1235">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="77eee-1235">Az.EventGrid</span></span>
* <span data-ttu-id="77eee-1236">'New-AzEventGridSubscription' ドキュメントのタイポを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1236">Fix typo in 'New-AzEventGridSubscription' documentation</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-1237">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1237">Az.IotHub</span></span>
* <span data-ttu-id="77eee-1238">承認ポリシー キーの再生成のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1238">Add support to regenerate authorization policy keys.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1239">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1239">Az.Network</span></span>
* <span data-ttu-id="77eee-1240">パブリック ip タグに 'RoutingPreference' を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1240">Added 'RoutingPreference' to public ip tags</span></span>
* <span data-ttu-id="77eee-1241">'Get-AzNetworkServiceTag' リファレンス ドキュメントの例を改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1241">Improve examples for 'Get-AzNetworkServiceTag' reference documentation</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-1242">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1242">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-1243">Get-AzPolicyState の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1243">Fix null reference issue in Get-AzPolicyState</span></span>
    - <span data-ttu-id="77eee-1244">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/9446</span><span class="sxs-lookup"><span data-stu-id="77eee-1244">More information here: https://github.com/Azure/azure-powershell/issues/9446</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-1245">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1245">Az.OperationalInsights</span></span>
* <span data-ttu-id="77eee-1246">Get AzOperationalInsightsDataSource で返される CustomLog データソース モデルを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1246">Fixed CustomLog datasource model returned in Get-AzOperationalInsightsDataSource</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1247">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1247">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1248">IaaSVMs の get-policy コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1248">Fix for get-policy command for IaaSVMs</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1249">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1249">Az.Resources</span></span>
    - <span data-ttu-id="77eee-1250">Get-AzPolicyState -Top パラメーターのヘルプ テキストを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1250">Fix help text for Get-AzPolicyState -Top parameter</span></span>
    - <span data-ttu-id="77eee-1251">Get-AzPolicyAlias のクライアント側ページングのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1251">Add client-side paging support for Get-AzPolicyAlias</span></span>
    - <span data-ttu-id="77eee-1252">Set-AzPolicyAssignment、-PolicyParameters、および -PolicyParametersObject の新しいパラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1252">Add new parameters for Set-AzPolicyAssignment, -PolicyParameters and -PolicyParametersObject</span></span>
    - <span data-ttu-id="77eee-1253">ポリシー コマンドレットの少数のドキュメントと例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1253">Handful of doc and example updates for Policy cmdlets</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="77eee-1254">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="77eee-1254">Az.ServiceBus</span></span>
* <span data-ttu-id="77eee-1255">問題 #4938 を修正しました - New-AzureRmServiceBusQueue により MaxSizeInMegabytes 設定時に BadRequest が返される問題</span><span class="sxs-lookup"><span data-stu-id="77eee-1255">Fix for issue #4938 - New-AzureRmServiceBusQueue returns BadRequest when setting MaxSizeInMegabytes</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1256">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1256">Az.Sql</span></span>
* <span data-ttu-id="77eee-1257">プレビュー リリースから公開リリースへのインスタンス フェールオーバー グループ コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1257">Add Instance Failover Group cmdlets from preview release to public release</span></span>
* <span data-ttu-id="77eee-1258">新しいコマンドレットによる Azure SQL Server\Database 監査をサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-1258">Support Azure SQL Server\Database Auditing with new cmdlets.</span></span>
    - <span data-ttu-id="77eee-1259">Set-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="77eee-1259">Set-AzSqlServerAudit</span></span>
    - <span data-ttu-id="77eee-1260">Get-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="77eee-1260">Get-AzSqlServerAudit</span></span>
    - <span data-ttu-id="77eee-1261">Remove-AzSqlServerAudit</span><span class="sxs-lookup"><span data-stu-id="77eee-1261">Remove-AzSqlServerAudit</span></span>
    - <span data-ttu-id="77eee-1262">Set-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="77eee-1262">Set-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="77eee-1263">Get-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="77eee-1263">Get-AzSqlDatabaseAudit</span></span>
    - <span data-ttu-id="77eee-1264">Remove-AzSqlDatabaseAudit</span><span class="sxs-lookup"><span data-stu-id="77eee-1264">Remove-AzSqlDatabaseAudit</span></span>
* <span data-ttu-id="77eee-1265">脆弱性評価の設定から電子メールの制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1265">Remove email constraints from Vulnerability Assessment settings</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1266">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1266">Az.Storage</span></span>
* <span data-ttu-id="77eee-1267">2 つのパラメーター '-IndexDocument' と '-ErrorDocument404Path' を次のコマンドレットで必須から省略可能に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1267">Change 2 parameters '-IndexDocument' and '-ErrorDocument404Path' from required to optional  in cmdlet:</span></span>
    -  <span data-ttu-id="77eee-1268">Enable-AzStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="77eee-1268">Enable-AzStorageStaticWebsite</span></span>
* <span data-ttu-id="77eee-1269">例を追加して Get AzStorageBlobContent のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1269">Update help of Get-AzStorageBlobContent by add an example</span></span>
* <span data-ttu-id="77eee-1270">StorageException でコマンドレットが失敗したときにより詳細なエラー情報を表示</span><span class="sxs-lookup"><span data-stu-id="77eee-1270">Show more error information when cmdlet failed with StorageException</span></span>
* <span data-ttu-id="77eee-1271">Azure Files AAD DS 認証を持つストレージ アカウントの作成または更新をサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-1271">Support create or update Storage account with Azure Files AAD DS Authentication</span></span>
    -  <span data-ttu-id="77eee-1272">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1272">New-AzStorageAccount</span></span>
    -  <span data-ttu-id="77eee-1273">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1273">Set-AzStorageAccount</span></span>
* <span data-ttu-id="77eee-1274">ファイル共有、ファイル ディレクトリ、またはファイルのファイル ハンドルを閉じるまたは一覧表示をサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-1274">Support list or close file handles of a file share, file directory or a file</span></span>
    - <span data-ttu-id="77eee-1275">Get-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="77eee-1275">Get-AzStorageFileHandle</span></span>
    - <span data-ttu-id="77eee-1276">Close-AzStorageFileHandle</span><span class="sxs-lookup"><span data-stu-id="77eee-1276">Close-AzStorageFileHandle</span></span>

#### <a name="azstoragesync"></a><span data-ttu-id="77eee-1277">Az.StorageSync</span><span class="sxs-lookup"><span data-stu-id="77eee-1277">Az.StorageSync</span></span>
* <span data-ttu-id="77eee-1278">このモジュールは、ロール アップ `Az` モジュールの一部として含まれるようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1278">This module is now included as a part of the roll-up `Az` module</span></span>

## <a name="232---june-2019"></a><span data-ttu-id="77eee-1279">2.3.2 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1279">2.3.2 - June 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1280">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1280">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1281">関数呼び出しにおいて、一部のケースで不適切な URL が使用されていたバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1281">Fix bug with incorrect URL being used in some cases for Functions calls</span></span>
    - <span data-ttu-id="77eee-1282">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8983</span><span class="sxs-lookup"><span data-stu-id="77eee-1282">More information here: https://github.com/Azure/azure-powershell/issues/8983</span></span>
* <span data-ttu-id="77eee-1283">AzureRM コマンドレットから Az コマンドレットへの移行におけるエイリアスの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1283">Fix Issue with aliases from AzureRM to Az cmdlets</span></span>
  - <span data-ttu-id="77eee-1284">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span><span class="sxs-lookup"><span data-stu-id="77eee-1284">Set-AzureRmVMBootDiagnostics -> Set-AzVMBootDiagnostic</span></span>
  - <span data-ttu-id="77eee-1285">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span><span class="sxs-lookup"><span data-stu-id="77eee-1285">Export-AzureRMLogAnalyticThrottledRequests -> Export-AzLogAnalyticThrottledRequest</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1286">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1286">Az.Compute</span></span>
* <span data-ttu-id="77eee-1287">単純なパラメーター セット New-AzVm および New-AzVmss で "ProximityPlacementGroup" パラメーターが受け入れられるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1287">New-AzVm and New-AzVmss simple parameter sets now accept the 'ProximityPlacementGroup' parameter.</span></span>
* <span data-ttu-id="77eee-1288">"New-AzVM" のリファレンス ドキュメントの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1288">Fix typo in 'New-AzVM' reference documentation</span></span>

#### <a name="azdns"></a><span data-ttu-id="77eee-1289">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="77eee-1289">Az.Dns</span></span>
* <span data-ttu-id="77eee-1290">"Set-AzDnsZone" ヘルプの例の入力ミスを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1290">Fixed a typo in 'Set-AzDnsZone' help examples.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="77eee-1291">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="77eee-1291">Az.EventGrid</span></span>
* <span data-ttu-id="77eee-1292">2019-06-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1292">Updated to use the 2019-06-01 API version.</span></span>
* <span data-ttu-id="77eee-1293">新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-1293">New cmdlets:</span></span>
    - <span data-ttu-id="77eee-1294">New-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="77eee-1294">New-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="77eee-1295">新しい Azure Event Grid ドメインを作成します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1295">Creates a new Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="77eee-1296">Get-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="77eee-1296">Get-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="77eee-1297">Event Grid ドメインの詳細を取得するか、現在の Azure サブスクリプション内のすべての Event Grid ドメインの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1297">Gets the details of an Event Grid Domain, or gets a list of all Event Grid Domains in the current Azure subscription.</span></span>
    - <span data-ttu-id="77eee-1298">Remove-AzureRmEventGridDomain</span><span class="sxs-lookup"><span data-stu-id="77eee-1298">Remove-AzureRmEventGridDomain</span></span>
        - <span data-ttu-id="77eee-1299">Azure Event Grid ドメインを削除します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1299">Removes an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="77eee-1300">New-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="77eee-1300">New-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="77eee-1301">Azure Event Grid ドメインの共有アクセス キーを再生成します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1301">Regenerates the shared access key for an Azure Event Grid Domain.</span></span>
    - <span data-ttu-id="77eee-1302">Get-AzureRmEventGridDomainKey</span><span class="sxs-lookup"><span data-stu-id="77eee-1302">Get-AzureRmEventGridDomainKey</span></span>
        - <span data-ttu-id="77eee-1303">Event Grid ドメインにイベントを発行するために使用される共有アクセス キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1303">Gets the shared access keys used to publish events to an Event Grid Domain.</span></span>
    - <span data-ttu-id="77eee-1304">New-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="77eee-1304">New-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="77eee-1305">新しい Azure Event Grid ドメイン トピックを作成します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1305">Creates a new Azure Event Grid Domain Topic.</span></span>
    - <span data-ttu-id="77eee-1306">Get-AzureRmEventGridDomainTopic</span><span class="sxs-lookup"><span data-stu-id="77eee-1306">Get-AzureRmEventGridDomainTopic</span></span>
        - <span data-ttu-id="77eee-1307">Event Grid ドメイン トピックの詳細を取得するか、現在の Azure 内の特定の Event Grid ドメイン下のすべての Event Grid ドメイン トピックの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1307">Gets the details of an Event Grid Domain Topic, or gets a list of all Event Grid Domain Topics under specific Event Grid Domain in the current Azure</span></span>
    - <span data-ttu-id="77eee-1308">Remove-AzureRmEventGridDomainTopic:</span><span class="sxs-lookup"><span data-stu-id="77eee-1308">Remove-AzureRmEventGridDomainTopic:</span></span>
        - <span data-ttu-id="77eee-1309">既存の Azure Event Grid ドメイン トピックを削除します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1309">Removes an existing Azure Event Grid Domain Topic.</span></span>
* <span data-ttu-id="77eee-1310">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-1310">Updated cmdlets:</span></span>
    - <span data-ttu-id="77eee-1311">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="77eee-1311">New-AzureRmEventGridSubscription/Update-AzureRmEventGridSubscription:</span></span>
        - <span data-ttu-id="77eee-1312">新しい Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1312">Add new mandatory parameters to support piping for the new Event Grid Domain and Event Grid Domain Topic to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="77eee-1313">新しい Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下に新しいイベント サブスクリプションを作成できるようにするために新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1313">Add new mandatory parameters for specifying the new Event Grid Domain name and/or Event Grid Domain Topic name to allow creating new event subscription under these resources.</span></span>
        - <span data-ttu-id="77eee-1314">既存のパラメーターの再利用を許可するためにドメインとドメイン トピック用の新しいパラメーター セットを追加しました (EndPointType、SubjectBeginsWith など)。</span><span class="sxs-lookup"><span data-stu-id="77eee-1314">Add new Parameter sets for domains and domain topics to allow reusing existing parameters (e.g., EndPointType, SubjectBeginsWith, etc).</span></span>
        - <span data-ttu-id="77eee-1315">以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="77eee-1315">Add new optional parameters for specifying:</span></span>
            - <span data-ttu-id="77eee-1316">イベント サブスクリプションの有効期限の日付</span><span class="sxs-lookup"><span data-stu-id="77eee-1316">Event subscription expiration date,</span></span>
            - <span data-ttu-id="77eee-1317">高度なフィルター パラメーター</span><span class="sxs-lookup"><span data-stu-id="77eee-1317">Advanced filtering parameters.</span></span>
        - <span data-ttu-id="77eee-1318">宛先として servicebusqueue の新しい列挙型を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1318">Add new enum for servicebusqueue as destination.</span></span>
        - <span data-ttu-id="77eee-1319">-IncludedEventType オプションの "All" の使用を不許可にし、以下に置き換えました</span><span class="sxs-lookup"><span data-stu-id="77eee-1319">Disallow usage of 'All' in -IncludedEventType option and replace it with</span></span>
    - <span data-ttu-id="77eee-1320">Get-AzEventGridTopic、Get-AzEventGridDomain、Get-AzEventGridDomainTopic、Get-AzEventGridSubscription:</span><span class="sxs-lookup"><span data-stu-id="77eee-1320">Get-AzEventGridTopic, Get-AzEventGridDomain, Get-AzEventGridDomainTopic, Get-AzEventGridSubscription:</span></span>
        - <span data-ttu-id="77eee-1321">結果の改ページ位置の自動修正とフィルター処理をサポートするために省略可能な新しいパラメーター (Top、ODataQuery、NextLink) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1321">Add new optional parameters (Top, ODataQuery and NextLink) to support results pagination and filtering.</span></span>
    - <span data-ttu-id="77eee-1322">Remove-AzureRmEventGridSubscription</span><span class="sxs-lookup"><span data-stu-id="77eee-1322">Remove-AzureRmEventGridSubscription</span></span>
        - <span data-ttu-id="77eee-1323">Event Grid ドメインと Event Grid ドメイン トピックのパイプ処理をサポートしてこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1323">Add new mandatory parameters to support piping for Event Grid Domain and Event Grid Domain Topic to allow removing existing event subscription under these resources.</span></span>
        - <span data-ttu-id="77eee-1324">Event Grid ドメイン名または Event Grid ドメイン トピック名を指定してこれらのリソース下での既存イベント サブスクリプションの削除を許可するように新しい必須のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1324">Add new mandatory parameters for specifying the Event Grid Domain name and/or Event Grid Domain Topic name to allow removing existing event subscription under these resources.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="77eee-1325">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-1325">Az.FrontDoor</span></span>
* <span data-ttu-id="77eee-1326">New-AzFrontDoorWafMatchConditionObject</span><span class="sxs-lookup"><span data-stu-id="77eee-1326">New-AzFrontDoorWafMatchConditionObject</span></span>
    - <span data-ttu-id="77eee-1327">変換のサポートと新しい演算子のオート コンプリート値 (RegEx) を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1327">Add transforms support and new operator auto-complete value (RegEx)</span></span>
* <span data-ttu-id="77eee-1328">New-AzFrontDoorWafManagedRuleObject</span><span class="sxs-lookup"><span data-stu-id="77eee-1328">New-AzFrontDoorWafManagedRuleObject</span></span>
    - <span data-ttu-id="77eee-1329">新しいオート コンプリート値を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1329">Add new auto-complete values</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1330">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1330">Az.Network</span></span>
* <span data-ttu-id="77eee-1331">仮想ネットワーク ゲートウェイ リソースのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1331">Add support for Virtual Network Gateway Resource</span></span>
    - <span data-ttu-id="77eee-1332">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1332">New cmdlets</span></span>
        - <span data-ttu-id="77eee-1333">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span><span class="sxs-lookup"><span data-stu-id="77eee-1333">Get-AzVirtualNetworkGatewayVpnClientConnectionHealth</span></span>
* <span data-ttu-id="77eee-1334">AvailablePrivateEndpointType を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1334">Add AvailablePrivateEndpointType</span></span>
    - <span data-ttu-id="77eee-1335">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1335">New cmdlets</span></span>
        - <span data-ttu-id="77eee-1336">Get-AzAvailablePrivateEndpointType</span><span class="sxs-lookup"><span data-stu-id="77eee-1336">Get-AzAvailablePrivateEndpointType</span></span>
* <span data-ttu-id="77eee-1337">PrivatePrivateLinkService を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1337">Add PrivatePrivateLinkService</span></span>
    - <span data-ttu-id="77eee-1338">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1338">New cmdlets</span></span>
        - <span data-ttu-id="77eee-1339">Get-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="77eee-1339">Get-AzPrivateLinkService</span></span>
        - <span data-ttu-id="77eee-1340">New-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="77eee-1340">New-AzPrivateLinkService</span></span>
        - <span data-ttu-id="77eee-1341">Remove-AzPrivateLinkService</span><span class="sxs-lookup"><span data-stu-id="77eee-1341">Remove-AzPrivateLinkService</span></span>
        - <span data-ttu-id="77eee-1342">New-AzPrivateLinkServiceIpConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1342">New-AzPrivateLinkServiceIpConfig</span></span>
        - <span data-ttu-id="77eee-1343">Set-AzPrivateEndpointConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-1343">Set-AzPrivateEndpointConnection</span></span>
* <span data-ttu-id="77eee-1344">PrivateEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1344">Add PrivateEndpoint</span></span>
    - <span data-ttu-id="77eee-1345">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1345">New cmdlets</span></span>
        - <span data-ttu-id="77eee-1346">Get-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="77eee-1346">Get-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="77eee-1347">New-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="77eee-1347">New-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="77eee-1348">Remove-AzPrivateEndpoint</span><span class="sxs-lookup"><span data-stu-id="77eee-1348">Remove-AzPrivateEndpoint</span></span>
        - <span data-ttu-id="77eee-1349">New-AzPrivateLinkServiceConnection</span><span class="sxs-lookup"><span data-stu-id="77eee-1349">New-AzPrivateLinkServiceConnection</span></span>
* <span data-ttu-id="77eee-1350">次の機能のために以下のコマンドを更新しました。VpnConnection 上の UseLocalAzureIpAddress フラグ</span><span class="sxs-lookup"><span data-stu-id="77eee-1350">Updated below commands for feature: UseLocalAzureIpAddress flag on VpnConnection</span></span>
    - <span data-ttu-id="77eee-1351">New-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1351">Updated New-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
    - <span data-ttu-id="77eee-1352">Set-AzVpnConnection を更新:接続の初期化時にローカルの azure ip アドレスをソース アドレスとして使用する必要があることを示すために、省略可能なパラメーター -UseLocalAzureIpAddress を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1352">Updated Set-AzVpnConnection: Added optional parameter -UseLocalAzureIpAddress to indicate that local azure ip address should be used as source address while initiating connection.</span></span>
* <span data-ttu-id="77eee-1353">ExpressRoute ピアリングに読み取り専用フィールド PeeredConnections を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1353">Added readonly field PeeredConnections in ExpressRoute peering.</span></span>
* <span data-ttu-id="77eee-1354">ExpressRoute に読み取り専用フィールド GlobalReachEnabled を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1354">Added readonly field GlobalReachEnabled in ExpressRoute.</span></span>
* <span data-ttu-id="77eee-1355">ExpressRouteCircuit モデル内の AllowGlobalReach フィールドの廃止に注意を向けるために破壊的変更属性を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1355">Added breaking change attribute to call out deprecation of AllowGlobalReach field in ExpressRouteCircuit model</span></span>
* <span data-ttu-id="77eee-1356">TargetListenerID を AzApplicationGatewayRedirectConfiguration コマンドレットと共に使用するとエラーが発生する問題 8756 を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1356">Fixed Issue 8756 Error using TargetListenerID with AzApplicationGatewayRedirectConfiguration cmdlets</span></span>
* <span data-ttu-id="77eee-1357">書き換えルールセットの設定を妨げる New-AzApplicationGatewayPathRuleConfig のバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1357">Fixed bug in New-AzApplicationGatewayPathRuleConfig that prevented the rewrite ruleset from being set.</span></span>
* <span data-ttu-id="77eee-1358">NetworkInterfaceIpConfiguration での VirtualNetworkTaps 表示を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1358">Fixed displaying of VirtualNetworkTaps in NetworkInterfaceIpConfiguration</span></span>
* <span data-ttu-id="77eee-1359">すべての部分を一覧表示するための Cortex Get コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1359">Fixed Cortex Get cmdlets for list all part</span></span>
* <span data-ttu-id="77eee-1360">ExpressRouteGateways、VpnGateway の VirtualHub リファレンス作成を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1360">Fixed VirtualHub reference creation for ExpressRouteGateways, VpnGateway</span></span>
* <span data-ttu-id="77eee-1361">AzureFirewall および NatGateway の Availability Zones のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1361">Added support for Availability Zones in AzureFirewall and NatGateway</span></span>
* <span data-ttu-id="77eee-1362">Get-AzNetworkServiceTag コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1362">Added cmdlet Get-AzNetworkServiceTag</span></span>
* <span data-ttu-id="77eee-1363">Azure Firewall の複数のパブリック IP アドレスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1363">Add support for multiple public IP addresses for Azure Firewall</span></span>
    - <span data-ttu-id="77eee-1364">New-AzFirewall コマンドレットを更新:</span><span class="sxs-lookup"><span data-stu-id="77eee-1364">Updated New-AzFirewall cmdlet:</span></span>
        - <span data-ttu-id="77eee-1365">1 つ以上のパブリック IP アドレス オブジェクトを受け入れるパラメーター -PublicIpAddress を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1365">Added parameter -PublicIpAddress which accepts one or more Public IP Address objects</span></span>
        - <span data-ttu-id="77eee-1366">仮想ネットワーク オブジェクトを受け入れるパラメーター -VirtualNetwork を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1366">Added parameter -VirtualNetwork which accepts a Virtual Network object</span></span>
        - <span data-ttu-id="77eee-1367">ファイアウォール オブジェクトにメソッド AddPublicIpAddress および RemovePublicIpAddress を追加しました (これらは入力としてパブリック IP アドレス オブジェクトを受け入れます)</span><span class="sxs-lookup"><span data-stu-id="77eee-1367">Added methods AddPublicIpAddress and RemovePublicIpAddress on firewall object - these accept a Public IP Address object as input</span></span>
        - <span data-ttu-id="77eee-1368">パラメーター -PublicIpName および -VirtualNetworkName が非推奨になりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1368">Deprecated parameters -PublicIpName and -VirtualNetworkName</span></span>
* <span data-ttu-id="77eee-1369">次の機能のために以下のコマンドを更新しました。仮想ネットワーク ゲートウェイ リソースに VpnClient AAD 認証オプションを設定しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1369">Updated below commands for feature: Set VpnClient AAD authentication options to Virtual network gateway resource.</span></span>
    - <span data-ttu-id="77eee-1370">New-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1370">Updated New-AzVirtualNetworkGateway: Added optional parameters AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="77eee-1371">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイ上で VpnClient AAD 認証オプションを設定するための省略可能なパラメーター AadTenantUri、AadAudienceId、および AadIssuerUri を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1371">Updated Set-AzVirtualNetworkGateway: Added optional parameter AadTenantUri,AadAudienceId,AadIssuerUri to set VpnClient AAD authentication options on Gateway.</span></span>
    - <span data-ttu-id="77eee-1372">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイから VpnClient AAD 認証オプションを削除するための省略可能なスイッチ パラメーター RemoveAadAuthentication を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1372">Updated Set-AzVirtualNetworkGateway: Added optional switch parameter RemoveAadAuthentication to remove VpnClient AAD authentication options from Gateway.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-1373">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1373">Az.OperationalInsights</span></span>
* <span data-ttu-id="77eee-1374">"New-AzureRmOperationalInsightsWorkspace" コマンドでの **pergb2018** 価格レベルを有効しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1374">Enable **pergb2018** pricing tier in 'New-AzureRmOperationalInsightsWorkspace' command</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1375">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1375">Az.Resources</span></span>
* <span data-ttu-id="77eee-1376">追加の [テンプレートのエクスポート] オプションがサポートされました</span><span class="sxs-lookup"><span data-stu-id="77eee-1376">Support for additional Template Export options</span></span>
    - <span data-ttu-id="77eee-1377">Export-AzResourceGroup に "-SkipResourceNameParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1377">Add '-SkipResourceNameParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="77eee-1378">Export-AzResourceGroup に "-SkipAllParameterization" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1378">Add '-SkipAllParameterization' parameter to Export-AzResourceGroup</span></span>
    - <span data-ttu-id="77eee-1379">エクスポートされたリソースのフィルター処理用に Export-AzResourceGroup に "-Resource" パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1379">Add '-Resource' parameter to Export-AzResourceGroup for exported resource filtering</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-1380">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-1380">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-1381">場合によって、ByExistingKeyVault の証明書追加で誤ったサムプリントが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1381">Fix add certificate ByExistingKeyVault getting the wrong thumbprint in some cases</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1382">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1382">Az.Sql</span></span>
* <span data-ttu-id="77eee-1383">Advanced Threat Protection ストレージ エンドポイント サフィックスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1383">Fix Advanced Threat Protection storage endpoint suffix</span></span>
* <span data-ttu-id="77eee-1384">Advanced Data Security を有効にする Advanced Threat Protection ポリシーのオーバーライドを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1384">Fix Advanced Data Security enable overrides Advanced Threat Protection policy</span></span>
* <span data-ttu-id="77eee-1385">Management.Sql 用の新しいコマンドレットにより、マネージド インスタンスへの TDE キーの追加と TDE プロテクターの設定が可能になりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1385">New Cmdlets for Management.Sql to allow customers to add TDE keys and set TDE protector for managed instances</span></span>
   - <span data-ttu-id="77eee-1386">Add-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="77eee-1386">Add-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="77eee-1387">Get-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="77eee-1387">Get-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="77eee-1388">Remove-AzSqlInstanceKeyVaultKey</span><span class="sxs-lookup"><span data-stu-id="77eee-1388">Remove-AzSqlInstanceKeyVaultKey</span></span>
   - <span data-ttu-id="77eee-1389">Get-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="77eee-1389">Get-AzSqlInstanceTransparentDataEncryptionProtector</span></span>
   - <span data-ttu-id="77eee-1390">Set-AzSqlInstanceTransparentDataEncryptionProtector</span><span class="sxs-lookup"><span data-stu-id="77eee-1390">Set-AzSqlInstanceTransparentDataEncryptionProtector</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1391">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1391">Az.Storage</span></span>
* <span data-ttu-id="77eee-1392">ストレージ アカウントの作成時の Kind FileStorage および SkuName Premium_ZRS のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1392">Support Kind FileStorage and SkuName Premium_ZRS when create Storage account</span></span>
    - <span data-ttu-id="77eee-1393">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1393">New-AzStorageAccount</span></span>
* <span data-ttu-id="77eee-1394">BLOB 不変コマンドレットの説明を明確化しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1394">Clarified description of blob immutability cmdlet</span></span>
    -  <span data-ttu-id="77eee-1395">Remove-AzRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-1395">Remove-AzRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1396">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1396">Az.Websites</span></span>
* <span data-ttu-id="77eee-1397">クライアントではなくサーバー上のリソース グループでフィルター処理するように Get-AzWebAppCertificate を最適化しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1397">Optimizes Get-AzWebAppCertificate to filter by resource group on the server instead of the client</span></span>
* <span data-ttu-id="77eee-1398">Get-AzWebAppSnapshot に -UseDisasterRecovery スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1398">Adds -UseDisasterRecovery switch parameter to Get-AzWebAppSnapshot</span></span>

## <a name="220---june-2019"></a><span data-ttu-id="77eee-1399">2.2.0 - 2019 年 6 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1399">2.2.0 - June 2019</span></span>
#### <a name="azcdn"></a><span data-ttu-id="77eee-1400">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-1400">Az.Cdn</span></span>
* <span data-ttu-id="77eee-1401">API バージョン 2019-04-15 に基づいて rulesEngine 機能をサポートするようにコマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1401">Updated cmdlets to support rulesEngine feature based on API version 2019-04-15.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1402">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1402">Az.Compute</span></span>
* <span data-ttu-id="77eee-1403">操作を開始し、操作が完了する前にすぐに戻す、`NoWait` パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1403">Added `NoWait` parameter that starts the operation and returns immediately, before the operation is completed.</span></span>
    - <span data-ttu-id="77eee-1404">更新されたコマンドレット: Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span><span class="sxs-lookup"><span data-stu-id="77eee-1404">Updated cmdlets:   Export-AzLogAnalyticRequestRateByInterval   Export-AzLogAnalyticThrottledRequest   Remove-AzVM   Remove-AzVMAccessExtension   Remove-AzVMAEMExtension   Remove-AzVMChefExtension   Remove-AzVMCustomScriptExtension   Remove-AzVMDiagnosticsExtension   Remove-AzVMDiskEncryptionExtension   Remove-AzVMDscExtension   Remove-AzVMSqlServerExtension   Restart-AzVM   Set-AzVM   Set-AzVMAccessExtension   Set-AzVMADDomainExtension   Set-AzVMAEMExtension   Set-AzVMBginfoExtension   Set-AzVMChefExtension   Set-AzVMCustomScriptExtension   Set-AzVMDiagnosticsExtension   Set-AzVMDscExtension   Set-AzVMExtension   Start-AzVM   Stop-AzVM   Update-AzVM</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-1405">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1405">Az.EventHub</span></span>
* <span data-ttu-id="77eee-1406">#9231 (Get AzEventHubNamespace がタグを返さない) を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1406">Fix for #9231 - Get-AzEventHubNamespace does not return tags</span></span>
* <span data-ttu-id="77eee-1407">#9230 (Get-AzEventHubNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1407">Fix for #9230 - Get-AzEventHubNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1408">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1408">Az.Network</span></span>
* <span data-ttu-id="77eee-1409">Nat Gateway の ResourceId と InputObject を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1409">Update ResourceId and InputObject for Nat Gateway</span></span>
    - <span data-ttu-id="77eee-1410">ResourceId と InputObject のエイリアスを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1410">Add alias for ResourceId and InputObject</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-1411">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1411">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-1412">Get-AzPolicyEvent の null 参照の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1412">Fix Null reference issue in Get-AzPolicyEvent</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1413">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1413">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1414">IaaSVM ポリシーの最小リテンション期間の日数を 1 日から 7 日に変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1414">IaaSVM policy minimum retention in days changed to 7 from 1</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="77eee-1415">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="77eee-1415">Az.ServiceBus</span></span>
* <span data-ttu-id="77eee-1416">#9182 (Get-AzServiceBusNamespace が ResourceGroupName ではなく ResourceGroup を返す) を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1416">Fix for issue #9182 - Get-AzServiceBusNamespace returns ResourceGroup instead of ResourceGroupName</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-1417">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-1417">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-1418">'Update-AzServiceFabricReliability' に対するエラー メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1418">Fix typo in error message for 'Update-AzServiceFabricReliability'</span></span>
* <span data-ttu-id="77eee-1419">Service Fabric のコマンドラインの文字の欠落を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1419">Fix missing character in Service Fabric cmdlines</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1420">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1420">Az.Sql</span></span>
* <span data-ttu-id="77eee-1421">Managed Instance で AutoDr をサポートするために、New-AzureSqlInstance コマンドレットに DnsZonePartner パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1421">Add DnsZonePartner Parameter for New-AzureSqlInstance cmdlet to support AutoDr for Managed Instance.</span></span>
* <span data-ttu-id="77eee-1422">Get-AzSqlDatabaseSecureConnectionPolicy コマンドレットを非推奨化</span><span class="sxs-lookup"><span data-stu-id="77eee-1422">Deprecating Get-AzSqlDatabaseSecureConnectionPolicy cmdlet</span></span>
* <span data-ttu-id="77eee-1423">Threat Protection の名前を Advanced Threat Protection に変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1423">Rename Threat Detection cmdlets to Advanced Threat Protection</span></span>
* <span data-ttu-id="77eee-1424">New-AzSqlInstance の -StorageSizeInGB パラメーターと -LicenseType パラメーターが省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1424">New-AzSqlInstance -StorageSizeInGB and -LicenseType parameters are now optional.</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1425">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1425">Az.Websites</span></span>
* <span data-ttu-id="77eee-1426">Set-AzWebApp と Set-AzWebAppSlot を -WebApp プロパティと共に使用するとタグが削除されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1426">fixes the issue where using  Set-AzWebApp and Set-AzWebAppSlot with -WebApp property was removing the tags</span></span>

## <a name="210---may-2019"></a><span data-ttu-id="77eee-1427">2.1.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1427">2.1.0 - May 2019</span></span>
#### <a name="azapimanagement"></a><span data-ttu-id="77eee-1428">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-1428">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-1429">グローバルと API スコープでの診断を管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1429">Created new Cmdlets for managing diagnostics at the global and API Scope</span></span>
    - <span data-ttu-id="77eee-1430">**Get-AzApiManagementDiagnostic** - グローバルまたは API スコープ構成済みの診断を取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-1430">**Get-AzApiManagementDiagnostic** - Get the diagnostics configured a global or api Scope</span></span>
    - <span data-ttu-id="77eee-1431">**New-AzApiManagementDiagnostic** - グローバルまたは API スコープで新しい診断を作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-1431">**New-AzApiManagementDiagnostic** - Create new diagnostics at the global scope or api Scope</span></span>
    - <span data-ttu-id="77eee-1432">**New-AzApiManagementHttpMessageDiagnostic** - ログに記録するヘッダーと Body Bytes のサイズの診断設定を作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-1432">**New-AzApiManagementHttpMessageDiagnostic** - Create diagnostic setting for which Headers to log and the size of Body Bytes</span></span>
    - <span data-ttu-id="77eee-1433">**New-AzApiManagementPipelineDiagnosticSetting** - ゲートウェイとの HTTP メッセージの着信/発信の診断設定を作成します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1433">**New-AzApiManagementPipelineDiagnosticSetting** - Create Diagnostic settings for incoming/outgoing HTTP messages to the Gateway.</span></span>
    - <span data-ttu-id="77eee-1434">**New-AzApiManagementSamplingSetting** - 診断の要求/応答のサンプリング設定を作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-1434">**New-AzApiManagementSamplingSetting** - Create Sampling Setting  for the requests/response for a diagnostic</span></span>
    - <span data-ttu-id="77eee-1435">**Remove-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-1435">**Remove-AzApiManagementDiagnostic** - Remove a diagnostic entity at global or api scope</span></span>
    - <span data-ttu-id="77eee-1436">**Set-AzApiManagementDiagnostic** - グローバルまたは API スコープで診断エンティティを更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-1436">**Set-AzApiManagementDiagnostic** - Update a diagnostic Entity at global or api scope</span></span>
* <span data-ttu-id="77eee-1437">ApiManagement サービスのキャッシュを管理するための新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1437">Created new Cmdlets for managing Cache in ApiManagement service</span></span>
    - <span data-ttu-id="77eee-1438">**Get-AzApiManagementCache** - 識別子で指定されたキャッシュ、またはすべてのキャッシュの詳細を取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-1438">**Get-AzApiManagementCache** - Get the details of the Cache specified by identifier or all caches</span></span>
    - <span data-ttu-id="77eee-1439">**New-AzApiManagementCache** - 新しい 'default' のキャッシュ、または Azure の特定の 'region' にキャッシュを作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-1439">**New-AzApiManagementCache** - Create a new 'default' Cache or Cache in a particular azure 'region'</span></span>
    - <span data-ttu-id="77eee-1440">**Remove-AzApiManagementCache** - キャッシュを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-1440">**Remove-AzApiManagementCache** - Remove a cache</span></span>
    - <span data-ttu-id="77eee-1441">**Update-AzApiManagementCache** - キャッシュを更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-1441">**Update-AzApiManagementCache** - Update a cache</span></span>
* <span data-ttu-id="77eee-1442">API スキーマの管理用に作成された新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1442">Created new Cmdlets for managing API Schema</span></span>
    - <span data-ttu-id="77eee-1443">**New-AzApiManagementSchema** - API の新しいスキーマを作成します</span><span class="sxs-lookup"><span data-stu-id="77eee-1443">**New-AzApiManagementSchema** - Create a new Schema for an API</span></span>
    - <span data-ttu-id="77eee-1444">**Get-AzApiManagementSchema** - API で構成されたスキーマを取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-1444">**Get-AzApiManagementSchema** - Get the schemas configured in the API</span></span>
    - <span data-ttu-id="77eee-1445">**Remove-AzApiManagementSchema** - API で構成されたスキーマを削除します</span><span class="sxs-lookup"><span data-stu-id="77eee-1445">**Remove-AzApiManagementSchema** - Remove the schema configured in the API</span></span>
    - <span data-ttu-id="77eee-1446">**Set-AzApiManagementSchema** - API で構成されたスキーマを更新します</span><span class="sxs-lookup"><span data-stu-id="77eee-1446">**Set-AzApiManagementSchema** - Update the schema configured in the API</span></span>
* <span data-ttu-id="77eee-1447">ユーザー トークンを生成するための新しいコマンドレットを作成しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1447">Created new Cmdlet for generating a User Token.</span></span>
    - <span data-ttu-id="77eee-1448">**New-AzApiManagementUserToken** - 既定で 8 時間有効な新しいユーザー トークンを生成します。'GIT' ユーザーのトークンは、このコマンドレットを使用して生成できます。/</span><span class="sxs-lookup"><span data-stu-id="77eee-1448">**New-AzApiManagementUserToken** - Generate a new User Token valid for 8 hours by default.Token for the 'GIT' user can be generated using this cmdlet./</span></span>
* <span data-ttu-id="77eee-1449">ネットワークの状態を取得する新しいコマンドレットを作成しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1449">Created a new cmdlet to retrieving the Network Status</span></span>
    - <span data-ttu-id="77eee-1450">**Get-AzApiManagementNetworkStatus** - API Management サービスが依存しているリソースのネットワークの状態の接続性を取得します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1450">**Get-AzApiManagementNetworkStatus** - Get the Network status connectivity of resources on which API Management service depends on.</span></span> <span data-ttu-id="77eee-1451">これは、ApiManagement サービスを仮想ネットワークにデプロイし、依存関係のいずれかが壊れているかどうかを確認する場合に便利です。</span><span class="sxs-lookup"><span data-stu-id="77eee-1451">This is useful when deploying ApiManagement service into a Virtual Network and validing whether any of the dependencies are broken.</span></span>
* <span data-ttu-id="77eee-1452">ApiManagement サービスを管理するためにコマンドレット **New-AzApiManagement** を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1452">Updated cmdlet **New-AzApiManagement** to manage ApiManagement service</span></span>
    - <span data-ttu-id="77eee-1453">新しい 'Consumption' SKU のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1453">Added support for the new 'Consumption' SKU</span></span>
    - <span data-ttu-id="77eee-1454">'Consumption' SKU 用に 'EnableClientCertificate' フラグをオンにするサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1454">Added support to turn the 'EnableClientCertificate' flag on for 'Consumption' SKU</span></span>
    - <span data-ttu-id="77eee-1455">新しいコマンドレット **New-AzApiManagementSslSetting** により 'Backend' と 'Frontend' に 'TLS/SSL' 設定を構成できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-1455">The new cmdlet **New-AzApiManagementSslSetting** allows configuring 'TLS/SSL' setting on the 'Backend' and 'Frontend'.</span></span> <span data-ttu-id="77eee-1456">これを使用して、ApiManagement サービスの 'Frontend' に '3DES' のような 'Ciphers' と 'Http2' のような 'ServerProtocols' を構成することもできます。</span><span class="sxs-lookup"><span data-stu-id="77eee-1456">This can also be used to configure 'Ciphers' like '3DES' and 'ServerProtocols' like 'Http2' on the 'Frontend' of an ApiManagement service.</span></span>
    - <span data-ttu-id="77eee-1457">ApiManagement サービスに 'DeveloperPortal' ホスト名を構成するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1457">Added support for configuring the 'DeveloperPortal' hostname on ApiManagement service.</span></span>
* <span data-ttu-id="77eee-1458">'PsApiManagement' オブジェクトを入力としてとるようにコマンドレット **Get-AzApiManagementSsoToken** を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1458">Updated cmdlets **Get-AzApiManagementSsoToken** to take 'PsApiManagement' object as input</span></span>
* <span data-ttu-id="77eee-1459">エラー メッセージをインラインで表示するコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1459">Updated the cmdlet to display Error Messages inline</span></span>
     > <span data-ttu-id="77eee-1460">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy :Error Code:ValidationError Error Message:One or more fields contain incorrect values:Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10:Logger not found, Target=log-to-eventhub]</span><span class="sxs-lookup"><span data-stu-id="77eee-1460">PS D:\github\azure-powershell> Set-AzApiManagementPolicy -Context  -PolicyFilePath C:\wrongpolicy.xml -ApiId httpbin Set-AzApiManagementPolicy : Error Code: ValidationError Error Message: One or more fields contain incorrect values: Error Details:    [Code=ValidationError, Message=Error in element 'log-to-eventhub' on line 3, column 10: Logger not found, Target=log-to-eventhub]</span></span>
* <span data-ttu-id="77eee-1461">API を 'OpenApi 3.0' 形式でエクスポートするためにコマンドレット **Export-AzApiManagementApi** を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1461">Updated cmdlet **Export-AzApiManagementApi** to export APIs in 'OpenApi 3.0' format</span></span>
* <span data-ttu-id="77eee-1462">コマンドレット **Import-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1462">Updated cmdlet **Import-AzApiManagementApi**</span></span>
    - <span data-ttu-id="77eee-1463">API を 'OpenApi 3.0' ドキュメント仕様からインポートする</span><span class="sxs-lookup"><span data-stu-id="77eee-1463">To import Api from 'OpenApi 3.0' document specification</span></span>
    - <span data-ttu-id="77eee-1464">任意の ('Swagger'、'Wadl'、'Wsdl'、'OpenApi') のドキュメントに指定された 'PsApiManagementSchema' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="77eee-1464">To override the 'PsApiManagementSchema' property specified in any ('Swagger', 'Wadl', 'Wsdl', 'OpenApi') document.</span></span>
    - <span data-ttu-id="77eee-1465">任意のドキュメントに指定された 'ServiceUrl' プロパティをオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="77eee-1465">To override the 'ServiceUrl' property specified in any document.</span></span>
* <span data-ttu-id="77eee-1466">'rawxml' を使用して xml 以外でエスケープされた 'format' でポリシーを返すために、コマンドレット **Get-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1466">Updated cmdlet **Get-AzApiManagementPolicy** to return policy in Non-Xml escaped 'format' using 'rawxml'</span></span>
* <span data-ttu-id="77eee-1467">'rawxml' を使用して xml 以外でエスケープされた 'format' と 'xml' を使用して xml でエスケープされた形式でポリシーを受け入れるために、コマンドレット **Set-AzApiManagementPolicy** を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1467">Updated cmdlet **Set-AzApiManagementPolicy** to accept policy in Non-Xml escaped 'format' using 'rawxml' and Xml escaped using 'xml'</span></span>
* <span data-ttu-id="77eee-1468">コマンドレット **New-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1468">Updated cmdlet **New-AzApiManagementApi**</span></span>
    - <span data-ttu-id="77eee-1469">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="77eee-1469">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="77eee-1470">'ApiVersionSet' に API を作成する</span><span class="sxs-lookup"><span data-stu-id="77eee-1470">To create an API in an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="77eee-1471">'SourceApiId' と 'SourceApiRevision' を使用して API を複製する。</span><span class="sxs-lookup"><span data-stu-id="77eee-1471">To clone an API using 'SourceApiId' and 'SourceApiRevision'.</span></span>
    - <span data-ttu-id="77eee-1472">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1472">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="77eee-1473">コマンドレット **Set-AzApiManagementApi** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1473">Updated cmdlet **Set-AzApiManagementApi**</span></span>
    - <span data-ttu-id="77eee-1474">'OpenId' 承認サーバーで API を構成する。</span><span class="sxs-lookup"><span data-stu-id="77eee-1474">To configure API with 'OpenId' authorization server.</span></span>
    - <span data-ttu-id="77eee-1475">'ApiVersionSet' に API を更新する</span><span class="sxs-lookup"><span data-stu-id="77eee-1475">To updated an API into an 'ApiVersionSet'</span></span>
    - <span data-ttu-id="77eee-1476">API スコープで 'SubscriptionRequired' を構成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1476">Ability to configure 'SubscriptionRequired' at the Api scope.</span></span>
* <span data-ttu-id="77eee-1477">コマンドレット **New-AzApiManagementRevision** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1477">Updated cmdlet **New-AzApiManagementRevision**</span></span>
    - <span data-ttu-id="77eee-1478">'SourceApiRevision' を使用して既存のリビジョンを複製する (コピー タグ、製品、操作、およびポリシー)。</span><span class="sxs-lookup"><span data-stu-id="77eee-1478">To clone (copy tags, products, operations and policies) an existing revision using 'SourceApiRevision'.</span></span> <span data-ttu-id="77eee-1479">新しいリビジョンは親の 'ApiId' を前提としています。</span><span class="sxs-lookup"><span data-stu-id="77eee-1479">The new Revision assumes the 'ApiId' of the parent.</span></span>
    - <span data-ttu-id="77eee-1480">'ApiRevisionDescription' を入力する</span><span class="sxs-lookup"><span data-stu-id="77eee-1480">To provide an 'ApiRevisionDescription'</span></span>
    - <span data-ttu-id="77eee-1481">API を複製するときに 'ServiceUrl' をオーバーライドする。</span><span class="sxs-lookup"><span data-stu-id="77eee-1481">To override the 'ServiceUrl' when cloning an API.</span></span>
* <span data-ttu-id="77eee-1482">コマンドレット **New-AzApiManagementIdentityProvider** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1482">Updated cmdlet **New-AzApiManagementIdentityProvider**</span></span>
    - <span data-ttu-id="77eee-1483">'AAD' または 'AADB2C' と 'Authority' を構成する</span><span class="sxs-lookup"><span data-stu-id="77eee-1483">To configure 'AAD' or 'AADB2C' with an 'Authority'</span></span>
    - <span data-ttu-id="77eee-1484">'SignupPolicy'、'SigninPolicy'、'ProfileEditingPolicy'、および 'PasswordResetPolicy' を設定する</span><span class="sxs-lookup"><span data-stu-id="77eee-1484">To setup 'SignupPolicy', 'SigninPolicy', 'ProfileEditingPolicy' and 'PasswordResetPolicy'</span></span>
* <span data-ttu-id="77eee-1485">コマンドレット **New-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1485">Updated cmdlet **New-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="77eee-1486">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="77eee-1486">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="77eee-1487">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="77eee-1487">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="77eee-1488">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1488">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="77eee-1489">コマンドレット **Set-AzApiManagementSubscription** を次のように更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1489">Updated cmdlet **Set-AzApiManagementSubscription**</span></span>
    - <span data-ttu-id="77eee-1490">'Scope' と 'UserId' を使用して新しい SubscriptonModel に対応する</span><span class="sxs-lookup"><span data-stu-id="77eee-1490">To account for the new SubscriptonModel using 'Scope' and 'UserId'</span></span>
    - <span data-ttu-id="77eee-1491">'ProductId' と 'UserId' を使用して古いサブスクリプション モデルに対応する</span><span class="sxs-lookup"><span data-stu-id="77eee-1491">To account for the old subscription model using 'ProductId' and 'UserId'</span></span>
    - <span data-ttu-id="77eee-1492">サブスクリプション レベルで 'AllowTracing' を有効にするサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1492">Add support to enable 'AllowTracing' at the subscription level.</span></span>
* <span data-ttu-id="77eee-1493">'ResourceId' を入力として受け入れるように、次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1493">Updated following cmdlets to accept 'ResourceId' as input</span></span>
    - <span data-ttu-id="77eee-1494">'New-AzApiManagementContext'</span><span class="sxs-lookup"><span data-stu-id="77eee-1494">'New-AzApiManagementContext'</span></span>
        > <span data-ttu-id="77eee-1495">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span><span class="sxs-lookup"><span data-stu-id="77eee-1495">New-AzApiManagementContext -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso</span></span>
    - <span data-ttu-id="77eee-1496">'Get-AzApiManagementApiRelease'</span><span class="sxs-lookup"><span data-stu-id="77eee-1496">'Get-AzApiManagementApiRelease'</span></span>
        > <span data-ttu-id="77eee-1497">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span><span class="sxs-lookup"><span data-stu-id="77eee-1497">Get-AzApiManagementApiRelease -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/apis/echo-api/releases/releaseId</span></span>
    - <span data-ttu-id="77eee-1498">'Get-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="77eee-1498">'Get-AzApiManagementApiVersionSet'</span></span>
        > <span data-ttu-id="77eee-1499">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span><span class="sxs-lookup"><span data-stu-id="77eee-1499">Get-AzApiManagementApiVersionSet -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/constoso/apiversionsets/pathversionset</span></span>
    - <span data-ttu-id="77eee-1500">'Get-AzApiManagementAuthorizationServer'</span><span class="sxs-lookup"><span data-stu-id="77eee-1500">'Get-AzApiManagementAuthorizationServer'</span></span>
    - <span data-ttu-id="77eee-1501">'Get-AzApiManagementBackend'</span><span class="sxs-lookup"><span data-stu-id="77eee-1501">'Get-AzApiManagementBackend'</span></span>
        > <span data-ttu-id="77eee-1502">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span><span class="sxs-lookup"><span data-stu-id="77eee-1502">Get-AzApiManagementBackend -ResourceId /subscriptions/subid/resourceGroups/rgName/providers/Microsoft.ApiManagement/service/contoso/backends/servicefabric</span></span>
    - <span data-ttu-id="77eee-1503">'Get-AzApiManagementCertificate'</span><span class="sxs-lookup"><span data-stu-id="77eee-1503">'Get-AzApiManagementCertificate'</span></span>
    - <span data-ttu-id="77eee-1504">'Remove-AzApiManagementApiVersionSet'</span><span class="sxs-lookup"><span data-stu-id="77eee-1504">'Remove-AzApiManagementApiVersionSet'</span></span>
    - <span data-ttu-id="77eee-1505">'Remove-AzApiManagementSubscription'</span><span class="sxs-lookup"><span data-stu-id="77eee-1505">'Remove-AzApiManagementSubscription'</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1506">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1506">Az.Automation</span></span>
* <span data-ttu-id="77eee-1507">JSON およびテキスト レコードの値を処理するために、Get AzAutomationJobOutputRecord を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1507">Updated Get-AzAutomationJobOutputRecord to handle JSON and Text record values.</span></span>
    - <span data-ttu-id="77eee-1508">次の問題を修正: https://github.com/Azure/azure-powershell/issues/7977</span><span class="sxs-lookup"><span data-stu-id="77eee-1508">Fix for issue https://github.com/Azure/azure-powershell/issues/7977</span></span>
    - <span data-ttu-id="77eee-1509">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8600</span><span class="sxs-lookup"><span data-stu-id="77eee-1509">Fix for issue https://github.com/Azure/azure-powershell/issues/8600</span></span>
* <span data-ttu-id="77eee-1510">Start-AzAutomationDscCompilationJob の動作を、その完了を待つのではなく、単にジョブを開始するように変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1510">Changed behavior for Start-AzAutomationDscCompilationJob to just start the job instead of waiting for its completion.</span></span>
    * <span data-ttu-id="77eee-1511">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8347</span><span class="sxs-lookup"><span data-stu-id="77eee-1511">Fix for issue https://github.com/Azure/azure-powershell/issues/8347</span></span>
* <span data-ttu-id="77eee-1512">-Name を使用するとすべてのノードが返される場合の Get-AzAutomationDscNode を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1512">Fix for Get-AzAutomationDscNode when using -Name returns all node.</span></span> <span data-ttu-id="77eee-1513">これで一致するノードのみが返されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1513">Now it returns matching node only.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1514">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1514">Az.Compute</span></span>
* <span data-ttu-id="77eee-1515">AzVmssVM コマンドレットに ProtectFromScaleIn パラメーターと ProtectFromScaleSetAction パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1515">Add ProtectFromScaleIn and ProtectFromScaleSetAction parameters to Update-AzVmssVM cmdlet.</span></span>
* <span data-ttu-id="77eee-1516">これで、'East US' がサポートされていない場合は、New-AzVM の wimple パラメーター セットが既定で使用可能な場所を使用するようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1516">New-AzVM wimple parameter set now uses by default an available location if 'East US' is not supported</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-1517">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-1517">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-1518">httpclient を使用し、データプレーン テストを Azure Freamework と統合するために、ADLS SDK を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1518">Update the ADLS sdk to use httpclient, integrate dataplane testing with azure framework</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-1519">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-1519">Az.Monitor</span></span>
* <span data-ttu-id="77eee-1520">ヘルプの例で正しくないパラメーター名を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1520">Fixed incorrect parameter names in help examples</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1521">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1521">Az.Network</span></span>
* <span data-ttu-id="77eee-1522">有効なルート テーブルの出力に DisableBgpRoutePropagation フラグを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1522">Add DisableBgpRoutePropagation flag to Effective Route Table output</span></span>
    - <span data-ttu-id="77eee-1523">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="77eee-1523">Updated cmdlet:</span></span>
        - <span data-ttu-id="77eee-1524">Get-AzEffectiveRouteTable</span><span class="sxs-lookup"><span data-stu-id="77eee-1524">Get-AzEffectiveRouteTable</span></span>
* <span data-ttu-id="77eee-1525">New-AzApplicationGatewayTrustedRootCertificate ドキュメントの二重ダッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1525">Fix double dash in New-AzApplicationGatewayTrustedRootCertificate documentation</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1526">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1526">Az.Resources</span></span>
* <span data-ttu-id="77eee-1527">拒否割り当てを取得するための新しいコマンドレット Get-AzureRmDenyAssignment を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1527">Add new cmdlet Get-AzureRmDenyAssignment for retrieving deny assignments</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1528">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1528">Az.Sql</span></span>
* <span data-ttu-id="77eee-1529">Advanced Threat Protection コマンドレットの名前を Advanced Data Security に変更し、既定で脆弱性評価を有効にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1529">Rename Advanced Threat Protection cmdlets to Advanced Data Security and enable Vulnerability Assessment by default</span></span>

## <a name="200---may-2019"></a><span data-ttu-id="77eee-1530">2.0.0 - 2019 年 5 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1530">2.0.0 - May 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1531">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1531">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1532">ユーザー名/パスワード認証での ADFS の問題を修正するために Authentication Library を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1532">Update Authentication Library to fix ADFS issues with username/password auth</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-1533">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1533">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-1534">Bing Search Services について、Bing の免責事項のみを表示します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1534">Only display Bing disclaimer for Bing Search Services.</span></span>
* <span data-ttu-id="77eee-1535">アカウントの作成が失敗したときのエラーを改善しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1535">Improve error when create account failed.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1536">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1536">Az.Compute</span></span>
* <span data-ttu-id="77eee-1537">近接通信配置グループ機能。</span><span class="sxs-lookup"><span data-stu-id="77eee-1537">Proximity placement group feature.</span></span>
    - <span data-ttu-id="77eee-1538">次の新しいコマンドレッドを追加しました。 New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span><span class="sxs-lookup"><span data-stu-id="77eee-1538">The following new cmdlets are added:   New-AzProximityPlacementGroup   Get-AzProximityPlacementGroup   Remove-AzProximityPlacementGroup</span></span>
    - <span data-ttu-id="77eee-1539">新しいパラメーター ProximityPlacementGroupId を次のコマンドレットに追加しました。 New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-1539">The new parameter, ProximityPlacementGroupId, is added to the following cmdlets:   New-AzAvailabilitySet   New-AzVMConfig   New-AzVmssConfig</span></span>
* <span data-ttu-id="77eee-1540">New-AzGalleryImageVersion に StorageAccountType パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1540">StorageAccountType parameter is added to New-AzGalleryImageVersion.</span></span>
* <span data-ttu-id="77eee-1541">New-AzGalleryImageVersion の TargetRegion に StorageAccountType を含めることができるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1541">TargetRegion of New-AzGalleryImageVersion can contain StorageAccountType.</span></span>
* <span data-ttu-id="77eee-1542">Stop-AzVM と Stop-AzVmss に SkipShutdown スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1542">SkipShutdown switch parameter is added to Stop-AzVM and Stop-AzVmss</span></span>
* <span data-ttu-id="77eee-1543">重大な変更</span><span class="sxs-lookup"><span data-stu-id="77eee-1543">Breaking changes</span></span>
    - <span data-ttu-id="77eee-1544">Set-AzVMBootDiagnostics が Set-AzVMBootDiagnostic に変更されています。</span><span class="sxs-lookup"><span data-stu-id="77eee-1544">Set-AzVMBootDiagnostics is changed to Set-AzVMBootDiagnostic.</span></span>
    - <span data-ttu-id="77eee-1545">Export-AzLogAnalyticThrottledRequests が Export-AzLogAnalyticThrottledRequests に変更されています。</span><span class="sxs-lookup"><span data-stu-id="77eee-1545">Export-AzLogAnalyticThrottledRequests is changed to Export-AzLogAnalyticThrottledRequests.</span></span>

#### <a name="azdeploymentmanager"></a><span data-ttu-id="77eee-1546">Az.DeploymentManager</span><span class="sxs-lookup"><span data-stu-id="77eee-1546">Az.DeploymentManager</span></span>
* <span data-ttu-id="77eee-1547">Azure Deployment Manager コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="77eee-1547">First Generally Available release of Azure Deployment Manager cmdlets</span></span>

#### <a name="azdns"></a><span data-ttu-id="77eee-1548">Az.Dns</span><span class="sxs-lookup"><span data-stu-id="77eee-1548">Az.Dns</span></span>
* <span data-ttu-id="77eee-1549">DNS NameServer の自動委任</span><span class="sxs-lookup"><span data-stu-id="77eee-1549">Automatic DNS NameServer Delegation</span></span>
    - <span data-ttu-id="77eee-1550">DNS ゾーンの作成コマンドレットは、省略可能な追加のパラメーターとして親ゾーンの名前を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="77eee-1550">Create DNS zone cmdlet accepts parent zone name as additional optional parameter.</span></span>
    - <span data-ttu-id="77eee-1551">新しく作成された子ゾーンの親ゾーンに、NS レコードを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1551">Adds NS records in the parent zone for newly created child zone.</span></span>

#### <a name="azfrontdoor"></a><span data-ttu-id="77eee-1552">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-1552">Az.FrontDoor</span></span>
* <span data-ttu-id="77eee-1553">Azure FrontDoor コマンドレットの最初の一般公開リリース</span><span class="sxs-lookup"><span data-stu-id="77eee-1553">First Generally Available Release of Azure FrontDoor cmdlets</span></span>
* <span data-ttu-id="77eee-1554">WAF コマンドレットの名前を変更して "Waf" が含まれるようにしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1554">Rename WAF cmdlets to include 'Waf'</span></span>
    - `Get-AzFrontDoorFireWallPolicy --> Get-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorCustomRuleObject --> New-AzFrontDoorWafCustomRuleObject`
    - `New-AzFrontDoorFireWallPolicy --> New-AzFrontDoorWafPolicy`
    - `New-AzFrontDoorManagedRuleObject --> New-AzFrontDoorWafManagedRuleObject`
    - `New-AzFrontDoorManagedRuleOverrideObject --> New-AzFrontDoorWafManagedRuleOverrideObject`
    - `New-AzFrontDoorMatchConditionObject --> New-AzFrontDoorWafMatchConditionObject`
    - `New-AzFrontDoorRuleGroupOverrideObject --> New-AzFrontDoorWafRuleGroupOverrideObject`
    - `Remove-AzFrontDoorFireWallPolicy --> Remove-AzFrontDoorWafPolicy`
    - `Update-AzFrontDoorFireWallPolicy --> Update-AzFrontDoorWafPolicy`
#### <a name="azhdinsight"></a><span data-ttu-id="77eee-1555">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-1555">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-1556">次の 2 つのコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1556">Removed two cmdlets:</span></span>
    - <span data-ttu-id="77eee-1557">Grant-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="77eee-1557">Grant-AzHDInsightHttpServicesAccess</span></span>
    - <span data-ttu-id="77eee-1558">Revoke-AzHDInsightHttpServicesAccess</span><span class="sxs-lookup"><span data-stu-id="77eee-1558">Revoke-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="77eee-1559">Grant-AzHDInsightHttpServicesAccess に置き換わる新しいコマンドレット Set-AzHDInsightGatewayCredential を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1559">Added a new cmdlet Set-AzHDInsightGatewayCredential to replace Grant-AzHDInsightHttpServicesAccess</span></span>
* <span data-ttu-id="77eee-1560">閲覧者ロールと hdinsight オペレーター ロールを区別するようにコマンドレット Get-AzHDInsightJobOutput を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1560">Update cmdlet Get-AzHDInsightJobOutput to distinguish reader role and hdinsight operator role:</span></span>
    - <span data-ttu-id="77eee-1561">閲覧者ロールを持つユーザーは、'DefaultStorageAccountKey' パラメーターを明示的に指定する必要があります。そうしないと、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1561">Users with reader role need to specify 'DefaultStorageAccountKey' parameter explicitly, otherwise error occurs.</span></span>
    - <span data-ttu-id="77eee-1562">hdinsight オペレーター ロールを持つユーザーは影響を受けません。</span><span class="sxs-lookup"><span data-stu-id="77eee-1562">Users with hdinsight operator role will not be affected.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-1563">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-1563">Az.Monitor</span></span>
* <span data-ttu-id="77eee-1564">SQR API の新しいコマンドレット (スケジュール済みクエリ ルール)</span><span class="sxs-lookup"><span data-stu-id="77eee-1564">New cmdlets for SQR API (Scheduled Query Rule)</span></span>
    - <span data-ttu-id="77eee-1565">New-AzScheduledQueryRuleAlertingAction</span><span class="sxs-lookup"><span data-stu-id="77eee-1565">New-AzScheduledQueryRuleAlertingAction</span></span>
    - <span data-ttu-id="77eee-1566">New-AzScheduledQueryRuleAznsActionGroup</span><span class="sxs-lookup"><span data-stu-id="77eee-1566">New-AzScheduledQueryRuleAznsActionGroup</span></span>
    - <span data-ttu-id="77eee-1567">New-AzScheduledQueryRuleLogMetricTrigger</span><span class="sxs-lookup"><span data-stu-id="77eee-1567">New-AzScheduledQueryRuleLogMetricTrigger</span></span>
    - <span data-ttu-id="77eee-1568">New-AzScheduledQueryRuleSchedule</span><span class="sxs-lookup"><span data-stu-id="77eee-1568">New-AzScheduledQueryRuleSchedule</span></span>
    - <span data-ttu-id="77eee-1569">New-AzScheduledQueryRuleSource</span><span class="sxs-lookup"><span data-stu-id="77eee-1569">New-AzScheduledQueryRuleSource</span></span>
    - <span data-ttu-id="77eee-1570">New-AzScheduledQueryRuleTriggerCondition</span><span class="sxs-lookup"><span data-stu-id="77eee-1570">New-AzScheduledQueryRuleTriggerCondition</span></span>
    - <span data-ttu-id="77eee-1571">New-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="77eee-1571">New-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="77eee-1572">Get-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="77eee-1572">Get-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="77eee-1573">Set-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="77eee-1573">Set-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="77eee-1574">Update-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="77eee-1574">Update-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="77eee-1575">Remove-AzScheduledQueryRule</span><span class="sxs-lookup"><span data-stu-id="77eee-1575">Remove-AzScheduledQueryRule</span></span>
    - <span data-ttu-id="77eee-1576">SQR API に関する[詳細](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules)情報</span><span class="sxs-lookup"><span data-stu-id="77eee-1576">[More](https://docs.microsoft.com/rest/api/monitor/scheduledqueryrules) information about SQR API</span></span>
    - <span data-ttu-id="77eee-1577">GenV2 (非クラシック) メトリックベースのアラート ルールのコマンドレットが含まれるように Az.Monitor.md を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1577">Updated Az.Monitor.md to include cmdlets for GenV2(non classic) metric-based alert rule</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1578">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1578">Az.Network</span></span>
* <span data-ttu-id="77eee-1579">Nat Gateway Resource に対するサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1579">Add support for Nat Gateway Resource</span></span>
    - <span data-ttu-id="77eee-1580">新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1580">New cmdlets</span></span>
        - <span data-ttu-id="77eee-1581">New-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="77eee-1581">New-AzNatGateway</span></span>
        - <span data-ttu-id="77eee-1582">Get-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="77eee-1582">Get-AzNatGateway</span></span>
        - <span data-ttu-id="77eee-1583">Set-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="77eee-1583">Set-AzNatGateway</span></span>
        - <span data-ttu-id="77eee-1584">Remove-AzNatGateway</span><span class="sxs-lookup"><span data-stu-id="77eee-1584">Remove-AzNatGateway</span></span>
   - <span data-ttu-id="77eee-1585">更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1585">Updated cmdlets</span></span>
        - <span data-ttu-id="77eee-1586">New-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="77eee-1586">New-AzureVirtualNetworkSubnetConfigCommand</span></span>
        - <span data-ttu-id="77eee-1587">Add-AzureVirtualNetworkSubnetConfigCommand</span><span class="sxs-lookup"><span data-stu-id="77eee-1587">Add-AzureVirtualNetworkSubnetConfigCommand</span></span>
* <span data-ttu-id="77eee-1588">次の機能のために以下のコマンドを更新しました。Brooklyn Gateway でのカスタム ルートの設定/削除。</span><span class="sxs-lookup"><span data-stu-id="77eee-1588">Updated below commands for feature: Custom routes set/remove on Brooklyn Gateway.</span></span>
    - <span data-ttu-id="77eee-1589">New-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1589">Updated New-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>
    - <span data-ttu-id="77eee-1590">Set-AzVirtualNetworkGateway を更新しました。ゲートウェイで設定されるカスタム ルートとしてアドレス プレフィックスを設定するために、省略可能なパラメーター -CustomRoute を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1590">Updated Set-AzVirtualNetworkGateway: Added optional parameter -CustomRoute to set the address prefixes as custom routes to set on Gateway.</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-1591">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1591">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-1592">ポリシーの評価の詳細をクエリするためのサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-1592">Support for querying policy evaluation details.</span></span>
    - <span data-ttu-id="77eee-1593">Get-AzPolicyState に '-Expand' パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1593">Add '-Expand' parameter to Get-AzPolicyState.</span></span> <span data-ttu-id="77eee-1594">'-Expand PolicyEvaluationDetails' がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="77eee-1594">Support '-Expand PolicyEvaluationDetails'.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1595">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1595">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1596">Azure から Azure へのクロス サブスクリプション サイト回復のサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-1596">Support for Cross subscription Azure to Azure site recovery.</span></span>
* <span data-ttu-id="77eee-1597">Azure Site Recovery に対する今後の重要な変更へのマーク付け。</span><span class="sxs-lookup"><span data-stu-id="77eee-1597">Marking upcoming breaking changes for Azure Site Recovery.</span></span>
* <span data-ttu-id="77eee-1598">Azure Site Recovery 復旧計画のアクション終了計画の修正。</span><span class="sxs-lookup"><span data-stu-id="77eee-1598">Fix for Azure Site Recovery recovery plan end action plan.</span></span>
* <span data-ttu-id="77eee-1599">Azure Site Recovery の Azure から Azure へのネットワーク マッピング更新の修正。</span><span class="sxs-lookup"><span data-stu-id="77eee-1599">Fix for Azure Site Recovery Update network mapping for Azure to Azure.</span></span>
* <span data-ttu-id="77eee-1600">マネージド ディスクの Azure から Azure への Azure Site Recovery 保護方向の更新の修正。</span><span class="sxs-lookup"><span data-stu-id="77eee-1600">Fix for Azure Site Recovery update protection direction for Azure to Azure for managed disk.</span></span>
* <span data-ttu-id="77eee-1601">その他の軽微な修正。</span><span class="sxs-lookup"><span data-stu-id="77eee-1601">Other minor fixes.</span></span>

#### <a name="azrelay"></a><span data-ttu-id="77eee-1602">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="77eee-1602">Az.Relay</span></span>
* <span data-ttu-id="77eee-1603">顧客向けメッセージの入力ミスを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1603">Fix typos in customer-facing messages</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="77eee-1604">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="77eee-1604">Az.ServiceBus</span></span>
* <span data-ttu-id="77eee-1605">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1605">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1606">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1606">Az.Storage</span></span>
* <span data-ttu-id="77eee-1607">ストレージ クライアント ライブラリ 10.0.1 にアップグレードしました (この SDK のすべてのオブジェクトの名前空間は、"Microsoft.WindowsAzure.Storage. *" から "Microsoft.Azure.Storage.* " に変更されています)</span><span class="sxs-lookup"><span data-stu-id="77eee-1607">Upgrade to Storage Client Library 10.0.1 (the namespace of all objects from this SDK change from 'Microsoft.WindowsAzure.Storage.*' to 'Microsoft.Azure.Storage.*')</span></span>
* <span data-ttu-id="77eee-1608">新しい API バージョン 2019-04-01 をサポートするために、Microsoft.Azure.Management.Storage 11.0.0 にアップグレードしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1608">Upgrade to Microsoft.Azure.Management.Storage 11.0.0, to support new API version 2019-04-01.</span></span>
* <span data-ttu-id="77eee-1609">ストレージ アカウントの作成での既定のストレージ アカウントの種類を "Storage" から "StorageV2" に変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1609">The default Storage account Kind in Create Storage account change from 'Storage' to 'StorageV2'</span></span>
    - <span data-ttu-id="77eee-1610">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1610">New-AzStorageAccount</span></span>
* <span data-ttu-id="77eee-1611">"-" を追加して、ストレージ アカウント コマンドレット出力 Sku.Name が入力 SkuName と対応するように変更しました (たとえば、"StandardLRS" は "Standard_LRS" に変更されます)</span><span class="sxs-lookup"><span data-stu-id="77eee-1611">Change the Storage account cmdlet output Sku.Name to be aligned with input SkuName by add '-', like 'StandardLRS' change to 'Standard_LRS'</span></span>
    - <span data-ttu-id="77eee-1612">New-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1612">New-AzStorageAccount</span></span>
    - <span data-ttu-id="77eee-1613">Get-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1613">Get-AzStorageAccount</span></span>
    - <span data-ttu-id="77eee-1614">Set-AzStorageAccount</span><span class="sxs-lookup"><span data-stu-id="77eee-1614">Set-AzStorageAccount</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1615">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1615">Az.Websites</span></span>
* <span data-ttu-id="77eee-1616">Get-AzWebApp によって返される PSSite オブジェクトに 'Kind' プロパティを設定できるようになります</span><span class="sxs-lookup"><span data-stu-id="77eee-1616">'Kind' property will now be set for PSSite objects returned by Get-AzWebApp</span></span>
* <span data-ttu-id="77eee-1617">Get-AzWebApp\*Metrics および Get-AzAppServicePlanMetrics は非推奨のマークが付けられました</span><span class="sxs-lookup"><span data-stu-id="77eee-1617">Get-AzWebApp\*Metrics and Get-AzAppServicePlanMetrics marked deprecated</span></span>

## <a name="180---april-2019"></a><span data-ttu-id="77eee-1618">1.8.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1618">1.8.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="77eee-1619">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-1619">Highlights since the last major release</span></span>
* <span data-ttu-id="77eee-1620">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="77eee-1620">General availability of `Az` module</span></span>
* <span data-ttu-id="77eee-1621">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="77eee-1621">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="77eee-1622">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="77eee-1622">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="77eee-1623">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1623">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="77eee-1624">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1624">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="77eee-1625">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1625">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="77eee-1626">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1626">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-1627">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1627">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1628">Mac でモジュールを正常に削除するように Uninstall-AzureRm を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1628">Update Uninstall-AzureRm to correctly delete modules in Mac</span></span>

#### <a name="azbatch"></a><span data-ttu-id="77eee-1629">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="77eee-1629">Az.Batch</span></span>
* <span data-ttu-id="77eee-1630">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1630">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-1631">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-1631">Az.Cdn</span></span>
* <span data-ttu-id="77eee-1632">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1632">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-1633">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1633">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-1634">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1634">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1635">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1635">Az.Compute</span></span>
* <span data-ttu-id="77eee-1636">ディスクのリソース ID に小文字の resourcegroups がある場合の AEM インストールの問題を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1636">Fix issue with AEM installation if resource ids of disks had lowercase resourcegroups in resource id</span></span>
* <span data-ttu-id="77eee-1637">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1637">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="77eee-1638">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1638">Fix documentation for wildcards</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1639">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1639">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1640">マネージド型の統合ランタイムの NodeCount が null でない場合の SsisProperties を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1640">Add SsisProperties if NodeCount not null for managed integration runtime.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-1641">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-1641">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-1642">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1642">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="77eee-1643">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="77eee-1643">Az.EventGrid</span></span>
* <span data-ttu-id="77eee-1644">作成/更新イベントのサブスクリプション コマンドレットを使用する前にリソースが作成される必要があることを示すようにエンドポイントのヘルプ テキストを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1644">Updated the help text for endpoint to indicate that resources should be created before using the create/update event subscription cmdlets.</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-1645">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1645">Az.EventHub</span></span>
* <span data-ttu-id="77eee-1646">名前空間の NetworkRuleSet 用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1646">Added new cmdlets for NetworkRuleSet of Namespace</span></span>

#### <a name="azhdinsight"></a><span data-ttu-id="77eee-1647">Az.HDInsight</span><span class="sxs-lookup"><span data-stu-id="77eee-1647">Az.HDInsight</span></span>
* <span data-ttu-id="77eee-1648">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1648">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-1649">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1649">Az.IotHub</span></span>
* <span data-ttu-id="77eee-1650">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1650">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-1651">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-1651">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-1652">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1652">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="77eee-1653">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1653">Fix documentation for wildcards</span></span>

#### <a name="azmachinelearning"></a><span data-ttu-id="77eee-1654">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="77eee-1654">Az.MachineLearning</span></span>
* <span data-ttu-id="77eee-1655">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1655">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmedia"></a><span data-ttu-id="77eee-1656">Az.Media</span><span class="sxs-lookup"><span data-stu-id="77eee-1656">Az.Media</span></span>
* <span data-ttu-id="77eee-1657">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1657">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-1658">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-1658">Az.Monitor</span></span>
  * <span data-ttu-id="77eee-1659">GenV2 (クラシック以外) メトリックベースのアラート ルールの新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1659">New cmdlets for GenV2(non classic) metric-based alert rule</span></span>
      - <span data-ttu-id="77eee-1660">New-AzMetricAlertRuleV2DimensionSelection</span><span class="sxs-lookup"><span data-stu-id="77eee-1660">New-AzMetricAlertRuleV2DimensionSelection</span></span>
      - <span data-ttu-id="77eee-1661">New-AzMetricAlertRuleV2Criteria</span><span class="sxs-lookup"><span data-stu-id="77eee-1661">New-AzMetricAlertRuleV2Criteria</span></span>
      - <span data-ttu-id="77eee-1662">Remove-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="77eee-1662">Remove-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="77eee-1663">Get-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="77eee-1663">Get-AzMetricAlertRuleV2</span></span>
      - <span data-ttu-id="77eee-1664">Add-AzMetricAlertRuleV2</span><span class="sxs-lookup"><span data-stu-id="77eee-1664">Add-AzMetricAlertRuleV2</span></span>
  * <span data-ttu-id="77eee-1665">Monitor SDK をバージョン 0.22.0-preview に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1665">Updated Monitor SDK to version 0.22.0-preview</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1666">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1666">Az.Network</span></span>
* <span data-ttu-id="77eee-1667">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1667">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="77eee-1668">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1668">Fix documentation for wildcards</span></span>

#### <a name="aznotificationhubs"></a><span data-ttu-id="77eee-1669">Az.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="77eee-1669">Az.NotificationHubs</span></span>
* <span data-ttu-id="77eee-1670">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1670">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-1671">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1671">Az.OperationalInsights</span></span>
* <span data-ttu-id="77eee-1672">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1672">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azpowerbiembedded"></a><span data-ttu-id="77eee-1673">Az.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="77eee-1673">Az.PowerBIEmbedded</span></span>
* <span data-ttu-id="77eee-1674">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1674">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1675">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1675">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1676">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1676">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="77eee-1677">Azure VM で SQL のテーブル形式を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1677">Updated table format for SQL in azure VM</span></span>
* <span data-ttu-id="77eee-1678">AzureFileShare で場所をフェッチするよう代替の方法を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1678">Added alternate method to fetch location in AzureFileShare</span></span>
* <span data-ttu-id="77eee-1679">タイムゾーンに従って SchedulePolicy オブジェクトの ScheduleRunDays を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1679">Updated ScheduleRunDays in SchedulePolicy object according to timezone</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="77eee-1680">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="77eee-1680">Az.RedisCache</span></span>
* <span data-ttu-id="77eee-1681">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1681">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1682">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1682">Az.Resources</span></span>
* <span data-ttu-id="77eee-1683">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1683">Fix documentation for wildcards</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1684">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1684">Az.Sql</span></span>
* <span data-ttu-id="77eee-1685">Monitor SDK の依存関係が一般的なコードに置き換えられます</span><span class="sxs-lookup"><span data-stu-id="77eee-1685">Replace dependency on Monitor SDK with common code</span></span>
* <span data-ttu-id="77eee-1686">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1686">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="77eee-1687">複数列の分類のプロセスを強化しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1687">Enhanced process of multiple columns classification.</span></span>
* <span data-ttu-id="77eee-1688">Get-AzSqlServerServiceObjective からの応答に sku プロパティ (sku 名、ファミリ、容量) を含め、既定でテーブルとして書式設定されるようにしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1688">Include sku properties (sku name, family, capacity) in response from Get-AzSqlServerServiceObjective and format as table by default.</span></span>
* <span data-ttu-id="77eee-1689">リージョン内に既存のサーバーを必要としない場所別の Get-AzSqlServerServiceObjective 機能。</span><span class="sxs-lookup"><span data-stu-id="77eee-1689">Ability to Get-AzSqlServerServiceObjective by location without needing a preexisting server in the region.</span></span>
* <span data-ttu-id="77eee-1690">Managed Instance 作成でのタイム ゾーン パラメーターのサポート。</span><span class="sxs-lookup"><span data-stu-id="77eee-1690">Support for time zone parameter in Managed Instance create.</span></span>
* <span data-ttu-id="77eee-1691">ワイルドカードのドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1691">Fix documentation for wildcards</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1692">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1692">Az.Websites</span></span>
* <span data-ttu-id="77eee-1693">実行時にタグを削除しないように Set-AzWebApp と Set-AzWebAppSlot を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1693">fixes the Set-AzWebApp and Set-AzWebAppSlot to not remove the tags on execution</span></span>
* <span data-ttu-id="77eee-1694">コマンドレットを複数形名詞から単数形に更新し、複数形名詞が非推奨になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1694">Updated cmdlets with plural nouns to singular, and deprecated plural names.</span></span>
* <span data-ttu-id="77eee-1695">WebSites SDK を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1695">Updated the WebSites SDK.</span></span>
* <span data-ttu-id="77eee-1696">PSAppServicePlan から AdminSiteName プロパティを削除しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1696">Removed the AdminSiteName property from PSAppServicePlan.</span></span>

## <a name="170---april-2019"></a><span data-ttu-id="77eee-1697">1.7.0 - 2019 年 4 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1697">1.7.0 - April 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="77eee-1698">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-1698">Highlights since the last major release</span></span>
* <span data-ttu-id="77eee-1699">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="77eee-1699">General availability of `Az` module</span></span>
* <span data-ttu-id="77eee-1700">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="77eee-1700">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="77eee-1701">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="77eee-1701">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="77eee-1702">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1702">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="77eee-1703">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1703">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="77eee-1704">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1704">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="77eee-1705">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1705">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azaccounts"></a><span data-ttu-id="77eee-1706">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1706">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1707">AzureAnalysisServicesEndpointResourceId パラメーターを受け取るように、Add-AzEnvironment および Set-AzEnvironment を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1707">Updated Add-AzEnvironment and Set-AzEnvironment to accept parameter AzureAnalysisServicesEndpointResourceId</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="77eee-1708">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1708">Az.AnalysisServices</span></span>
* <span data-ttu-id="77eee-1709">データプレーン コマンドレットで ServiceClient の使用と、元の認証ロジックの削除</span><span class="sxs-lookup"><span data-stu-id="77eee-1709">Using ServiceClient in dataplane cmdlets and removing the original authentication logic</span></span>
* <span data-ttu-id="77eee-1710">Add-AzureASAccount を Connect-AzAccount のラッパーとし、破壊的変更を回避しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1710">Making Add-AzureASAccount a wrapper of Connect-AzAccount to avoid a breaking change</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1711">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1711">Az.Automation</span></span>
* <span data-ttu-id="77eee-1712">New-AzAutomationSoftwareUpdateConfiguration コマンドレットのインクルージョンのバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1712">Fixed New-AzAutomationSoftwareUpdateConfiguration cmdlet bug for Inclusions.</span></span> <span data-ttu-id="77eee-1713">IncludedKbNumber パラメーターと IncludedPackageNameMask パラメーターが機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1713">Now parameter IncludedKbNumber and IncludedPackageNameMask should work.</span></span>
* <span data-ttu-id="77eee-1714">Azure Automation Update Management の動的グループのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1714">Bug fix for azure automation update management dynamic group</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1715">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1715">Az.Compute</span></span>
* <span data-ttu-id="77eee-1716">HyperVGeneration パラメーターを New-AzDiskConfig と New-AzSnapshotConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1716">Add HyperVGeneration parameter to New-AzDiskConfig and New-AzSnapshotConfig</span></span>
* <span data-ttu-id="77eee-1717">他のテナントのギャラリー イメージを使用して VM を作成できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1717">Allow VM creation with galley image from other tenants.</span></span>

#### <a name="azcontainerinstance"></a><span data-ttu-id="77eee-1718">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-1718">Az.ContainerInstance</span></span>
* <span data-ttu-id="77eee-1719">末尾の空の引数に追加される、New-AzContainerGroup の -Command パラメーターに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1719">Fixed issue in the -Command parameter of New-AzContainerGroup which added a trailing empty argument</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1720">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1720">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1721">ADF .Net SDK のバージョンを 3.0.2 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1721">Updated ADF .Net SDK version to 3.0.2</span></span>
* <span data-ttu-id="77eee-1722">Set-AzDataFactoryV2 コマンドレットを更新し、RepoConfiguration 関連の設定用のパラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1722">Updated Set-AzDataFactoryV2 cmdlet with extra parameters for RepoConfiguration related settings.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1723">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1723">Az.Resources</span></span>
* <span data-ttu-id="77eee-1724">"-ResourceId" パラメーターまたは "-ResourceGroupName"、"-Name"、および "-ResourceType" パラメーターを指定するときに、"Get-AzResource" のプロバイダーの処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1724">Improve handling of providers for 'Get-AzResource' when providing '-ResourceId' or '-ResourceGroupName', '-Name' and '-ResourceType' parameters</span></span>
* <span data-ttu-id="77eee-1725">"Test-AzDeployment" と "Test-AzResourceGroupDeployment" のエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1725">Improve error handling for 'Test-AzDeployment' and 'Test-AzResourceGroupDeployment'</span></span>
    - <span data-ttu-id="77eee-1726">デプロイ検証の外部でスローされたエラーを処理し、代わりにコマンドの出力に含めました</span><span class="sxs-lookup"><span data-stu-id="77eee-1726">Handle errors thrown outside of deployment validation and include them in output of command instead</span></span>
    - <span data-ttu-id="77eee-1727">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="77eee-1727">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>
* <span data-ttu-id="77eee-1728">スクリプトおよびジョブ シナリオでプロンプトをスキップするように、一連のデプロイ コマンドレットに "-IgnoreDynamicParameters" スイッチ パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1728">Add '-IgnoreDynamicParameters' switch parameter to set of deployment cmdlets to skip prompt in script and job scenarios</span></span>
    - <span data-ttu-id="77eee-1729">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/6856</span><span class="sxs-lookup"><span data-stu-id="77eee-1729">More information here: https://github.com/Azure/azure-powershell/issues/6856</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1730">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1730">Az.Sql</span></span>
* <span data-ttu-id="77eee-1731">データベースのデータ分類をサポートしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1731">Support Database Data Classification.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1732">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1732">Az.Storage</span></span>
* <span data-ttu-id="77eee-1733">-UseConnectedAccount パラメーターを使用してストレージ コンテキストを作成する場合、Azure アカウントへのログインなしでも詳細なエラーが報告されます</span><span class="sxs-lookup"><span data-stu-id="77eee-1733">Report detail error when create Storage context with parameter -UseConnectedAccount, but without login Azure account</span></span>
    - <span data-ttu-id="77eee-1734">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="77eee-1734">New-AzStorageContext</span></span>
* <span data-ttu-id="77eee-1735">管理プレーン API を使用して、指定したストレージ アカウントの Blob service プロパティの管理がサポートされました</span><span class="sxs-lookup"><span data-stu-id="77eee-1735">Support Manage Blob Service Properties of a specified Storage account with Management plane API</span></span>
    - <span data-ttu-id="77eee-1736">Update-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="77eee-1736">Update-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="77eee-1737">Get-AzStorageBlobServiceProperty</span><span class="sxs-lookup"><span data-stu-id="77eee-1737">Get-AzStorageBlobServiceProperty</span></span>
    - <span data-ttu-id="77eee-1738">Enable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-1738">Enable-AzStorageBlobDeleteRetentionPolicy</span></span>
    - <span data-ttu-id="77eee-1739">Disable-AzStorageBlobDeleteRetentionPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-1739">Disable-AzStorageBlobDeleteRetentionPolicy</span></span>
* <span data-ttu-id="77eee-1740">-AsJob で、BLOB とファイルのアップロード/ダウンロード コマンドレットがサポートされました</span><span class="sxs-lookup"><span data-stu-id="77eee-1740">-AsJob support for Blob and file upload and download cmdlets</span></span>
    - <span data-ttu-id="77eee-1741">Get-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1741">Get-AzStorageBlobContent</span></span>
    - <span data-ttu-id="77eee-1742">Set-AzStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1742">Set-AzStorageBlobContent</span></span>
    - <span data-ttu-id="77eee-1743">Get-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1743">Get-AzStorageFileContent</span></span>
    - <span data-ttu-id="77eee-1744">Set-AzStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="77eee-1744">Set-AzStorageFileContent</span></span>

## <a name="160---march-2019"></a><span data-ttu-id="77eee-1745">1.6.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1745">1.6.0 - March 2019</span></span>
### <a name="highlights-since-the-last-major-release"></a><span data-ttu-id="77eee-1746">前回のメジャー リリース以降のハイライト</span><span class="sxs-lookup"><span data-stu-id="77eee-1746">Highlights since the last major release</span></span>
* <span data-ttu-id="77eee-1747">`Az` モジュールの一般提供</span><span class="sxs-lookup"><span data-stu-id="77eee-1747">General availability of `Az` module</span></span>
* <span data-ttu-id="77eee-1748">`Az` モジュールの詳細については、次のリンクを参照してください。 https://aka.ms/azps-announce</span><span class="sxs-lookup"><span data-stu-id="77eee-1748">For more information about the `Az` module, please visit the following: https://aka.ms/azps-announce</span></span>
* <span data-ttu-id="77eee-1749">Location、ResourceGroup、および ResourceName 入力候補を追加: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span><span class="sxs-lookup"><span data-stu-id="77eee-1749">Added Location, ResourceGroup, and ResourceName completers: https://azure.microsoft.com/blog/completers-in-azure-powershell/</span></span>
* <span data-ttu-id="77eee-1750">Az.Compute および Az.Network 用の Get コマンドレットにワイルドカードのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1750">Added wildcard support to Get cmdlets for Az.Compute and Az.Network</span></span>
* <span data-ttu-id="77eee-1751">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1751">Added interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="77eee-1752">Az.Automation の Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1752">Added support for Python 2 runbooks in Az.Automation</span></span>
* <span data-ttu-id="77eee-1753">Az.LogicApp:統合アカウント アセンブリとバッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1753">Az.LogicApp: New cmdlets for Integration Account Assemblies and Batch Configuration</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1754">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1754">Az.Automation</span></span>
* <span data-ttu-id="77eee-1755">Azure Automation の更新プログラム管理が次の新機能をサポートするように変更されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1755">Azure automation update management change to support the following new features :</span></span>
    * <span data-ttu-id="77eee-1756">動的なグループ化</span><span class="sxs-lookup"><span data-stu-id="77eee-1756">Dynamic grouping</span></span>
    * <span data-ttu-id="77eee-1757">プリ/ポスト スクリプト</span><span class="sxs-lookup"><span data-stu-id="77eee-1757">Pre-Post script</span></span>
    * <span data-ttu-id="77eee-1758">再起動設定</span><span class="sxs-lookup"><span data-stu-id="77eee-1758">Reboot Setting</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1759">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1759">Az.Compute</span></span>
* <span data-ttu-id="77eee-1760">Get-AzVmBootDiagnosticsData のパス解決の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1760">Fix issue with path resolution in Get-AzVmBootDiagnosticsData</span></span>
* <span data-ttu-id="77eee-1761">Compute クライアント ライブラリを 25.0.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1761">Update Compute client library to 25.0.0.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-1762">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-1762">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-1763">KeyVault コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1763">Added wildcard support to KeyVault cmdlets</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1764">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1764">Az.Network</span></span>
* <span data-ttu-id="77eee-1765">Azure Firewall 用の脅威インテリジェンスのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1765">Add Threat Intelligence support for Azure Firewall</span></span>
* <span data-ttu-id="77eee-1766">Application Gateway ファイアウォール ポリシーの最上位レベルのリソースとカスタム規則を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1766">Add Application Gateway Firewall Policy top level resource and Custom Rules</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1767">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1767">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1768">インスタント RP をサポートするために Azure VM ポリシーに SnapshotRetentionInDays を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1768">Added SnapshotRetentionInDays in Azure VM policy to support Instant RP</span></span>
* <span data-ttu-id="77eee-1769">コンテナーの登録解除用にパイプ サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1769">Added pipe support for unregister container</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1770">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1770">Az.Resources</span></span>
* <span data-ttu-id="77eee-1771">Get-AzResource と Get-AzResourceGroup のワイルドカードのサポートを更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1771">Update wildcard support for Get-AzResource and Get-AzResourceGroup</span></span>
* <span data-ttu-id="77eee-1772">ARM へのジェネリック呼び出しを行うときに使用される資格情報を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1772">Update credentials used when making generic calls to ARM</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1773">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1773">Az.Sql</span></span>
* <span data-ttu-id="77eee-1774">新しい DetectionTypes が追加されたときの将来の保証と、オートコンプリートのサポートのために、脅威検出のコマンドレット パラメーター (ExcludeDetectionType) を DetectionType から string[] に変更しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1774">changed Threat Detection's cmdlets param (ExcludeDetectionType) from DetectionType to string[] to make it future proof when new DetectionTypes are added and to support autocomplete as well.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1775">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1775">Az.Storage</span></span>
* <span data-ttu-id="77eee-1776">ストレージ アカウントで管理の取得/設定/削除ポリシーをサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-1776">Support Get/Set/Remove Management Policy on a Storage account</span></span>
    - <span data-ttu-id="77eee-1777">Set-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-1777">Set-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="77eee-1778">Get-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-1778">Get-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="77eee-1779">Remove-AzStorageAccountManagementPolicy</span><span class="sxs-lookup"><span data-stu-id="77eee-1779">Remove-AzStorageAccountManagementPolicy</span></span>
    - <span data-ttu-id="77eee-1780">Add-AzStorageAccountManagementPolicyAction</span><span class="sxs-lookup"><span data-stu-id="77eee-1780">Add-AzStorageAccountManagementPolicyAction</span></span>
    - <span data-ttu-id="77eee-1781">New-AzStorageAccountManagementPolicyFilter</span><span class="sxs-lookup"><span data-stu-id="77eee-1781">New-AzStorageAccountManagementPolicyFilter</span></span>
    - <span data-ttu-id="77eee-1782">New-AzStorageAccountManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="77eee-1782">New-AzStorageAccountManagementPolicyRule</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1783">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1783">Az.Websites</span></span>
* <span data-ttu-id="77eee-1784">'New-AzWebApp -IncludeSourceWebAppSlots' を使用してすべてのスロットの複製を中断させる ARM テンプレート バグを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1784">Fix ARM template bug that breaks cloning all slots using 'New-AzWebApp -IncludeSourceWebAppSlots'</span></span>

## <a name="150---march-2019"></a><span data-ttu-id="77eee-1785">1.5.0 - 2019 年 3 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1785">1.5.0 - March 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1786">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1786">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1787">AutoRest で生成されたコマンドレットをサポートするために、"Register-AzModule" コマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1787">Add 'Register-AzModule' command to support AutoRest generated cmdlets</span></span>
* <span data-ttu-id="77eee-1788">Connect-AzAccount の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1788">Update examples for Connect-AzAccount</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1789">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1789">Az.Automation</span></span>
* <span data-ttu-id="77eee-1790">複数の Azure Automation コマンドレットで特定の月ごとのスケジュール取得する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1790">Fixed issue when retreiving certain monthly schedules in several Azure Automation cmdlets</span></span>
* <span data-ttu-id="77eee-1791">Get-AzAutomationDscNode で上位 20 個のノードのみが返される問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1791">Fix Get-AzAutomationDscNode returning just top 20 nodes.</span></span> <span data-ttu-id="77eee-1792">現在はすべてのノードが返されるようになりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1792">Now it returns all nodes</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-1793">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-1793">Az.Cdn</span></span>
* <span data-ttu-id="77eee-1794">カスタム ドメイン HTTPS を有効/無効にする新しい PowerShell コマンドレットを追加し、古いコマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1794">Added new Powershell cmdlets for Enable/Disable Custom Domain Https and deprecated the old ones</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1795">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1795">Az.Compute</span></span>
* <span data-ttu-id="77eee-1796">Get コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1796">Add wildcard support to Get cmdlets</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1797">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1797">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1798">ADF .Net SDK のバージョンを 3.0.1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1798">Updated ADF .Net SDK version to 3.0.1</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="77eee-1799">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="77eee-1799">Az.LogicApp</span></span>
* <span data-ttu-id="77eee-1800">ListWorkflows で結果の最初のページのみが取得される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1800">Fix for ListWorkflows only retrieving the first page of results</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1801">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1801">Az.Network</span></span>
* <span data-ttu-id="77eee-1802">Network コマンドレットにワイルドカードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1802">Add wildcard support to Network cmdlets</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1803">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1803">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1804">Azure VM での SQL Server のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1804">Added Sql server in Azure VM support</span></span>
* <span data-ttu-id="77eee-1805">SDK の更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1805">SDK Update</span></span>
* <span data-ttu-id="77eee-1806">Get-ProtectableItem で VMappContainer チェックを削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1806">Removed VMappContainer check in Get-ProtectableItem</span></span>
* <span data-ttu-id="77eee-1807">Get-ProtectableItem のパラメーターとして Name と ServerName を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1807">Added Name and ServerName as parameters for Get-ProtectableItem</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1808">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1808">Az.Resources</span></span>
* <span data-ttu-id="77eee-1809">デプロイ コマンドレットに `-TemplateObject` パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1809">Add `-TemplateObject` parameter to deployment cmdlets</span></span>
    - <span data-ttu-id="77eee-1810">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2933</span><span class="sxs-lookup"><span data-stu-id="77eee-1810">More information here: https://github.com/Azure/azure-powershell/issues/2933</span></span>
* <span data-ttu-id="77eee-1811">`Get-AzResource` の結果を `Set-AzResource` にパイプ処理する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1811">Fix issue when piping the result of `Get-AzResource` to `Set-AzResource`</span></span>
    - <span data-ttu-id="77eee-1812">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8240</span><span class="sxs-lookup"><span data-stu-id="77eee-1812">More information here: https://github.com/Azure/azure-powershell/issues/8240</span></span>
* <span data-ttu-id="77eee-1813">`Set-AzResource` の実行時の JSON データ型の変更に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1813">Fix issue with JSON data type change when running `Set-AzResource`</span></span>
    - <span data-ttu-id="77eee-1814">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7930</span><span class="sxs-lookup"><span data-stu-id="77eee-1814">More information here: https://github.com/Azure/azure-powershell/issues/7930</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1815">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1815">Az.Sql</span></span>
* <span data-ttu-id="77eee-1816">AuditingEndpointsCommunicator を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1816">Updating AuditingEndpointsCommunicator.</span></span>
    - <span data-ttu-id="77eee-1817">新しい診断設定を作成する際のエッジ ケースの動作を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1817">Fixing the behavior of an edge case while creating new diagnostic settings.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1818">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1818">Az.Storage</span></span>
* <span data-ttu-id="77eee-1819">New-AzStorageAccount で Storage アカウントを作成する場合に、BlockBlobStorage の種類がサポートされました</span><span class="sxs-lookup"><span data-stu-id="77eee-1819">Support Kind BlockBlobStorage when create Storage account      - New-AzStorageAccount</span></span>

## <a name="140---february-2019"></a><span data-ttu-id="77eee-1820">1.4.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1820">1.4.0 - February 2019</span></span>
#### <a name="azanalysisservices"></a><span data-ttu-id="77eee-1821">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1821">Az.AnalysisServices</span></span>
* <span data-ttu-id="77eee-1822">AddAzureASAccount コマンドレットを非推奨にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-1822">Deprecated AddAzureASAccount cmdlet</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1823">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1823">Az.Automation</span></span>
* <span data-ttu-id="77eee-1824">Import-AzAutomationDscNodeConfiguration のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1824">Update help for Import-AzAutomationDscNodeConfiguration</span></span>
* <span data-ttu-id="77eee-1825">Import-AzAutomationDscConfiguration コマンドレットに構成名検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1825">Added configuration name validation to Import-AzAutomationDscConfiguration cmdlet</span></span>
* <span data-ttu-id="77eee-1826">Import-AzAutomationDscConfiguration コマンドレットのエラー処理を改善しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1826">Improved error handling for Import-AzAutomationDscConfiguration cmdlet</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-1827">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1827">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-1828">New-AzCognitiveServicesAccount の新しい省略可能なパラメーターとして CustomSubdomainName を追加しました。これはリソースのサブドメインを指定するために使用します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1828">Added CustomSubdomainName as a new optional parameter for New-AzCognitiveServicesAccount which is used to specify subdomain for the resource.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1829">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1829">Az.Compute</span></span>
* <span data-ttu-id="77eee-1830">ID パラメーター セットに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1830">Fix issue with ID parameter sets</span></span>
* <span data-ttu-id="77eee-1831">Name パラメーターが指定されていない場合に、インストールされているすべての拡張機能を一覧表示するように Get-AzVMExtension を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1831">Update Get-AzVMExtension to list all installed extension if Name parameter is not provided</span></span>
* <span data-ttu-id="77eee-1832">Update-AzImage コマンドレットに Tag パラメーターと ResourceId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1832">Add Tag and ResourceId parameters to Update-AzImage cmdlet</span></span>
* <span data-ttu-id="77eee-1833">Get-AzVmssVM にインスタンス ID を指定せず、InstanceView を使用すると、インスタンス ビューで VMSS VM を一覧表示できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-1833">Get-AzVmssVM without instance ID and with InstanceView can list VMSS VMs with instance view.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-1834">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-1834">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-1835">ADL で削除された項目を列挙して復元するコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1835">Add cmdlets for ADL deleted item enumerate and restore</span></span>

#### <a name="azeventhub"></a><span data-ttu-id="77eee-1836">Az.EventHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1836">Az.EventHub</span></span>
* <span data-ttu-id="77eee-1837">EventHub の CaptureDescription クラス内で空のアーカイブをスキップするための新しいブール値プロパティ SkipEmptyArchives を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1837">Added new boolean property SkipEmptyArchives to Skip Empty Archives in CaptureDescription class of Eventhub</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-1838">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-1838">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-1839">Set-AzKeyVaultSecret のタグ付けを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1839">Fix tagging on Set-AzKeyVaultSecret</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="77eee-1840">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="77eee-1840">Az.LogicApp</span></span>
* <span data-ttu-id="77eee-1841">統合アカウントに Basic SKU を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1841">Add in Basic sku for Integration Accounts</span></span>
* <span data-ttu-id="77eee-1842">XSLT 2.0、XSLT 3.0、および Liquid マップの種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1842">Add in XSLT 2.0, XSLT 3.0 and Liquid Map Types</span></span>
* <span data-ttu-id="77eee-1843">統合アカウント アセンブリ用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1843">New cmdlets for Integration Account Assemblies</span></span>
    - <span data-ttu-id="77eee-1844">Get-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="77eee-1844">Get-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="77eee-1845">New-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="77eee-1845">New-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="77eee-1846">Remove-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="77eee-1846">Remove-AzIntegrationAccountAssembly</span></span>
    - <span data-ttu-id="77eee-1847">Set-AzIntegrationAccountAssembly</span><span class="sxs-lookup"><span data-stu-id="77eee-1847">Set-AzIntegrationAccountAssembly</span></span>
* <span data-ttu-id="77eee-1848">統合アカウント バッチ構成用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-1848">New cmdlets for Integration Account Batch Configuration</span></span>
    - <span data-ttu-id="77eee-1849">Get-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="77eee-1849">Get-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="77eee-1850">New-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="77eee-1850">New-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="77eee-1851">Remove-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="77eee-1851">Remove-AzIntegrationAccountBatchConfiguration</span></span>
    - <span data-ttu-id="77eee-1852">Set-AzIntegrationAccountBatchConfiguration</span><span class="sxs-lookup"><span data-stu-id="77eee-1852">Set-AzIntegrationAccountBatchConfiguration</span></span>
* <span data-ttu-id="77eee-1853">Logic Apps SDK をバージョン 4.1.0 に更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1853">Update Logic App SDK to version 4.1.0</span></span>

#### <a name="azmonitor"></a><span data-ttu-id="77eee-1854">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-1854">Az.Monitor</span></span>
* <span data-ttu-id="77eee-1855">Get-AzMetric のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1855">Update help for Get-AzMetric</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1856">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1856">Az.Network</span></span>
* <span data-ttu-id="77eee-1857">Add-AzApplicationGatewayCustomError のヘルプの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1857">Update help example for Add-AzApplicationGatewayCustomError</span></span>

#### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-1858">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-1858">Az.OperationalInsights</span></span>
* <span data-ttu-id="77eee-1859">ApplicationInsights のデータ ソースを新規作成および取得するためのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1859">Additional support for New and Get ApplicationInsights data source.</span></span>
    - <span data-ttu-id="77eee-1860">指定のワークスペースについて、特定またはすべての ApplicationInsights データ ソースを取得できるようにする、新しい "ApplicationInsights" の種類を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1860">Added new 'ApplicationInsights' kind to support Get specific and Get all ApplicationInsights data sources for given workspace.</span></span>
    - <span data-ttu-id="77eee-1861">ApplicationInsights のリソース パラメーター (サブスクリプション ID、resourceGroupName、および名前) を指定してデータ ソースを作成するための New-AzOperationalInsightsApplicationInsightsDataSource コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1861">Added New-AzOperationalInsightsApplicationInsightsDataSource cmdlet for creating data source by given Application-Insights resource parameters: subscription Id, resourceGroupName and name.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1862">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1862">Az.Resources</span></span>
* <span data-ttu-id="77eee-1863">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="77eee-1863">Fix for issue https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="77eee-1864">次の問題を修正: https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="77eee-1864">Fix for issue https://github.com/Azure/azure-powershell/issues/8235</span></span>
* <span data-ttu-id="77eee-1865">次の問題を修正: https://github.com/Azure/azure-powershell/issues/6219</span><span class="sxs-lookup"><span data-stu-id="77eee-1865">Fix for issue https://github.com/Azure/azure-powershell/issues/6219</span></span>
* <span data-ttu-id="77eee-1866">KeyCredentials の繰り返し作成を妨げるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1866">Fix bug preventing repeat creation of KeyCredentials</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1867">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1867">Az.Sql</span></span>
* <span data-ttu-id="77eee-1868">SQL DB のハイパースケール レベルのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1868">Add support for SQL DB Hyperscale tier</span></span>
* <span data-ttu-id="77eee-1869">復元要求で不要なプロパティを設定したことによって復元が失敗する可能性が生じるバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1869">Fixed bug where restore could fail due to setting unnecessary properties in restore request</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1870">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1870">Az.Websites</span></span>
* <span data-ttu-id="77eee-1871">Get-AzWebAppSlotMetrics の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1871">Correct example in Get-AzWebAppSlotMetrics</span></span>

## <a name="130---february-2019"></a><span data-ttu-id="77eee-1872">1.3.0 - 2019 年 2 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1872">1.3.0 - February 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1873">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1873">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1874">ClientRuntime を最新バージョンに更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1874">Update to latest version of ClientRuntime</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="77eee-1875">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1875">Az.AnalysisServices</span></span>
<span data-ttu-id="77eee-1876">Az.AnalysisServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="77eee-1876">General availability for Az.AnalysisServices module.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1877">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1877">Az.Compute</span></span>
* <span data-ttu-id="77eee-1878">AEM 拡張機能:UltraSSD と、P60、P70、P80 のディスクのサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1878">AEM extension: Add support for UltraSSD and P60,P70 and P80 disks</span></span>
* <span data-ttu-id="77eee-1879">Set-AzVMBootDiagnostics のヘルプの説明を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1879">Update help description for Set-AzVMBootDiagnostics</span></span>
* <span data-ttu-id="77eee-1880">Update-AzImage のヘルプの説明と例を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1880">Update help description and example for Update-AzImage</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1881">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1881">Az.RecoveryServices</span></span>
<span data-ttu-id="77eee-1882">Az.RecoveryServices モジュールを一般公開</span><span class="sxs-lookup"><span data-stu-id="77eee-1882">General availability for Az.RecoveryServices module.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1883">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1883">Az.Resources</span></span>
* <span data-ttu-id="77eee-1884">リソース グループのタグ付けを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1884">Fix tagging for resource groups</span></span>
    - <span data-ttu-id="77eee-1885">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8166</span><span class="sxs-lookup"><span data-stu-id="77eee-1885">More information here: https://github.com/Azure/azure-powershell/issues/8166</span></span>
* <span data-ttu-id="77eee-1886">`Get-AzureRmRoleAssignment` で -ErrorAction が考慮されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1886">Fix issue where `Get-AzureRmRoleAssignment` doesn't respect -ErrorAction</span></span>
    - <span data-ttu-id="77eee-1887">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8235</span><span class="sxs-lookup"><span data-stu-id="77eee-1887">More information here: https://github.com/Azure/azure-powershell/issues/8235</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1888">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1888">Az.Sql</span></span>
* <span data-ttu-id="77eee-1889">Get/Set-AzSqlDatabaseBackupShortTermRetentionPolicy を追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1889">Add Get/Set AzSqlDatabaseBackupShortTermRetentionPolicy</span></span>
* <span data-ttu-id="77eee-1890">SQL コマンドレットの実行時に Azure アカウントにログインしていない場合は nullref 例外が発生する問題を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1890">Fix issue where not being logged into Azure account would result in nullref exception when executing SQL cmdlets</span></span>
* <span data-ttu-id="77eee-1891">Get-AzSqlCapability の null ref 例外を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1891">Fixed null ref exception in Get-AzSqlCapability</span></span>

## <a name="121---january-2019"></a><span data-ttu-id="77eee-1892">1.2.1 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1892">1.2.1 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1893">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1893">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1894">正しいバージョンの認証によるリリース</span><span class="sxs-lookup"><span data-stu-id="77eee-1894">Release with correct version of Authentication</span></span>

#### <a name="azanalysisservices"></a><span data-ttu-id="77eee-1895">Az.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1895">Az.AnalysisServices</span></span>
* <span data-ttu-id="77eee-1896">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="77eee-1896">Release with updated Authentication dependency</span></span>

#### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-1897">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-1897">Az.RecoveryServices</span></span>
* <span data-ttu-id="77eee-1898">認証の依存関係の更新によるリリース</span><span class="sxs-lookup"><span data-stu-id="77eee-1898">Release with updated Authentication dependency</span></span>

## <a name="120---january-2019"></a><span data-ttu-id="77eee-1899">1.2.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1899">1.2.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1900">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1900">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1901">Windows PowerShell 5.1 のみにユーザー名/パスワードの対話型認証を追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1901">Add interactive and username/password authentication for Windows PowerShell 5.1 only</span></span>
* <span data-ttu-id="77eee-1902">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1902">Update incorrect online help URLs</span></span>
* <span data-ttu-id="77eee-1903">Uninstall-AzureRm 用に PowerShell Core の警告メッセージを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1903">Add warning message in PS Core for Uninstall-AzureRm</span></span>

#### <a name="azaks"></a><span data-ttu-id="77eee-1904">Az.Aks</span><span class="sxs-lookup"><span data-stu-id="77eee-1904">Az.Aks</span></span>
* <span data-ttu-id="77eee-1905">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1905">Update incorrect online help URLs</span></span>

#### <a name="azautomation"></a><span data-ttu-id="77eee-1906">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-1906">Az.Automation</span></span>
* <span data-ttu-id="77eee-1907">Python 2 Runbook のサポートを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1907">Added support for Python 2 runbooks</span></span>
* <span data-ttu-id="77eee-1908">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1908">Update incorrect online help URLs</span></span>

#### <a name="azcdn"></a><span data-ttu-id="77eee-1909">Az.Cdn</span><span class="sxs-lookup"><span data-stu-id="77eee-1909">Az.Cdn</span></span>
* <span data-ttu-id="77eee-1910">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1910">Update incorrect online help URLs</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1911">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1911">Az.Compute</span></span>
* <span data-ttu-id="77eee-1912">Invoke-AzVMReimage コマンドレットを追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1912">Add Invoke-AzVMReimage cmdlet</span></span>
* <span data-ttu-id="77eee-1913">TempDisk パラメーターを Set-AzVmss に追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1913">Add TempDisk parameter to Set-AzVmss</span></span>
* <span data-ttu-id="77eee-1914">New-AzVM の警告メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1914">Fix the warning message of New-AzVM</span></span>

#### <a name="azcontainerregistry"></a><span data-ttu-id="77eee-1915">Az.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="77eee-1915">Az.ContainerRegistry</span></span>
* <span data-ttu-id="77eee-1916">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1916">Update incorrect online help URLs</span></span>

#### <a name="azdatafactory"></a><span data-ttu-id="77eee-1917">Az.DataFactory</span><span class="sxs-lookup"><span data-stu-id="77eee-1917">Az.DataFactory</span></span>
* <span data-ttu-id="77eee-1918">ADF .Net SDK のバージョンを 3.0.0 に更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1918">Updated ADF .Net SDK version to 3.0.0</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-1919">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-1919">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-1920">MSI を使用するときの ADLS エンドポイントの問題を解決</span><span class="sxs-lookup"><span data-stu-id="77eee-1920">Fix issue with ADLS endpoint when using MSI</span></span>
    - <span data-ttu-id="77eee-1921">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7462</span><span class="sxs-lookup"><span data-stu-id="77eee-1921">More information here: https://github.com/Azure/azure-powershell/issues/7462</span></span>
* <span data-ttu-id="77eee-1922">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1922">Update incorrect online help URLs</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-1923">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1923">Az.IotHub</span></span>
* <span data-ttu-id="77eee-1924">エンコード形式を Add-IotHubRoutingEndpoint コマンドレットに追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1924">Add Encoding format to Add-IotHubRoutingEndpoint cmdlet.</span></span>

#### <a name="azkeyvault"></a><span data-ttu-id="77eee-1925">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-1925">Az.KeyVault</span></span>
* <span data-ttu-id="77eee-1926">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1926">Update incorrect online help URLs</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-1927">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-1927">Az.Network</span></span>
* <span data-ttu-id="77eee-1928">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1928">Update incorrect online help URLs</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1929">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1929">Az.Resources</span></span>
* <span data-ttu-id="77eee-1930">'New-AzADAppCredential' および 'New-AzADSpCredential' のリファレンス ドキュメントの誤った例を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1930">Fix incorrect examples in 'New-AzADAppCredential' and 'New-AzADSpCredential' reference documentation</span></span>
* <span data-ttu-id="77eee-1931">リソース グループのデプロイ コマンドレットを実行する前に '-TemplateFile' パラメーターのパスが解決されない問題を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1931">Fix issue where path for '-TemplateFile' parameter was not being resolved before executing resource group deployment cmdlets</span></span>
* <span data-ttu-id="77eee-1932">Az.Resources:New-AzureRmPolicyDefinition の -Mode の既定値に関するドキュメントを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1932">Az.Resources: Correct documentation for New-AzureRmPolicyDefinition -Mode default value</span></span>
* <span data-ttu-id="77eee-1933">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/7522</span><span class="sxs-lookup"><span data-stu-id="77eee-1933">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/7522</span></span>
* <span data-ttu-id="77eee-1934">Az.Resources:次の問題を修正: https://github.com/Azure/azure-powershell/issues/5747</span><span class="sxs-lookup"><span data-stu-id="77eee-1934">Az.Resources: Fix for issue https://github.com/Azure/azure-powershell/issues/5747</span></span>
* <span data-ttu-id="77eee-1935">'PSResourceGroupDeployment' オブジェクトの書式設定の問題を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1935">Fix formatting issue with 'PSResourceGroupDeployment' object</span></span>
    - <span data-ttu-id="77eee-1936">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/2123</span><span class="sxs-lookup"><span data-stu-id="77eee-1936">More information here: https://github.com/Azure/azure-powershell/issues/2123</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-1937">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-1937">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-1938">証明書が VMSS モデルに追加されたときにロールバックするが、例外がスローされるのはバグの修正のためである: https://github.com/Azure/service-fabric-issues/issues/932</span><span class="sxs-lookup"><span data-stu-id="77eee-1938">Rollback when a certificate is added to VMSS model but an exception is thrown this is to fix bug: https://github.com/Azure/service-fabric-issues/issues/932</span></span>
* <span data-ttu-id="77eee-1939">一部のエラー メッセージを修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1939">Fix some error messages.</span></span>
* <span data-ttu-id="77eee-1940">Az への移行を扱っていなかった New-AzServiceFabriCluster で、既定の ARM テンプレートを使用したクラスターの作成を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1940">Fix create cluster with default ARM template for New-AzServiceFabriCluster which was not working with migration to Az.</span></span>
* <span data-ttu-id="77eee-1941">拡張機能でクラスター ID をチェックすることで、クラスターに対応する VM Scale Sets のみに追加するように、クラスター/アプリケーション証明書の追加を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1941">Fix add cluster/application certificate to only add to VM Scale Sets that correspond to the cluster by checking cluster id in the extension.</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="77eee-1942">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="77eee-1942">Az.SignalR</span></span>
* <span data-ttu-id="77eee-1943">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1943">Update incorrect online help URLs</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1944">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1944">Az.Sql</span></span>
* <span data-ttu-id="77eee-1945">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1945">Update incorrect online help URLs</span></span>
* <span data-ttu-id="77eee-1946">LicenseType パラメーターの説明の使用可能な値を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1946">Updated parameter description for LicenseType parameter with possible values</span></span>
* <span data-ttu-id="77eee-1947">更新されるプロパティが マネージド インスタンス ID のみである場合は動作しないように、マネージド インスタンス ID の更新を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1947">Fix for updating managed instance identity not working when it is the only updated property</span></span>
* <span data-ttu-id="77eee-1948">マネージド インスタンスでカスタム照合順序をサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-1948">Support for custom collation on managed instance</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1949">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1949">Az.Storage</span></span>
* <span data-ttu-id="77eee-1950">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1950">Update incorrect online help URLs</span></span>
* <span data-ttu-id="77eee-1951">Premium Storage アカウントではクラシック ログ/メトリックをサポートしていないため、Premium Storage アカウントでクラシック ログ/メトリックを取得または設定するときの詳細エラー メッセージを付与</span><span class="sxs-lookup"><span data-stu-id="77eee-1951">Give detail error message when get/set classic Logging/Metric on Premium Storage Account, since Premium Storage Account not supoort classic Logging/Metric.</span></span>
    - <span data-ttu-id="77eee-1952">Get/Set-AzStorageServiceLoggingProperty</span><span class="sxs-lookup"><span data-stu-id="77eee-1952">Get/Set-AzStorageServiceLoggingProperty</span></span>
    - <span data-ttu-id="77eee-1953">Get/Set-AzStorageServiceMetricsProperty</span><span class="sxs-lookup"><span data-stu-id="77eee-1953">Get/Set-AzStorageServiceMetricsProperty</span></span>

#### <a name="aztrafficmanager"></a><span data-ttu-id="77eee-1954">Az.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="77eee-1954">Az.TrafficManager</span></span>
* <span data-ttu-id="77eee-1955">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1955">Update incorrect online help URLs</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-1956">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-1956">Az.Websites</span></span>
* <span data-ttu-id="77eee-1957">誤ったオンライン ヘルプの URL を更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1957">Update incorrect online help URLs</span></span>
* <span data-ttu-id="77eee-1958">アプリが ASE にホストされている場合に正しいリソース グループと場所に証明書をアップロードするように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1958">Fixes 'New-AzWebAppSSLBinding' to upload the certificate to the correct resourcegroup+location if the app is hosted on an ASE.</span></span>
* <span data-ttu-id="77eee-1959">SSL 証明書をアプリにバインドするときにタグを上書きしないように、'New-AzWebAppSSLBinding' を修正</span><span class="sxs-lookup"><span data-stu-id="77eee-1959">Fixes 'New-AzWebAppSSLBinding' to not overwrite the tags on binding an SSL certificate to an app</span></span>

## <a name="110---january-2019"></a><span data-ttu-id="77eee-1960">1.1.0 - 2019 年 1 月</span><span class="sxs-lookup"><span data-stu-id="77eee-1960">1.1.0 - January 2019</span></span>
#### <a name="azaccounts"></a><span data-ttu-id="77eee-1961">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-1961">Az.Accounts</span></span>
* <span data-ttu-id="77eee-1962">"ローカル" スコープを Enable-AzureRmAlias に追加</span><span class="sxs-lookup"><span data-stu-id="77eee-1962">Add 'Local' Scope to Enable-AzureRmAlias</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-1963">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-1963">Az.Compute</span></span>
* <span data-ttu-id="77eee-1964">名前が Restart/Start/Stop/Remove/Set-AzVM および Save-AzVMImage の ID パラメーター セットで省略可能になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1964">Name is now optional in ID parameter set for Restart/Start/Stop/Remove/Set-AzVM and Save-AzVMImage</span></span>
* <span data-ttu-id="77eee-1965">ヘルプ ファイル内の ID の説明が更新されました</span><span class="sxs-lookup"><span data-stu-id="77eee-1965">Updated the description of ID in help files</span></span>
* <span data-ttu-id="77eee-1966">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1966">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-1967">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-1967">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-1968">SDK の修正のために、データプレーンの sdk のバージョンを 1.1.14 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1968">Update the sdk version of dataplane to 1.1.14 for SDK fixes.</span></span>
    - <span data-ttu-id="77eee-1969">getfilestatus と liststatus の負の acesstime と modificationtime の処理を修正し、非同期キャンセル トークンを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1969">Fix handling of negative acesstime and modificationtime for getfilestatus and liststatus, Fix async cancellation token</span></span>

#### <a name="azeventgrid"></a><span data-ttu-id="77eee-1970">Az.EventGrid</span><span class="sxs-lookup"><span data-stu-id="77eee-1970">Az.EventGrid</span></span>
* <span data-ttu-id="77eee-1971">2019-01-01 API バージョンを使用するように更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1971">Updated to use the 2019-01-01 API version.</span></span>
* <span data-ttu-id="77eee-1972">2019-01-01 API バージョンで新しいシナリオをサポートするように次のコマンドレットを更新</span><span class="sxs-lookup"><span data-stu-id="77eee-1972">Update the following cmdlets to support new scenario in 2019-01-01 API version</span></span>
    - <span data-ttu-id="77eee-1973">New-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="77eee-1973">New-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="77eee-1974">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="77eee-1974">Event Time-To-Live,</span></span>
        - <span data-ttu-id="77eee-1975">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="77eee-1975">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="77eee-1976">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="77eee-1976">Dead letter endpoint.</span></span>
    - <span data-ttu-id="77eee-1977">Update-AzureRmEventGridSubscription:以下を指定するための新しい省略可能なパラメーターを追加:</span><span class="sxs-lookup"><span data-stu-id="77eee-1977">Update-AzureRmEventGridSubscription: Add new optional parameters for specifying:</span></span>
        - <span data-ttu-id="77eee-1978">イベントの Time-To-Live</span><span class="sxs-lookup"><span data-stu-id="77eee-1978">Event Time-To-Live,</span></span>
        - <span data-ttu-id="77eee-1979">イベントの配信試行の最大数</span><span class="sxs-lookup"><span data-stu-id="77eee-1979">Maximum number of delivery attempts for the events,</span></span>
        - <span data-ttu-id="77eee-1980">配信不能エンドポイント</span><span class="sxs-lookup"><span data-stu-id="77eee-1980">Dead letter endpoint.</span></span>
* <span data-ttu-id="77eee-1981">New-AzureRmEventGridSubscription と Update-AzureRmEventGridSubscription コマンドレットの EndpointType オプション用の新しい列挙値 (つまり storageQueue と hybridConnection) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1981">Add new enum values (namely, storageQueue and hybridConnection) for EndpointType option in New-AzureRmEventGridSubscription and Update-AzureRmEventGridSubscription cmdlets.</span></span>
* <span data-ttu-id="77eee-1982">イベント サブスクリプションの作成または更新にユーザーからの手動のアクションが必要になると想定される場合、警告メッセージを表示します。</span><span class="sxs-lookup"><span data-stu-id="77eee-1982">Show warning message if creating or updating the event subscription is expected to entail manual action from user.</span></span>

#### <a name="aziothub"></a><span data-ttu-id="77eee-1983">Az.IotHub</span><span class="sxs-lookup"><span data-stu-id="77eee-1983">Az.IotHub</span></span>
* <span data-ttu-id="77eee-1984">IotHub SDK の最新バージョンに更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1984">Updated to the latest version of the IotHub SDK</span></span>

#### <a name="azlogicapp"></a><span data-ttu-id="77eee-1985">Az.LogicApp</span><span class="sxs-lookup"><span data-stu-id="77eee-1985">Az.LogicApp</span></span>
* <span data-ttu-id="77eee-1986">Get-AzLogicApp によって指定された名前なしですべてが一覧表示されます</span><span class="sxs-lookup"><span data-stu-id="77eee-1986">Get-AzLogicApp lists all without specified Name</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-1987">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-1987">Az.Resources</span></span>
* <span data-ttu-id="77eee-1988">'Get-AzResource' 用の '-ODataQuery' および '-ResourceId' パラメーターを指定するときのパラメーター セットの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1988">Fix parameter set issue when providing '-ODataQuery' and '-ResourceId' parameters for 'Get-AzResource'</span></span>
    - <span data-ttu-id="77eee-1989">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/7875</span><span class="sxs-lookup"><span data-stu-id="77eee-1989">More information here: https://github.com/Azure/azure-powershell/issues/7875</span></span>
* <span data-ttu-id="77eee-1990">New/Set-AzPolicyDefinition での -Custom パラメーターの処理を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1990">Fix handling of the -Custom parameter in New/Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="77eee-1991">New-AzDeployment ドキュメントのタイポを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1991">Fix typo in New-AzDeployment documentation</span></span>
* <span data-ttu-id="77eee-1992">'New-AzADUser' に '-MailNickname' パラメーターが必須となりました</span><span class="sxs-lookup"><span data-stu-id="77eee-1992">Made '-MailNickname' parameter mandatory for 'New-AzADUser'</span></span>
    - <span data-ttu-id="77eee-1993">詳細については、次を参照してください。 https://github.com/Azure/azure-powershell/issues/8220</span><span class="sxs-lookup"><span data-stu-id="77eee-1993">More information here: https://github.com/Azure/azure-powershell/issues/8220</span></span>

#### <a name="azsignalr"></a><span data-ttu-id="77eee-1994">Az.SignalR</span><span class="sxs-lookup"><span data-stu-id="77eee-1994">Az.SignalR</span></span>
* <span data-ttu-id="77eee-1995">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-1995">Fix backward compatibility issue with Az.Accounts module</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-1996">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-1996">Az.Sql</span></span>
* <span data-ttu-id="77eee-1997">ストレージ管理のクライアント依存関係が、一般的な SDK 実装に変換されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-1997">Converted the Storage management client dependency to the common SDK implementation.</span></span>

#### <a name="azstorage"></a><span data-ttu-id="77eee-1998">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-1998">Az.Storage</span></span>
* <span data-ttu-id="77eee-1999">ストレージ コンテキストの StorageAccountName が Sas Token、OAuth、または Anonymous と共に作成された場合、これを実際のストレージ アカウント名として設定します</span><span class="sxs-lookup"><span data-stu-id="77eee-1999">Set the StorageAccountName of Storage context as the real Storage Account Name, when it's created with Sas Token, OAuth or Anonymous</span></span>
    - <span data-ttu-id="77eee-2000">New-AzStorageContext</span><span class="sxs-lookup"><span data-stu-id="77eee-2000">New-AzStorageContext</span></span>
* <span data-ttu-id="77eee-2001">'-FullUri' パラメーターを持つ BLOB スナップショット オブジェクトの Sas トークンを作成し、返された Uri がスナップショット Uri となるように修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2001">Create Sas Token of Blob Snapshot Object with '-FullUri' parameter, fix the returned Uri to be the sanpshot Uri</span></span>
    - <span data-ttu-id="77eee-2002">New-AzStorageBlobSASToken</span><span class="sxs-lookup"><span data-stu-id="77eee-2002">New-AzStorageBlobSASToken</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-2003">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-2003">Az.Websites</span></span>
* <span data-ttu-id="77eee-2004">'Get-AzDeletedWebApp' のバグ解析日を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2004">Fixed a date parsing bug in 'Get-AzDeletedWebApp'</span></span>
* <span data-ttu-id="77eee-2005">Az.Accounts モジュールの下位互換性の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2005">Fix backward compatibility issue with Az.Accounts module</span></span>

## <a name="100---december-2018"></a><span data-ttu-id="77eee-2006">1.0.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2006">1.0.0 - December 2018</span></span>
### <a name="general"></a><span data-ttu-id="77eee-2007">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-2007">General</span></span>

- <span data-ttu-id="77eee-2008">Az モジュールの一般公開</span><span class="sxs-lookup"><span data-stu-id="77eee-2008">General Availability of Az Module</span></span>
- <span data-ttu-id="77eee-2009">各モジュールのオンライン ヘルプ</span><span class="sxs-lookup"><span data-stu-id="77eee-2009">Online help for each module</span></span>
- <span data-ttu-id="77eee-2010">詳細とロードマップについては、[Az のお知らせのページ](https://aka.ms/azps-announce)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2010">For more details and a roadmap, see the [Az Announcement page](https://aka.ms/azps-announce)</span></span>
- <span data-ttu-id="77eee-2011">AzureRM から移行するときの詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2011">See the [Migration Guide](https://aka.ms/azps-migration-guide) for information on migrating from AzureRM</span></span>

### <a name="azaccounts"></a><span data-ttu-id="77eee-2012">Az.Accounts</span><span class="sxs-lookup"><span data-stu-id="77eee-2012">Az.Accounts</span></span>
- <span data-ttu-id="77eee-2013">Az.Profile から変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2013">Changed from Az.Profile</span></span>
- <span data-ttu-id="77eee-2014">プロファイルの表形式とコンテキストの種類を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2014">Fixed table formats for profile and context types</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="77eee-2015">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-2015">Az.ApiManagement</span></span>
- <span data-ttu-id="77eee-2016">#7002 の修正プログラム</span><span class="sxs-lookup"><span data-stu-id="77eee-2016">Fixes for #7002</span></span>
- <span data-ttu-id="77eee-2017">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2017">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbatch"></a><span data-ttu-id="77eee-2018">Az.Batch</span><span class="sxs-lookup"><span data-stu-id="77eee-2018">Az.Batch</span></span>
- <span data-ttu-id="77eee-2019">Azure Batch ノード エージェントのどのバージョンがプール内の各 VM で実行されているかを `PSComputeNode` の新しい `NodeAgentInformation` プロパティを使用して確認する機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2019">Added the ability to see what version of the Azure Batch Node Agent is running on each of the VMs in a pool, via the new `NodeAgentInformation` property on `PSComputeNode`.</span></span>
- <span data-ttu-id="77eee-2020">`PSDataDisk` の `Caching` の既定が、`None` の代わりに `ReadWrite` になりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2020">The `Caching` default for `PSDataDisk` is now `ReadWrite` instead of `None`.</span></span>
- <span data-ttu-id="77eee-2021">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2021">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azbilling"></a><span data-ttu-id="77eee-2022">Az.Billing</span><span class="sxs-lookup"><span data-stu-id="77eee-2022">Az.Billing</span></span>
- <span data-ttu-id="77eee-2023">課金、消費、および UsageAggregates コマンドレットを組み合わせます。詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2023">Combines Billing, Consumption, and UsageAggregates cmdlets, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azcognitivservices"></a><span data-ttu-id="77eee-2024">Az.CognitivServices</span><span class="sxs-lookup"><span data-stu-id="77eee-2024">Az.CognitivServices</span></span>
- <span data-ttu-id="77eee-2025">New-AzureRmCognitiveServicesAccount の操作時に利用可能な SkuName と Typem の入力候補を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2025">Add completers for SkuName and Typem available on New-AzureRmCognitiveServicesAccount operation</span></span>
- <span data-ttu-id="77eee-2026">Get-AzCognitiveServicesAccountSkus から設定される GetSkusWithAccountParamSetName パラメーターを削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2026">Removed GetSkusWithAccountParamSetName parameter set from Get-AzCognitiveServicesAccountSkus</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="77eee-2027">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-2027">Az.ContainerInstance</span></span>
- <span data-ttu-id="77eee-2028">ManagedIdentity サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2028">Added ManagedIdentity support</span></span>

### <a name="azdatalakeanalytics"></a><span data-ttu-id="77eee-2029">Az.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="77eee-2029">Az.DataLakeAnalytics</span></span>
- <span data-ttu-id="77eee-2030">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2030">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="77eee-2031">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-2031">Az.DataLakeStore</span></span>
- <span data-ttu-id="77eee-2032">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2032">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azmonitor"></a><span data-ttu-id="77eee-2033">Az.Monitor</span><span class="sxs-lookup"><span data-stu-id="77eee-2033">Az.Monitor</span></span>
- <span data-ttu-id="77eee-2034">Az.Insights の名前を Az.Monitor に変更しました。その他の小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2034">Renamed Az.Insights to Az.Monitor and other minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azkeyvault"></a><span data-ttu-id="77eee-2035">Az.KeyVault</span><span class="sxs-lookup"><span data-stu-id="77eee-2035">Az.KeyVault</span></span>
- <span data-ttu-id="77eee-2036">出力の種類から非推奨の "PurgeDisabled" プロパティを削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2036">Removed the deprecated 'PurgeDisabled' property from output types</span></span>

### <a name="azmachinelearning"></a><span data-ttu-id="77eee-2037">Az.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="77eee-2037">Az.MachineLearning</span></span>
- <span data-ttu-id="77eee-2038">Az.MachineLearningCompute モジュールのコマンドレットを組み込みました</span><span class="sxs-lookup"><span data-stu-id="77eee-2038">Included cmdlets from Az.MachineLearningCompute module</span></span>

### <a name="azmedia"></a><span data-ttu-id="77eee-2039">Az.Media</span><span class="sxs-lookup"><span data-stu-id="77eee-2039">Az.Media</span></span>
- <span data-ttu-id="77eee-2040">非推奨の "-Tags" エイリアスを New-AzMediaService から削除しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2040">Remove deprecated -Tags alias from New-AzMediaService</span></span>

### <a name="aznetwork"></a><span data-ttu-id="77eee-2041">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-2041">Az.Network</span></span>
<span data-ttu-id="77eee-2042">Application Gateway での RewriteRuleSets の構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2042">Added support for the configuring RewriteRuleSets in the Application Gateway</span></span>
    - <span data-ttu-id="77eee-2043">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-2043">New cmdlets added:</span></span>
        - <span data-ttu-id="77eee-2044">Add-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-2044">Add-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="77eee-2045">Get-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-2045">Get-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="77eee-2046">New-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-2046">New-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="77eee-2047">Remove-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-2047">Remove-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="77eee-2048">Set-AzureRmApplicationGatewayRewriteRuleSet</span><span class="sxs-lookup"><span data-stu-id="77eee-2048">Set-AzureRmApplicationGatewayRewriteRuleSet</span></span>
        - <span data-ttu-id="77eee-2049">New-AzureRmApplicationGatewayRewriteRule</span><span class="sxs-lookup"><span data-stu-id="77eee-2049">New-AzureRmApplicationGatewayRewriteRule</span></span>
        - <span data-ttu-id="77eee-2050">New-AzureRmApplicationGatewayRewriteRuleActionSet</span><span class="sxs-lookup"><span data-stu-id="77eee-2050">New-AzureRmApplicationGatewayRewriteRuleActionSet</span></span>
        - <span data-ttu-id="77eee-2051">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span><span class="sxs-lookup"><span data-stu-id="77eee-2051">New-AzureRmApplicationGatewayRewriteRuleHeaderConfiguration</span></span>
    - <span data-ttu-id="77eee-2052">省略可能なパラメーター -RewriteRuleSet を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-2052">Cmdlets updated with optional parameter -RewriteRuleSet</span></span>
        - <span data-ttu-id="77eee-2053">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="77eee-2053">New-AzureRmApplicationGateway</span></span>
        - <span data-ttu-id="77eee-2054">New-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="77eee-2054">New-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="77eee-2055">Add-AzureRmApplicationGatewayRequestRoutingRule</span><span class="sxs-lookup"><span data-stu-id="77eee-2055">Add-AzureRmApplicationGatewayRequestRoutingRule</span></span>
        - <span data-ttu-id="77eee-2056">New-AzureRmApplicationGatewayPathRuleConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-2056">New-AzureRmApplicationGatewayPathRuleConfig</span></span>
        - <span data-ttu-id="77eee-2057">Add-AzureRmApplicationGatewayUrlPathMapConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-2057">Add-AzureRmApplicationGatewayUrlPathMapConfig</span></span>
        - <span data-ttu-id="77eee-2058">New-AzureRmApplicationGatewayUrlPathMapConfig Application Gateway の KeyVault のサポートを ID を使用して追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2058">New-AzureRmApplicationGatewayUrlPathMapConfig Added KeyVault Support to Application Gateway using Identity.</span></span>
    - <span data-ttu-id="77eee-2059">省略可能なパラメーター -KeyVaultSecretId、-KeyVaultSecret を持つように更新されたコマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-2059">Cmdlets updated with optonal parameter -KeyVaultSecretId, -KeyVaultSecret</span></span>
        - <span data-ttu-id="77eee-2060">Add-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="77eee-2060">Add-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="77eee-2061">New-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="77eee-2061">New-AzApplicationGatewaySslCertificate</span></span>
        - <span data-ttu-id="77eee-2062">Set-AzApplicationGatewaySslCertificate</span><span class="sxs-lookup"><span data-stu-id="77eee-2062">Set-AzApplicationGatewaySslCertificate</span></span>
    - <span data-ttu-id="77eee-2063">省略可能なパラメーター -UserAssignedIdentity を持つように更新された New-AzApplicationGateway コマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-2063">New-AzApplicationGateway cmdlet updated with optional parameter -UserAssignedIdentity</span></span>
- <span data-ttu-id="77eee-2064">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2064">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azoperationalinsights"></a><span data-ttu-id="77eee-2065">Az.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-2065">Az.OperationalInsights</span></span>
- <span data-ttu-id="77eee-2066">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2066">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azprofile"></a><span data-ttu-id="77eee-2067">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="77eee-2067">Az.Profile</span></span>
- <span data-ttu-id="77eee-2068">モジュール名を Az.Accounts に変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2068">Changed module name to Az.Accounts</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-2069">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-2069">Az.RecoveryServices</span></span>
- <span data-ttu-id="77eee-2070">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2070">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azresources"></a><span data-ttu-id="77eee-2071">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-2071">Az.Resources</span></span>
- <span data-ttu-id="77eee-2072">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2072">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="77eee-2073">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-2073">Az.ServiceFabric</span></span>
- <span data-ttu-id="77eee-2074">共通名および拇印別での証明書の指定をサポートします</span><span class="sxs-lookup"><span data-stu-id="77eee-2074">Support specfying certificate by common name and thumbprint</span></span>
- <span data-ttu-id="77eee-2075">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2075">Mnor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azsignalr"></a><span data-ttu-id="77eee-2076">Az.SIgnalR</span><span class="sxs-lookup"><span data-stu-id="77eee-2076">Az.SIgnalR</span></span>
- <span data-ttu-id="77eee-2077">SIgnalR 用の PowerShell コマンドレットの一般公開</span><span class="sxs-lookup"><span data-stu-id="77eee-2077">General Availability for PowerShell cmdlets for SIgnalR</span></span>

### <a name="azsql"></a><span data-ttu-id="77eee-2078">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-2078">Az.Sql</span></span>
- <span data-ttu-id="77eee-2079">新しい Data_Exfiltration および Unsafe_Action の検出の種類を脅威の検出のコマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2079">Added new Data_Exfiltration and Unsafe_Action detection types to Threat Detection's cmdlets</span></span>
- <span data-ttu-id="77eee-2080">SQL 監査コマンドレットのドキュメントの例を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2080">Updated documentation examples for Sql Auditing cmdlets</span></span>
- <span data-ttu-id="77eee-2081">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2081">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azstorage"></a><span data-ttu-id="77eee-2082">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-2082">Az.Storage</span></span>
- <span data-ttu-id="77eee-2083">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2083">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

### <a name="azwebsites"></a><span data-ttu-id="77eee-2084">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-2084">Az.Websites</span></span>
- <span data-ttu-id="77eee-2085">小さな破壊的変更の詳細については、[移行ガイド](https://aka.ms/azps-migration-guide)を参照してください</span><span class="sxs-lookup"><span data-stu-id="77eee-2085">Minor breaking changes, see the [Migration Guide](https://aka.ms/azps-migration-guide)  for details</span></span>

## <a name="070---december-2018"></a><span data-ttu-id="77eee-2086">0.7.0 - 2018 年 12 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2086">0.7.0 - December 2018</span></span>

### <a name="general"></a><span data-ttu-id="77eee-2087">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-2087">General</span></span>

* <span data-ttu-id="77eee-2088">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="77eee-2088">Minor changes for upcoming AzureRM to Az transition</span></span>

### <a name="azcompute"></a><span data-ttu-id="77eee-2089">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-2089">Az.Compute</span></span>

* <span data-ttu-id="77eee-2090">`New-AzVm(ss)` コマンドレットの単純なパラメーター セットでの UltraSSD とギャラリー イメージのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2090">Add support for UltraSSD and Gallery Images in the simple param sets for `New-AzVm(ss)` cmdlets.</span></span>

### <a name="azdatalakestore"></a><span data-ttu-id="77eee-2091">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-2091">Az.DataLakeStore</span></span>

* <span data-ttu-id="77eee-2092">ADLS アカウントのドメインの末尾のスラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2092">Fix the trailing slash of the domain of adls account</span></span>

### <a name="azfrontdoor"></a><span data-ttu-id="77eee-2093">Az.FrontDoor</span><span class="sxs-lookup"><span data-stu-id="77eee-2093">Az.FrontDoor</span></span>

* <span data-ttu-id="77eee-2094">壊れたリンクを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2094">Fixed some broken links</span></span>
    - <span data-ttu-id="77eee-2095">New-AzureRmFrontDoor および Set-AzureRmFrontDoor の記事では、New-AzureRmFrontDoorHealthProbeSettingObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2095">In the New-AzureRmFrontDoor and Set-AzureRmFrontDoor articles, fixed the link to the New-AzureRmFrontDoorHealthProbeSettingObject cmdlet article.</span></span>
    - <span data-ttu-id="77eee-2096">New-AzureRmFrontDoorManagedRuleObject の記事では、New-AzureRmFrontDoorRuleGroupOverrideObject コマンドレットの記事へのリンクを修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2096">In the New-AzureRmFrontDoorManagedRuleObject article, fixed the link to the New-AzureRmFrontDoorRuleGroupOverrideObject cmdlet article.</span></span>

### <a name="azrecoveryservices"></a><span data-ttu-id="77eee-2097">Az.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="77eee-2097">Az.RecoveryServices</span></span>

* <span data-ttu-id="77eee-2098">Azure ファイル共有の復元操作にクライアント側の検証を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2098">Added client side validations for Azure File Share restore operations.</span></span>
* <span data-ttu-id="77eee-2099">AFS 復元について storageAccountName および storageAccountResourceGroupName を省略可能にしました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2099">Made storageAccountName and storageAccountResourceGroupName optional for afs restore.</span></span>

### <a name="azresources"></a><span data-ttu-id="77eee-2100">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-2100">Az.Resources</span></span>

* <span data-ttu-id="77eee-2101">https://github.com/Azure/azure-powershell/issues/7679 を修正しました </span><span class="sxs-lookup"><span data-stu-id="77eee-2101">Fix for https://github.com/Azure/azure-powershell/issues/7679</span></span>
    - <span data-ttu-id="77eee-2102">従来の管理者を要求するときにサブスクリプションのスコープを指定する場合、サブスクリプションのスコープを使用するように Get-AzureRmRoleAssignment を更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2102">Update Get-AzureRmRoleAssignment to use the subscription scope if it is provided when requesting classic administrators.</span></span>

### <a name="azsql"></a><span data-ttu-id="77eee-2103">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-2103">Az.Sql</span></span>

* <span data-ttu-id="77eee-2104">AzureRM から Az に切り替えるための軽微な変更</span><span class="sxs-lookup"><span data-stu-id="77eee-2104">Minor changes for upcoming AzureRM to Az transition</span></span>
* <span data-ttu-id="77eee-2105">.Net Core と合わせた Get-AzureRmSqlDatabaseVulnerabilityAssessment の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2105">Fixed issue with using Get-AzureRmSqlDatabaseVulnerabilityAssessment with DotNet core</span></span>
* <span data-ttu-id="77eee-2106">SQL 監査コマンドレットに関連するヘルプ メッセージのドキュメントを変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2106">Modified documentation of help messages related to SQL Auditing cmdlets.</span></span>

### <a name="azstorage"></a><span data-ttu-id="77eee-2107">Az.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-2107">Az.Storage</span></span>

* <span data-ttu-id="77eee-2108">New-AzureRmStorageAccount に -EnableHierarchicalNamespace を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2108">Add -EnableHierarchicalNamespace to New-AzureRmStorageAccount</span></span>
* <span data-ttu-id="77eee-2109">-DestContext を入力しないときに、ファイル コピーのコマンドレットで移行先のソース コンテキストを再利用できない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2109">Fix issue that Copy File cmdlet can't reuse source context in destination when not input -DestContext</span></span>
    - <span data-ttu-id="77eee-2110">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="77eee-2110">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="77eee-2111">静的な Web サイトの構成のサポート</span><span class="sxs-lookup"><span data-stu-id="77eee-2111">Support Static Website configuration</span></span>
    - <span data-ttu-id="77eee-2112">Enable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="77eee-2112">Enable-AzureStorageStaticWebsite</span></span>
    - <span data-ttu-id="77eee-2113">Disable-AzureStorageStaticWebsite</span><span class="sxs-lookup"><span data-stu-id="77eee-2113">Disable-AzureStorageStaticWebsite</span></span>

### <a name="azwebsites"></a><span data-ttu-id="77eee-2114">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-2114">Az.Websites</span></span>

* <span data-ttu-id="77eee-2115">Set-AzureRmWebApp と Set-AzureRmWebAppSlot</span><span class="sxs-lookup"><span data-stu-id="77eee-2115">Set-AzureRmWebApp and Set-AzureRmWebAppSlot</span></span>
    - <span data-ttu-id="77eee-2116">Windows および Linux のコンテナー アプリでマウントされる Azure Storage のパスを指定するために、新しいパラメーター (-AzureStoragePath) を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2116">New parameter (-AzureStoragePath) added to specify Azure Storage paths to be mounted in Windows and Linux container apps.</span></span> <span data-ttu-id="77eee-2117">Azure Storage のパスを設定するために、パラメーターとして新しい New-AzureRmWebAppAzureStoragePath コマンドレットの出力を使用します</span><span class="sxs-lookup"><span data-stu-id="77eee-2117">Use the output of the new cmdlet New-AzureRmWebAppAzureStoragePath as a parameter to set the Azure Storage paths.</span></span>

## <a name="061---november-2018"></a><span data-ttu-id="77eee-2118">0.6.1 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2118">0.6.1 - November 2018</span></span>

### <a name="azapimanagement"></a><span data-ttu-id="77eee-2119">Az.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="77eee-2119">Az.ApiManagement</span></span>
* <span data-ttu-id="77eee-2120">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2120">Update dependencies for type mapping issue</span></span>

### <a name="azautomation"></a><span data-ttu-id="77eee-2121">Az.Automation</span><span class="sxs-lookup"><span data-stu-id="77eee-2121">Az.Automation</span></span>
* <span data-ttu-id="77eee-2122">Swagger ベースの Azure Automation コマンドレット</span><span class="sxs-lookup"><span data-stu-id="77eee-2122">Swagger based Azure Automation cmdlets</span></span>
* <span data-ttu-id="77eee-2123">Update Management コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2123">Added Update Management cmdlets</span></span>
* <span data-ttu-id="77eee-2124">ソース管理コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2124">Added Source Control cmdlets</span></span>
* <span data-ttu-id="77eee-2125">Remove-AzureRmAutomationHybridWorkerGroup コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2125">Added Remove-AzureRmAutomationHybridWorkerGroup cmdlet</span></span>
* <span data-ttu-id="77eee-2126">DSC Register Node コマンドを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2126">Fixed the DSC Register Node command</span></span>

### <a name="azcompute"></a><span data-ttu-id="77eee-2127">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-2127">Az.Compute</span></span>
* <span data-ttu-id="77eee-2128">SystemAssigned ID の ID の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2128">Fixed identity issue for SystemAssigned identity</span></span>
* <span data-ttu-id="77eee-2129">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2129">Update dependencies for type mapping issue</span></span>

### <a name="azcontainerinstance"></a><span data-ttu-id="77eee-2130">Az.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-2130">Az.ContainerInstance</span></span>
* <span data-ttu-id="77eee-2131">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2131">Update dependencies for type mapping issue</span></span>

### <a name="azmarketplaceordering"></a><span data-ttu-id="77eee-2132">Az.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="77eee-2132">Az.MarketplaceOrdering</span></span>
* <span data-ttu-id="77eee-2133">marketplace コマンドレットの例の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2133">update the examples description for marketplace cmdlets</span></span>

### <a name="aznetwork"></a><span data-ttu-id="77eee-2134">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-2134">Az.Network</span></span>
* <span data-ttu-id="77eee-2135">New-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayCustomError、Get-AzureRmApplicationGatewayCustomError、Set-AzureRmApplicationGatewayCustomError、Remove-AzureRmApplicationGatewayCustomError、Add-AzureRmApplicationGatewayHttpListenerCustomError、Get-AzureRmApplicationGatewayHttpListenerCustomError、Set-AzureRmApplicationGatewayHttpListenerCustomError、Remove-AzureRmApplicationGatewayHttpListenerCustomError の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2135">Added cmdlet New-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayCustomError, Get-AzureRmApplicationGatewayCustomError, Set-AzureRmApplicationGatewayCustomError, Remove-AzureRmApplicationGatewayCustomError, Add-AzureRmApplicationGatewayHttpListenerCustomError, Get-AzureRmApplicationGatewayHttpListenerCustomError, Set-AzureRmApplicationGatewayHttpListenerCustomError, Remove-AzureRmApplicationGatewayHttpListenerCustomError</span></span>
* <span data-ttu-id="77eee-2136">サポートされている AzureFirewall ネットワーク プロトコルに ICMP を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2136">Added ICMP back to supported AzureFirewall Network Protocols</span></span>
* <span data-ttu-id="77eee-2137">Test-AzureRmNetworkWatcherConnectivity コマンドレットを更新し、宛先 ID、アドレス、およびポートの検証を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2137">Update cmdlet Test-AzureRmNetworkWatcherConnectivity, add validation on destination id, address and port.</span></span>
* <span data-ttu-id="77eee-2138">VirtualNetwork マップのメモリ使用量に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2138">Fix issues with memory usage in VirtualNetwork map</span></span>

### <a name="azrecoveryservicesbackup"></a><span data-ttu-id="77eee-2139">Az.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="77eee-2139">Az.RecoveryServices.Backup</span></span>
* <span data-ttu-id="77eee-2140">保護されたファイル共有のポリシーの変更を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2140">Fix for modifying policy for a protected file share.</span></span>
* <span data-ttu-id="77eee-2141">ポリシーのタイムゾーンを大文字に変換しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2141">Converted policy timezone to uppercase.</span></span>

### <a name="azrecoveryservicessiterecovery"></a><span data-ttu-id="77eee-2142">Az.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="77eee-2142">Az.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="77eee-2143">New-AzureRmRecoveryServicesAsrProtectableItem の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2143">Corrected example in New-AzureRmRecoveryServicesAsrProtectableItem</span></span>
* <span data-ttu-id="77eee-2144">型マッピングの問題に対応するために依存関係を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2144">Update dependencies for type mapping issue</span></span>

### <a name="azrelay"></a><span data-ttu-id="77eee-2145">Az.Relay</span><span class="sxs-lookup"><span data-stu-id="77eee-2145">Az.Relay</span></span>
* <span data-ttu-id="77eee-2146">New-AzureRmRelayKey コマンドレットに省略可能なパラメーターである -KeyValue を追加しました。これにより、ユーザーは KeyValue を指定できるようになります</span><span class="sxs-lookup"><span data-stu-id="77eee-2146">Added optional Parameter -KeyValue to New-AzureRmRelayKey cmdlet, which enables user to provide KeyValue.</span></span>

### <a name="azresources"></a><span data-ttu-id="77eee-2147">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-2147">Az.Resources</span></span>
* <span data-ttu-id="77eee-2148">`New-AzureRmPolicyAssignment` および `Set-AzureRmPolicyAssignment` のリソース ID 関連パラメーターに関するヘルプ ドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2148">Update help documentation for resource identity related parameters in `New-AzureRmPolicyAssignment` and `Set-AzureRmPolicyAssignment`</span></span>
* <span data-ttu-id="77eee-2149">-Metadata を使用する New-AzureRmPolicyDefinition の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2149">Add an example for New-AzureRmPolicyDefinition that uses -Metadata</span></span>
* <span data-ttu-id="77eee-2150">NetStandard のタグ キーで大文字小文字を保持できるように修正しました: #7678 #7703</span><span class="sxs-lookup"><span data-stu-id="77eee-2150">Fix to allow case preservation in Tag keys in NetStandard: #7678 #7703</span></span>

### <a name="azservicefabric"></a><span data-ttu-id="77eee-2151">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-2151">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-2152">今後の破壊的変更に備えて、非推奨を示すメッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2152">Add deprecation messages for upcoming breaking changes</span></span>

### <a name="azsql"></a><span data-ttu-id="77eee-2153">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-2153">Az.Sql</span></span>
* <span data-ttu-id="77eee-2154">Azure SQL Database Managed Instance と Azure SQL Managed Database に CRUD 操作用の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2154">Added new cmdlets for CRUD operations on Azure Sql Database Managed Instance and Azure Sql Managed Database</span></span>
    - <span data-ttu-id="77eee-2155">Get-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-2155">Get-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="77eee-2156">New-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-2156">New-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="77eee-2157">Set-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-2157">Set-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="77eee-2158">Remove-AzureRmSqlInstance</span><span class="sxs-lookup"><span data-stu-id="77eee-2158">Remove-AzureRmSqlInstance</span></span>
    - <span data-ttu-id="77eee-2159">Get-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="77eee-2159">Get-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="77eee-2160">New-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="77eee-2160">New-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="77eee-2161">Restore-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="77eee-2161">Restore-AzureRmSqlInstanceDatabase</span></span>
    - <span data-ttu-id="77eee-2162">Remove-AzureRmSqlInstanceDatabase</span><span class="sxs-lookup"><span data-stu-id="77eee-2162">Remove-AzureRmSqlInstanceDatabase</span></span>
* <span data-ttu-id="77eee-2163">サーバーまたはデータベース上での拡張監査ポリシー管理を有効にしました</span><span class="sxs-lookup"><span data-stu-id="77eee-2163">Enabled Extended Auditing Policy management on a server or a database.</span></span>
    - <span data-ttu-id="77eee-2164">監査ログのフィルター処理を有効にするために、新しいパラメーター (PredicateExpression) を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2164">New parameter (PredicateExpression) was added to enable filtering of audit logs.</span></span>
    - <span data-ttu-id="77eee-2165">レガシ クライアントの代わりに SQL クライアントを使用するようにコマンドレットを変更しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2165">Cmdlets were modified to use SQL clients instead of Legacy clients.</span></span>
    - <span data-ttu-id="77eee-2166">Set-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="77eee-2166">Set-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="77eee-2167">Get-AzureRmSqlServerAuditing</span><span class="sxs-lookup"><span data-stu-id="77eee-2167">Get-AzureRmSqlServerAuditing.</span></span>
    - <span data-ttu-id="77eee-2168">Set-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="77eee-2168">Set-AzureRmSqlDatabaseAuditing.</span></span>
    - <span data-ttu-id="77eee-2169">Get-AzureRmSqlDatabaseAuditing</span><span class="sxs-lookup"><span data-stu-id="77eee-2169">Get-AzureRmSqlDatabaseAuditing.</span></span>
* <span data-ttu-id="77eee-2170">ストレージ アカウント名パラメーターが設定された Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings の使用に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2170">Fixed issue with using Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings with storage account name parameter set</span></span>

## <a name="050---november-2018"></a><span data-ttu-id="77eee-2171">0.5.0 - 2018 年 11 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2171">0.5.0 - November 2018</span></span>
#### <a name="general"></a><span data-ttu-id="77eee-2172">全般</span><span class="sxs-lookup"><span data-stu-id="77eee-2172">General</span></span>
* <span data-ttu-id="77eee-2173">リソースの入力候補を多くの核となるコマンドレットに追加しました - コマンドレットを対話的に呼び出すときに、既存のリソース名を使ってタブ移動できるようになります</span><span class="sxs-lookup"><span data-stu-id="77eee-2173">Added Resource Completers to many core cmdlets - these alloow you to tab through existing resource names when invoking cmdlets interactively</span></span>

#### <a name="azprofile"></a><span data-ttu-id="77eee-2174">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="77eee-2174">Az.Profile</span></span>
* <span data-ttu-id="77eee-2175">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2175">Update common code to use latest version of ClientRuntime</span></span>
* <span data-ttu-id="77eee-2176">Connect-AzAccount コマンドレットのパラメーター TenantId の名前を Tenant に変更し、TenantId の別名を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2176">Rename param TenantId in cmdlet Connect-AzAccount to Tenant and add an alias for TenantId</span></span>
* <span data-ttu-id="77eee-2177">Connect-AzAccount の TenantId の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2177">Updated TenantId description for Connect-AzAccount</span></span>
* <span data-ttu-id="77eee-2178">テナントのドメインを指定した場合の、失敗したログインのエラー メッセージを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2178">Fix error message for failed login when providing tenant domain</span></span>
    - https://github.com/Azure/azure-powershell/issues/6936
* <span data-ttu-id="77eee-2179">テナント内にサブスクリプションを持たないアカウントでコンテキスト名の競合が発生する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2179">Fix issue with context name clashing for accounts with no subscriptions in tenant</span></span>
    - https://github.com/Azure/azure-powershell/issues/7453
* <span data-ttu-id="77eee-2180">MSI を使用した場合の、DataLake エンドポイントに関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2180">Fix issue with DataLake endpoints when using MSI</span></span>
    - https://github.com/Azure/azure-powershell/issues/7462
* <span data-ttu-id="77eee-2181">接続されていない場合に "Disconnect-AzAccount" でエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2181">Fix issue where 'Disconnect-AzAccount' would throw if not connected</span></span>
    - https://github.com/Azure/azure-powershell/issues/7167

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-2182">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-2182">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-2183">Get-AzCognitiveServicesAccountSkus 操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2183">Add Get-AzCognitiveServicesAccountSkus operation.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-2184">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-2184">Az.Compute</span></span>
* <span data-ttu-id="77eee-2185">Add-AzVmssVMDataDisk および Remove-AzVmssVMDataDisk コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2185">Add Add-AzVmssVMDataDisk and Remove-AzVmssVMDataDisk cmdlets</span></span>
* <span data-ttu-id="77eee-2186">Get-AzVMImage では AutomaticOSUpgradeProperties が表示されます</span><span class="sxs-lookup"><span data-stu-id="77eee-2186">Get-AzVMImage shows AutomaticOSUpgradeProperties</span></span>
* <span data-ttu-id="77eee-2187">SetAzVMChefExtension の -BootstrapOptions および -JsonAttribute オプション値は、JSON 形式で設定されない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2187">Fixed SetAzVMChefExtension -BootstrapOptions and -JsonAttribute option values are not setting in json format.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-2188">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-2188">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-2189">DataLake パッケージは 1.1.10 に更新されました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2189">Update the DataLake package to 1.1.10.</span></span>
* <span data-ttu-id="77eee-2190">マルチスレッド操作に既定のコンカレンシーを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2190">Add default Concurrency to multithreaded operations.</span></span>

#### <a name="azinsights"></a><span data-ttu-id="77eee-2191">Az.Insights</span><span class="sxs-lookup"><span data-stu-id="77eee-2191">Az.Insights</span></span>
* <span data-ttu-id="77eee-2192">問題 #7267 (自動スケーリングの領域) を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2192">Fixed issue #7267 (Autoscale area)</span></span>
    - <span data-ttu-id="77eee-2193">新しい自動スケーリング ルールを作成すると、列挙されたパラメーターが正しく設定されない (常に既定値に設定される) 問題。</span><span class="sxs-lookup"><span data-stu-id="77eee-2193">Issues with creating a new autoscale rule not properly setting enumerated parameters (would always set them to the default value).</span></span>
* <span data-ttu-id="77eee-2194">Set-AzDiagnosticSetting で、設定の作成時にカテゴリを明示的に指定する必要がある問題 #7513 [Insights] を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2194">Fixed issue #7513 [Insights] Set-AzDiagnosticSetting requires explicit specification of categories during creation of setting</span></span>
    - <span data-ttu-id="77eee-2195">このコマンドレットでは、作成時にカテゴリの明示を有効にする必要がなくなりました。つまり、ドキュメントに記載されたとおりに動作します</span><span class="sxs-lookup"><span data-stu-id="77eee-2195">Now the cmdlet does not require explicit indication of the categories to enable during creation, i.e. it works as it is documented</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-2196">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-2196">Az.Network</span></span>
* <span data-ttu-id="77eee-2197">次のコマンドレットの PeeringType パラメーターを必須パラメーターに変更しました:</span><span class="sxs-lookup"><span data-stu-id="77eee-2197">Changed PeeringType to be a mandatory parameter for the following cmdlets:-</span></span>
    - <span data-ttu-id="77eee-2198">Get-AzExpressRouteCircuitRouteTable</span><span class="sxs-lookup"><span data-stu-id="77eee-2198">Get-AzExpressRouteCircuitRouteTable</span></span>
    - <span data-ttu-id="77eee-2199">Get-AzExpressRouteCircuitARPTable</span><span class="sxs-lookup"><span data-stu-id="77eee-2199">Get-AzExpressRouteCircuitARPTable</span></span>
    - <span data-ttu-id="77eee-2200">Get-AzExpressRouteCircuitRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="77eee-2200">Get-AzExpressRouteCircuitRouteTableSummary</span></span>
    - <span data-ttu-id="77eee-2201">Get-AzExpressRouteCrossConnectionArpTable</span><span class="sxs-lookup"><span data-stu-id="77eee-2201">Get-AzExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="77eee-2202">Get-AzExpressRouteCrossConnectionRouteTable</span><span class="sxs-lookup"><span data-stu-id="77eee-2202">Get-AzExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="77eee-2203">Get-AzExpressRouteCrossConnectionRouteTableSummary</span><span class="sxs-lookup"><span data-stu-id="77eee-2203">Get-AzExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azpolicyinsights"></a><span data-ttu-id="77eee-2204">Az.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="77eee-2204">Az.PolicyInsights</span></span>
* <span data-ttu-id="77eee-2205">ポリシー修復コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2205">Added policy remediation cmdlets</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-2206">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-2206">Az.Resources</span></span>
* <span data-ttu-id="77eee-2207">https://github.com/Azure/azure-powershell/issues/7402 を修正しました </span><span class="sxs-lookup"><span data-stu-id="77eee-2207">Fix for https://github.com/Azure/azure-powershell/issues/7402</span></span>
    - <span data-ttu-id="77eee-2208">"Get-AzResource" の "-ResourceId" パラメーターを使用してリソースを一覧表示できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2208">Allow listing resources using the '-ResourceId' parameter for 'Get-AzResource'</span></span>

#### <a name="azservicebus"></a><span data-ttu-id="77eee-2209">Az.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="77eee-2209">Az.ServiceBus</span></span>
* <span data-ttu-id="77eee-2210">移行の状態の把握に役立つ MigrationState 読み取り専用プロパティを、PSServiceBusMigrationConfigurationAttributes に追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2210">Added MigrationState read-only property to PSServiceBusMigrationConfigurationAttributes which will help to know the Migration state.</span></span>

#### <a name="azservicefabric"></a><span data-ttu-id="77eee-2211">Az.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="77eee-2211">Az.ServiceFabric</span></span>
* <span data-ttu-id="77eee-2212">Linux VMSS への証明書の追加を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2212">Fix add certificate to Linux Vmss.</span></span>
* <span data-ttu-id="77eee-2213">"Add-AzServiceFabricClusterCertificate" を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2213">Fix 'Add-AzServiceFabricClusterCertificate'</span></span>
    - <span data-ttu-id="77eee-2214">新しい証明書の適切な拇印が使用されます (Azure/service-fabric-issues#932)。</span><span class="sxs-lookup"><span data-stu-id="77eee-2214">Using correct thumbprint from new certificate (Azure/service-fabric-issues#932).</span></span>
    - <span data-ttu-id="77eee-2215">例外が正しく表示されます (Azure/service-fabric-issues#1054)。</span><span class="sxs-lookup"><span data-stu-id="77eee-2215">Display exception correctly (Azure/service-fabric-issues#1054).</span></span>
* <span data-ttu-id="77eee-2216">VMSS CreateOrUpdate 操作を開始する前にクラスター構成が更新されるように、"Update-AzServiceFabricDurability" を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2216">Fix 'Update-AzServiceFabricDurability' to update cluster configuration before starting Vmss CreateOrUpdate operation.</span></span>

## <a name="040---october-2018"></a><span data-ttu-id="77eee-2217">0.4.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2217">0.4.0 - October 2018</span></span>
#### <a name="azprofile"></a><span data-ttu-id="77eee-2218">Az.Profile</span><span class="sxs-lookup"><span data-stu-id="77eee-2218">Az.Profile</span></span>
* <span data-ttu-id="77eee-2219">CloudShell での Get-AzSubscription に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2219">Fix issue with Get-AzSubscription in CloudShell</span></span>
* <span data-ttu-id="77eee-2220">最新バージョンの ClientRuntime を使用するように共通コードを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2220">Update common code to use latest version of ClientRuntime</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-2221">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-2221">Az.Compute</span></span>
* <span data-ttu-id="77eee-2222">"New-AzVm" の単純なパラメーター セットの使用時に高速ネットワークが有効になる VM サイズのホワイトリストに新しいサイズを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2222">Added new sizes to the whitelist of VM sizes for which accelerated networking will be turned on when using the simple param set for 'New-AzVm'</span></span>
* <span data-ttu-id="77eee-2223">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2223">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azdatalakestore"></a><span data-ttu-id="77eee-2224">Az.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="77eee-2224">Az.DataLakeStore</span></span>
* <span data-ttu-id="77eee-2225">仮想ネットワーク規則のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2225">Adding support for Virtual Network Rules</span></span>
    - <span data-ttu-id="77eee-2226">Get-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを取得または一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="77eee-2226">Get-AzDataLakeStoreVirtualNetworkRule: Gets or Lists Azure Data Lake Store virtual network rule.</span></span>
    - <span data-ttu-id="77eee-2227">Add-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウントに仮想ネットワーク ルールを追加します。</span><span class="sxs-lookup"><span data-stu-id="77eee-2227">Add-AzDataLakeStoreVirtualNetworkRule: Adds a virtual network rule to the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="77eee-2228">Set-AzDataLakeStoreVirtualNetworkRule:指定された Data Lake Store アカウント内の指定された仮想ネットワーク ルールを変更します。</span><span class="sxs-lookup"><span data-stu-id="77eee-2228">Set-AzDataLakeStoreVirtualNetworkRule: Modifies the specified virtual network rule in the specified Data Lake Store account.</span></span>
    - <span data-ttu-id="77eee-2229">Remove-AzDataLakeStoreVirtualNetworkRule:Azure Data Lake Store の仮想ネットワーク ルールを削除します。</span><span class="sxs-lookup"><span data-stu-id="77eee-2229">Remove-AzDataLakeStoreVirtualNetworkRule: Deletes an Azure Data Lake Store virtual network rule.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-2230">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-2230">Az.Network</span></span>
* <span data-ttu-id="77eee-2231">プロトコル値をバックエンドに渡すように、Test-AzNetworkWatcherConnectivity コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2231">Update cmdlet Test-AzNetworkWatcherConnectivity, pass the protocol value to backend.</span></span>
* <span data-ttu-id="77eee-2232">ResourceName 引数の入力候補をすべてのコマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2232">Added ResourceName argument completer to all cmdlets.</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-2233">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-2233">Az.Resources</span></span>
* <span data-ttu-id="77eee-2234">シナリオに意味のある例外を追加することで、(既定のプロファイルにサブスクリプションがなく、スコープが指定されていないときに) Get-AzRoleDefinition が理解できない例外をスローする問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2234">Fix isssue where Get-AzRoleDefinition throws an unintelligible exception (when the default profile has no subscription in it and no scope is specified) by adding a meaningful exception in the scenario.</span></span> <span data-ttu-id="77eee-2235">また、既定のパラメーター セットを "RoleDefinitionNameParameterSet" に設定しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2235">Also set the default param set to 'RoleDefinitionNameParameterSet'.</span></span>

## <a name="030---october-2018"></a><span data-ttu-id="77eee-2236">0.3.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2236">0.3.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="77eee-2237">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="77eee-2237">Azure.Storage</span></span>
* <span data-ttu-id="77eee-2238">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2238">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="77eee-2239">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="77eee-2239">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="77eee-2240">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="77eee-2240">Start-AzureStorageFileCopy</span></span>
* <span data-ttu-id="77eee-2241">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2241">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="77eee-2242">Get-AzStorageUsage</span><span class="sxs-lookup"><span data-stu-id="77eee-2242">Get-AzStorageUsage</span></span>

#### <a name="azcognitiveservices"></a><span data-ttu-id="77eee-2243">Az.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="77eee-2243">Az.CognitiveServices</span></span>
* <span data-ttu-id="77eee-2244">既存のアカウントなしでの Get-AzCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2244">Support Get-AzCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azcompute"></a><span data-ttu-id="77eee-2245">Az.Compute</span><span class="sxs-lookup"><span data-stu-id="77eee-2245">Az.Compute</span></span>
* <span data-ttu-id="77eee-2246">必要に応じて 50 を超える結果が返されるように Get-AzVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2246">Fix Get-AzVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="77eee-2247">"SimpleParameterSet" の例を New-AzVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2247">Added an example of the 'SimpleParameterSet' to New-AzVmss cmdlet help.</span></span>
* <span data-ttu-id="77eee-2248">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2248">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azdatafactoryv2"></a><span data-ttu-id="77eee-2249">Az.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="77eee-2249">Az.DataFactoryV2</span></span>
* <span data-ttu-id="77eee-2250">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2250">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="aznetwork"></a><span data-ttu-id="77eee-2251">Az.Network</span><span class="sxs-lookup"><span data-stu-id="77eee-2251">Az.Network</span></span>
* <span data-ttu-id="77eee-2252">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="77eee-2252">Added NetworkProfile functionality.</span></span> <span data-ttu-id="77eee-2253">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="77eee-2253">new cmdlets added</span></span>
    - <span data-ttu-id="77eee-2254">Get-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="77eee-2254">Get-AzNetworkProfile</span></span>
    - <span data-ttu-id="77eee-2255">New-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="77eee-2255">New-AzNetworkProfile</span></span>
    - <span data-ttu-id="77eee-2256">Remove-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="77eee-2256">Remove-AzNetworkProfile</span></span>
    - <span data-ttu-id="77eee-2257">Set-AzNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="77eee-2257">Set-AzNetworkProfile</span></span>
    - <span data-ttu-id="77eee-2258">New-AzContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-2258">New-AzContainerNicConfig</span></span>
    - <span data-ttu-id="77eee-2259">New-AzContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="77eee-2259">New-AzContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="77eee-2260">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2260">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="77eee-2261">New-AzVirtualNetworkTap、Get-AzVirtualNetworkTap、Set-AzVirtualNetworkTap、Remove-AzVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2261">Added cmdlet New-AzVirtualNetworkTap, Get-AzVirtualNetworkTap, Set-AzVirtualNetworkTap, Remove-AzVirtualNetworkTap</span></span>
* <span data-ttu-id="77eee-2262">Set-AzNEtworkInterfaceTapConfig、Get-AzNEtworkInterfaceTapConfig、Remove-AzNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2262">Added cmdlet Set-AzNEtworkInterfaceTapConfig, Get-AzNEtworkInterfaceTapConfig, Remove-AzNEtworkInterfaceTapConfig</span></span>

#### <a name="azrediscache"></a><span data-ttu-id="77eee-2263">Az.RedisCache</span><span class="sxs-lookup"><span data-stu-id="77eee-2263">Az.RedisCache</span></span>
* <span data-ttu-id="77eee-2264">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="77eee-2264">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="77eee-2265">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2265">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azresources"></a><span data-ttu-id="77eee-2266">Az.Resources</span><span class="sxs-lookup"><span data-stu-id="77eee-2266">Az.Resources</span></span>
* <span data-ttu-id="77eee-2267">欠落していた -Mode パラメーターを Set-AzPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2267">Add missing -Mode parameter to Set-AzPolicyDefinition</span></span>
* <span data-ttu-id="77eee-2268">配信元にユーザーが含まれる操作について Get-AzProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2268">Fix Get-AzProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azsql"></a><span data-ttu-id="77eee-2269">Az.Sql</span><span class="sxs-lookup"><span data-stu-id="77eee-2269">Az.Sql</span></span>
* <span data-ttu-id="77eee-2270">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="77eee-2270">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azwebsites"></a><span data-ttu-id="77eee-2271">Az.Websites</span><span class="sxs-lookup"><span data-stu-id="77eee-2271">Az.Websites</span></span>
* <span data-ttu-id="77eee-2272">新しいコマンドレット: Get-AzWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="77eee-2272">New Cmdlet Get-AzWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="77eee-2273">新しいコマンドレット: New-AzWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="77eee-2273">New Cmdlets New-AzWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="020---september-2018"></a><span data-ttu-id="77eee-2274">0.2.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="77eee-2274">0.2.0 - September 2018</span></span>
 <span data-ttu-id="77eee-2275">最初のリリース</span><span class="sxs-lookup"><span data-stu-id="77eee-2275">Initial Release</span></span>
