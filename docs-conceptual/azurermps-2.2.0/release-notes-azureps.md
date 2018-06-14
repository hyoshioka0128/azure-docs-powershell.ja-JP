---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: ca25f3c66f8e8f4c64fc04275da2bd28e32d2f6c
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/08/2018
ms.locfileid: "34854615"
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-220"></a>バージョン 2.2.0
* コンピューティング
  - AzureDiskEncryptionForLinux 拡張機能の暗号化状態を照会できるようになりました。
* DataFactory
  - アクティビティ ウィンドウを列挙するための新しいコマンドレットを追加しました。
    + Get-AzureRmDataFactoryActivityWindow
* DataLake
  - パラメーター `Host` を `DatabaseHost` に変更し、`Host` へのエイリアスを追加しました。
    + New-AzureRmDataLakeAnalyticsCatalogSecret
    + Set-AzureRmDataLakeAnalyticsCatalogSecret
  - 新たに ACL と既定の ACL の削除に対応しました。
  - ファイルやフォルダーに対する無名のアクセス許可を取得したり設定したりできるようになりました。
* KeyVault
  - 証明書関連の機能が追加されました。
    + Add-AzureKeyVaultCertificate
    + Add-AzureKeyVaultCertificateContact
    + Get-AzureKeyVaultCertificate
    + Get-AzureKeyVaultCertificateContact
    + Get-AzureKeyVaultCertificateIssuer
    + Get-AzureKeyVaultCertificateOperation
    + Get-AzureKeyVaultCertificatePolicy
    + Import-AzureKeyVaultCertificate
    + New-AzureKeyVaultCertificateAdministratorDetails
    + New-AzureKeyVaultCertificateOrganizationDetails
    + New-AzureKeyVaultCertificatePolicy
    + Remove-AzureKeyVaultCertificate
    + Remove-AzureKeyVaultCertificateContact
    + Remove-AzureKeyVaultCertificateIssuer
    + Remove-AzureKeyVaultCertificateOperation
    + Set-AzureKeyVaultCertificateAttribute
    + Set-AzureKeyVaultCertificateIssuer
    + Set-AzureKeyVaultCertificatePolicy
    + Stop-AzureKeyVaultCertificateOperation
* ネットワーク

  - ネットワーク インターフェイスで高速ネットワークの有効/無効を切り替える新しいスイッチ パラメーターが追加されました (+New-AzureRmNetworkInterface -EnableAcceleratedNetworking)。
  - アクティブ/アクティブ ゲートウェイ機能を実現する PowerShell コマンドレット
    + Add-AzureRmVirtualNetworkGatewayIpConfig
    + Remove-AzureRmVirtualNetworkGatewayIpConfig
  - 新しいコマンドレットを追加しました。
    + Test-AzureRmPrivateIpAddressAvailability
* リソース
  - プロバイダー コマンドレットとリソース コマンドレットでゾーンに対応しました。
    + Get-AzureRmProvider
    + New-AzureRmResource
    + Set-AzureRmResource
* SQL
  - Azure SQL 脅威検出ポリシーをサーバー レベルで管理するための新しいコマンドレットを追加しました。
    + Get-AzureRmSqlServerThreatDetectionPolicy
    + Remove-AzureRmSqlServerThreatDetectionPolicy
    + Set-AzureRmSqlServerThreatDetectionPolicy
  - SQL Azure Data Warehouse の GeoBackupPolicy の有効化/無効化に対応する新しいコマンドレットを追加しました。
    + Get-AzureRmSqlDatabaseGeoBackupPolicy
    + Set-AzureRmSqlDatabaseGeoBackupPolicy
  - Azure Sql Advisors と Recommended Actions API 用の新しいコマンドレットを追加しました。
    + Get-AzureRmSqlDatabaseAdvisor
    + Get-AzureRmSqlElasticPoolAdvisor
    + Get-AzureRmSqlServerAdvisor
    + Get-AzureRmSqlDatabaseRecommendedActions
    + Get-AzureRmSqlElasticPoolRecommendedActions
    + Get-AzureRmSqlServerRecommendedActions
    + Set-AzureRmSqlDatabaseAdvisorAutoExecuteStatus
    + Set-AzureRmSqlElasticPoolAdvisorAutoExecuteStatus
    + Set-AzureRmSqlServerAdvisorAutoExecuteStatus
    + Set-AzureRmSqlDatabaseRecommendedActionState
    + Set-AzureRmSqlElasticPoolRecommendedActionState
    + Set-AzureRmSqlServerRecommendedActionState
