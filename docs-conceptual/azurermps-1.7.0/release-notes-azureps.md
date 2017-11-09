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
ms.openlocfilehash: 0a3f152751fee569d3ac5fba6bcff8c1737f7b8c
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-170"></a>バージョン 1.7.0

* **全コマンドレットを対象に、-Force、-Confirm、$ConfirmPreference の各パラメーターの動作を変更しました。Microsoft では、PowerShell のガイドラインに合わせてこの実装変更を進めています。これにより、ほとんどのコマンドレットで、Force パラメーターが削除されることになります。ShouldProcess プロンプトをスキップするためには、ユーザーがその PowerShell スクリプトでパラメーター "-Confirm:$false" を追加する必要があります。** この変更によって次の問題が解決されます。
  - -WhatIf 機能を正しく実装する。ユーザーは、実際に変更を加えずにコマンドレットまたはスクリプトの影響を確認できます。
  - セッション全体の $ConfirmPreference を使ってプロンプトを制御する。予想される変更の影響 (コマンドレットの ConfirmImpact 設定で指定) に基づいてプロンプトが表示されます。
  - -Confirm パラメーターを使ってコマンドレットごとに確認プロンプトを制御する。
  - 変更の性格が特殊 (隠しファイルの削除など) であるためにユーザーの確認を必要とするような操作についてのみ ShouldContinue と -Force パラメーターを使用するように全コマンドレットで統一する。
  - 他のコマンドレットで身に付けた PowerShell スクリプト作成の知識をそのまま Azure PowerShell のコマンドレットに応用できるように他の PowerShell コマンドレットとの一貫性を確保する。

**今後、Azure PowerShell コマンドレットで "*すべてのプロンプトをあらゆる状況で自動的にスキップ*" するためには、次の 2 つのパラメーターを指定する必要があります。**
```powershell
My-CmdletWithConfirmation –Confirm:$false -Force
```
* Azure コンピューティング
  - Set-AzureRmVMADDomainExtension
  - Get-AzureRmVMADDomainExtension
  - Restart-AzureVM の -Redeploy パラメーター
  - Move-AzureService、Move-AzureStorageAccount、Move-AzureVirtualNetwork の -Validate パラメーター
  - 従来と同様、拡張機能のコマンドレットに対する名前とバージョンのパラメーターは省略可能です。
  - New-AzureVM で VM オブジェクトのライセンス タイプを取得できます。
* Azure Storage (Azure Storage)
  - Tags パラメーターを Tag に変更し、パラメーター エイリアスとして Tags を追加しました。
    + New-AzureRmStorageAccount
    + Set-AzureRmStorageAccount
* Azure ネットワーク
  - 仮想ネットワーク ピアリング用の新しいコマンドレットを追加しました。
* Azure Redis Cache
  - 新しいコマンドレット Reset-AzureRmRedisCache を追加しました。
  - 新しいコマンドレット Export-AzureRmRedisCache を追加しました。
  - 新しいコマンドレット Import-AzureRmRedisCache を追加しました。
  - vNet に関するパラメーターの変更を反映するためにコマンドレット New-AzureRmRedisCache を変更しました。
* Azure SQL DB バックアップ/復元
  - LTR (長期的な保有期間) バックアップ機能のコマンドレット
  - Get-AzureRmSqlServerBackupLongTermRetentionVault
  - Get-AzureRmSqlDatabaseBackupLongTermRetentionPolicy
  - Set-AzureRmSqlServerBackupLongTermRetentionVault
  - Set-AzureRmSqlDatabaseBackupLongTermRetentionPolicy
  - 削除されたデータベースを Restore-AzureRmSqlDatabase で特定の時点まで復元できるようになりました。
  - Restore-AzureRmSqlDatabase が長期的な保有期間バックアップからの復元に対応しました。
* Azure LogicApp
  - LogicApp 統合アカウントのコマンドレットを追加しました。
  - Get-AzureRmIntegrationAccountAgreement
  - Get-AzureRmIntegrationAccountCallbackUrl
  - Get-AzureRmIntegrationAccountCertificate
  - Get-AzureRmIntegrationAccount
  - Get-AzureRmIntegrationAccountMap
  - Get-AzureRmIntegrationAccountPartner
  - Get-AzureRmIntegrationAccountSchema
  - New-AzureRmIntegrationAccountAgreement
  - New-AzureRmIntegrationAccountCertificate
  - New-AzureRmIntegrationAccount
  - New-AzureRmIntegrationAccountMap
  - New-AzureRmIntegrationAccountPartner
  - New-AzureRmIntegrationAccountSchema
  - Remove-AzureRmIntegrationAccountAgreement
  - Remove-AzureRmIntegrationAccountCertificate
  - Remove-AzureRmIntegrationAccount
  - Remove-AzureRmIntegrationAccountMap
  - Remove-AzureRmIntegrationAccountPartner
  - Remove-AzureRmIntegrationAccountSchema
  - Set-AzureRmIntegrationAccountAgreement
  - Set-AzureRmIntegrationAccountCertificate
  - Set-AzureRmIntegrationAccount
  - Set-AzureRmIntegrationAccountMap
  - Set-AzureRmIntegrationAccountPartner
  - Set-AzureRmIntegrationAccountSchema
* Azure Data Lake Store
  - ファイルとフォルダーのアップロードとダウンロードのパフォーマンスが大幅に向上しています。
  - ダウンロードに関してパラメーター名がわずかに変更されたほか、アップロードに関しては、次のパラメーターが新たに 2 つ追加されました。
    + NumThreads -> PerFileThreadCount。1 ファイルあたりのスレッド数を指定する目的で使用します。
    + ConcurrentFileCount。フォルダーのアップロード/ダウンロード時に同時にアップロード/ダウンロードするファイル数を指定する目的で使用します。
  - 既定のスレッド値。ほとんどのファイル サイズで良好なスループットが得られるように意図された値が指定されています。 適切なパフォーマンスが得られない場合は、要件を満たすように上記の値を変更することができます。
* Azure Data Lake Analytics
  - Get-AzureRMDataLakeAnalyticsDataSource に引数を指定しなかった場合、すべてのデータ ソースが返されるようになりました。
  - この変更に伴い、対応するデータ ソース タイプ パラメーターがコマンドレットから削除されています。
  - この変更に伴い、次のプロパティを使ったリスト操作で新しいオブジェクトが返されます。
    + Type: データ ソースの種類。
    + Name: データ ソースの名前。
    + IsDefault: アカウントの既定のデータ ソースである場合は true に設定します。
  - submittedBefore と submittedAfter を条件としてフィルタリングを行う際の特定の日時オフセット値のリストに関して、Get-AzureRMDataLakeAnalyticsJob を修正しました。
* Web Apps
  - 通常のスワップとプレビュー付きスワップに対応した Swap-AzureRmWebAppSlot コマンドレットを追加しました。
  - Set-AzureRmWebAppSlot コマンドレットを拡張し、自動スワップに対応しました。
* Azure API Management
  - AzureChinaCloud の Azure API Management デプロイ コマンドレットを修正しました。
  - Git アクセスは既定で有効になっているため、Set-AzureRmApiManagementTenantGitAccess コマンドレットは削除しました。
* Azure Recovery Services バックアップ
  - 新たに Azure SQL ワークロードに対応しました。
  - 暗号化された Azure VM のバックアップと復元に新たに対応しました。
  - Backup-AzureRmRecoveryServicesBackupItem - 復旧ポイントに関してオプションの保持期間機能を追加しました。
  - Get-AzureRmRecoveryServicesBackupContainer コマンドレットと Get-AzureRmRecoveryServicesBackupItem コマンドレットのフィルターに関連した小さなバグを修正しました。
* Azure Automation
  - Get-AzureRmAutomationHybridWorkerGroup を追加しました。
