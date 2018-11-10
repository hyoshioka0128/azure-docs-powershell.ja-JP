---
title: Azure Stack PowerShell の概要 | Microsoft Docs
description: Azure Stack PowerShell の概要と、インストールおよび構成の手順。
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: cd415e862bfaa2b767cce108689ebaf34ef74305
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51274400"
---
# <a name="azurerm-module-230"></a>AzureRM モジュール 2.3.0

## <a name="requirements"></a>要件:
サポートされている Azure Stack の最小バージョンは 1808 です。

注: 以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください。


## <a name="install"></a>Install
```powershell-interactive
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module -Name AzureRM -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force -ErrorAction Continue
Uninstall-Module AzureRM.AzureStackStorage -Force -ErrorAction Continue
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force
Get-Module Azure.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

```

## <a name="release-notes"></a>リリース ノート
* リリース 2.3.0 には破壊的変更の一覧が含まれています。 バージョン 1.2.11 からのアップグレードについては、移行ガイドをご用意しました (https://aka.ms/azspowershellmigration)
* このリリースは、AzureStack 固有の API プロファイル 2018-03-01-hybrid に対応しています
* すべてのモジュールで、AzureRm.Profile モジュールへの同等以上の依存関係が確立されます。
* 各モジュールでサポートされている API バージョンが更新されています。 
    * コンピューティング - 2017-03-30
    * ネットワーク - 2017-10-01
    * ストレージ - 2016-01-01
    * リソース - 2018-02-01
    * Keyvault - 2016-10-01
    * DNS - 2016-04-01
* リソースの種類それぞれに対する詳細な API バージョン マップについては、 https://github.com/Azure/azure-rest-api-specs/blob/master/profile/2018-03-01-hybrid.json をご覧ください

## <a name="content"></a>内容:
### <a name="azure-bridge"></a>Azure Bridge
Azure Stack AzureBridge 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure からイメージを配信できます。

### <a name="backup"></a>バックアップ
Backup 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。
- バックアップの保存先の構成
- バックアップの実行
- 完了したバックアップの表示と復元

### <a name="commerce"></a>コマース
Azure Stack Commerce 管理者モジュールのプレビュー リリース。このモジュールを使用して、Azure Stack システム全体の集計データの使用状況を表示できます。

### <a name="compute"></a>コンピューティング
Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、マネージド ディスク、および仮想マシン拡張機能を管理する機能を提供します。

### <a name="fabric"></a>Fabric
Azure Stack Fabric 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用してインフラストラクチャ コンポーネントを表示および管理できます。
- スケール ユニット ノードの停止、起動、シャットダウン
- FRU 関連のアクティビティに対応するためのスケール ユニット ノードのドレインと再開
- スケール ユニット ノードの修復
- インフラストラクチャ ロールの再起動
- インフラストラクチャ ロール インスタンスの停止、起動、シャットダウン
- 新しい IP プールの作成


### <a name="gallery"></a>[ギャラリー]
Azure Stack Gallery 管理者モジュールのプレビュー リリース。このモジュールは、Azure Stack Marketplace のギャラリー項目を管理する機能を提供します。

### <a name="infrastructure-insights"></a>Infrastructure Insights
Infrastructure Insights 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して以下を行うことができます。
- Azure Stack スタンプ リソースの正常性の表示
- アラートの表示と管理

### <a name="keyvault"></a>KeyVault
Azure Stack KeyVault 管理者モジュールのプレビュー リリース。管理者は、このモジュールを使用して KeyVault クォータを表示できます。

### <a name="network"></a>ネットワーク
Network 管理者モジュールのプレビュー リリース。このモジュールでは次のことが可能です。
- ネットワーク クォータの管理
- 割り当て済みのネットワーク リソース (パブリック IP アドレス、仮想ネットワーク、ロード バランサーなど) の表示
- 管理者の概要を表示するコマンドレットの提供

### <a name="storage"></a>Storage
Azure Stack Storage 管理者モジュールのプレビュー リリース。  このリリースには、次の機能が用意されています。
- ストレージ クォータの管理
- 削除されたストレージ リソースのガベージ コレクションの実行
- 削除されたストレージ アカウントの復元
- 共有間でのコンテナーの移行
- 個々のストレージ コンポーネントに関する情報の表示
- 使用状況とパフォーマンスの情報の表示

### <a name="subscription-admin"></a>サブスクリプション管理
Azure Stack Subscription 管理者モジュールのプレビュー リリース。  このモジュールは、管理者向けの次の機能を提供します。
- プランとオファーの管理
- 使用状況とパフォーマンスの情報の表示
- RBAC の管理

### <a name="subscription"></a>サブスクリプション
Azure Stack Subscription モジュールのプレビュー リリース。  このモジュールは、ユーザー向けの次の機能を提供します。
- サブスクリプションの作成、削除、更新

### <a name="update"></a>アップデート
Azure Stack Update 管理者モジュールのプレビュー リリース。  このモジュールでは、管理者は以下を行うことができます。
- 使用可能な更新プログラムの表示とインストール
- 中断された更新の再開
- インストール済みの更新プログラムの表示
