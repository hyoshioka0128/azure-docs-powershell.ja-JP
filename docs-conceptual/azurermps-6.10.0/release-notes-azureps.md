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
ms.openlocfilehash: 6a33d1a85fc61d0281bf1183163185b0dc4d3a12
ms.sourcegitcommit: f6f5e256143aa6c097de3e57e930d8badea49f30
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/18/2018
ms.locfileid: "49399061"
---
# <a name="release-notes"></a><span data-ttu-id="a1232-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="a1232-103">Release notes</span></span>

<span data-ttu-id="a1232-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a1232-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

---
## <a name="6100---october-2018"></a><span data-ttu-id="a1232-105">6.10.0 - 2018 年 10 月</span><span class="sxs-lookup"><span data-stu-id="a1232-105">6.10.0 - October 2018</span></span>
#### <a name="azurestorage"></a><span data-ttu-id="a1232-106">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-106">Azure.Storage</span></span>
* <span data-ttu-id="a1232-107">コピー先にメタデータがある場合、BLOB/ファイルのコピーではメタデータがコピーされない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-107">Fix Copy Blob/File won't copy metadata when destination has metadata issue</span></span>
    - <span data-ttu-id="a1232-108">Start-AzureStorageBlobCopy</span><span class="sxs-lookup"><span data-stu-id="a1232-108">Start-AzureStorageBlobCopy</span></span>
    - <span data-ttu-id="a1232-109">Start-AzureStorageFileCopy</span><span class="sxs-lookup"><span data-stu-id="a1232-109">Start-AzureStorageFileCopy</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="a1232-110">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a1232-110">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="a1232-111">既存のアカウントなしでの Get-AzureRmCognitiveServicesAccountSkus がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="a1232-111">Support Get-AzureRmCognitiveServicesAccountSkus without an existing account.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-112">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-112">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-113">必要に応じて 50 を超える結果が返されるように Get-AzureRmVM -ResourceGroupName <rg> を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-113">Fix Get-AzureRmVM -ResourceGroupName <rg> to return more than 50 results if needed</span></span>
* <span data-ttu-id="a1232-114">"SimpleParameterSet" の例を New-AzureRmVmss コマンドレットのヘルプに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-114">Added an example of the 'SimpleParameterSet' to New-AzureRmVmss cmdlet help.</span></span>
* <span data-ttu-id="a1232-115">Azure Disk Encryption の進行状況メッセージの誤りを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-115">Fixed a typo in the Azure Disk Encryption progress message</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="a1232-116">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a1232-116">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="a1232-117">ADF .Net SDK のバージョンを 2.3.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-117">Updated the ADF .Net SDK version to 2.3.0.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-118">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-118">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-119">NetworkProfile 機能を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-119">Added NetworkProfile functionality.</span></span> <span data-ttu-id="a1232-120">追加された新しいコマンドレットは次のとおりです</span><span class="sxs-lookup"><span data-stu-id="a1232-120">new cmdlets added</span></span>
    - <span data-ttu-id="a1232-121">Get-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a1232-121">Get-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="a1232-122">New-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a1232-122">New-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="a1232-123">Remove-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a1232-123">Remove-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="a1232-124">Set-AzureRMNetworkProfile</span><span class="sxs-lookup"><span data-stu-id="a1232-124">Set-AzureRMNetworkProfile</span></span>
    - <span data-ttu-id="a1232-125">New-AzureRMContainerNicConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-125">New-AzureRMContainerNicConfig</span></span>
    - <span data-ttu-id="a1232-126">New-AzureRmContainerNicConfigIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-126">New-AzureRmContainerNicConfigIpConfig</span></span>
* <span data-ttu-id="a1232-127">サブネット モデルでサービスの関連付けリンクを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-127">Added service association link on Subnet Model</span></span>
* <span data-ttu-id="a1232-128">New-AzureRmVirtualNetworkTap、Get-AzureRmVirtualNetworkTap、Set-AzureRmVirtualNetworkTap、Remove-AzureRmVirtualNetworkTap の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-128">Added cmdlet New-AzureRmVirtualNetworkTap, Get-AzureRmVirtualNetworkTap, Set-AzureRmVirtualNetworkTap, Remove-AzureRmVirtualNetworkTap</span></span>
* <span data-ttu-id="a1232-129">Set-AzureRmNEtworkInterfaceTapConfig、Get-AzureRmNEtworkInterfaceTapConfig、Remove-AzureRmNEtworkInterfaceTapConfig の各コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-129">Added cmdlet Set-AzureRmNEtworkInterfaceTapConfig, Get-AzureRmNEtworkInterfaceTapConfig, Remove-AzureRmNEtworkInterfaceTapConfig</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="a1232-130">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a1232-130">AzureRM.RedisCache</span></span>
* <span data-ttu-id="a1232-131">今後、サイズ パラメーターとして任意の文字列を追加できます。</span><span class="sxs-lookup"><span data-stu-id="a1232-131">Allow any string as Size parameter going forward.</span></span> <span data-ttu-id="a1232-132">PSArgumentCompleter ポップアップで P5 を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-132">Add P5 in PSArgumentCompleter popup</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-133">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-133">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-134">欠落していた -Mode パラメーターを Set-AzureRmPolicyDefinition に追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-134">Add missing -Mode parameter to Set-AzureRmPolicyDefinition</span></span>
* <span data-ttu-id="a1232-135">配信元にユーザーが含まれる操作について Get-AzureRmProviderOperation コマンドレットのバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-135">Fix Get-AzureRmProviderOperation commandlet bug for operations with Origin containing User</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="a1232-136">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-136">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-137">一部のバックアップ コマンドレットで現在の Azure サブスクリプションが認識されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-137">Fixed issue where some backup cmdlets would not recognize the current azure subscription</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="a1232-138">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-138">AzureRM.Storage</span></span>
* <span data-ttu-id="a1232-139">特定の場所におけるストレージ リソースの使用状況を取得できるるようになったため、グローバルなストレージ リソースの使用状況の取得が廃止されたことを通知する警告メッセージを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-139">Support get the Storage resource usage of a specific location, and add warning message for get global Storage resource usage is obsolete.</span></span>
    - <span data-ttu-id="a1232-140">Get-AzureRmStorageUsage</span><span class="sxs-lookup"><span data-stu-id="a1232-140">Get-AzureRmStorageUsage</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-141">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-141">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-142">新しいコマンドレット: Get-AzureRMWebAppContainerContinuousDeploymentUrl - コンテナーの継続的配置 Webhook URL を取得します</span><span class="sxs-lookup"><span data-stu-id="a1232-142">New Cmdlet Get-AzureRMWebAppContainerContinuousDeploymentUrl - Gets the Container Continuous Deployment Webhook URL</span></span>
* <span data-ttu-id="a1232-143">新しいコマンドレット: New-AzureRMWebAppContainerPSSession および Enter-WebAppContainerPSSession - Windows コンテナー アプリへの PowerShell リモート セッションを開始します</span><span class="sxs-lookup"><span data-stu-id="a1232-143">New Cmdlets New-AzureRMWebAppContainerPSSession and Enter-WebAppContainerPSSession  - Initiates a PowerShell remote session into a windows container app</span></span>

## <a name="690---september-2018"></a><span data-ttu-id="a1232-144">6.9.0 - 2018 年 9 月</span><span class="sxs-lookup"><span data-stu-id="a1232-144">6.9.0 - September 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a1232-145">全般</span><span class="sxs-lookup"><span data-stu-id="a1232-145">General</span></span>
* <span data-ttu-id="a1232-146">AzureRM.SignalR が AzureRM ロールアップ モジュールに追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-146">AzureRM.SignalR was added to the AzureRM rollup module</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="a1232-147">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-147">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-148">ストレージの一般的なコードに対する軽微な変更</span><span class="sxs-lookup"><span data-stu-id="a1232-148">Minor changes to the storage common code</span></span>
* <span data-ttu-id="a1232-149">完全なパラメーター型を含めるようにヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-149">Updated help files to include full parameter types.</span></span>
- <span data-ttu-id="a1232-150">ServicePrincipalCertificateWithSubscriptionId パラメーター セットの -ServicePrincipal を "任意" に変更しました</span><span class="sxs-lookup"><span data-stu-id="a1232-150">Changed -ServicePrincipal to non-mandatory in the ServicePrincipalCertificateWithSubscriptionId parameter set</span></span> 

#### <a name="azurestorage"></a><span data-ttu-id="a1232-151">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-151">Azure.Storage</span></span>
* <span data-ttu-id="a1232-152">OAuth でのストレージ コンテキストの作成がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="a1232-152">Support create Storage Context with OAuth.</span></span> 
    - <span data-ttu-id="a1232-153">New-AzureStorageContext</span><span class="sxs-lookup"><span data-stu-id="a1232-153">New-AzureStorageContext</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="a1232-154">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="a1232-154">AzureRM.Cdn</span></span>
* <span data-ttu-id="a1232-155">CDN 価格 SKU に Standard_Microsoft を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-155">Added Standard_Microsoft in Cdn pricing sku.</span></span> 

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-156">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-156">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-157">Keyvault および Storage への依存関係を一般的な依存関係に移動しました</span><span class="sxs-lookup"><span data-stu-id="a1232-157">Move dependencies on Keyvault and Storage to the common dependencies</span></span>
* <span data-ttu-id="a1232-158">より多くの仮想マシンのサイズのサポートを AEM コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-158">Add support for more virutal machine sizes to AEM cmdlets</span></span>
* <span data-ttu-id="a1232-159">PublicIPPrefix パラメーターを New-AzureRmVmssIpConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-159">Add PublicIPPrefix parameter to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="a1232-160">ResourceId パラメーターを Invoke-AzureRmVMRunCommand コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-160">Add ResourceId parameter to Invoke-AzureRmVMRunCommand cmdelt</span></span>
* <span data-ttu-id="a1232-161">Invoke-AzureRmVmssVMRunCommand コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-161">Add Invoke-AzureRmVmssVMRunCommand cmdlet</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="a1232-162">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="a1232-162">AzureRM.Dns</span></span>
* <span data-ttu-id="a1232-163">DNS レコード作成中のエイリアス レコードのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-163">Added support for alias record during dns record creation</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="a1232-164">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="a1232-164">AzureRM.Insights</span></span>
* <span data-ttu-id="a1232-165">#6833 および #7102 の問題を修正しました (診断設定領域)</span><span class="sxs-lookup"><span data-stu-id="a1232-165">Fixed issues #6833 and #7102 (Diagnostic Settings area)</span></span>
    - <span data-ttu-id="a1232-166">診断設定の作成および表示/取得中の既定の名前 ("service") に関する問題</span><span class="sxs-lookup"><span data-stu-id="a1232-166">Issues with the default name, i.e. 'service', during creation and listing/getting of diagnostic settings</span></span>
    - <span data-ttu-id="a1232-167">カテゴリでの診断設定の作成に関する問題</span><span class="sxs-lookup"><span data-stu-id="a1232-167">Issues creating diagnostic settings with categories</span></span>
* <span data-ttu-id="a1232-168">メトリック時間グレイン パラメーターの非推奨メッセージを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-168">Added deprecation message for metrics time grains parameters</span></span>
    - <span data-ttu-id="a1232-169">Timegrains パラメーターは引き続き利用できますが (これは破壊的変更ではありません)、PT1M のみが有効であるため、バックエンドでは無視されます</span><span class="sxs-lookup"><span data-stu-id="a1232-169">Timegrains parameters are still being accepted (this is a non-breaking change,) but they are ignored in the backend since only PT1M is valid</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-170">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-170">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-171">LoadBalancer コマンドレットへの変更</span><span class="sxs-lookup"><span data-stu-id="a1232-171">Changes to LoadBalancer cmdlets</span></span>
  - <span data-ttu-id="a1232-172">LoadBalancerInboundNatPoolConfig: IdleTimeoutInMinutes パラメーター、EnableFloatingIp パラメーター、EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-172">LoadBalancerInboundNatPoolConfig: added parameters IdleTimeoutInMinutes, EnableFloatingIp and EnableTcpReset</span></span>
  - <span data-ttu-id="a1232-173">LoadBalancerInboundNatRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-173">LoadBalancerInboundNatRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="a1232-174">LoadBalancerRuleConfig: EnableTcpReset パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-174">LoadBalancerRuleConfig: added parameter EnableTcpReset</span></span>
  - <span data-ttu-id="a1232-175">LoadBalancerProbeConfig: Protocol パラメーターの "HTTPS" 値のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-175">LoadBalancerProbeConfig: added support for value "Https" for parameter Protocol</span></span>
* <span data-ttu-id="a1232-176">新しい LoadBalancer のサブリソース OutboundRule について新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-176">Added new commands for new LoadBalancer's subresource OutboundRule</span></span>
  - <span data-ttu-id="a1232-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-177">Add-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="a1232-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-178">Get-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="a1232-179">New-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-179">New-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="a1232-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-180">Set-AzureRmLoadBalancerOutboundRuleConfig</span></span>
  - <span data-ttu-id="a1232-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-181">Remove-AzureRmLoadBalancerOutboundRuleConfig</span></span>
* <span data-ttu-id="a1232-182">PSNetworkInterface の新しい HostedWorkloads プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-182">Added new HostedWorkloads property for PSNetworkInterface</span></span>
* <span data-ttu-id="a1232-183">ARM 経由の Azure Firewall 機能のために新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-183">Added new cmdlets for feature: Azure Firewall via ARM</span></span>
  - <span data-ttu-id="a1232-184">Get-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-184">Added Get-AzureRmFirewall</span></span>
  - <span data-ttu-id="a1232-185">Set-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-185">Added Set-AzureRmFirewall</span></span>
  - <span data-ttu-id="a1232-186">New-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-186">Added New-AzureRmFirewall</span></span>
  - <span data-ttu-id="a1232-187">Remove-AzureRmFirewall を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-187">Added Remove-AzureRmFirewall</span></span>
  - <span data-ttu-id="a1232-188">New-AzureRmFirewallApplicationRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-188">Added New-AzureRmFirewallApplicationRuleCollection</span></span>
  - <span data-ttu-id="a1232-189">New-AzureRmFirewallApplicationRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-189">Added New-AzureRmFirewallApplicationRule</span></span>
  - <span data-ttu-id="a1232-190">New-AzureRmFirewallNatRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-190">Added New-AzureRmFirewallNatRuleCollection</span></span>
  - <span data-ttu-id="a1232-191">New-AzureRmFirewallNatRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-191">Added New-AzureRmFirewallNatRule</span></span>
  - <span data-ttu-id="a1232-192">New-AzureRmFirewallNetworkRuleCollection を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-192">Added New-AzureRmFirewallNetworkRuleCollection</span></span>
  - <span data-ttu-id="a1232-193">New-AzureRmFirewallNetworkRule を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-193">Added New-AzureRmFirewallNetworkRule</span></span>
* <span data-ttu-id="a1232-194">Application Gateway での信頼されたルート証明書と自動スケーリング構成のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-194">Added support for Trusted Root certificate and Autoscale configuration in Application Gateway</span></span>
  - <span data-ttu-id="a1232-195">追加された新しいコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="a1232-195">New Cmdlets added:</span></span>
      - <span data-ttu-id="a1232-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-196">Add-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="a1232-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-197">Get-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="a1232-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-198">New-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="a1232-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-199">Remove-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="a1232-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-200">Set-AzureRmApplicationGatewayTrustedRootCertificate</span></span>
      - <span data-ttu-id="a1232-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-201">Get-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="a1232-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-202">New-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="a1232-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-203">Remove-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
      - <span data-ttu-id="a1232-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-204">Set-AzureRmApplicationGatewayAutoscaleConfiguration</span></span>
  - <span data-ttu-id="a1232-205">省略可能なパラメーターで更新されたコマンドレット -TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-205">Cmdlets updated with optonal parameter -TrustedRootCertificate</span></span>
      - <span data-ttu-id="a1232-206">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a1232-206">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="a1232-207">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a1232-207">Set-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="a1232-208">New-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="a1232-208">New-AzureRmApplicationGatewayBackendHttpSetting</span></span>
      - <span data-ttu-id="a1232-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span><span class="sxs-lookup"><span data-stu-id="a1232-209">Set-AzureRmApplicationGatewayBackendHttpSetting</span></span>
  - <span data-ttu-id="a1232-210">省略可能なパラメーターで更新されたコマンドレット - AutoscaleConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-210">Cmdlets updated with optonal parameter -AutoscaleConfiguration</span></span>
      - <span data-ttu-id="a1232-211">New-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a1232-211">New-AzureRmApplicationGateway</span></span>
      - <span data-ttu-id="a1232-212">Set-AzureRmApplicationGateway</span><span class="sxs-lookup"><span data-stu-id="a1232-212">Set-AzureRmApplicationGateway</span></span>
* <span data-ttu-id="a1232-213">インターフェイス エンドポイントのコマンドレット Get-AzureInterfaceEndpoint を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-213">Add cmdlet for Interface Endpoint Get-AzureInterfaceEndpoint</span></span>
* <span data-ttu-id="a1232-214">サブネットでの複数のアドレス プレフィックスのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-214">Added support for multiple address prefixes in a subnet.</span></span> <span data-ttu-id="a1232-215">更新されたコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="a1232-215">Updated cmdlets:</span></span>
  - <span data-ttu-id="a1232-216">New-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-216">New-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="a1232-217">Set-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-217">Set-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="a1232-218">Add-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-218">Add-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="a1232-219">Get-AzureRmVirtualNetworkSubnetConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-219">Get-AzureRmVirtualNetworkSubnetConfig</span></span>
  - <span data-ttu-id="a1232-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-220">Add-AzureRmApplicationGatewayAuthenticationCertificate</span></span>
  - <span data-ttu-id="a1232-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-221">Add-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="a1232-222">New-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-222">New-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="a1232-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-223">Set-AzureRmApplicationGatewayFrontendIPConfig</span></span>
  - <span data-ttu-id="a1232-224">Add-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-224">Add-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="a1232-225">New-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-225">New-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="a1232-226">Set-AzureRmApplicationGatewayIPConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-226">Set-AzureRmApplicationGatewayIPConfiguration</span></span>
  - <span data-ttu-id="a1232-227">Add-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-227">Add-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="a1232-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-228">New-AzureRmNetworkInterfaceIpConfig  - Set-AzureRmNetworkInterfaceIpConfig</span></span>
  - <span data-ttu-id="a1232-229">New-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-229">New-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="a1232-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-230">Add-AzureRmVirtualNetworkGatewayIpConfig</span></span>
  - <span data-ttu-id="a1232-231">Set-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-231">Set-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="a1232-232">Add-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-232">Add-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="a1232-233">New-AzureRmLoadBalancerFrontendIpConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-233">New-AzureRmLoadBalancerFrontendIpConfig</span></span>
  - <span data-ttu-id="a1232-234">New-AzureRmNetworkInterface</span><span class="sxs-lookup"><span data-stu-id="a1232-234">New-AzureRmNetworkInterface</span></span>
* <span data-ttu-id="a1232-235">サブネット委任のコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-235">Adding cmdlets for subnet delegation.</span></span>
  - <span data-ttu-id="a1232-236">New-AzureRmDelegation: 新しい委任を作成します。これはサブネットに追加できます</span><span class="sxs-lookup"><span data-stu-id="a1232-236">New-AzureRmDelegation: Creates a new delegation, which can be added to a subnet</span></span>
  - <span data-ttu-id="a1232-237">Remove-AzureRmDelegation: サブネットを受け取り、指定された委任の名前をそのサブネットから削除します</span><span class="sxs-lookup"><span data-stu-id="a1232-237">Remove-AzureRmDelegation: Takes in a subnet and removes the provided delegation name from that subnet</span></span>
  - <span data-ttu-id="a1232-238">Add-AzureRmDelegation: サブネットを受け取り、指定されたサービス名を委任としてそのサブネットに追加します</span><span class="sxs-lookup"><span data-stu-id="a1232-238">Add-AzureRmDelegation: Takes in a subnet and adds the provided service name as a delegation to that subnet</span></span>
  - <span data-ttu-id="a1232-239">Get-AzureRmDelegation</span><span class="sxs-lookup"><span data-stu-id="a1232-239">Get-AzureRmDelegation</span></span>
  - <span data-ttu-id="a1232-240">Get-AzureRmAvailableServiceDelegations</span><span class="sxs-lookup"><span data-stu-id="a1232-240">Get-AzureRmAvailableServiceDelegations</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="a1232-241">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a1232-241">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a1232-242">管理対象のマネージド ディスクのサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-242">Support for managed Managed disk</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="a1232-243">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a1232-243">AzureRM.RedisCache</span></span>
* <span data-ttu-id="a1232-244">Insights の依存関係を更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-244">Updated Insights dependency.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-245">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-245">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-246">New-AzureRmResourceGroupDeployment を新しい RollbackAction パラメーターで更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-246">Update New-AzureRmResourceGroupDeployment with new parameter RollbackAction</span></span>
    - <span data-ttu-id="a1232-247">新しいパラメーターを使用して OnErrorDeployment のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-247">Add support for OnErrorDeployment with the new parameter.</span></span>
* <span data-ttu-id="a1232-248">ポリシー割り当てでマネージド ID をサポートします。</span><span class="sxs-lookup"><span data-stu-id="a1232-248">Support managed identity on policy assignments.</span></span>
* <span data-ttu-id="a1232-249">"New-AzureRmPolicyAssignment" を指定してポリシーを割り当てるとき、既定値を持つパラメーターが不要になりました</span><span class="sxs-lookup"><span data-stu-id="a1232-249">Parameters with default values are no longer requred when assigning a policy with 'New-AzureRmPolicyAssignment'</span></span>
* <span data-ttu-id="a1232-250">ポリシー エイリアスを取得するための新しい Get AzureRmPolicyAlias コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-250">Add new cmdlet Get-AzureRmPolicyAlias for retrieving policy aliases</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-251">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-251">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-252">問題 #7161 を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-252">Fixed issue #7161</span></span>

#### <a name="azurermsignalr"></a><span data-ttu-id="a1232-253">AzureRM.SignalR</span><span class="sxs-lookup"><span data-stu-id="a1232-253">AzureRM.SignalR</span></span>
* <span data-ttu-id="a1232-254">SKU 名を Free_F1 および Standard_S1 に更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-254">Update SKU names to Free_F1 and Standard_S1</span></span>
* <span data-ttu-id="a1232-255">バージョン フィールドを PSSignalRResource オブジェクトに、接続文字列を PSSignalRKeys オブジェクトに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-255">Add version field to the PSSignalRResource object and connection string to the PSSignalRKeys object.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="a1232-256">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-256">AzureRM.Storage</span></span>
* <span data-ttu-id="a1232-257">AzureRm.Storage での不変ポリシーをサポートします</span><span class="sxs-lookup"><span data-stu-id="a1232-257">Support Immutability Policy in AzureRm.Storage</span></span> 
    - <span data-ttu-id="a1232-258">Remove-AzureRmStorageAccountNetworkRule</span><span class="sxs-lookup"><span data-stu-id="a1232-258">Remove-AzureRmStorageAccountNetworkRule</span></span>
    - <span data-ttu-id="a1232-259">Get-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="a1232-259">Get-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="a1232-260">Update-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="a1232-260">Update-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="a1232-261">New-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="a1232-261">New-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="a1232-262">Remove-AzureRmStorageContainer</span><span class="sxs-lookup"><span data-stu-id="a1232-262">Remove-AzureRmStorageContainer</span></span>
    - <span data-ttu-id="a1232-263">Add-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="a1232-263">Add-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="a1232-264">Remove-AzureRmStorageContainerLegalHold</span><span class="sxs-lookup"><span data-stu-id="a1232-264">Remove-AzureRmStorageContainerLegalHold</span></span>
    - <span data-ttu-id="a1232-265">Set-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a1232-265">Set-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="a1232-266">Get-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a1232-266">Get-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="a1232-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a1232-267">Remove-AzureRmStorageContainerImmutabilityPolicy</span></span>
    - <span data-ttu-id="a1232-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span><span class="sxs-lookup"><span data-stu-id="a1232-268">Lock-AzureRmStorageContainerImmutabilityPolicy</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-269">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-269">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-270">Get-AzureRmDeletedWebApp と Restore-AzureRmDeletedWebApp の 2 つの新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-270">Added two new cmdlets: Get-AzureRmDeletedWebApp and Restore-AzureRmDeletedWebApp</span></span>
* <span data-ttu-id="a1232-271">Windows コンテナーでの App Service プランの作成用に New-AzureRmAppServicePlan -HyperV スイッチが追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-271">New-AzureRmAppServicePlan -HyperV switch is added for create app service plan with windows container</span></span>
* <span data-ttu-id="a1232-272">Windows コンテナー アプリを作成および管理用に、New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New パラメーター (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) が追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-272">New-AzureRmWebApp/ New-AzureRmWebAppSlot/ Set-AzureRmWebApp/ Set-AzureRmWebAppSlot - New parameters (–ContainerRegistryUser string -ContainerRegistryPassword secureString -EnableContainerContinuousDeployment) added for creating and managing windows container app</span></span>

## <a name="681---august-2018"></a><span data-ttu-id="a1232-273">6.8.1 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="a1232-273">6.8.1 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a1232-274">全般</span><span class="sxs-lookup"><span data-stu-id="a1232-274">General</span></span>
* <span data-ttu-id="a1232-275">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-275">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="a1232-276">共通ランタイム アセンブリを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-276">Updated common runtime assemblies</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="a1232-277">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a1232-277">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="a1232-278">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-278">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="a1232-279">修正された問題 https://github.com/Azure/azure-powershell/issues/6603</span><span class="sxs-lookup"><span data-stu-id="a1232-279">Fixed issue https://github.com/Azure/azure-powershell/issues/6603</span></span>
    - <span data-ttu-id="a1232-280">Import-AzureRmApiManagementApi コマンドレットおよび \*-AzureRmApiManagementCertificate コマンドレットで、相対パスを処理できるようになりました</span><span class="sxs-lookup"><span data-stu-id="a1232-280">Import-AzureRmApiManagementApi and \*-AzureRmApiManagementCertificate cmdlets now handle relative Paths</span></span>
* <span data-ttu-id="a1232-281">修正された問題 https://github.com/Azure/azure-powershell/issues/6879</span><span class="sxs-lookup"><span data-stu-id="a1232-281">Fixed issue https://github.com/Azure/azure-powershell/issues/6879</span></span>
    - <span data-ttu-id="a1232-282">CertificateInformation は、Set-AzureRmApiManagement コマンドレットが適切に動作できるようにする設定可能なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="a1232-282">The CertificateInformation is a settable property allowing for Set-AzureRmApiManagement cmdlet to work property.</span></span> <span data-ttu-id="a1232-283">4.0.4-preview NuGet へのアップグレードによって修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-283">Fixed by upgrading to 4.0.4-preview nuget</span></span>
* <span data-ttu-id="a1232-284">修正された問題 https://github.com/Azure/azure-powershell/issues/6853</span><span class="sxs-lookup"><span data-stu-id="a1232-284">Fixed issue https://github.com/Azure/azure-powershell/issues/6853</span></span>
    - <span data-ttu-id="a1232-285">製品を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-285">Fixed the Odata filter for Search by Name on Product</span></span>
* <span data-ttu-id="a1232-286">修正された問題 https://github.com/Azure/azure-powershell/issues/6814</span><span class="sxs-lookup"><span data-stu-id="a1232-286">Fixed issue https://github.com/Azure/azure-powershell/issues/6814</span></span>
    - <span data-ttu-id="a1232-287">API を名前で検索するための Odata フィルターを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-287">Fixed the Odata filter for Search by Name on Api</span></span>
* <span data-ttu-id="a1232-288">AzureMonitor ロガーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-288">Added support for AzureMonitor logger</span></span>


#### <a name="azurermcompute"></a><span data-ttu-id="a1232-289">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-289">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-290">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-290">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="a1232-291">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-291">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="a1232-292">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-292">Fixed issue with default resource groups not being set.</span></span>
* <span data-ttu-id="a1232-293">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-293">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-294">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-294">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-295">コマンドレット出力の既定の表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="a1232-295">Changed default cmdlet output presentation to table view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="a1232-296">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a1232-296">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="a1232-297">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-297">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>


#### <a name="azurermresources"></a><span data-ttu-id="a1232-298">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-298">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-299">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-299">Fixed issue with creating managed applications from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-300">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-300">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-301">修正された問題</span><span class="sxs-lookup"><span data-stu-id="a1232-301">Fixed issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="a1232-302">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a1232-302">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="a1232-303">複数値ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-303">Added Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="a1232-304">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="a1232-304">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="a1232-305">サブネット ルーティング方式のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-305">Added Support for the Subnet routing method</span></span>
    - <span data-ttu-id="a1232-306">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-306">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="a1232-307">プロファイルでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-307">Added Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="a1232-308">プロファイルでの予期される状態コード範囲のサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-308">Added Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="a1232-309">エンドポイントでのカスタム ヘッダーのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-309">Added Support for Custom Headers in endpoints</span></span>

## <a name="680---august-2018"></a><span data-ttu-id="a1232-310">6.8.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="a1232-310">6.8.0 - August 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a1232-311">全般</span><span class="sxs-lookup"><span data-stu-id="a1232-311">General</span></span>
* <span data-ttu-id="a1232-312">既定のリソース グループが設定されていないという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-312">Fixed issue with default resource groups not being set.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="a1232-313">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-313">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-314">Connect-AzureRmAccount 中に返されるトークンに有効期限プロパティを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-314">Added expiration property to tokens returned during Connect-AzureRmAccount</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-315">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-315">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-316">エラー出力にターゲットが見つからない問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-316">Fixed the issue that target is missing in error output.</span></span>
* <span data-ttu-id="a1232-317">マネージド ディスクを含む VM 用ストレージ アカウントの種類に関する問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-317">Fixed issue with storage account type for VM with managed disk</span></span>
* <span data-ttu-id="a1232-318">Azure 中国など、他の環境における AEM 拡張機能コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-318">Fix AEM Extension cmdlets for other environments, for example Azure China</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="a1232-319">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="a1232-319">AzureRM.IotHub</span></span>
* <span data-ttu-id="a1232-320">New-AzureRmIotHubExportDevices および New-AzureRmIotHubImportDevices の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-320">Fix examples for New-AzureRmIotHubExportDevices and New-AzureRmIotHubImportDevices</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-321">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-321">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-322">既定のモデルの表示をテーブル ビューに変更しました</span><span class="sxs-lookup"><span data-stu-id="a1232-322">Changed default models representation to table-view</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="a1232-323">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a1232-323">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="a1232-324">一時停止された容量をスケーリングしようとしたときに発生していた Update-AzureRmPowerBIEmbeddedCapacity のエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-324">Fix failure in Update-AzureRmPowerBIEmbeddedCapacity when trying to scale paused capacity</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-325">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-325">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-326">Marketplace からのマネージド アプリケーション作成に関する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-326">Fixed issue with creating managed application from the MarketPlace.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-327">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-327">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-328">問題の修正</span><span class="sxs-lookup"><span data-stu-id="a1232-328">Fix for issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/5058
    - https://github.com/Azure/azure-powershell/issues/5055
    - https://github.com/Azure/azure-powershell/issues/6891

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="a1232-329">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a1232-329">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="a1232-330">複数値ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-330">Support for the MultiValue routing method</span></span>
    - <span data-ttu-id="a1232-331">複数値ルーティング用の新しい "MaxReturn" パラメーター</span><span class="sxs-lookup"><span data-stu-id="a1232-331">New parameter 'MaxReturn' for MultiValue routing</span></span>
* <span data-ttu-id="a1232-332">サブネット ルーティング方式のサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-332">Support for the Subnet routing method</span></span>
    - <span data-ttu-id="a1232-333">エンドポイントでの IP アドレス範囲 (サブネット) のサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-333">Support for IP address ranges (subnets) in endpoints</span></span>
* <span data-ttu-id="a1232-334">プロファイルでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-334">Support for Custom Headers in profiles</span></span>
* <span data-ttu-id="a1232-335">プロファイルでの予期される状態コード範囲のサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-335">Support for Expected status code ranges in profiles</span></span>
* <span data-ttu-id="a1232-336">エンドポイントでのカスタム ヘッダーのサポート</span><span class="sxs-lookup"><span data-stu-id="a1232-336">Support for Custom Headers in endpoints</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-337">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-337">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-338">既定のリソース グループが間違って設定されているという問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-338">Fixed issue with default resource group being set incorrectly.</span></span>

## <a name="670---august-2018"></a><span data-ttu-id="a1232-339">6.7.0 - 2018 年 8 月</span><span class="sxs-lookup"><span data-stu-id="a1232-339">6.7.0 - August 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="a1232-340">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-340">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-341">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-341">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="a1232-342">コンテキストの競合を回避するために既定のコンテキスト名にユーザー ID を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-342">Add user id to default context name to avoid context clashing</span></span>
    - https://github.com/Azure/azure-powershell/issues/6489
* <span data-ttu-id="a1232-343">コンテキスト #6398 の選択に関する問題の原因となっていた Clear-AzureRmContext の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-343">Fix issues with Clear-AzureRmContext that caused issues with selecting a context #6398</span></span>
* <span data-ttu-id="a1232-344">"Connect-AzureRmAccount" の "-TenantId" パラメーターにテナント ドメインを渡すことができるようにしました</span><span class="sxs-lookup"><span data-stu-id="a1232-344">Enable tenant domain to be passed to '-TenantId' parameter for 'Connect-AzureRmAccount'</span></span>
    - https://github.com/Azure/azure-powershell/issues/3974
    - https://github.com/Azure/azure-powershell/issues/6709

#### <a name="azurestorage"></a><span data-ttu-id="a1232-345">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-345">Azure.Storage</span></span>
* <span data-ttu-id="a1232-346">Azure ファイル共有のクォータについて 5 TB の制限を削除しました</span><span class="sxs-lookup"><span data-stu-id="a1232-346">Remove the 5TB limitation for Azure File Share quota</span></span>
- <span data-ttu-id="a1232-347">Set-AzureStorageShareQuota</span><span class="sxs-lookup"><span data-stu-id="a1232-347">Set-AzureStorageShareQuota</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="a1232-348">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a1232-348">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="a1232-349">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-349">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azureanalysisservices"></a><span data-ttu-id="a1232-350">Azure.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a1232-350">Azure.AnalysisServices</span></span>
* <span data-ttu-id="a1232-351">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-351">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="a1232-352">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a1232-352">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="a1232-353">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-353">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermapplicationinsights"></a><span data-ttu-id="a1232-354">AzureRM.ApplicationInsights</span><span class="sxs-lookup"><span data-stu-id="a1232-354">AzureRM.ApplicationInsights</span></span>
* <span data-ttu-id="a1232-355">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-355">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="a1232-356">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="a1232-356">AzureRM.Automation</span></span>
* <span data-ttu-id="a1232-357">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-357">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbackup"></a><span data-ttu-id="a1232-358">AzureRM.Backup</span><span class="sxs-lookup"><span data-stu-id="a1232-358">AzureRM.Backup</span></span>
* <span data-ttu-id="a1232-359">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-359">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="a1232-360">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="a1232-360">AzureRM.Batch</span></span>
* <span data-ttu-id="a1232-361">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-361">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermbilling"></a><span data-ttu-id="a1232-362">AzureRM.Billing</span><span class="sxs-lookup"><span data-stu-id="a1232-362">AzureRM.Billing</span></span>
* <span data-ttu-id="a1232-363">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-363">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcdn"></a><span data-ttu-id="a1232-364">AzureRM.Cdn</span><span class="sxs-lookup"><span data-stu-id="a1232-364">AzureRM.Cdn</span></span>
* <span data-ttu-id="a1232-365">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-365">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcognitiveservices"></a><span data-ttu-id="a1232-366">AzureRM.CognitiveServices</span><span class="sxs-lookup"><span data-stu-id="a1232-366">AzureRM.CognitiveServices</span></span>
* <span data-ttu-id="a1232-367">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-367">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-368">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-368">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-369">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-369">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="a1232-370">EvictionPolicy パラメーターを New-AzureRmVmssConfig に追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-370">Add EvictionPolicy parameter to New-AzureRmVmssConfig</span></span>
* <span data-ttu-id="a1232-371">場所が指定されていない場合、New-AzureRmVm の DiskFileParameterSet で既定の場所を使用します。</span><span class="sxs-lookup"><span data-stu-id="a1232-371">Use default location in the DiskFileParameterSet of New-AzureRmVm if no Location is specified.</span></span>
* <span data-ttu-id="a1232-372">Save-AzureRmVMImage のパラメーターの説明を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-372">Fix parameter description in Save-AzureRmVMImage</span></span>
* <span data-ttu-id="a1232-373">単一パスに関連する一部シナリオに対応できるように Get-AzureRmVMDiskEncryptionStatus コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-373">Fix Get-AzureRmVMDiskEncryptionStatus cmdlet for certain singlepass related scenarios</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="a1232-374">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="a1232-374">AzureRM.Consumption</span></span>
* <span data-ttu-id="a1232-375">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-375">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerinstance"></a><span data-ttu-id="a1232-376">AzureRM.ContainerInstance</span><span class="sxs-lookup"><span data-stu-id="a1232-376">AzureRM.ContainerInstance</span></span>
* <span data-ttu-id="a1232-377">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-377">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermcontainerregistry"></a><span data-ttu-id="a1232-378">AzureRM.ContainerRegistry</span><span class="sxs-lookup"><span data-stu-id="a1232-378">AzureRM.ContainerRegistry</span></span>
* <span data-ttu-id="a1232-379">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-379">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactories"></a><span data-ttu-id="a1232-380">AzureRM.DataFactories</span><span class="sxs-lookup"><span data-stu-id="a1232-380">AzureRM.DataFactories</span></span>
* <span data-ttu-id="a1232-381">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-381">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="a1232-382">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a1232-382">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="a1232-383">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-383">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="a1232-384">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a1232-384">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="a1232-385">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-385">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="a1232-386">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a1232-386">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="a1232-387">DebugPreference が PowerShell コマンド ラインから設定されているときのデバッグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-387">Fix debugging when DebugPreference is set from powershell command line</span></span>
* <span data-ttu-id="a1232-388">Set-AzureRmDataLakeStoreItemAcl の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-388">Update example for Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="a1232-389">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-389">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="a1232-390">Set-AzureRmDataLakeStoreItemAclEntry の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-390">Update example for Set-AzureRmDataLakeStoreItemAclEntry</span></span>

#### <a name="azurermdevtestlabs"></a><span data-ttu-id="a1232-391">AzureRM.DevTestLabs</span><span class="sxs-lookup"><span data-stu-id="a1232-391">AzureRM.DevTestLabs</span></span>
* <span data-ttu-id="a1232-392">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-392">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermdns"></a><span data-ttu-id="a1232-393">AzureRM.Dns</span><span class="sxs-lookup"><span data-stu-id="a1232-393">AzureRM.Dns</span></span>
* <span data-ttu-id="a1232-394">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-394">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="a1232-395">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a1232-395">AzureRM.EventGrid</span></span>
* <span data-ttu-id="a1232-396">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-396">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="a1232-397">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="a1232-397">AzureRM.EventHub</span></span>
* <span data-ttu-id="a1232-398">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-398">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermhdinsight"></a><span data-ttu-id="a1232-399">AzureRM.HDInsight</span><span class="sxs-lookup"><span data-stu-id="a1232-399">AzureRM.HDInsight</span></span>
* <span data-ttu-id="a1232-400">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-400">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="a1232-401">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="a1232-401">AzureRM.Insights</span></span>
* <span data-ttu-id="a1232-402">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-402">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermiothub"></a><span data-ttu-id="a1232-403">AzureRM.IotHub</span><span class="sxs-lookup"><span data-stu-id="a1232-403">AzureRM.IotHub</span></span>
* <span data-ttu-id="a1232-404">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-404">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="a1232-405">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a1232-405">AzureRM.KeyVault</span></span>
* <span data-ttu-id="a1232-406">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-406">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="a1232-407">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a1232-407">AzureRM.LogicApp</span></span>
* <span data-ttu-id="a1232-408">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-408">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearning"></a><span data-ttu-id="a1232-409">AzureRM.MachineLearning</span><span class="sxs-lookup"><span data-stu-id="a1232-409">AzureRM.MachineLearning</span></span>
* <span data-ttu-id="a1232-410">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-410">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmachinelearningcompute"></a><span data-ttu-id="a1232-411">AzureRM.MachineLearningCompute</span><span class="sxs-lookup"><span data-stu-id="a1232-411">AzureRM.MachineLearningCompute</span></span>
* <span data-ttu-id="a1232-412">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-412">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmarketplaceordering"></a><span data-ttu-id="a1232-413">AzureRM.MarketplaceOrdering</span><span class="sxs-lookup"><span data-stu-id="a1232-413">AzureRM.MarketplaceOrdering</span></span>
* <span data-ttu-id="a1232-414">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-414">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermmedia"></a><span data-ttu-id="a1232-415">AzureRM.Media</span><span class="sxs-lookup"><span data-stu-id="a1232-415">AzureRM.Media</span></span>
* <span data-ttu-id="a1232-416">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-416">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-417">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-417">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-418">Set-AzureRmLocalNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-418">Added example for Set-AzureRmLocalNetworkGateway</span></span>
* <span data-ttu-id="a1232-419">Add-AzureRmVirtualNetworkGatewayIpConfig、Get-AzureRmVirtualNetworkGatewayConnectionSharedKey、および New-AzureRmVirtualNetworkGatewayConnection の例と説明を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-419">Added examples and descriptions for Add-AzureRmVirtualNetworkGatewayIpConfig, Get-AzureRmVirtualNetworkGatewayConnectionSharedKey and New-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a1232-420">Remove-AzureRmVirtualNetworkGatewayIpConfig と Reset-AzureRmVirtualNetworkGateway の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-420">Added examples for Remove-AzureRmVirtualNetworkGatewayIpConfig and Reset-AzureRmVirtualNetworkGateway</span></span>
* <span data-ttu-id="a1232-421">Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-421">Added example for Reset-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="a1232-422">Set-AzureRmVirtualNetworkGatewayConnectionSharedKey の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-422">Added example for Set-AzureRmVirtualNetworkGatewayConnectionSharedKey</span></span>
* <span data-ttu-id="a1232-423">Set-AzureRmVirtualNetworkGatewayConnection の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-423">Added example for Set-AzureRmVirtualNetworkGatewayConnection</span></span>
* <span data-ttu-id="a1232-424">最新のコード ジェネレータ―を使用して ApplicationSecurityGroup、RouteTable、および Usage のコマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="a1232-424">Re-generated cmdlets for ApplicationSecurityGroup, RouteTable and Usage using latest code generator</span></span>
* <span data-ttu-id="a1232-425">存在しないサブネットを取得しようとしたときの Get-AzureRmVirtualNetworkSubnetConfig のエラー メッセージを明確化しました</span><span class="sxs-lookup"><span data-stu-id="a1232-425">Clarified error message for Get-AzureRmVirtualNetworkSubnetConfig when attempting to get a subnet that does not exitc</span></span>

#### <a name="azurermnotificationhubs"></a><span data-ttu-id="a1232-426">AzureRM.NotificationHubs</span><span class="sxs-lookup"><span data-stu-id="a1232-426">AzureRM.NotificationHubs</span></span>
* <span data-ttu-id="a1232-427">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-427">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermoperationalinsights"></a><span data-ttu-id="a1232-428">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a1232-428">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="a1232-429">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-429">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="a1232-430">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a1232-430">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="a1232-431">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-431">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermpowerbiembedded"></a><span data-ttu-id="a1232-432">AzureRM.PowerBIEmbedded</span><span class="sxs-lookup"><span data-stu-id="a1232-432">AzureRM.PowerBIEmbedded</span></span>
* <span data-ttu-id="a1232-433">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-433">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservices"></a><span data-ttu-id="a1232-434">AzureRM.RecoveryServices</span><span class="sxs-lookup"><span data-stu-id="a1232-434">AzureRM.RecoveryServices</span></span>
* <span data-ttu-id="a1232-435">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-435">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="a1232-436">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a1232-436">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a1232-437">ポリシー フィルターを Get-AzureRmRecoveryServicesBackItem コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-437">Added policy filter to Get-AzureRmRecoveryServicesBackItem cmdlet.</span></span> <span data-ttu-id="a1232-438">指定したポリシー ID によって保護されているバックアップ項目の一覧がコマンドによって返されます。</span><span class="sxs-lookup"><span data-stu-id="a1232-438">The command returns the list of backup items protected by the given policy id.</span></span>
* <span data-ttu-id="a1232-439">Microsoft.Azure.Management.RecoveryServices.Backup をバージョン 3.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-439">Updated Microsoft.Azure.Management.RecoveryServices.Backup to version 3.0.0-preview.</span></span>
* <span data-ttu-id="a1232-440">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-440">Updated to the latest version of the Azure ClientRuntime.</span></span>
* <span data-ttu-id="a1232-441">TargetResourceGroupName パラメーターを Restore-AzureRmRecoveryServicesBackupItem に追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-441">Added TargetResourceGroupName parameter to Restore-AzureRmRecoveryServicesBackupItem.</span></span> <span data-ttu-id="a1232-442">マネージド ディスクの復元先となるリソース グループ。</span><span class="sxs-lookup"><span data-stu-id="a1232-442">The resource group to which the managed disks are restored.</span></span> <span data-ttu-id="a1232-443">マネージド ディスクを含む VM のバックアップに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a1232-443">Applicable to backup of VM with managed disks.</span></span>

#### <a name="azurermrecoveryservicessiterecovery"></a><span data-ttu-id="a1232-444">AzureRM.RecoveryServices.SiteRecovery</span><span class="sxs-lookup"><span data-stu-id="a1232-444">AzureRM.RecoveryServices.SiteRecovery</span></span>
* <span data-ttu-id="a1232-445">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-445">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrediscache"></a><span data-ttu-id="a1232-446">AzureRM.RedisCache</span><span class="sxs-lookup"><span data-stu-id="a1232-446">AzureRM.RedisCache</span></span>
* <span data-ttu-id="a1232-447">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-447">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="a1232-448">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="a1232-448">AzureRM.Relay</span></span>
* <span data-ttu-id="a1232-449">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-449">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-450">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-450">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-451">サブスクリプション スコープでテンプレートのデプロイをサポートします。</span><span class="sxs-lookup"><span data-stu-id="a1232-451">Support template deployment at subscription scope.</span></span> <span data-ttu-id="a1232-452">新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-452">Add new Cmdlets:</span></span>
    - <span data-ttu-id="a1232-453">New-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="a1232-453">New-AzureRmDeployment</span></span>
    - <span data-ttu-id="a1232-454">Get-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="a1232-454">Get-AzureRmDeployment</span></span>
    - <span data-ttu-id="a1232-455">Test-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="a1232-455">Test-AzureRmDeployment</span></span>
    - <span data-ttu-id="a1232-456">Remove-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="a1232-456">Remove-AzureRmDeployment</span></span>
    - <span data-ttu-id="a1232-457">Stop-AzureRmDeployment</span><span class="sxs-lookup"><span data-stu-id="a1232-457">Stop-AzureRmDeployment</span></span>
    - <span data-ttu-id="a1232-458">Save-AzureRmDeploymentTemplate</span><span class="sxs-lookup"><span data-stu-id="a1232-458">Save-AzureRmDeploymentTemplate</span></span>
    - <span data-ttu-id="a1232-459">Get-AzureRmDeploymentOperation</span><span class="sxs-lookup"><span data-stu-id="a1232-459">Get-AzureRmDeploymentOperation</span></span>
* <span data-ttu-id="a1232-460">コンテキストを Set-AzureRmResource に渡したときにエラーがスローされる問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-460">Fix issue where error is thrown when passing a context to Set-AzureRmResource</span></span>
    - https://github.com/Azure/azure-powershell/issues/5705
* <span data-ttu-id="a1232-461">New-AzureRmResourceGroupDeployment の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-461">Fix example in New-AzureRmResourceGroupDeployment</span></span>
* <span data-ttu-id="a1232-462">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-462">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="a1232-463">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="a1232-463">AzureRM.Scheduler</span></span>
* <span data-ttu-id="a1232-464">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-464">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-465">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-465">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-466">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-466">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="a1232-467">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a1232-467">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="a1232-468">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-468">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="a1232-469">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-469">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-470">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-470">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="a1232-471">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-471">AzureRM.Storage</span></span>
* <span data-ttu-id="a1232-472">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-472">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermstreamanalytics"></a><span data-ttu-id="a1232-473">AzureRM.StreamAnalytics</span><span class="sxs-lookup"><span data-stu-id="a1232-473">AzureRM.StreamAnalytics</span></span>
* <span data-ttu-id="a1232-474">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-474">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="a1232-475">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="a1232-475">AzureRM.Tags</span></span>
* <span data-ttu-id="a1232-476">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-476">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="a1232-477">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a1232-477">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="a1232-478">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-478">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermusageaggregates"></a><span data-ttu-id="a1232-479">AzureRM.UsageAggregates</span><span class="sxs-lookup"><span data-stu-id="a1232-479">AzureRM.UsageAggregates</span></span>
* <span data-ttu-id="a1232-480">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-480">Updated to the latest version of the Azure ClientRuntime.</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-481">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-481">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-482">Azure ClientRuntime の最新バージョンに更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-482">Updated to the latest version of the Azure ClientRuntime.</span></span>

## <a name="660---july-2018"></a><span data-ttu-id="a1232-483">6.6.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="a1232-483">6.6.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a1232-484">全般</span><span class="sxs-lookup"><span data-stu-id="a1232-484">General</span></span>
* <span data-ttu-id="a1232-485">完全なパラメーターの種類および正しい入出力の種類が含まれるように、すべてのヘルプ ファイルを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-485">Updated all help files to include full parameter types and correct input/output types.</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="a1232-486">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-486">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-487">リソースの現在の構成とターゲット リソースの間に互換性があることを検証できるように、Common.Strategy ライブラリを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-487">Updated Common.Strategy library to be able to validate that the current config for a resource is compatible with the target resource.</span></span>
* <span data-ttu-id="a1232-488">Common.Storage に ps1xml の種類を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-488">Added ps1xml types to Common.Storage</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="a1232-489">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-489">Azure.Storage</span></span>
* <span data-ttu-id="a1232-490">DefaultProfile からストレージ コンテキストを取得するためのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-490">Added support for getting Storage Context from DefaultProfile</span></span>
* <span data-ttu-id="a1232-491">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-491">Added Ps1XmlAttribute to cmdlets output types properties.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="a1232-492">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a1232-492">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="a1232-493">修正された問題 https://github.com/Azure/azure-powershell/issues/6370</span><span class="sxs-lookup"><span data-stu-id="a1232-493">Fixed issue https://github.com/Azure/azure-powershell/issues/6370</span></span>
    - <span data-ttu-id="a1232-494">PsApiManagementApi が ApiContract に変換されるように、Automapper のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-494">Fixed bug in Automapper to translate PsApiManagementApi to ApiContract</span></span>
* <span data-ttu-id="a1232-495">修正された問題 https://github.com/Azure/azure-powershell/issues/6515</span><span class="sxs-lookup"><span data-stu-id="a1232-495">Fixed issue https://github.com/Azure/azure-powershell/issues/6515</span></span>
    - <span data-ttu-id="a1232-496">エンコードの種類でオーバーロードされないように File.Save のバグを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-496">Fixed bug in File.Save to not overload with Encoding Type</span></span>
* <span data-ttu-id="a1232-497">修正された問題 https://github.com/Azure/azure-powershell/issues/6560</span><span class="sxs-lookup"><span data-stu-id="a1232-497">Fixed issue https://github.com/Azure/azure-powershell/issues/6560</span></span>
    - <span data-ttu-id="a1232-498">Nuget バージョン 4.0.3 にアップグレードしたことで、apiId でのパターンの例外が修正されました</span><span class="sxs-lookup"><span data-stu-id="a1232-498">Upgraded to 4.0.3 Nuget version which fixes the pattern exception on apiId</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-499">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-499">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-500">New-AzureRmVm での DiskFileParameterSet を使用した VM の作成が、PremiumLRS ストレージ アカウントの種類の名前変更が原因で失敗する問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-500">Fix issue with creating a vm using DiskFileParameterSet in New-AzureRmVm failing because of PremiumLRS storage account type renaming.</span></span>
* <span data-ttu-id="a1232-501">Invoke-AzureRmVMRunCommand コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-501">Fix Invoke-AzureRmVMRunCommand cmdlet</span></span>
* <span data-ttu-id="a1232-502">サブスクリプション内のすべての可用性セットを一覧表示できるように、Get-AzureRmAvailabilitySet を更新しました </span><span class="sxs-lookup"><span data-stu-id="a1232-502">Update Get-AzureRmAvailabilitySet to enable list all availability sets in a subscription.</span></span>  <span data-ttu-id="a1232-503">(ResouceGroupName パラメーターは省略可能になりました)。</span><span class="sxs-lookup"><span data-stu-id="a1232-503">(ResouceGroupName parameter is now optional.)</span></span>
* <span data-ttu-id="a1232-504">条件に合う VM で高速ネットワークを有効にできるように "New-AzureRmVm" の SimpleParameterSet を更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-504">Update SimpleParameterSet of 'New-AzureRmVm' to enable Accelerated Network on qualifying vms.</span></span>
* <span data-ttu-id="a1232-505">ユーザーが指定した LB が既に存在する場合 vmss の作成が失敗するように、New-AzureRmVmss の単純なパラメーター セットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-505">Update New-AzureRmVmss simple parameter set to fail creating the vmss when a user specified LB already exists.</span></span>
* <span data-ttu-id="a1232-506">New-AzureRmDisk の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-506">Update example for New-AzureRmDisk</span></span>
* <span data-ttu-id="a1232-507">"New-AzureRmVM" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-507">Add example for 'New-AzureRmVM'</span></span>
* <span data-ttu-id="a1232-508">Set-AzureRmVMOSDisk の説明を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-508">Update description for Set-AzureRmVMOSDisk</span></span>
* <span data-ttu-id="a1232-509">スペルとプレフィックスを修正するために、Set-AzureRmVMBginfoExtension の例 1 を更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-509">Update Example 1 for Set-AzureRmVMBginfoExtension to correct spelling and prefix.</span></span> 

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="a1232-510">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a1232-510">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="a1232-511">ADF .NET SDK のバージョンを 1.1.0 に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-511">Updated the ADF .Net SDK version to 1.1.0.</span></span>
* <span data-ttu-id="a1232-512">データ ファクトリ間でのセルフホステッド統合ランタイムの共有がサポートされました。</span><span class="sxs-lookup"><span data-stu-id="a1232-512">Support self-hosted integration runtime sharing across data factories.</span></span>
     - <span data-ttu-id="a1232-513">新しいパラメーター -SharedIntegrationRuntimeResourceId を Set-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-513">Add new parameter -SharedIntegrationRuntimeResourceId to Set-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>
     - <span data-ttu-id="a1232-514">新しい省略可能なパラメーター -LinkedDataFactoryName を Remove-AzureRmDataFactoryV2IntegrationRuntime コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-514">Add new optional parameter -LinkedDataFactoryName to Remove-AzureRmDataFactoryV2IntegrationRuntime cmdlet.</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="a1232-515">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a1232-515">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="a1232-516">データプレーン SDK (Microsoft.Azure.DataLake.Store) のバージョンを 1.1.9 に更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-516">Updated the DataPlane SDK (Microsoft.Azure.DataLake.Store) version to 1.1.9</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="a1232-517">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="a1232-517">AzureRM.EventHub</span></span>
* <span data-ttu-id="a1232-518">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-518">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>

#### <a name="azurerminsights"></a><span data-ttu-id="a1232-519">AzureRM.Insights</span><span class="sxs-lookup"><span data-stu-id="a1232-519">AzureRM.Insights</span></span>
* <span data-ttu-id="a1232-520">ヘルプ ファイルの OutputType のフォーマットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-520">Fixed formatting of OutputType in help files</span></span>
* <span data-ttu-id="a1232-521">Microsoft.Azure.Management.Monitor SDK 0.19.1-preview を使用します</span><span class="sxs-lookup"><span data-stu-id="a1232-521">Using Microsoft.Azure.Management.Monitor SDK 0.19.1-preview</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="a1232-522">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a1232-522">AzureRM.KeyVault</span></span>
* <span data-ttu-id="a1232-523">Set-AzureRmKeyVaultAccessPolicy のパイプ処理の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-523">Fix piping issue in Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-524">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-524">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-525">LoadBalancerInboundNatPoolConfig コマンドレットの例を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-525">Added examples for LoadBalancerInboundNatPoolConfig cmdlets.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-526">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-526">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-527">"Get-AzureRmResource" のタグ名と値の両方を指定する際の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-527">Fix issue when providing both tag name and value for 'Get-AzureRmResource'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6765
* <span data-ttu-id="a1232-528">"Set-AzureRmResource" を使用するパイプ処理シナリオを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-528">Fix piping scenario with 'Set-AzureRmResource'</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-529">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-529">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-530">削除コマンドレットの InputObject および ResourceId のパイプ処理を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-530">Updated piping for InputObject and ResourceId in remove cmdlets</span></span>
* <span data-ttu-id="a1232-531">いくつかの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-531">fixed few issues</span></span>
    - https://github.com/Azure/azure-powershell/issues/3780
    - https://github.com/Azure/azure-powershell/issues/4340

#### <a name="azurermsql"></a><span data-ttu-id="a1232-532">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-532">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-533">次のコマンドレットでサーバーの Advanced Threat Protection のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-533">Adding Server Advanced Threat Protection support with the following cmdlets:</span></span>
    - <span data-ttu-id="a1232-534">Enable-AzureRmSqlServerAdvancedThreatProtection、Disable-AzureRmSqlServerAdvancedThreatProtection、Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="a1232-534">Enable-AzureRmSqlServerAdvancedThreatProtection; Disable-AzureRmSqlServerAdvancedThreatProtection; Get-AzureRmSqlServerAdvancedThreatProtectionPolicy</span></span>
* <span data-ttu-id="a1232-535">次のコマンドレットで脆弱性評価のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-535">Adding Vulnerability Assessment support with the following cmdlets:</span></span>
    - <span data-ttu-id="a1232-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span><span class="sxs-lookup"><span data-stu-id="a1232-536">Update-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Get-AzureRmSqlDatabaseVulnerabilityAssessmentSettings; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentSettings</span></span>
    - <span data-ttu-id="a1232-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline、Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span><span class="sxs-lookup"><span data-stu-id="a1232-537">Set-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Get-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline; Clear-AzureRmSqlDatabaseVulnerabilityAssessmentRuleBaseline</span></span>
    - <span data-ttu-id="a1232-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan、Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord、Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span><span class="sxs-lookup"><span data-stu-id="a1232-538">Convert-AzureRmSqlDatabaseVulnerabilityAssessmentScan; Get-AzureRmSqlDatabaseVulnerabilityAssessmentScanRecord; Start-AzureRmSqlDatabaseVulnerabilityAssessmentScan</span></span>
* <span data-ttu-id="a1232-539">Remove-AzureRmSqlServerFirewallRule の例を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-539">Fixed example in Remove-AzureRmSqlServerFirewallRule</span></span>
* <span data-ttu-id="a1232-540">Get-AzureSqlSyncGroupLog で米国以外のカルチャの datetime が不適切に処理されていたのを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-540">Fix datetime handling incorrectly for non-us base culture in Get-AzureSqlSyncGroupLog</span></span>

#### <a name="azurermstorage"></a><span data-ttu-id="a1232-541">AzureRM.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-541">AzureRM.Storage</span></span>
* <span data-ttu-id="a1232-542">Ps1XmlAttribute をコマンドレットの出力の種類のプロパティに追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-542">Add Ps1XmlAttribute to cmdlets output types properties</span></span>
* <span data-ttu-id="a1232-543">StorageAccount コマンドレットの出力をテーブル ビューで表示します</span><span class="sxs-lookup"><span data-stu-id="a1232-543">Show StorageAccount cmdlet output in table view</span></span>
    - <span data-ttu-id="a1232-544">Get-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a1232-544">Get-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="a1232-545">New-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a1232-545">New-AzureRmStorageAccount</span></span>
    - <span data-ttu-id="a1232-546">Set-AzureRmStorageAccount</span><span class="sxs-lookup"><span data-stu-id="a1232-546">Set-AzureRmStorageAccount</span></span>

#### <a name="azurermtags"></a><span data-ttu-id="a1232-547">AzureRM.Tags</span><span class="sxs-lookup"><span data-stu-id="a1232-547">AzureRM.Tags</span></span>
* <span data-ttu-id="a1232-548">Tag コマンドレットのヘルプから間違ったステートメントを削除しました</span><span class="sxs-lookup"><span data-stu-id="a1232-548">Remove incorrect statement from Tag cmdlet help</span></span>
    - https://github.com/Azure/azure-powershell/issues/3878

## <a name="650---july-2018"></a><span data-ttu-id="a1232-549">6.5.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="a1232-549">6.5.0 - July 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="a1232-550">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-550">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-551">"Get-AzureRmContextAutosaveSetting" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-551">Updated help for 'Get-AzureRmContextAutosaveSetting'</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="a1232-552">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-552">Azure.Storage</span></span>
* <span data-ttu-id="a1232-553">書き込み専用の SAS トークンを使用した BLOB またはファイルのアップロードがサポートされます</span><span class="sxs-lookup"><span data-stu-id="a1232-553">Support Upload Blob or File with write only Sas token</span></span>
- <span data-ttu-id="a1232-554">Set-AzureStorageBlobContent</span><span class="sxs-lookup"><span data-stu-id="a1232-554">Set-AzureStorageBlobContent</span></span>
- <span data-ttu-id="a1232-555">Set-AzureStorageFileContent</span><span class="sxs-lookup"><span data-stu-id="a1232-555">Set-AzureStorageFileContent</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="a1232-556">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a1232-556">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="a1232-557">必須プロパティ ResourceGroupName を AS に追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-557">Add required property ResourceGroupName to AS.</span></span>

#### <a name="azurermautomation"></a><span data-ttu-id="a1232-558">AzureRM.Automation</span><span class="sxs-lookup"><span data-stu-id="a1232-558">AzureRM.Automation</span></span>
* <span data-ttu-id="a1232-559">"New-AzureRMAutomationSchedule" のヘルプを更新し、例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-559">Update help and add example for 'New-AzureRMAutomationSchedule'</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-560">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-560">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-561">Update/New-AzureRmAvailabilitySet に -Tag パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-561">Add -Tag parameter to Update/New-AzureRmAvailabilitySet</span></span>
* <span data-ttu-id="a1232-562">"Add-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-562">Add example for 'Add-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="a1232-563">"Remove-AzureRmVmssExtension" の例を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-563">Add examples for 'Remove-AzureRmVmssExtension'</span></span>
* <span data-ttu-id="a1232-564">"Set-AzureRmVMAccessExtension" のヘルプを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-564">Update help for 'Set-AzureRmVMAccessExtension'</span></span>
* <span data-ttu-id="a1232-565">New-AzureRmVmss の SimpleParameterSet が更新され、SinglePlacementGroup が既定で false に設定されるようになりました。また、ユーザーが 1 つの配置グループ内に VMSS を作成できるスイッチ パラメーター "SinglePlacementGroup" が追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-565">Update SimpleParameterSet for New-AzureRmVmss to set SinglePlacementGroup to false by default and add switch parameter 'SinglePlacementGroup' that enables the user to create the VMSS in a single placement group.</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="a1232-566">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="a1232-566">AzureRM.EventHub</span></span>
* <span data-ttu-id="a1232-567">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSEventHubDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-567">Added a readonly property 'PendingReplicationOperationsCount' to PSEventHubDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="a1232-568">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a1232-568">AzureRM.KeyVault</span></span>
* <span data-ttu-id="a1232-569">Set-AzureRmKeyVaultAccessPolicy のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-569">Update error message for Set-AzureRmKeyVaultAccessPolicy</span></span>

#### <a name="azurermlogicapp"></a><span data-ttu-id="a1232-570">AzureRM.LogicApp</span><span class="sxs-lookup"><span data-stu-id="a1232-570">AzureRM.LogicApp</span></span>
* <span data-ttu-id="a1232-571">New-AzureRmLogicApp の "parameter set could not be resolved"\(パラメーター セットを解決できませんでした\) というエラーを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-571">Fixed "parameter set could not be resolved" error in New-AzureRmLogicApp</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-572">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-572">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-573">Set/Add-AzureRmVirtualNetworkPeering で、複数のテナントの仮想ネットワーク間のピアリングを有効にしました</span><span class="sxs-lookup"><span data-stu-id="a1232-573">Enable peering across Virtual Networks in multiple Tenants for Set/Add-AzureRmVirtualNetworkPeering</span></span>
* <span data-ttu-id="a1232-574">Application Gateway の次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-574">Updated below cmdlets for Application Gateway</span></span>
    - <span data-ttu-id="a1232-575">New-AzureRmApplicationGateway: EnableFIPS フラグとゾーンのサポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-575">New-AzureRmApplicationGateway : Added EnableFIPS flag and Zones support</span></span>
    - <span data-ttu-id="a1232-576">New-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-576">New-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
    - <span data-ttu-id="a1232-577">Set-AzureRmApplicationGatewaySku: 新しい SKU として、Standard_v2 と WAF_v2 を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-577">Set-AzureRmApplicationGatewaySku : Added new skus Standard_v2 and WAF_v2</span></span>
* <span data-ttu-id="a1232-578">最新のジェネレーター バージョンで RouteTable コマンドレットを再生成しました</span><span class="sxs-lookup"><span data-stu-id="a1232-578">Regenerated RouteTable cmdlets with the latest generator version</span></span>

#### <a name="azurermrelay"></a><span data-ttu-id="a1232-579">AzureRM.Relay</span><span class="sxs-lookup"><span data-stu-id="a1232-579">AzureRM.Relay</span></span>
* <span data-ttu-id="a1232-580">マークダウン ファイルを更新し、例のパラメーター名の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-580">Updated markdown files, fix for the parameter name issue in example</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-581">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-581">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-582">Roleassignment および roledefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-582">Update Roleassignment and roledefinition cmdlets:</span></span>
    - <span data-ttu-id="a1232-583">ページングの一部として実行される追加の roledefinition 呼び出しを削除しました</span><span class="sxs-lookup"><span data-stu-id="a1232-583">Remove extra roledefinition calls done as part of paging.</span></span>
* <span data-ttu-id="a1232-584">Get-AzureRmRoleAssignment コマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-584">Fix Get-AzureRmRoleAssignment cmdlet</span></span>
    - <span data-ttu-id="a1232-585">-ExpandPrincipalGroups コマンド パラメーター機能を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-585">Fix -ExpandPrincipalGroups command parameter functionality</span></span>
* <span data-ttu-id="a1232-586">"-ResourceType" パラメーターで大文字と小文字が区別されていた "Get-AzureRmResource" の問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-586">Fix issue with 'Get-AzureRmResource' where '-ResourceType' parameter was case sensitive</span></span>

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-587">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-587">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-588">コマンドレットを一覧表示するために、top および skip パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-588">Added top and skip parameter to list cmdlets</span></span>
* <span data-ttu-id="a1232-589">Standard から Premium 名前空間への移行コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-589">Added Standard to Premium NameSpace migration cmdlets :</span></span>
    - <span data-ttu-id="a1232-590">Start-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="a1232-590">Start-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="a1232-591">Get-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="a1232-591">Get-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="a1232-592">Complete-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="a1232-592">Complete-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="a1232-593">Stop-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="a1232-593">Stop-AzureRmServiceBusMigration</span></span>
    - <span data-ttu-id="a1232-594">Remove-AzureRmServiceBusMigration</span><span class="sxs-lookup"><span data-stu-id="a1232-594">Remove-AzureRmServiceBusMigration</span></span>
* <span data-ttu-id="a1232-595">レプリケーションの進行中に保留中のレプリケーション操作数を示す読み取り専用プロパティ "PendingReplicationOperationsCount" を、PSServiceBusDRConfigurationAttributes クラスに追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-595">Added a readonly property 'PendingReplicationOperationsCount' to PSServiceBusDRConfigurationAttributes class, which gives the pending replication operations count while replication is in progress</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="a1232-596">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a1232-596">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="a1232-597">"New-AzureRmServiceFabricCluster" の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-597">Update example for 'New-AzureRmServiceFabricCluster'</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="a1232-598">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-598">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-599">ユーザーが SQL Server インスタンスまたはマネージド インスタンスに TDE 証明書を追加できるようにする、Management.Sql の新しいコマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-599">Adding new Cmdlets for Management.Sql to allow customers to add TDE Certificate to Sql Server instance or a Managed Instance</span></span>
    - <span data-ttu-id="a1232-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-600">Add-AzureRmSqlServerTransparentDataEncryptionCertificate</span></span>
    - <span data-ttu-id="a1232-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-601">Add-AzureRmSqlManagedInstanceTransparentDataEncryptionCertificate</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-602">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-602">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-603">`Set-AzureRmWebApp -AssignIdentity` および `Set-AzureRmWebAppSlot -AssignIdentity` を false に設定すると、サイト オブジェクトから Identity プロパティが削除されるようになりました。preview タグも削除されます</span><span class="sxs-lookup"><span data-stu-id="a1232-603">`Set-AzureRmWebApp -AssignIdentity` and  `Set-AzureRmWebAppSlot -AssignIdentity` when set to false will now remove the Identity property from the site object.Removing preview tag as well.</span></span>
* <span data-ttu-id="a1232-604">`Get-AzureRmWebAppMetrics`、`Get-AzureRmAppServicePlanMetrics` の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-604">`Get-AzureRmWebAppMetrics`,`Get-AzureRmAppServicePlanMetrics` example updated</span></span>
* <span data-ttu-id="a1232-605">`Set-AzureRmWebApp -PhpVersion` で、有効な php バージョンとして off がサポートされます</span><span class="sxs-lookup"><span data-stu-id="a1232-605">`Set-AzureRmWebApp -PhpVersion` supports off as a valid php version</span></span>

## <a name="640---july-2018"></a><span data-ttu-id="a1232-606">6.4.0 - 2018 年 7 月</span><span class="sxs-lookup"><span data-stu-id="a1232-606">6.4.0 - July 2018</span></span>
#### <a name="general"></a><span data-ttu-id="a1232-607">全般</span><span class="sxs-lookup"><span data-stu-id="a1232-607">General</span></span>
* <span data-ttu-id="a1232-608">ほとんどのモジュールのヘルプ ファイルで OutputType の書式設定を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-608">Fixed formatting of OutputType in help files for most modules</span></span>

#### <a name="azurermprofile"></a><span data-ttu-id="a1232-609">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-609">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-610">Ps1Xml 属性が基本的な出力の種類に追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-610">Ps1Xml attribute added to the basic output types</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-611">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-611">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-612">VMSS の IP タグ機能</span><span class="sxs-lookup"><span data-stu-id="a1232-612">IP Tag feature for VMSS</span></span>
    - <span data-ttu-id="a1232-613">"New-AzureRmVmssIpTagConfig" コマンドレットが追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-613">'New-AzureRmVmssIpTagConfig' cmdlet is added</span></span>
    - <span data-ttu-id="a1232-614">IpTag パラメーターが New-AzureRmVmssIpConfig に追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-614">IpTag parameter is added to New-AzureRmVmssIpConfig</span></span>
* <span data-ttu-id="a1232-615">VMSS の自動 OS ロールバック機能</span><span class="sxs-lookup"><span data-stu-id="a1232-615">Auto OS Rollback feature for VMSS</span></span>
    - <span data-ttu-id="a1232-616">DisableAutoRollback パラメーターが New-AzureRmVmssConfig と Update-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-616">DisableAutoRollback parameters are added to New-AzureRmVmssConfig and Update-AzureRmVmss</span></span>
* <span data-ttu-id="a1232-617">VMSS の OS アップグレード履歴機能</span><span class="sxs-lookup"><span data-stu-id="a1232-617">OS Upgrade History feature for Vmss</span></span>
    - <span data-ttu-id="a1232-618">OSUpgradeHistory スイッチ パラメーターが Get-AzureRmVmss に追加されました</span><span class="sxs-lookup"><span data-stu-id="a1232-618">OSUpgradeHistory switch parameter is added to Get-AzureRmVmss</span></span>

#### <a name="azurermdatalakeanalytics"></a><span data-ttu-id="a1232-619">AzureRM.DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="a1232-619">AzureRM.DataLakeAnalytics</span></span>
* <span data-ttu-id="a1232-620">次のコマンドでカタログ ACL に対応するようになりました。</span><span class="sxs-lookup"><span data-stu-id="a1232-620">Add support for Catalog ACLs through the following commands:</span></span>
    - <span data-ttu-id="a1232-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="a1232-621">Get-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="a1232-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="a1232-622">Set-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>
    - <span data-ttu-id="a1232-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span><span class="sxs-lookup"><span data-stu-id="a1232-623">Remove-AzureRmDataLakeAnalyticsCatalogItemAclEntry</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="a1232-624">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a1232-624">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="a1232-625">Set-AzureRmDataLakeStoreItemAclEntry、Remove-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl でキャンセルと進捗状況の追跡に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="a1232-625">Add cancellation support and progress tracking for Set-AzureRmDataLakeStoreItemAclEntry, Remove-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl</span></span>
* <span data-ttu-id="a1232-626">Export-AzureRmDataLakeStoreChildItemProperties でキャンセルに対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="a1232-626">Add cancellation support for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="a1232-627">再帰的な操作を行うコマンドレットのデバッグ メッセージのフラッシュを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-627">Fix flushing of debug messages for cmdlets that does recursive operations</span></span>
* <span data-ttu-id="a1232-628">DataLake コマンドレットのテストの場所を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-628">Fix location of test of DataLake cmdlets</span></span>

#### <a name="azurermeventhub"></a><span data-ttu-id="a1232-629">AzureRM.EventHub</span><span class="sxs-lookup"><span data-stu-id="a1232-629">AzureRM.EventHub</span></span>
* <span data-ttu-id="a1232-630">省略可能な MaxCount パラメーターを、List 操作の Get-AzureRmEventHub コマンドレットと Get-AzureRmEventHubConsumerGroup コマンドレットに追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-630">Added Optional MaxCount parameter to List Operations cmdlet Get-AzureRmEventHub and Get-AzureRmEventHubConsumerGroup</span></span>
* <span data-ttu-id="a1232-631">新しい EventHub を作成するときに少なくとも 1 つのパラメーターが必要だった New-AzureRmEventHub コマンドレットの問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-631">Fixed issue in New-AzureRmEventHub cmdlet where at least one parameter needed while creating New EventHub.</span></span> <span data-ttu-id="a1232-632">既定のパラメーター セットが提供されます。</span><span class="sxs-lookup"><span data-stu-id="a1232-632">Provided Default Parameter set.</span></span>
* <span data-ttu-id="a1232-633">省略可能な Parameter -KeyValue を New-AzureRmEventHubKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="a1232-633">Added optional Parameter -KeyValue to New-AzureRmEventHubKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="a1232-634">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a1232-634">AzureRM.KeyVault</span></span>
* <span data-ttu-id="a1232-635">Get-AzureRmKeyVault -Tag によりすべてのリソースが返されていた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-635">Fix issue where all resources were being returned by Get-AzureRmKeyVault -Tag</span></span>

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-636">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-636">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-637">ゾーン冗長 VirtualNetworkGateways の新しい SKU を公開しました</span><span class="sxs-lookup"><span data-stu-id="a1232-637">Expose new Skus for Zone-Redundant VirtualNetworkGateways</span></span>
* <span data-ttu-id="a1232-638">ARM を介した ExpressRoute パートナー API 機能の新しいコマンドを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-638">Added new commands for feature: ExpressRoute Partner APIs via ARM</span></span>
    - <span data-ttu-id="a1232-639">Get-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-639">Added Get-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="a1232-640">Set-AzureRmExpressRouteCrossConnection を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-640">Added Set-AzureRmExpressRouteCrossConnection</span></span>
    - <span data-ttu-id="a1232-641">Add-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-641">Added Add-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="a1232-642">Get-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-642">Added Get-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="a1232-643">Remove-AzureRmExpressRouteCrossConnectionPeering を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-643">Added Remove-AzureRmExpressRouteCrossConnectionPeering</span></span>
    - <span data-ttu-id="a1232-644">Get-AzureRMExpressRouteCrossConnectionArpTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-644">Added Get-AzureRMExpressRouteCrossConnectionArpTable</span></span>
    - <span data-ttu-id="a1232-645">Get-AzureRMExpressRouteCrossConnectionRouteTable を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-645">Added Get-AzureRMExpressRouteCrossConnectionRouteTable</span></span>
    - <span data-ttu-id="a1232-646">Get-AzureRMExpressRouteCrossConnectionRouteTableSummary を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-646">Added Get-AzureRMExpressRouteCrossConnectionRouteTableSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="a1232-647">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a1232-647">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a1232-648">Get-AzureRmRecoveryServicesBackupStatus コマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-648">Added Get-AzureRmRecoveryServicesBackupStatus cmdlet.</span></span> <span data-ttu-id="a1232-649">このコマンドレットは VM ID を取得し、その VM が、サブスクリプションのコンテナーによって保護されているかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="a1232-649">This cmdlet takes a VM ID and checks if the VM is protected by some vault in the subscription.</span></span> <span data-ttu-id="a1232-650">このようなコンテナーが存在する場合、コマンドレットによって、そのコンテナーの詳細が出力されます。</span><span class="sxs-lookup"><span data-stu-id="a1232-650">If there exists such a vault, the cmdlet outputs the vault details.</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-651">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-651">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-652">Get-AzureRmPolicyAssignment コマンドレットを更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-652">Update Get-AzureRmPolicyAssignment cmdlets:</span></span>
    - <span data-ttu-id="a1232-653">管理グループ レベルでの -Scope 値の一覧表示に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="a1232-653">Add support for listing -Scope values at management group level</span></span>
    - <span data-ttu-id="a1232-654">管理グループ レベルでの -Scope 値を含む個別の割り当ての取得に対応するようになりました</span><span class="sxs-lookup"><span data-stu-id="a1232-654">Add support for retrieving individual assignments with -Scope values at management group level</span></span>
    - <span data-ttu-id="a1232-655">パラメーターを制御するための -Effective スイッチと -All スイッチを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-655">Add -Effective and -All switches to control  parameter</span></span>
* <span data-ttu-id="a1232-656">Get/New/Remove/Set-AzureRmPolicyDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-656">Update Get/New/Remove/Set-AzureRmPolicyDefinition cmdlets</span></span>
    - <span data-ttu-id="a1232-657">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-657">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="a1232-658">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-658">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="a1232-659">Get/New/Remove/Set-AzureRmPolicySetDefinition コマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-659">Update Get/New/Remove/Set-AzureRmPolicySetDefinition cmdlets</span></span>
    - <span data-ttu-id="a1232-660">指定した管理グループに操作を適用するための -ManagementGroupName パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-660">Add -ManagementGroupName parameter to apply operations to a given management group</span></span>
    - <span data-ttu-id="a1232-661">指定したサブスクリプションに操作を適用するための -SubscriptionId パラメーターを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-661">Add -SubscriptionId parameter to apply operations to a given subscription</span></span>
* <span data-ttu-id="a1232-662">"New-AzureRmResourceGroupDeployment" で "TemplateParameterObject" を使用するときの、パラメーターでの KeyVault シークレット参照サポートを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-662">Add KeyVault secret reference support in parameters when using 'TemplateParameterObject' in 'New-AzureRmResourceGroupDeployment'</span></span>
* <span data-ttu-id="a1232-663">"New-AzureRmADAppCredential" で "-EndDate" パラメーターが無視される問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-663">Fix issue where '-EndDate' parameter was ignored for 'New-AzureRmADAppCredential'</span></span>
    - https://github.com/Azure/azure-powershell/issues/6505
* <span data-ttu-id="a1232-664">"Add-AzureRmADGroupMember" が誤った URL を使用して要求を行う問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-664">Fix issue where 'Add-AzureRmADGroupMember' used incorrect URL to make request</span></span>
    - https://github.com/Azure/azure-powershell/issues/6485

#### <a name="azurermservicebus"></a><span data-ttu-id="a1232-665">AzureRM.ServiceBus</span><span class="sxs-lookup"><span data-stu-id="a1232-665">AzureRM.ServiceBus</span></span>
* <span data-ttu-id="a1232-666">省略可能な Parameter -KeyValue を New-AzureRmServiceBusKey コマンドレットに追加しました。これによりユーザーが KeyValue を提供できます。</span><span class="sxs-lookup"><span data-stu-id="a1232-666">Added optional Parameter -KeyValue to New-AzureRmServiceBusKey cmdlet, which enables user to provide KeyValue.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="a1232-667">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-667">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-668">New-AzureRmSqlDatabaseRestorePoint ヘルプの SQLDW に対するユーザー定義の復元ポイントを明確化しました</span><span class="sxs-lookup"><span data-stu-id="a1232-668">Clarified User-Defined Restore Points for SQLDW in New-AzureRmSqlDatabaseRestorePoint help</span></span>
* <span data-ttu-id="a1232-669">複数のコマンドレットの -ComputeGeneration パラメーターのドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-669">Updated documentation of -ComputeGeneration parameter in several cmdlets</span></span>

## <a name="630---june-2018"></a><span data-ttu-id="a1232-670">6.3.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="a1232-670">6.3.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="a1232-671">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-671">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-672">Enable-AzureRmContextAutoSave のエラー メッセージを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-672">Updated error messages for Enable-AzureRmContextAutoSave</span></span>
* <span data-ttu-id="a1232-673">以前のコンテキストなしで "Connect-AzureRmAccount" を実行すると、サブスクリプションごとにコンテキストが作成されます</span><span class="sxs-lookup"><span data-stu-id="a1232-673">Create a context for each subscription when running 'Connect-AzureRmAccount' with no previous context</span></span>

#### <a name="azurestorage"></a><span data-ttu-id="a1232-674">Azure.Storage</span><span class="sxs-lookup"><span data-stu-id="a1232-674">Azure.Storage</span></span>
* <span data-ttu-id="a1232-675">-Permissions パラメーターに関する追加情報をヘルプ ファイルに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-675">Added additional information about -Permissions parameter in help files.</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-676">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-676">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-677">"Get-AzureRmVmDiskEncryptionStatus" で、データ ディスクのない VM で発生していた問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-677">'Get-AzureRmVmDiskEncryptionStatus' fixes an issue observed for VMs with no data disks</span></span> 
* <span data-ttu-id="a1232-678">Compute クライアント ライブラリ バージョンを更新し、次のコマンドレットを修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-678">Update Compute client library version to fix following cmdlets</span></span>
    - <span data-ttu-id="a1232-679">Grant-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="a1232-679">Grant-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="a1232-680">Grant-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="a1232-680">Grant-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="a1232-681">Save-AzureRmVMImage</span><span class="sxs-lookup"><span data-stu-id="a1232-681">Save-AzureRmVMImage</span></span>
* <span data-ttu-id="a1232-682">"操作 ID" と "操作の状態" が正しく表示されるように、次のコマンドレットを修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-682">Fixed following cmdlets to show 'operation ID' and 'operation status' correctly:</span></span>
    - <span data-ttu-id="a1232-683">Start-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="a1232-683">Start-AzureRmVM</span></span>
    - <span data-ttu-id="a1232-684">Stop-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="a1232-684">Stop-AzureRmVM</span></span>
    - <span data-ttu-id="a1232-685">Restart-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="a1232-685">Restart-AzureRmVM</span></span>
    - <span data-ttu-id="a1232-686">Set-AzureRmVM</span><span class="sxs-lookup"><span data-stu-id="a1232-686">Set-AzureRmVM</span></span>
    - <span data-ttu-id="a1232-687">Remove-AzuerRmVM</span><span class="sxs-lookup"><span data-stu-id="a1232-687">Remove-AzuerRmVM</span></span>
    - <span data-ttu-id="a1232-688">Set-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="a1232-688">Set-AzureRmVmss</span></span>
    - <span data-ttu-id="a1232-689">Start-AzureRmVmssRollingOSUpgrade</span><span class="sxs-lookup"><span data-stu-id="a1232-689">Start-AzureRmVmssRollingOSUpgrade</span></span>
    - <span data-ttu-id="a1232-690">Stop-AzureRmVmssRollingUpgrade</span><span class="sxs-lookup"><span data-stu-id="a1232-690">Stop-AzureRmVmssRollingUpgrade</span></span>
    - <span data-ttu-id="a1232-691">Start-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="a1232-691">Start-AzureRmVmss</span></span>
    - <span data-ttu-id="a1232-692">Restart-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="a1232-692">Restart-AzureRmVmss</span></span>
    - <span data-ttu-id="a1232-693">Stop-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="a1232-693">Stop-AzureRmVmss</span></span>
    - <span data-ttu-id="a1232-694">Remove-AzureRmVmss</span><span class="sxs-lookup"><span data-stu-id="a1232-694">Remove-AzureRmVmss</span></span>
    - <span data-ttu-id="a1232-695">ConvertTo-AzureRmVMManagedDisk</span><span class="sxs-lookup"><span data-stu-id="a1232-695">ConvertTo-AzureRmVMManagedDisk</span></span>
    - <span data-ttu-id="a1232-696">Revoke-AzureRmSnapshotAccess</span><span class="sxs-lookup"><span data-stu-id="a1232-696">Revoke-AzureRmSnapshotAccess</span></span>
    - <span data-ttu-id="a1232-697">Remove-AzureRmSnapshot</span><span class="sxs-lookup"><span data-stu-id="a1232-697">Remove-AzureRmSnapshot</span></span>
    - <span data-ttu-id="a1232-698">Revoke-AzureRmDiskAccess</span><span class="sxs-lookup"><span data-stu-id="a1232-698">Revoke-AzureRmDiskAccess</span></span>
    - <span data-ttu-id="a1232-699">Remove-AzureRmDisk</span><span class="sxs-lookup"><span data-stu-id="a1232-699">Remove-AzureRmDisk</span></span>
    - <span data-ttu-id="a1232-700">Remove-AzureRmContainerService</span><span class="sxs-lookup"><span data-stu-id="a1232-700">Remove-AzureRmContainerService</span></span>
    - <span data-ttu-id="a1232-701">Remove-AzureRmAvailabilitySet</span><span class="sxs-lookup"><span data-stu-id="a1232-701">Remove-AzureRmAvailabilitySet</span></span>

#### <a name="azurermeventgrid"></a><span data-ttu-id="a1232-702">AzureRM.EventGrid</span><span class="sxs-lookup"><span data-stu-id="a1232-702">AzureRM.EventGrid</span></span>
* <span data-ttu-id="a1232-703">Update-AzureRmEventGridSubscription コマンドレットの SubjectBeginsWith/SubjectEndsWith の ValidateNotNullOrEmpty 検証条件が削除され、必要に応じてこれらのパラメーターを空の文字列に変更できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a1232-703">Remove ValidateNotNullOrEmpty validation conditions for SubjectBeginsWith/SubjectEndsWith in Update-AzureRmEventGridSubscription cmdlet to allow changing these parameters to empty string if needed.</span></span>

#### <a name="azurermkeyvault"></a><span data-ttu-id="a1232-704">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a1232-704">AzureRM.KeyVault</span></span>
* <span data-ttu-id="a1232-705">Get-AzureRmKeyVault -Tag を実行したときにタグが返されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-705">Fix issue where no Tags are being returned when Get-AzureRmKeyVault -Tag is run</span></span>

#### <a name="azurermpolicyinsights"></a><span data-ttu-id="a1232-706">AzureRM.PolicyInsights</span><span class="sxs-lookup"><span data-stu-id="a1232-706">AzureRM.PolicyInsights</span></span>
* <span data-ttu-id="a1232-707">Policy Insights コマンドレットのパブリック リリース</span><span class="sxs-lookup"><span data-stu-id="a1232-707">Public release of Policy Insights cmdlets</span></span>
    - <span data-ttu-id="a1232-708">API バージョン 2018-04-04 を使用します</span><span class="sxs-lookup"><span data-stu-id="a1232-708">Use API version 2018-04-04</span></span>
    - <span data-ttu-id="a1232-709">Get-AzureRmPolicyStateSummary の結果に PolicyDefinitionReferenceId を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-709">Add PolicyDefinitionReferenceId to the results of Get-AzureRmPolicyStateSummary</span></span>

#### <a name="azurermrecoveryservicesbackup"></a><span data-ttu-id="a1232-710">AzureRM.RecoveryServices.Backup</span><span class="sxs-lookup"><span data-stu-id="a1232-710">AzureRM.RecoveryServices.Backup</span></span>
* <span data-ttu-id="a1232-711">RecoveryServices.Backup コマンドレットに -Vault パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-711">Added -Vault parameter to RecoveryServices.Backup cmdlets.</span></span> <span data-ttu-id="a1232-712">このパラメーターが渡されると、Set-AzureRmRecoveryServicesContext コマンドレットがオーバーライドされます。</span><span class="sxs-lookup"><span data-stu-id="a1232-712">When passed, this will override the Set-AzureRmRecoveryServicesContext cmdlet.</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="a1232-713">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-713">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-714">Get-AzureRmSqlDatabaseExpanded のヘルプ ファイル内の例を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-714">Updated example in the help file for Get-AzureRmSqlDatabaseExpanded</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="a1232-715">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a1232-715">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="a1232-716">Add-AzureRmTrafficManagerEndpointConfig のヘルプ ファイルを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-716">Updated the help file for Add-AzureRmTrafficManagerEndpointConfig</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-717">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-717">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-718">-AssignIdentity の使用時に AppSettings が上書きされないように、"Set-AzureRmWebApp" が更新されました</span><span class="sxs-lookup"><span data-stu-id="a1232-718">'Set-AzureRmWebApp' is updated to not overwrite the AppSettings when using -AssignIdentity</span></span>
* <span data-ttu-id="a1232-719">省略可能なパラメーターとして AppServicePlan を優先するように、"New-AzureRmWebAppSlot" が更新されました</span><span class="sxs-lookup"><span data-stu-id="a1232-719">'New-AzureRmWebAppSlot' is updated to honor AppServicePlan as an optional parameter</span></span>

## <a name="621---june-2018"></a><span data-ttu-id="a1232-720">6.2.1 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="a1232-720">6.2.1 - June 2018</span></span>
### <a name="azurermoperationalinsights"></a><span data-ttu-id="a1232-721">AzureRM.OperationalInsights</span><span class="sxs-lookup"><span data-stu-id="a1232-721">AzureRM.OperationalInsights</span></span>
* <span data-ttu-id="a1232-722">Network で型をパラメーターとして使用できるように PSWorkspace モデルを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-722">Updated PSWorkspace model to allow Network to use type as a parameter</span></span>

## <a name="620---june-2018"></a><span data-ttu-id="a1232-723">6.2.0 - 2018 年 6 月</span><span class="sxs-lookup"><span data-stu-id="a1232-723">6.2.0 - June 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="a1232-724">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-724">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-725">モジュールのインポート時に Newtonsoft.Json バージョン 10.0.3 が読み込まれない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-725">Fix issue where version 10.0.3 of Newtonsoft.Json wasn't being loaded on module import</span></span>

#### <a name="azurermcompute"></a><span data-ttu-id="a1232-726">AzureRM.Compute</span><span class="sxs-lookup"><span data-stu-id="a1232-726">AzureRM.Compute</span></span>
* <span data-ttu-id="a1232-727">VMSS VM 更新プログラムの機能</span><span class="sxs-lookup"><span data-stu-id="a1232-727">VMSS VM Update feature</span></span>
    - <span data-ttu-id="a1232-728">"Update-AzureRmVmssVM" コマンドレットと "New-AzureRmVMDataDisk" コマンドレットを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-728">Added 'Update-AzureRmVmssVM' and 'New-AzureRmVMDataDisk' cmdlets</span></span>
    - <span data-ttu-id="a1232-729">Vmss VM へのデータ ディスクの追加がサポートされるように、VirtualMachineScaleSetVM パラメーターを "Add-AzureRmVMDataDisk" コマンドレットに追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-729">Add VirtualMachineScaleSetVM parameter to 'Add-AzureRmVMDataDisk' cmdlet to support adding a data disk to Vmss VM.</span></span>

#### <a name="azurermdatafactoryv2"></a><span data-ttu-id="a1232-730">AzureRM.DataFactoryV2</span><span class="sxs-lookup"><span data-stu-id="a1232-730">AzureRM.DataFactoryV2</span></span>
* <span data-ttu-id="a1232-731">ADF .Net SDK バージョンを、次の変更を含む 0.8.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-731">Updated the ADF .Net SDK version to 0.8.0-preview containing following changes:</span></span>
    - <span data-ttu-id="a1232-732">ファクトリ リポジトリの構成操作を追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-732">Added Configure factory repository operation</span></span>
    - <span data-ttu-id="a1232-733">expose consumerKey プロパティおよび consumerSecret プロパティが公開されるように QuickBooks LinkedService を更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-733">Updated QuickBooks LinkedService to expose consumerKey and consumerSecret properties</span></span>
    - <span data-ttu-id="a1232-734">モデルの型をいくつか SecretBase から Object に更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-734">Updated Several model types from SecretBase to Object</span></span>
    - <span data-ttu-id="a1232-735">BLOB イベント トリガーを追加しました</span><span class="sxs-lookup"><span data-stu-id="a1232-735">Added Blob Events trigger</span></span>

### <a name="azurermkeyvault"></a><span data-ttu-id="a1232-736">AzureRM.KeyVault</span><span class="sxs-lookup"><span data-stu-id="a1232-736">AzureRM.KeyVault</span></span>
* <span data-ttu-id="a1232-737">出力例に関してドキュメントを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-737">Update documentation with example output</span></span>

### <a name="azurermnetwork"></a><span data-ttu-id="a1232-738">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-738">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-739">Network Watcher コマンドレットで Traffic Analytics パラメーターを有効にしました</span><span class="sxs-lookup"><span data-stu-id="a1232-739">Enable Traffic Analytics parameters on Network Watcher cmdlets</span></span>

#### <a name="azurermresources"></a><span data-ttu-id="a1232-740">AzureRM.Resources</span><span class="sxs-lookup"><span data-stu-id="a1232-740">AzureRM.Resources</span></span>
* <span data-ttu-id="a1232-741">"Get-AzureRmResource" から返される "PSResource" オブジェクトの "Properties" プロパティの問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-741">Fix issue with 'Properties' property of 'PSResource' object(s) returned from 'Get-AzureRmResource'</span></span>

#### <a name="azurermscheduler"></a><span data-ttu-id="a1232-742">AzureRM.Scheduler</span><span class="sxs-lookup"><span data-stu-id="a1232-742">AzureRM.Scheduler</span></span>
* <span data-ttu-id="a1232-743">ServiceBusQueueJob の更新で新しい Auth 値が設定されない問題を修正しました</span><span class="sxs-lookup"><span data-stu-id="a1232-743">Fix issue with update ServiceBusQueueJob not setting new Auth values</span></span>

### <a name="azurermsql"></a><span data-ttu-id="a1232-744">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-744">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-745">省略可能な LicenseType パラメーターに関して次のコマンドレットを更新しました</span><span class="sxs-lookup"><span data-stu-id="a1232-745">Updated the following cmdlets with optional LicenseType parameter</span></span>
    - <span data-ttu-id="a1232-746">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="a1232-746">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="a1232-747">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="a1232-747">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="a1232-748">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="a1232-748">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="a1232-749">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="a1232-749">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="a1232-750">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="a1232-750">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermwebsites"></a><span data-ttu-id="a1232-751">AzureRM.Websites</span><span class="sxs-lookup"><span data-stu-id="a1232-751">AzureRM.Websites</span></span>
* <span data-ttu-id="a1232-752">Strategy ライブラリの共通アルゴリズムが使用されるように "New-AzureRMWebApp" が更新されました。</span><span class="sxs-lookup"><span data-stu-id="a1232-752">'New-AzureRMWebApp' is updated to use common algorithms from the Strategy library.</span></span>

## <a name="610---may-2018"></a><span data-ttu-id="a1232-753">6.1.0 - 2018 年 5 月</span><span class="sxs-lookup"><span data-stu-id="a1232-753">6.1.0 - May 2018</span></span>
#### <a name="azurermprofile"></a><span data-ttu-id="a1232-754">AzureRM.Profile</span><span class="sxs-lookup"><span data-stu-id="a1232-754">AzureRM.Profile</span></span>
* <span data-ttu-id="a1232-755">"Clear-AzureRmContext" を実行したときに、以前の既定のコンテキストの名前で空のコンテキストが保持され、ユーザーが古い名前で新しいコンテキストを作成できなかった問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-755">Fix issue where running 'Clear-AzureRmContext' would keep an empty context with the name of the previous default context, which prevented the user from creating a new context with the old name</span></span>

#### <a name="azurermanalysisservices"></a><span data-ttu-id="a1232-756">AzureRM.AnalysisServices</span><span class="sxs-lookup"><span data-stu-id="a1232-756">AzureRM.AnalysisServices</span></span>
* <span data-ttu-id="a1232-757">AS 上でのゲートウェイの関連付け/関連付け解除操作を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a1232-757">Enable Gateway assocaite/disassociate operations on AS.</span></span>

#### <a name="azurermapimanagement"></a><span data-ttu-id="a1232-758">AzureRM.ApiManagement</span><span class="sxs-lookup"><span data-stu-id="a1232-758">AzureRM.ApiManagement</span></span>
* <span data-ttu-id="a1232-759">ApiVersions、ApiReleases、ApiRevisions のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-759">Added support for ApiVersions, ApiReleases and ApiRevisions</span></span>
* <span data-ttu-id="a1232-760">ServiceFabric Backend のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-760">Added suppport for ServiceFabric Backend</span></span>
* <span data-ttu-id="a1232-761">Application Insights Logger のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-761">Added support for Application Insights Logger</span></span>
* <span data-ttu-id="a1232-762">API Management サービスの有効な SKU として "Basic" SKU が認識されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a1232-762">Added support for recognizing 'Basic' sku as a valid sku of Api Management service</span></span>
* <span data-ttu-id="a1232-763">プライベート CA によってルートまたは CA として発行された証明書のインストールのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-763">Added support for installing Certificates issued by private CA as Root or CA</span></span>
* <span data-ttu-id="a1232-764">KeyVault および複数のプロキシ ホスト名を使用した、カスタム SSL 証明書の受け入れのサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-764">Added support for accepting Custom SSL certificates via KeyVault and Multiple proxy hostnames</span></span>
* <span data-ttu-id="a1232-765">MSI ID のサポートを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-765">Added support for MSI identity</span></span>
* <span data-ttu-id="a1232-766">URL を使用したポリシーの受け入れのサポートを追加しました。次のコマンドレットは、今後のリリースで非推奨になる予定です。</span><span class="sxs-lookup"><span data-stu-id="a1232-766">Added support for accepting Policies via Url NOTE: The following cmdlets will be deprecated in future release</span></span>
   - <span data-ttu-id="a1232-767">Import-AzureRmApiManagementHostnameCertificate</span><span class="sxs-lookup"><span data-stu-id="a1232-767">Import-AzureRmApiManagementHostnameCertificate</span></span>
   - <span data-ttu-id="a1232-768">New-AzureRmApiManagementHostnameConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-768">New-AzureRmApiManagementHostnameConfiguration</span></span>
   - <span data-ttu-id="a1232-769">Set-AzureRmApiManagementHostnames</span><span class="sxs-lookup"><span data-stu-id="a1232-769">Set-AzureRmApiManagementHostnames</span></span>
   - <span data-ttu-id="a1232-770">Update-AzureRmApiManagementDeployment</span><span class="sxs-lookup"><span data-stu-id="a1232-770">Update-AzureRmApiManagementDeployment</span></span>

#### <a name="azurermbatch"></a><span data-ttu-id="a1232-771">AzureRM.Batch</span><span class="sxs-lookup"><span data-stu-id="a1232-771">AzureRM.Batch</span></span>
* <span data-ttu-id="a1232-772">新しい Get-AzureBatchPoolNodeCounts コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="a1232-772">Release new cmdlet Get-AzureBatchPoolNodeCounts</span></span>
* <span data-ttu-id="a1232-773">新しい Start-AzureBatchComputeNodeServiceLogUpload コマンドレットをリリースしました。</span><span class="sxs-lookup"><span data-stu-id="a1232-773">Release new cmdlet Start-AzureBatchComputeNodeServiceLogUpload</span></span>

#### <a name="azurermconsumption"></a><span data-ttu-id="a1232-774">AzureRM.Consumption</span><span class="sxs-lookup"><span data-stu-id="a1232-774">AzureRM.Consumption</span></span>
* <span data-ttu-id="a1232-775">Get-AzureRmConsumptionUsageDetail コマンドレットの新しいパラメーターとして、Expand、ResourceGroup、InstanceName、InstanceId、Tags、Top を追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-775">Add new parameters Expand, ResourceGroup, InstanceName, InstanceId, Tags, and Top on Cmdlet Get-AzureRmConsumptionUsageDetail</span></span>

#### <a name="azurermdatalakestore"></a><span data-ttu-id="a1232-776">AzureRM.DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="a1232-776">AzureRM.DataLakeStore</span></span>
* <span data-ttu-id="a1232-777">Export-AzureRmDataLakeStoreChildItemProperties の例を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-777">Fix example for Export-AzureRmDataLakeStoreChildItemProperties</span></span>
* <span data-ttu-id="a1232-778">Set-AzureRmDataLakeStoreItemAclEntry の再帰処理での null パラメーター例外を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-778">Fix null parameter exception for Recurse case in Set-AzureRmDataLakeStoreItemAclEntry</span></span> 
* <span data-ttu-id="a1232-779">Set-AzureRmDataLakeStoreItemAclEntry、Set-AzureRmDataLakeStoreItemAcl、Remove-AzureRmDataLakeStoreItemAclEntry のヘルプ ファイルを修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-779">Fix the help files for Set-AzureRmDataLakeStoreItemAclEntry, Set-AzureRmDataLakeStoreItemAcl, Remove-AzureRmDataLakeStoreItemAclEntry</span></span> 

#### <a name="azurermnetwork"></a><span data-ttu-id="a1232-780">AzureRM.Network</span><span class="sxs-lookup"><span data-stu-id="a1232-780">AzureRM.Network</span></span>
* <span data-ttu-id="a1232-781">Network SDK バージョンを 18.0.0-preview から 19.0.0-preview に更新しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-781">Bump up Network SDK version from 18.0.0-preview to 19.0.0-preview</span></span>
* <span data-ttu-id="a1232-782">プロトコル構成を作成するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-782">Added cmdlet to create protocol configuration</span></span>
    - <span data-ttu-id="a1232-783">New-AzureRmNetworkWatcherProtocolConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1232-783">New-AzureRmNetworkWatcherProtocolConfiguration</span></span>
* <span data-ttu-id="a1232-784">既存の Express Route 回線に新しい回線接続を追加するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-784">Added cmdlet to add a new circuit connection to an existing express route circuit.</span></span>
    - <span data-ttu-id="a1232-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-785">Add-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="a1232-786">既存の Express Route 回線から回線接続を削除するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-786">Added cmdlet to remove a circuit connection from an existing express route circuit.</span></span>
    - <span data-ttu-id="a1232-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-787">Remove-AzureRmExpressRouteCircuitConnectionConfig</span></span>
* <span data-ttu-id="a1232-788">回路接続を取得するコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-788">Added cmdlet to retrieve a circuit connection</span></span>
    - <span data-ttu-id="a1232-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span><span class="sxs-lookup"><span data-stu-id="a1232-789">Get-AzureRmExpressRouteCircuitConnectionConfig</span></span>

#### <a name="azurermservicefabric"></a><span data-ttu-id="a1232-790">AzureRM.ServiceFabric</span><span class="sxs-lookup"><span data-stu-id="a1232-790">AzureRM.ServiceFabric</span></span>
* <span data-ttu-id="a1232-791">生成された証明書によるサーバー認証の使用方法を修正しました (問題 #5998)。</span><span class="sxs-lookup"><span data-stu-id="a1232-791">Fixed server authentication usage with generated certificates (Issue #5998)</span></span>

#### <a name="azurermsql"></a><span data-ttu-id="a1232-792">AzureRM.Sql</span><span class="sxs-lookup"><span data-stu-id="a1232-792">AzureRM.Sql</span></span>
* <span data-ttu-id="a1232-793">Auditing コマンドレットが更新され、AuditActions または AuditActionGroups を削除できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a1232-793">Updated Auditing cmdlets to allow removing AuditActions or AuditActionGroups</span></span>
* <span data-ttu-id="a1232-794">新しい柔軟なリテンション ポリシーの設定時に、"Configure long term retention policy with azure recovery service vault and policy is no longer supported. Please submit request with the new flexible retention policy"\(Azure Recovery Service コンテナーで長期リテンション ポリシーが構成されていますが、このポリシーはサポートされなくなりました。新しい柔軟なリテンション ポリシーを使用して要求を送信してください\) というエラーでコマンドが失敗する、</span><span class="sxs-lookup"><span data-stu-id="a1232-794">Fixed issue with Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy when setting a new flexible retention policy where the command would fail with 'Configure long term retention policy with azure recovery service vault and policy is no longer supported.</span></span> <span data-ttu-id="a1232-795">Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy の問題を修正しました。</span><span class="sxs-lookup"><span data-stu-id="a1232-795">Please submit request with the new flexible retention policy'.</span></span>
* <span data-ttu-id="a1232-796">新しい Database API を使用するために、Azure SQL Database/ElasticPool の作成/更新関連のすべてのコマンドレットが更新されました。これにより、スケールおよびレベル関連のプロパティで SKU プロパティがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="a1232-796">Update all Azure Sql Database/ElasticPool Creation/Update related cmdlets to use the new Database API, which support Sku property for scale and tier-related properties.</span></span>
* <span data-ttu-id="a1232-797">更新されたコマンドレットは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="a1232-797">The updated cmdlets including:</span></span> 
    - <span data-ttu-id="a1232-798">New-AzureRmSqlDatabase、Set-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="a1232-798">New-AzureRmSqlDatabase; Set-AzureRmSqlDatabase</span></span>
    - <span data-ttu-id="a1232-799">New-AzureRmSqlElasticPool、Set-AzureRmSqlElasticPool</span><span class="sxs-lookup"><span data-stu-id="a1232-799">New-AzureRmSqlElasticPool; Set-AzureRmSqlElasticPool</span></span>
    - <span data-ttu-id="a1232-800">New-AzureRmSqlDatabaseCopy</span><span class="sxs-lookup"><span data-stu-id="a1232-800">New-AzureRmSqlDatabaseCopy</span></span>
    - <span data-ttu-id="a1232-801">New-AzureRmSqlDatabaseSecondary</span><span class="sxs-lookup"><span data-stu-id="a1232-801">New-AzureRmSqlDatabaseSecondary</span></span>
    - <span data-ttu-id="a1232-802">Restore-AzureRmSqlDatabase</span><span class="sxs-lookup"><span data-stu-id="a1232-802">Restore-AzureRmSqlDatabase</span></span>

#### <a name="azurermtrafficmanager"></a><span data-ttu-id="a1232-803">AzureRM.TrafficManager</span><span class="sxs-lookup"><span data-stu-id="a1232-803">AzureRM.TrafficManager</span></span>
* <span data-ttu-id="a1232-804">"Get-AzureRmTrafficManagerProfile" のパラメーターが更新され、-Name パラメーターの使用時に -ResourceGroupName パラメーターが必須になりました。</span><span class="sxs-lookup"><span data-stu-id="a1232-804">Update the parameters for 'Get-AzureRmTrafficManagerProfile' so that -ResourceGroupName parameter is required when using -Name parameter.</span></span>
