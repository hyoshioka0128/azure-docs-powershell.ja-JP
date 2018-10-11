---
title: Azure Stack 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack 管理の PowerShell の概要と、インストールおよび構成の手順。
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: 72d147f5bc9c882083dda6b33b1c89663fd2eb34
ms.sourcegitcommit: a749eb729f583c9d0dd86141bbd04984d77ae9ab
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/11/2018
ms.locfileid: "48882369"
---
# <a name="azure-stack-module-140"></a>Azure Stack Module 1.4.0

## <a name="requirements"></a>要件:
サポートされている Azure Stack の最小バージョンは 1804 です。

注: 以前のバージョンを使用している場合は、バージョン 1.2.11 をインストールしてください。

## <a name="known-issues"></a>既知の問題:

- アラートを閉じるには、Azure Stack バージョン 1803 が必要です。
- New-AzsOffer では、状態が "パブリック" のオファーを作成することはできません。 状態を変更するには、後で Set-AzsOffer コマンドレットを呼び出す必要があります。
- 再デプロイせずに IP プールを削除することはできません。

## <a name="breaking-changes"></a>重大な変更
バージョン 1.3.0 からの重大な変更はありません。 1.2.11 からの移行に関する重大な変更はすべて https://aka.ms/azspowershellmigration に記載されています。

## <a name="install"></a>Install
```
# Remove previous versions of AzureStack modules
Uninstall-Module -Name AzureStack -Force 
Uninstall-Module AzureRM.AzureStackAdmin -Force
Uninstall-Module AzureRM.AzureStackStorage -Force
Get-Module Azs.* -ListAvailable | Uninstall-Module -Force


# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2017-03-09-profile -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.4.0
```
## <a name="release-notes"></a>リリース ノート
    * Azure Stack 1.4.0 バージョンには、以前のリリース 1.3.0 からの重大な変更はありません
    * Azs.AzureBridge.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Backup.Admin
        - Set-AzsBackupShare コマンドレットに、BackupFrequencyInHours、IsBackupSchedulerEnabled、BackupRetentionPeriodInDays の各パラメーターを追加しました
        - 暗号化キーの作成を容易にするために、New-EncyptionKeyBase64 コマンドレットを追加しました
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Commerce.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Fabric.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
        - 管理者が Azure Stack スタンプに新しいスケール ユニット ノードを追加できるように、Add-AzsScaleUnitNode コマンドレットを追加しました
        - スケール ユニット パラメーター オブジェクトの作成を容易にするために、New-AzsScaleUnitNodeObject コマンドレットを追加しました
    * Azs.Gallery.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.InfrastructureInsights.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Network.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Update.Admin
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Subscriptions
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム
    * Azs.Subscriptions.Admin
        - 委任されたプロバイダーのプラン間でサブスクリプションを移動するために、Move-AzsSubscription コマンドレットを追加しました
        - 委任されたプロバイダーのプラン間でユーザー サブスクリプションを移動できることを検証するために、Test-AzsMoveSubscription コマンドレットを追加しました
        - 改ページ調整された結果でシングル ページしか返されないバグに対する修正プログラム

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
Azure Stack Compute 管理者モジュールのプレビュー リリース。このモジュールは、コンピューティング クォータ、プラットフォーム イメージ、仮想マシン拡張機能を管理する機能を提供します。

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
