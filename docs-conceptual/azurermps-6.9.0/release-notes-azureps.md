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
ms.openlocfilehash: 3cb71087a61a0fcd06c014394e8f9e5654d4c1a8
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2018
ms.locfileid: "47179005"
---
# <a name="release-notes"></a><span data-ttu-id="18375-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="18375-103">Release notes</span></span>

<span data-ttu-id="18375-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="18375-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="690---september-2018"></a><span data-ttu-id="18375-105">6.9.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="18375-105">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="18375-106">全般</span><span class="sxs-lookup"><span data-stu-id="18375-106">General</span></span>
* <span data-ttu-id="18375-107">AzureRM.SignalR が AzureRM ロールアップ モジュールに追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-107">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="18375-108">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-108">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-109">ストレージの一般的なコードに対する軽微な変更</span><span class="sxs-lookup"><span data-stu-id="18375-109">Minor changes to the storage common code</span></span>
* <span data-ttu-id="18375-110">完全なパラメーター型を含めるようにヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-110">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="18375-111">ServicePrincipalCertificateWithSubscriptionId パラメーター セットの -ServicePrincipal を "任意" に変更しました</span><span class="sxs-lookup"><span data-stu-id="18375-111">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="18375-112">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-112">Azure.Storage</span></span>
* <span data-ttu-id="18375-113">OAuth でのストレージ コンテキストの作成がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="18375-113">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="18375-114">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="18375-114">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="18375-115">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="18375-115">AzureRM.Cdn</span></span>
* <span data-ttu-id="18375-116">CDN 価格 SKU に Standard_Microsoft を追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-116">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="18375-117">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-117">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-118">Keyvault および Storage への依存関係を一般的な依存関係に移動しました</span><span class="sxs-lookup"><span data-stu-id="18375-118">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="18375-119">より多くの仮想マシンのサイズのサポートを AEM コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-119">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="18375-120">PublicIPPrefix パラメーターを New-AzureRmVmssIpConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-120">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="18375-121">ResourceId パラメーターを Invoke-AzureRmVMRunCommand コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-121">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="18375-122">Invoke-AzureRmVmssVMRunCommand コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-122">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="18375-123">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="18375-123">AzureRM.Dns</span></span>
* <span data-ttu-id="18375-124">DNS レコード作成中のエイリアス レコードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-124">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="18375-125">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="18375-125">AzureRM.Insights</span></span>
* <span data-ttu-id="18375-126">#6833 および #7102 の問題を修正しました (診断設定領域)</span><span class="sxs-lookup"><span data-stu-id="18375-126">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="18375-127">診断設定の作成および表示/取得中の既定の名前 ("service") に関する問題</span><span class="sxs-lookup"><span data-stu-id="18375-127">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="18375-128">カテゴリでの診断設定の作成に関する問題</span><span class="sxs-lookup"><span data-stu-id="18375-128">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="18375-129">メトリック時間グレイン パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-129">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="18375-130">Timegrains パラメーターは引き続き利用できますが (これは破壊的変更ではありません)、PT1M のみが有効であるため、バックエンドでは無視されます</span><span class="sxs-lookup"><span data-stu-id="18375-130">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-131">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-131">AzureRM.Network</span></span>
* <span data-ttu-id="18375-132">LoadBalancer コマンドレットへの変更</span><span class="sxs-lookup"><span data-stu-id="18375-132">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="18375-133">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes パラメーター、EnableFloatingIp パラメーター、EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-133">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="18375-134">LoadBalancerInboundNatRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-134">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="18375-135">LoadBalancerRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-135">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="18375-136">LoadBalancerProbeConfig: Protocol パラメーターの "HTTPS" 値のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-136">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="18375-137">新しい LoadBalancer のサブリソース OutboundRule について新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-137">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="18375-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="18375-138">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="18375-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="18375-139">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="18375-140">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="18375-140">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="18375-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="18375-141">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="18375-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="18375-142">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="18375-143">PSNetworkInterface の新しい HostedWorkloads プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-143">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="18375-144">ARM 経由の Azure Firewall 機能のために新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-144">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="18375-145">Get-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-145">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="18375-146">Set-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-146">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="18375-147">New-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-147">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="18375-148">Remove-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-148">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="18375-149">New-AzureRmFirewallApplicationRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-149">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="18375-150">New-AzureRmFirewallApplicationRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-150">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="18375-151">New-AzureRmFirewallNatRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-151">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="18375-152">New-AzureRmFirewallNatRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-152">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="18375-153">New-AzureRmFirewallNetworkRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-153">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="18375-154">New-AzureRmFirewallNetworkRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-154">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="18375-155">Application Gateway での信頼されたルート証明書と自動スケーリング構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-155">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="18375-156">追加された新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="18375-156">New Cmdlets added:</span></span>
      - <span data-ttu-id="18375-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-157">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="18375-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-158">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="18375-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-159">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="18375-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-160">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="18375-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-161">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="18375-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-162">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="18375-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-163">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="18375-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-164">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="18375-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-165">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="18375-166">省略可能なパラメーターで更新されたコマンドレット -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-166">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="18375-167">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="18375-167">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="18375-168">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="18375-168">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="18375-169">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="18375-169">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="18375-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="18375-170">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="18375-171">省略可能なパラメーターで更新されたコマンドレット - AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-171">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="18375-172">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="18375-172">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="18375-173">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="18375-173">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="18375-174">インターフェイス エンドポイントのコマンドレット Get-AzureInterfaceEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-174">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="18375-175">サブネットでの複数のアドレス プレフィックスのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-175">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="18375-176">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="18375-176">Updated cmdlets:</span></span>
  - <span data-ttu-id="18375-177">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="18375-177">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="18375-178">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="18375-178">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="18375-179">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="18375-179">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="18375-180">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="18375-180">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="18375-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-181">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="18375-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="18375-182">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="18375-183">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="18375-183">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="18375-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="18375-184">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="18375-185">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-185">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="18375-186">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-186">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="18375-187">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-187">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="18375-188">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-188">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="18375-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-189">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="18375-190">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-190">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="18375-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-191">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="18375-192">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-192">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="18375-193">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-193">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="18375-194">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="18375-194">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="18375-195">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="18375-195">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="18375-196">サブネット委任のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-196">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="18375-197">New-AzureRmDelegation: 新しい委任を作成します。これはサブネットに追加できます</span><span class="sxs-lookup"><span data-stu-id="18375-197">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="18375-198">Remove-AzureRmDelegation: サブネットを受け取り、指定された委任の名前をそのサブネットから削除します</span><span class="sxs-lookup"><span data-stu-id="18375-198">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="18375-199">Add-AzureRmDelegation: サブネットを受け取り、指定されたサービス名を委任としてそのサブネットに追加します</span><span class="sxs-lookup"><span data-stu-id="18375-199">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="18375-200">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="18375-200">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="18375-201">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="18375-201">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="18375-202">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="18375-202">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="18375-203">管理対象のマネージド ディスクのサポート</span><span class="sxs-lookup"><span data-stu-id="18375-203">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="18375-204">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="18375-204">AzureRM.RedisCache</span></span>
* <span data-ttu-id="18375-205">Insights の依存関係を更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-205">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-206">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-206">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-207">New-AzureRmResourceGroupDeployment を新しい RollbackAction パラメーターで更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-207">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="18375-208">新しいパラメーターを使用して OnErrorDeployment のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-208">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="18375-209">ポリシー割り当てでマネージド ID をサポートします。</span><span class="sxs-lookup"><span data-stu-id="18375-209">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="18375-210">"New-AzureRmPolicyAssignment" を指定してポリシーを割り当てるとき、既定値を持つパラメーターが不要になりました</span><span class="sxs-lookup"><span data-stu-id="18375-210">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="18375-211">ポリシー エイリアスを取得するための新しい Get AzureRmPolicyAlias コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-211">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-212">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-212">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-213">問題 #7161 を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-213">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="18375-214">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="18375-214">AzureRM.SignalR</span></span>
* <span data-ttu-id="18375-215">SKU 名を Free_F1 および Standard_S1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-215">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="18375-216">バージョン フィールドを PSSignalRResource オブジェクトに、接続文字列を PSSignalRKeys オブジェクトに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-216">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="18375-217">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-217">AzureRM.Storage</span></span>
* <span data-ttu-id="18375-218">AzureRm.Storage での不変ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="18375-218">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="18375-219">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="18375-219">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="18375-220">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="18375-220">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="18375-221">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="18375-221">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="18375-222">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="18375-222">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="18375-223">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="18375-223">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="18375-224">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="18375-224">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="18375-225">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="18375-225">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="18375-226">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="18375-226">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="18375-227">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="18375-227">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="18375-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="18375-228">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="18375-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="18375-229">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="18375-230">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="18375-230">AzureRM.Websites</span></span>
* <span data-ttu-id="18375-231">Get-AzureRmDeletedWebApp と Restore-AzureRmDeletedWebApp の 2 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-231">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="18375-232">Windows コンテナーでの App Service プランの作成用に New-AzureRmAppServicePlan -HyperV スイッチが追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-232">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="18375-233">Windows コンテナー アプリを作成および管理用に、New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New パラメーター (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) が追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-233">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="18375-234">6.8.1 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="18375-234">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="18375-235">全般</span><span class="sxs-lookup"><span data-stu-id="18375-235">General</span></span>
* <span data-ttu-id="18375-236">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-236">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="18375-237">共通ランタイム アセンブリを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-237">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="18375-238">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="18375-238">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="18375-239">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-239">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="18375-240">修正された問題 https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="18375-240">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="18375-241">Import-AzureRmApiManagementApi コマンドレットおよび \*-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました</span><span class="sxs-lookup"><span data-stu-id="18375-241">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="18375-242">修正された問題 https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="18375-242">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="18375-243">CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="18375-243">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="18375-244">4.0.4-preview NuGet へのアップグレードによって修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-244">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="18375-245">修正された問題 https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="18375-245">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="18375-246">製品を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-246">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="18375-247">修正された問題 https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="18375-247">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="18375-248">API を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-248">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="18375-249">AzureMonitor ロガーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-249">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="18375-250">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-250">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-251">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-251">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="18375-252">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-252">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="18375-253">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-253">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="18375-254">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-254">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-255">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-255">AzureRM.Network</span></span>
* <span data-ttu-id="18375-256">コマンドレット出力の既定の表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="18375-256">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="18375-257">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="18375-257">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="18375-258">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-258">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="18375-259">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-259">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-260">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-260">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-261">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-261">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-262">修正された問題</span><span class="sxs-lookup"><span data-stu-id="18375-262">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="18375-263">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="18375-263">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="18375-264">複数値ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-264">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="18375-265">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="18375-265">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="18375-266">サブネット ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-266">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="18375-267">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="18375-267">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="18375-268">プロファイルでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-268">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="18375-269">プロファイルでの予期される状態コード範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-269">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="18375-270">エンドポイントでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-270">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="18375-271">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="18375-271">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="18375-272">全般</span><span class="sxs-lookup"><span data-stu-id="18375-272">General</span></span>
* <span data-ttu-id="18375-273">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-273">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="18375-274">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-274">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-275">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-275">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-276">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-276">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-277">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-277">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="18375-278">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-278">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="18375-279">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-279">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="18375-280">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="18375-280">AzureRM.IotHub</span></span>
* <span data-ttu-id="18375-281">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-281">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-282">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-282">AzureRM.Network</span></span>
* <span data-ttu-id="18375-283">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="18375-283">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="18375-284">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="18375-284">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="18375-285">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-285">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-286">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-286">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-287">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-287">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-288">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-288">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-289">問題の修正</span><span class="sxs-lookup"><span data-stu-id="18375-289">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="18375-290">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="18375-290">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="18375-291">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="18375-291">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="18375-292">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="18375-292">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="18375-293">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="18375-293">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="18375-294">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="18375-294">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="18375-295">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="18375-295">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="18375-296">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="18375-296">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="18375-297">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="18375-297">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="18375-298">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="18375-298">AzureRM.Websites</span></span>
* <span data-ttu-id="18375-299">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-299">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="18375-300">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="18375-300">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="18375-301">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-301">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-302">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-302">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="18375-303">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-303">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="18375-304">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-304">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="18375-305">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="18375-305">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="18375-306">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-306">Azure.Storage</span></span>
* <span data-ttu-id="18375-307">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="18375-307">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="18375-308">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="18375-308">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="18375-309">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="18375-309">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="18375-310">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-310">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="18375-311">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="18375-311">Azure.AnalysisServices</span></span>
* <span data-ttu-id="18375-312">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-312">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="18375-313">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="18375-313">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="18375-314">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-314">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="18375-315">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="18375-315">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="18375-316">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-316">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="18375-317">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="18375-317">AzureRM.Automation</span></span>
* <span data-ttu-id="18375-318">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-318">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="18375-319">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="18375-319">AzureRM.Backup</span></span>
* <span data-ttu-id="18375-320">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-320">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="18375-321">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="18375-321">AzureRM.Batch</span></span>
* <span data-ttu-id="18375-322">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-322">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="18375-323">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="18375-323">AzureRM.Billing</span></span>
* <span data-ttu-id="18375-324">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-324">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="18375-325">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="18375-325">AzureRM.Cdn</span></span>
* <span data-ttu-id="18375-326">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-326">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="18375-327">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="18375-327">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="18375-328">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-328">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-329">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-329">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-330">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-330">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="18375-331">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-331">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="18375-332">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="18375-332">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="18375-333">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-333">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="18375-334">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-334">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="18375-335">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="18375-335">AzureRM.Consumption</span></span>
* <span data-ttu-id="18375-336">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-336">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="18375-337">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="18375-337">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="18375-338">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-338">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="18375-339">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="18375-339">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="18375-340">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-340">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="18375-341">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="18375-341">AzureRM.DataFactories</span></span>
* <span data-ttu-id="18375-342">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-342">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="18375-343">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="18375-343">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="18375-344">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-344">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="18375-345">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="18375-345">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="18375-346">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-346">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="18375-347">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="18375-347">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="18375-348">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-348">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="18375-349">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-349">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="18375-350">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-350">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="18375-351">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-351">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="18375-352">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="18375-352">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="18375-353">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="18375-354">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="18375-354">AzureRM.Dns</span></span>
* <span data-ttu-id="18375-355">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="18375-356">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="18375-356">AzureRM.EventGrid</span></span>
* <span data-ttu-id="18375-357">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="18375-358">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="18375-358">AzureRM.EventHub</span></span>
* <span data-ttu-id="18375-359">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="18375-360">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="18375-360">AzureRM.HDInsight</span></span>
* <span data-ttu-id="18375-361">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="18375-362">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="18375-362">AzureRM.Insights</span></span>
* <span data-ttu-id="18375-363">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="18375-364">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="18375-364">AzureRM.IotHub</span></span>
* <span data-ttu-id="18375-365">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="18375-366">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="18375-366">AzureRM.KeyVault</span></span>
* <span data-ttu-id="18375-367">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="18375-368">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="18375-368">AzureRM.LogicApp</span></span>
* <span data-ttu-id="18375-369">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-369">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="18375-370">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="18375-370">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="18375-371">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-371">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="18375-372">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="18375-372">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="18375-373">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-373">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="18375-374">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="18375-374">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="18375-375">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="18375-376">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="18375-376">AzureRM.Media</span></span>
* <span data-ttu-id="18375-377">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-378">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-378">AzureRM.Network</span></span>
* <span data-ttu-id="18375-379">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-379">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="18375-380">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-380">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="18375-381">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-381">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="18375-382">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-382">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="18375-383">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-383">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="18375-384">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-384">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="18375-385">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="18375-385">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="18375-386">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="18375-386">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="18375-387">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="18375-387">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="18375-388">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-388">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="18375-389">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="18375-389">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="18375-390">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-390">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="18375-391">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="18375-391">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="18375-392">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="18375-393">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="18375-393">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="18375-394">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="18375-395">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="18375-395">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="18375-396">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="18375-397">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="18375-397">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="18375-398">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-398">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="18375-399">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="18375-399">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="18375-400">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-400">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="18375-401">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-401">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="18375-402">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-402">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="18375-403">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="18375-403">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="18375-404">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="18375-404">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="18375-405">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="18375-405">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="18375-406">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="18375-407">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="18375-407">AzureRM.RedisCache</span></span>
* <span data-ttu-id="18375-408">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="18375-409">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="18375-409">AzureRM.Relay</span></span>
* <span data-ttu-id="18375-410">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-411">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-411">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-412">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="18375-412">Support template deployment at subscription scope.</span></span> <span data-ttu-id="18375-413">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-413">Add new Cmdlets:</span></span>
    - <span data-ttu-id="18375-414">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="18375-414">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="18375-415">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="18375-415">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="18375-416">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="18375-416">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="18375-417">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="18375-417">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="18375-418">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="18375-418">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="18375-419">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="18375-419">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="18375-420">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="18375-420">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="18375-421">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-421">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="18375-422">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-422">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="18375-423">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-423">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="18375-424">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="18375-424">AzureRM.Scheduler</span></span>
* <span data-ttu-id="18375-425">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-425">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-426">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-426">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-427">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="18375-428">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="18375-428">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="18375-429">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="18375-430">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-430">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-431">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="18375-432">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-432">AzureRM.Storage</span></span>
* <span data-ttu-id="18375-433">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="18375-434">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="18375-434">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="18375-435">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="18375-436">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="18375-436">AzureRM.Tags</span></span>
* <span data-ttu-id="18375-437">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-437">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="18375-438">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="18375-438">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="18375-439">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-439">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="18375-440">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="18375-440">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="18375-441">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-441">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="18375-442">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="18375-442">AzureRM.Websites</span></span>
* <span data-ttu-id="18375-443">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-443">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="18375-444">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="18375-444">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="18375-445">全般</span><span class="sxs-lookup"><span data-stu-id="18375-445">General</span></span>
* <span data-ttu-id="18375-446">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-446">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="18375-447">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-447">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-448">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-448">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="18375-449">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-449">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="18375-450">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-450">Azure.Storage</span></span>
* <span data-ttu-id="18375-451">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-451">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="18375-452">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-452">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="18375-453">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="18375-453">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="18375-454">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="18375-454">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="18375-455">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-455">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="18375-456">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="18375-456">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="18375-457">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-457">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="18375-458">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="18375-458">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="18375-459">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="18375-459">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-460">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-460">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-461">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-461">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="18375-462">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-462">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="18375-463">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="18375-463">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="18375-464">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="18375-464">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="18375-465">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-465">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="18375-466">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-466">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="18375-467">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-467">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="18375-468">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-468">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="18375-469">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-469">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="18375-470">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-470">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="18375-471">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="18375-471">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="18375-472">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-472">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="18375-473">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="18375-473">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="18375-474">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-474">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="18375-475">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-475">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="18375-476">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="18375-476">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="18375-477">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-477">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="18375-478">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="18375-478">AzureRM.EventHub</span></span>
* <span data-ttu-id="18375-479">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-479">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="18375-480">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="18375-480">AzureRM.Insights</span></span>
* <span data-ttu-id="18375-481">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-481">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="18375-482">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="18375-482">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="18375-483">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="18375-483">AzureRM.KeyVault</span></span>
* <span data-ttu-id="18375-484">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-484">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-485">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-485">AzureRM.Network</span></span>
* <span data-ttu-id="18375-486">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-486">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-487">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-487">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-488">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-488">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="18375-489">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-489">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-490">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-490">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-491">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-491">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="18375-492">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-492">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="18375-493">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-493">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-494">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-494">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="18375-495">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="18375-495">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="18375-496">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-496">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="18375-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="18375-497">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="18375-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="18375-498">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="18375-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="18375-499">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="18375-500">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-500">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="18375-501">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-501">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="18375-502">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-502">AzureRM.Storage</span></span>
* <span data-ttu-id="18375-503">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-503">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="18375-504">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="18375-504">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="18375-505">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="18375-505">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="18375-506">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="18375-506">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="18375-507">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="18375-507">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="18375-508">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="18375-508">AzureRM.Tags</span></span>
* <span data-ttu-id="18375-509">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="18375-509">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="18375-510">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="18375-510">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="18375-511">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-511">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-512">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-512">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="18375-513">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-513">Azure.Storage</span></span>
* <span data-ttu-id="18375-514">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="18375-514">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="18375-515">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="18375-515">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="18375-516">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="18375-516">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="18375-517">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="18375-517">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="18375-518">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-518">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="18375-519">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="18375-519">AzureRM.Automation</span></span>
* <span data-ttu-id="18375-520">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-520">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-521">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-521">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-522">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-522">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="18375-523">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-523">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="18375-524">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-524">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="18375-525">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-525">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="18375-526">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-526">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="18375-527">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="18375-527">AzureRM.EventHub</span></span>
* <span data-ttu-id="18375-528">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-528">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="18375-529">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="18375-529">AzureRM.KeyVault</span></span>
* <span data-ttu-id="18375-530">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-530">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="18375-531">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="18375-531">AzureRM.LogicApp</span></span>
* <span data-ttu-id="18375-532">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-532">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-533">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-533">AzureRM.Network</span></span>
* <span data-ttu-id="18375-534">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="18375-534">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="18375-535">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-535">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="18375-536">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-536">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="18375-537">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-537">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="18375-538">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-538">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="18375-539">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="18375-539">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="18375-540">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="18375-540">AzureRM.Relay</span></span>
* <span data-ttu-id="18375-541">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-541">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-542">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-542">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-543">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-543">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="18375-544">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="18375-544">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="18375-545">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-545">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="18375-546">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-546">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="18375-547">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-547">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-548">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-548">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-549">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-549">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="18375-550">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-550">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="18375-551">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="18375-551">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="18375-552">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="18375-552">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="18375-553">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="18375-553">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="18375-554">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="18375-554">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="18375-555">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="18375-555">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="18375-556">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-556">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="18375-557">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="18375-557">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="18375-558">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-558">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="18375-559">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-559">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-560">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-560">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="18375-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-561">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="18375-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-562">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="18375-563">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="18375-563">AzureRM.Websites</span></span>
* <span data-ttu-id="18375-564">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="18375-564">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="18375-565">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-565">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="18375-566">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="18375-566">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="18375-567">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="18375-567">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="18375-568">全般</span><span class="sxs-lookup"><span data-stu-id="18375-568">General</span></span>
* <span data-ttu-id="18375-569">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-569">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="18375-570">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-570">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-571">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-571">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-572">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-572">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-573">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="18375-573">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="18375-574">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-574">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="18375-575">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-575">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="18375-576">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="18375-576">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="18375-577">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-577">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="18375-578">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="18375-578">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="18375-579">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="18375-579">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="18375-580">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="18375-580">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="18375-581">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="18375-581">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="18375-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="18375-582">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="18375-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="18375-583">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="18375-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="18375-584">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="18375-585">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="18375-585">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="18375-586">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="18375-586">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="18375-587">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="18375-587">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="18375-588">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-588">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="18375-589">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-589">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="18375-590">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="18375-590">AzureRM.EventHub</span></span>
* <span data-ttu-id="18375-591">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-591">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="18375-592">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-592">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="18375-593">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="18375-593">Provided Default Parameter set.</span></span>
* <span data-ttu-id="18375-594">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="18375-594">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="18375-595">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="18375-595">AzureRM.KeyVault</span></span>
* <span data-ttu-id="18375-596">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-596">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-597">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-597">AzureRM.Network</span></span>
* <span data-ttu-id="18375-598">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="18375-598">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="18375-599">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-599">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="18375-600">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-600">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="18375-601">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-601">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="18375-602">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-602">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="18375-603">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-603">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="18375-604">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-604">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="18375-605">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-605">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="18375-606">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-606">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="18375-607">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-607">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="18375-608">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="18375-608">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="18375-609">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-609">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="18375-610">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="18375-610">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="18375-611">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="18375-611">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-612">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-612">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-613">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-613">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="18375-614">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="18375-614">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="18375-615">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="18375-615">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="18375-616">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-616">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="18375-617">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-617">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="18375-618">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-618">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="18375-619">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-619">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="18375-620">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-620">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="18375-621">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-621">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="18375-622">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-622">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="18375-623">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-623">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="18375-624">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-624">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="18375-625">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-625">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="18375-626">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="18375-626">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="18375-627">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="18375-627">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="18375-628">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-628">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-629">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="18375-629">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="18375-630">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-630">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="18375-631">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="18375-631">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="18375-632">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-632">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-633">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-633">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="18375-634">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="18375-634">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="18375-635">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="18375-635">Azure.Storage</span></span>
* <span data-ttu-id="18375-636">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-636">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-637">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-637">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-638">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-638">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="18375-639">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-639">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="18375-640">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="18375-640">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="18375-641">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="18375-641">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="18375-642">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="18375-642">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="18375-643">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-643">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="18375-644">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="18375-644">Start-AzureRmVM</span></span>
    - <span data-ttu-id="18375-645">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="18375-645">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="18375-646">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="18375-646">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="18375-647">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="18375-647">Set-AzureRmVM</span></span>
    - <span data-ttu-id="18375-648">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="18375-648">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="18375-649">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="18375-649">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="18375-650">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="18375-650">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="18375-651">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="18375-651">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="18375-652">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="18375-652">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="18375-653">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="18375-653">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="18375-654">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="18375-654">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="18375-655">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="18375-655">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="18375-656">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="18375-656">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="18375-657">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="18375-657">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="18375-658">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="18375-658">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="18375-659">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="18375-659">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="18375-660">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="18375-660">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="18375-661">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="18375-661">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="18375-662">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="18375-662">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="18375-663">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="18375-663">AzureRM.EventGrid</span></span>
* <span data-ttu-id="18375-664">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="18375-664">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="18375-665">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="18375-665">AzureRM.KeyVault</span></span>
* <span data-ttu-id="18375-666">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-666">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="18375-667">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="18375-667">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="18375-668">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="18375-668">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="18375-669">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="18375-669">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="18375-670">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-670">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="18375-671">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="18375-671">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="18375-672">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-672">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="18375-673">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="18375-673">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="18375-674">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-674">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-675">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-675">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="18375-676">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="18375-676">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="18375-677">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-677">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="18375-678">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="18375-678">AzureRM.Websites</span></span>
* <span data-ttu-id="18375-679">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="18375-679">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="18375-680">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="18375-680">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="18375-681">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="18375-681">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="18375-682">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="18375-682">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="18375-683">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-683">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="18375-684">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="18375-684">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="18375-685">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-685">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-686">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-686">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="18375-687">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="18375-687">AzureRM.Compute</span></span>
* <span data-ttu-id="18375-688">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="18375-688">VMSS VM Update feature</span></span>
    - <span data-ttu-id="18375-689">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-689">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="18375-690">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-690">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="18375-691">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="18375-691">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="18375-692">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-692">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="18375-693">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-693">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="18375-694">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-694">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="18375-695">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-695">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="18375-696">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="18375-696">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="18375-697">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="18375-697">AzureRM.KeyVault</span></span>
* <span data-ttu-id="18375-698">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-698">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="18375-699">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-699">AzureRM.Network</span></span>
* <span data-ttu-id="18375-700">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="18375-700">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="18375-701">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="18375-701">AzureRM.Resources</span></span>
* <span data-ttu-id="18375-702">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-702">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="18375-703">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="18375-703">AzureRM.Scheduler</span></span>
* <span data-ttu-id="18375-704">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="18375-704">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="18375-705">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-705">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-706">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="18375-706">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="18375-707">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="18375-707">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="18375-708">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="18375-708">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="18375-709">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="18375-709">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="18375-710">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="18375-710">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="18375-711">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="18375-711">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="18375-712">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="18375-712">AzureRM.Websites</span></span>
* <span data-ttu-id="18375-713">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="18375-713">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="18375-714">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="18375-714">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="18375-715">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="18375-715">AzureRM.Profile</span></span>
* <span data-ttu-id="18375-716">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-716">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="18375-717">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="18375-717">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="18375-718">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="18375-718">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="18375-719">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="18375-719">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="18375-720">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-720">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="18375-721">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-721">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="18375-722">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-722">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="18375-723">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="18375-723">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="18375-724">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-724">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="18375-725">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-725">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="18375-726">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-726">Added support for MSI identity</span></span>
* <span data-ttu-id="18375-727">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="18375-727">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="18375-728">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="18375-728">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="18375-729">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-729">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="18375-730">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="18375-730">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="18375-731">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="18375-731">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="18375-732">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="18375-732">AzureRM.Batch</span></span>
* <span data-ttu-id="18375-733">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="18375-733">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="18375-734">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="18375-734">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="18375-735">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="18375-735">AzureRM.Consumption</span></span>
* <span data-ttu-id="18375-736">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-736">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="18375-737">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="18375-737">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="18375-738">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-738">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="18375-739">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-739">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="18375-740">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-740">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="18375-741">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="18375-741">AzureRM.Network</span></span>
* <span data-ttu-id="18375-742">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="18375-742">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="18375-743">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-743">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="18375-744">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="18375-744">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="18375-745">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-745">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="18375-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="18375-746">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="18375-747">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-747">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="18375-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="18375-748">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="18375-749">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="18375-749">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="18375-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="18375-750">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="18375-751">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="18375-751">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="18375-752">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="18375-752">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="18375-753">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="18375-753">AzureRM.Sql</span></span>
* <span data-ttu-id="18375-754">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="18375-754">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="18375-755">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="18375-755">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="18375-756">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="18375-756">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="18375-757">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="18375-757">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="18375-758">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="18375-758">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="18375-759">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="18375-759">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="18375-760">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="18375-760">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="18375-761">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="18375-761">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="18375-762">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="18375-762">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="18375-763">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="18375-763">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="18375-764">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="18375-764">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="18375-765">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="18375-765">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
