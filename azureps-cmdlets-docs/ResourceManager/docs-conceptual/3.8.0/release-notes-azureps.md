---
title: "Azure PowerShell の変更履歴 | Microsoft Docs"
description: "Azure PowerShell の最新リリースで行われた変更の履歴です。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 04f89e8d47d0825d46cb1b8817efbcc0cafa0acd
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="4d0dd-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="4d0dd-103">Release notes</span></span>
<a id="release-notes" class="xliff"></a>

<span data-ttu-id="4d0dd-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <span data-ttu-id="4d0dd-105">バージョン 3.8.0</span><span class="sxs-lookup"><span data-stu-id="4d0dd-105">Version 3.8.0</span></span>
<a id="version-380" class="xliff"></a>
* <span data-ttu-id="4d0dd-106">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="4d0dd-106">Compute</span></span>
  - <span data-ttu-id="4d0dd-107">Get-* コマンドレットのバグを修正し、複数ページのデータ (120 項目超) を取得できるようにしました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-107">Fix bug in Get-* cmdlets, to allow retrieving multiple pages of data (more than 120 items)</span></span>
* <span data-ttu-id="4d0dd-108">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="4d0dd-108">DataLakeAnalytics</span></span>
  - <span data-ttu-id="4d0dd-109">適切な表現や例を使うように、いくつかのコマンドのヘルプを修正しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-109">Fix help for some commands to have the proper verbage and examples.</span></span>
* <span data-ttu-id="4d0dd-110">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="4d0dd-110">DataLakeStore</span></span>
  - <span data-ttu-id="4d0dd-111">`Get-AzureRMDataLakeStoreItemContent` コマンドレットが新たに head と tail に対応しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-111">Add support for head and tail to the `Get-AzureRMDataLakeStoreItemContent` cmdlet.</span></span> <span data-ttu-id="4d0dd-112">上位 N 件や下位 N 件を改行区切りで取得して表示することができます。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-112">This enables returning the top N or last N new line delimited rows to be displayed.</span></span>
* <span data-ttu-id="4d0dd-113">HDInsight</span><span class="sxs-lookup"><span data-stu-id="4d0dd-113">HDInsight</span></span>
  - <span data-ttu-id="4d0dd-114">新たに RServer クラスター タイプに対応しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-114">Added support for RServer cluster type</span></span>
    + <span data-ttu-id="4d0dd-115">New-AzureRmHDInsightCluster または New-AzureRmHDInsightClusterConfig で、RServer クラスターに対してエッジ ノードの VM サイズを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-115">Edgenode VM size can be specified for RServer cluster in New-AzureRmHDInsightCluster or New-AzureRmHDInsightClusterConfig</span></span>
    + <span data-ttu-id="4d0dd-116">Add-AzureRmHDInsightConfigValues の構成オプションに RServer が追加されました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-116">RServer is now a configuration option in Add-AzureRmHDInsightConfigValues.</span></span> <span data-ttu-id="4d0dd-117">RStudio フラグを設定することで、R Studio のインストールが必要であることを指定できます。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-117">It allows for RStudio flag to be set to indicate that R Studio installation should be done.</span></span>
* <span data-ttu-id="4d0dd-118">LogicApp</span><span class="sxs-lookup"><span data-stu-id="4d0dd-118">LogicApp</span></span>
  - <span data-ttu-id="4d0dd-119">Set-AzureRmIntegrationAccountSchema コマンドレットと Set-AzureRmIntegrationAccountMap コマンドレットの contentlink の問題を修正しました (content と contentlink の両方が設定されて更新エラーが発生していました)。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-119">Set-AzureRmIntegrationAccountSchema and Set-AzureRmIntegrationAccountMap cmdlets are fixed for the contentlink issue(Both content and contentlink were set resulting in update failure).</span></span>
* <span data-ttu-id="4d0dd-120">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="4d0dd-120">Network</span></span>
  - <span data-ttu-id="4d0dd-121">Application Gateway が新しい Web アプリケーション ファイアウォール機能に対応しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-121">Added support for new web application firewall features to Application Gateways</span></span>
    + <span data-ttu-id="4d0dd-122">New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig を追加しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-122">Added New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig</span></span>
    + <span data-ttu-id="4d0dd-123">Get-AzureRmApplicationGatewayAvailableWafRuleSets (別名: List-AzureRmApplicationGatewayAvailableWafRuleSets) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-123">Added Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets)</span></span>
    + <span data-ttu-id="4d0dd-124">New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration を更新しました。-RuleSetType、-RuleSetVersion、-DisabledRuleGroups の各パラメーターが追加されています。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-124">Updated New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
    + <span data-ttu-id="4d0dd-125">Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration を更新しました。-RuleSetType、-RuleSetVersion、-DisabledRuleGroups の各パラメーターが追加されています。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-125">Updated Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
  - <span data-ttu-id="4d0dd-126">Virtual Network ゲートウェイ接続が、新たに IPSec ポリシーに対応しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-126">Added support for IPSec policies to Virtual Network Gateway Connections</span></span>
  - <span data-ttu-id="4d0dd-127">New-AzureRmIpsecPolicy を追加しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-127">Added New-AzureRmIpsecPolicy</span></span>
  - <span data-ttu-id="4d0dd-128">New-AzureRmVirtualNetworkGatewayConnection を更新しました。-IpsecPolicies パラメーターと -UsePolicyBasedTrafficSelectors パラメーターが追加されています。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-128">Updated New-AzureRmVirtualNetworkGatewayConnection: Added parameter -IpsecPolicies and -UsePolicyBasedTrafficSelectors</span></span>
* <span data-ttu-id="4d0dd-129">プロファイル</span><span class="sxs-lookup"><span data-stu-id="4d0dd-129">Profile</span></span>
  - <span data-ttu-id="4d0dd-130">"*廃止*": Save-AzureRmProfile は Save-AzureRmContext という名前に変更されました。変更前のコマンドレット名がエイリアスとして残されますが、そのエイリアスも次のリリースで削除されます。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-130">*Obsolete*: Save-AzureRmProfile is renamed to Save-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="4d0dd-131">"*廃止*": Select-AzureRmProfile は Import-AzureRmContext という名前に変更されました。変更前のコマンドレット名がエイリアスとして残されますが、そのエイリアスも次のリリースで削除されます。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-131">*Obsolete*: Select-AzureRmProfile is renamed to Import-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="4d0dd-132">プロファイル コマンドレットの出力タイプ PSAzureContext と PSAzureProfile は、次のリリースで変更される予定です。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-132">The PSAzureContext and PSAzureProfile output types of profile cmdlets will be changed in the next release.</span></span>
  - <span data-ttu-id="4d0dd-133">Save-AzureRmContext コマンドレットの OutputType は次のリリースで削除されます。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-133">The Save-AzureRmContext cmdlet will have no OutputType in the next release.</span></span>
  - <span data-ttu-id="4d0dd-134">コマンドレットに共通のコードのバグを修正しました。データ ハッシュに FIPS 準拠のアルゴリズムが使用されます (https://github.com/Azure/azure-powershell/issues/3651)。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-134">Fix bug in cmdlet common code to use FIPS-compliant algorithm for data hashes: https://github.com/Azure/azure-powershell/issues/3651</span></span>
* <span data-ttu-id="4d0dd-135">SQL</span><span class="sxs-lookup"><span data-stu-id="4d0dd-135">Sql</span></span>
  - <span data-ttu-id="4d0dd-136">Azure のフェールオーバー グループのコマンドレットにあるバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-136">Bug fixes on Azure Failover Group Cmdlets</span></span>
  - <span data-ttu-id="4d0dd-137">オペレーションのポーリングのための修正を行いました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-137">Fix for operation polling</span></span>
  - <span data-ttu-id="4d0dd-138">FailoverPolicy を Manual に設定するときの GracePeriodWithDataLossHour 値を修正しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-138">Fix GracePeriodWithDataLossHour value when setting FailoverPolicy to Manual</span></span>
* <span data-ttu-id="4d0dd-139">TrafficManager</span><span class="sxs-lookup"><span data-stu-id="4d0dd-139">TrafficManager</span></span>
  - <span data-ttu-id="4d0dd-140">地理的トラフィック ルーティング方式に対応しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-140">Support for the Geographic traffic routing method</span></span>
    + <span data-ttu-id="4d0dd-141">New-AzureRmTrafficManagerProfile の TrafficRoutingMethod パラメーターに新しい値 "Geographic" が追加されました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-141">New value 'Geographic' for the TrafficRoutingMethod parameter of New-AzureRmTrafficManagerProfile</span></span>
    + <span data-ttu-id="4d0dd-142">New-AzureRmTrafficManagerEndpoint と Add-AzureRmTrafficManagerEndpointConfig に新しいパラメーター "GeoMapping" が追加されました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-142">New parameter 'GeoMapping' for the New-AzureRmTrafficManagerEndpoint and Add-AzureRmTrafficManagerEndpointConfig</span></span>
    + <span data-ttu-id="4d0dd-143">Get-AzureRmTrafficManagerProfile でプロファイルのコレクションを取得する際のパイプ処理を修正しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-143">Fix piping for Get-AzureRmTrafficManagerProfile when it returns a collection of profiles</span></span>
* <span data-ttu-id="4d0dd-144">サービス管理</span><span class="sxs-lookup"><span data-stu-id="4d0dd-144">ServiceManagement</span></span>
  - <span data-ttu-id="4d0dd-145">Restart-AzureVM: VM の再起動中にメンテナンスを実行するための InitiateMaintenance パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-145">Restart-AzureVM: Added InitiateMaintenance parameter for performing maintenance during VM restart.</span></span>
  - <span data-ttu-id="4d0dd-146">Get-AzureVM: Maintenance Status フィールドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-146">Get-AzureVM: Added Maintenance Status field.</span></span>
  - <span data-ttu-id="4d0dd-147">Recovery Services コンテナーのアップグレードに対応するための新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="4d0dd-147">Added new cmdlets to support Recovery Services vault upgrade</span></span>
    + <span data-ttu-id="4d0dd-148">Test-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="4d0dd-148">Test-AzureRecoveryServicesVaultUpgrade</span></span>
    + <span data-ttu-id="4d0dd-149">Invoke-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="4d0dd-149">Invoke-AzureRecoveryServicesVaultUpgrade</span></span>
