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
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-380"></a>バージョン 3.8.0
* コンピューティング
  - Get-* コマンドレットのバグを修正し、複数ページのデータ (120 項目超) を取得できるようにしました。
* DataLakeAnalytics
  - 適切な表現や例を使うように、いくつかのコマンドのヘルプを修正しました。
* DataLakeStore
  - `Get-AzureRMDataLakeStoreItemContent` コマンドレットが新たに head と tail に対応しました。 上位 N 件や下位 N 件を改行区切りで取得して表示することができます。
* HDInsight
  - 新たに RServer クラスター タイプに対応しました。
    + New-AzureRmHDInsightCluster または New-AzureRmHDInsightClusterConfig で、RServer クラスターに対してエッジ ノードの VM サイズを指定することができます。
    + Add-AzureRmHDInsightConfigValues の構成オプションに RServer が追加されました。 RStudio フラグを設定することで、R Studio のインストールが必要であることを指定できます。
* LogicApp
  - Set-AzureRmIntegrationAccountSchema コマンドレットと Set-AzureRmIntegrationAccountMap コマンドレットの contentlink の問題を修正しました (content と contentlink の両方が設定されて更新エラーが発生していました)。
* ネットワーク
  - Application Gateway が新しい Web アプリケーション ファイアウォール機能に対応しました。
    + New-AzureRmApplicationGatewayFirewallDisabledRuleGroupConfig を追加しました。
    + Get-AzureRmApplicationGatewayAvailableWafRuleSets (別名: List-AzureRmApplicationGatewayAvailableWafRuleSets) を追加しました。
    + New-AzureRmApplicationGatewayWebApplicationFirewallConfiguration を更新しました。-RuleSetType、-RuleSetVersion、-DisabledRuleGroups の各パラメーターが追加されています。
    + Set-AzureRmApplicationGatewayWebApplicationFirewallConfiguration を更新しました。-RuleSetType、-RuleSetVersion、-DisabledRuleGroups の各パラメーターが追加されています。
  - Virtual Network ゲートウェイ接続が、新たに IPSec ポリシーに対応しました。
  - New-AzureRmIpsecPolicy を追加しました。
  - New-AzureRmVirtualNetworkGatewayConnection を更新しました。-IpsecPolicies パラメーターと -UsePolicyBasedTrafficSelectors パラメーターが追加されています。
* プロファイル
  - "*廃止*": Save-AzureRmProfile は Save-AzureRmContext という名前に変更されました。変更前のコマンドレット名がエイリアスとして残されますが、そのエイリアスも次のリリースで削除されます。
  - "*廃止*": Select-AzureRmProfile は Import-AzureRmContext という名前に変更されました。変更前のコマンドレット名がエイリアスとして残されますが、そのエイリアスも次のリリースで削除されます。
  - プロファイル コマンドレットの出力タイプ PSAzureContext と PSAzureProfile は、次のリリースで変更される予定です。
  - Save-AzureRmContext コマンドレットの OutputType は次のリリースで削除されます。
  - コマンドレットに共通のコードのバグを修正しました。データ ハッシュに FIPS 準拠のアルゴリズムが使用されます (https://github.com/Azure/azure-powershell/issues/3651)。
* SQL
  - Azure のフェールオーバー グループのコマンドレットにあるバグを修正しました。
  - オペレーションのポーリングのための修正を行いました。
  - FailoverPolicy を Manual に設定するときの GracePeriodWithDataLossHour 値を修正しました。
* TrafficManager
  - 地理的トラフィック ルーティング方式に対応しました。
    + New-AzureRmTrafficManagerProfile の TrafficRoutingMethod パラメーターに新しい値 "Geographic" が追加されました。
    + New-AzureRmTrafficManagerEndpoint と Add-AzureRmTrafficManagerEndpointConfig に新しいパラメーター "GeoMapping" が追加されました。
    + Get-AzureRmTrafficManagerProfile でプロファイルのコレクションを取得する際のパイプ処理を修正しました。
* サービス管理
  - Restart-AzureVM: VM の再起動中にメンテナンスを実行するための InitiateMaintenance パラメーターを追加しました。
  - Get-AzureVM: Maintenance Status フィールドを追加しました。
  - Recovery Services コンテナーのアップグレードに対応するための新しいコマンドレットを追加しました。
    + Test-AzureRecoveryServicesVaultUpgrade
    + Invoke-AzureRecoveryServicesVaultUpgrade
