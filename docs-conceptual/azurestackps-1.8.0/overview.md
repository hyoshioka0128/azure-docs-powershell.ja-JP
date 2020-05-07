---
title: Azure Stack 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack 管理の PowerShell の概要と、インストールおよび構成の手順。
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/24/2020
ms.openlocfilehash: ec406c80de6b457f7e340a23fe8caf2ab83be46a
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "78264412"
---
# <a name="azure-stack-module-180"></a>Azure Stack Module 1.8.0

## <a name="requirements"></a>要件:

サポートされている Azure Stack の最小バージョンは 1910 です。

注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。

## <a name="install"></a>インストール

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.8.0
```

## <a name="release-notes"></a>リリース ノート

* 1910 更新プログラムでサポートされています
* 変更内容:

    - **新しい DRP 管理モジュール**:デプロイ リソース プロバイダー (DRP) を使用すると、Azure Stack Hub に対するリソース プロバイダーの調整されたデプロイが可能になります。 これらのコマンドを使うと、DRP とやり取りする Azure Resource Manager レイヤーとやり取りできます。

    - **BRP**:
        - Azure Stack インフラストラクチャ バックアップの 1 つのロールの復元をサポートします。
        - パラメーター `RoleName` をコマンドレット R`estore-AzsBackup` に追加します。

    - **FRP**:API バージョン 2019-05-01 の**ドライブ**と**ボリューム** リソースの破壊的変更。 これらの機能は Azure Stack Hub 1910 以降でサポートされています。
        - ID、`Name`、`HealthStatus`、および `OperationalStatus` の値が変更されました。
        - **ドライブ** リソースの新しいプロパティ `FirmwareVersion`、`IsIndicationEnabled`、`Manufacturer`、`StoragePool` がサポートされるようになりました。
        - **ドライブ** リソースのプロパティ `CanPool` および `CannotPoolReason` は廃止されました。代わりに `OperationalStatus` を使用してください。
