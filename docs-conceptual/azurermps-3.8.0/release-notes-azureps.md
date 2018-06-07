---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 2e17b6f7f62f25d8d91c4d32a4a1ae5c45b8665d
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821804"
---
# <a name="release-notes"></a><span data-ttu-id="ce78d-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="ce78d-103">Release notes</span></span>

<span data-ttu-id="ce78d-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="ce78d-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-380"></a><span data-ttu-id="ce78d-105">バージョン 3.8.0</span><span class="sxs-lookup"><span data-stu-id="ce78d-105">Version 3.8.0</span></span>
* <span data-ttu-id="ce78d-106">コンピューティング</span><span class="sxs-lookup"><span data-stu-id="ce78d-106">Compute</span></span>
  - <span data-ttu-id="ce78d-107">Get-\* コマンドレットのバグを修正し、複数ページのデータ (120 項目超) を取得できるようにしました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-107">Fix bug in Get-\* cmdlets, to allow retrieving multiple pages of data (more than 120 items)</span></span>
* <span data-ttu-id="ce78d-108">DataLakeAnalytics</span><span class="sxs-lookup"><span data-stu-id="ce78d-108">DataLakeAnalytics</span></span>
  - <span data-ttu-id="ce78d-109">適切な表現や例を使うように、いくつかのコマンドのヘルプを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-109">Fix help for some commands to have the proper verbage and examples.</span></span>
* <span data-ttu-id="ce78d-110">DataLakeStore</span><span class="sxs-lookup"><span data-stu-id="ce78d-110">DataLakeStore</span></span>
  - <span data-ttu-id="ce78d-111">`Get-AzureRMDataLakeStoreItemContent` コマンドレットが新たに head と tail に対応しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-111">Add support for head and tail to the `Get-AzureRMDataLakeStoreItemContent` cmdlet.</span></span> <span data-ttu-id="ce78d-112">上位 N 件や下位 N 件を改行区切りで取得して表示することができます。</span><span class="sxs-lookup"><span data-stu-id="ce78d-112">This enables returning the top N or last N new line delimited rows to be displayed.</span></span>
* <span data-ttu-id="ce78d-113">HDInsight</span><span class="sxs-lookup"><span data-stu-id="ce78d-113">HDInsight</span></span>
  - <span data-ttu-id="ce78d-114">新たに RServer クラスター タイプに対応しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-114">Added support for RServer cluster type</span></span>
    + <span data-ttu-id="ce78d-115">New-AzureRmHDInsightCluster または New-AzureRmHDInsightClusterConfig で、RServer クラスターに対してエッジ ノードの VM サイズを指定することができます。</span><span class="sxs-lookup"><span data-stu-id="ce78d-115">Edgenode VM size can be specified for RServer cluster in New-AzureRmHDInsightCluster or New-AzureRmHDInsightClusterConfig</span></span>
    + <span data-ttu-id="ce78d-116">Add-AzureRmHDInsightConfigValues の構成オプションに RServer が追加されました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-116">RServer is now a configuration option in Add-AzureRmHDInsightConfigValues.</span></span> <span data-ttu-id="ce78d-117">RStudio フラグを設定することで、R Studio のインストールが必要であることを指定できます。</span><span class="sxs-lookup"><span data-stu-id="ce78d-117">It allows for RStudio flag to be set to indicate that R Studio installation should be done.</span></span>
* <span data-ttu-id="ce78d-118">LogicApp</span><span class="sxs-lookup"><span data-stu-id="ce78d-118">LogicApp</span></span>
  - <span data-ttu-id="ce78d-119">Set-AzureRmIntegrationAccountSchema コマンドレットと Set-AzureRmIntegrationAccountMap コマンドレットの contentlink の問題を修正しました (content と contentlink の両方が設定されて更新エラーが発生していました)。</span><span class="sxs-lookup"><span data-stu-id="ce78d-119">Set-AzureRmIntegrationAccountSchema and Set-AzureRmIntegrationAccountMap cmdlets are fixed for the contentlink issue(Both content and contentlink were set resulting in update failure).</span></span>
* <span data-ttu-id="ce78d-120">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="ce78d-120">Network</span></span>
  - <span data-ttu-id="ce78d-121">Application Gateway が新しい Web アプリケーション ファイアウォール機能に対応しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-121">Added support for new web application firewall features to Application Gateways</span></span>
    + <span data-ttu-id="ce78d-122">New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-122">Added New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig</span></span>
    + <span data-ttu-id="ce78d-123">Get-AzureRmApplicationGatewayAvailableWafRuleSets (別名: List-AzureRmApplicationGatewayAvailableWafRuleSets) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-123">Added Get-AzureRmApplicationGatewayAvailableWafRuleSets (Alias: List-AzureRmApplicationGatewayAvailableWafRuleSets)</span></span>
    + <span data-ttu-id="ce78d-124">New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration を更新しました。-RuleSetType、-RuleSetVersion、-DisabledRuleGroups の各パラメーターが追加されています。</span><span class="sxs-lookup"><span data-stu-id="ce78d-124">Updated New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
    + <span data-ttu-id="ce78d-125">Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration を更新しました。-RuleSetType、-RuleSetVersion、-DisabledRuleGroups の各パラメーターが追加されています。</span><span class="sxs-lookup"><span data-stu-id="ce78d-125">Updated Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration: Added parameter -RuleSetType -RuleSetVersion and -DisabledRuleGroups</span></span>
  - <span data-ttu-id="ce78d-126">Virtual Network ゲートウェイ接続が、新たに IPSec ポリシーに対応しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-126">Added support for IPSec policies to Virtual Network Gateway Connections</span></span>
  - <span data-ttu-id="ce78d-127">New-AzureRmIpsecPolicy を追加しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-127">Added New-AzureRmIpsecPolicy</span></span>
  - <span data-ttu-id="ce78d-128">New-AzureRmVirtualNetworkGatewayConnection を更新しました。-IpsecPolicies パラメーターと -UsePolicyBasedTrafficSelectors パラメーターが追加されています。</span><span class="sxs-lookup"><span data-stu-id="ce78d-128">Updated New-AzureRmVirtualNetworkGatewayConnection: Added parameter -IpsecPolicies and -UsePolicyBasedTrafficSelectors</span></span>
* <span data-ttu-id="ce78d-129">プロファイル</span><span class="sxs-lookup"><span data-stu-id="ce78d-129">Profile</span></span>
  - <span data-ttu-id="ce78d-130">"*廃止*": Save-AzureRmProfile は Save-AzureRmContext という名前に変更されました。変更前のコマンドレット名がエイリアスとして残されますが、そのエイリアスも次のリリースで削除されます。</span><span class="sxs-lookup"><span data-stu-id="ce78d-130">*Obsolete*: Save-AzureRmProfile is renamed to Save-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="ce78d-131">"*廃止*": Select-AzureRmProfile は Import-AzureRmContext という名前に変更されました。変更前のコマンドレット名がエイリアスとして残されますが、そのエイリアスも次のリリースで削除されます。</span><span class="sxs-lookup"><span data-stu-id="ce78d-131">*Obsolete*: Select-AzureRmProfile is renamed to Import-AzureRmContext, there is an alias to the old cmdlet name, the alias will be removed in the next release.</span></span>
  - <span data-ttu-id="ce78d-132">プロファイル コマンドレットの出力タイプ PSAzureContext と PSAzureProfile は、次のリリースで変更される予定です。</span><span class="sxs-lookup"><span data-stu-id="ce78d-132">The PSAzureContext and PSAzureProfile output types of profile cmdlets will be changed in the next release.</span></span>
  - <span data-ttu-id="ce78d-133">Save-AzureRmContext コマンドレットの OutputType は次のリリースで削除されます。</span><span class="sxs-lookup"><span data-stu-id="ce78d-133">The Save-AzureRmContext cmdlet will have no OutputType in the next release.</span></span>
  - <span data-ttu-id="ce78d-134">データ ハッシュに FIPS 準拠アルゴリズムを使用するコマンドレット共通コードのバグを修正しました (https://github.com/Azure/azure-powershell/issues/3651)。</span><span class="sxs-lookup"><span data-stu-id="ce78d-134">Fix bug in cmdlet common code to use FIPS-compliant algorithm for data hashes: https://github.com/Azure/azure-powershell/issues/3651</span></span>
* <span data-ttu-id="ce78d-135">SQL</span><span class="sxs-lookup"><span data-stu-id="ce78d-135">Sql</span></span>
  - <span data-ttu-id="ce78d-136">Azure のフェールオーバー グループのコマンドレットにあるバグを修正しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-136">Bug fixes on Azure Failover Group Cmdlets</span></span>
  - <span data-ttu-id="ce78d-137">オペレーションのポーリングのための修正を行いました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-137">Fix for operation polling</span></span>
  - <span data-ttu-id="ce78d-138">FailoverPolicy を Manual に設定するときの GracePeriodWithDataLossHour 値を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-138">Fix GracePeriodWithDataLossHour value when setting FailoverPolicy to Manual</span></span>
* <span data-ttu-id="ce78d-139">TrafficManager</span><span class="sxs-lookup"><span data-stu-id="ce78d-139">TrafficManager</span></span>
  - <span data-ttu-id="ce78d-140">地理的トラフィック ルーティング方式に対応しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-140">Support for the Geographic traffic routing method</span></span>
    + <span data-ttu-id="ce78d-141">New-AzureRmTrafficManagerProfile の TrafficRoutingMethod パラメーターに新しい値 "Geographic" が追加されました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-141">New value 'Geographic' for the TrafficRoutingMethod parameter of New-AzureRmTrafficManagerProfile</span></span>
    + <span data-ttu-id="ce78d-142">New-AzureRmTrafficManagerEndpoint と Add-AzureRmTrafficManagerEndpointConfig に新しいパラメーター "GeoMapping" が追加されました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-142">New parameter 'GeoMapping' for the New-AzureRmTrafficManagerEndpoint and Add-AzureRmTrafficManagerEndpointConfig</span></span>
    + <span data-ttu-id="ce78d-143">Get-AzureRmTrafficManagerProfile でプロファイルのコレクションを取得する際のパイプ処理を修正しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-143">Fix piping for Get-AzureRmTrafficManagerProfile when it returns a collection of profiles</span></span>
* <span data-ttu-id="ce78d-144">サービス管理</span><span class="sxs-lookup"><span data-stu-id="ce78d-144">ServiceManagement</span></span>
  - <span data-ttu-id="ce78d-145">Restart-AzureVM: VM の再起動中にメンテナンスを実行するための InitiateMaintenance パラメーターを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-145">Restart-AzureVM: Added InitiateMaintenance parameter for performing maintenance during VM restart.</span></span>
  - <span data-ttu-id="ce78d-146">Get-AzureVM: Maintenance Status フィールドを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-146">Get-AzureVM: Added Maintenance Status field.</span></span>
  - <span data-ttu-id="ce78d-147">Recovery Services コンテナーのアップグレードに対応するための新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="ce78d-147">Added new cmdlets to support Recovery Services vault upgrade</span></span>
    + <span data-ttu-id="ce78d-148">Test-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="ce78d-148">Test-AzureRecoveryServicesVaultUpgrade</span></span>
    + <span data-ttu-id="ce78d-149">Invoke-AzureRecoveryServicesVaultUpgrade</span><span class="sxs-lookup"><span data-stu-id="ce78d-149">Invoke-AzureRecoveryServicesVaultUpgrade</span></span>
