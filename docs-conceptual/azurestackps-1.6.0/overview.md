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
ms.openlocfilehash: b0e85bec82b9b7c876b2bbf337b603c8d68cf6a3
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "63053317"
---
# <a name="azure-stack-module-160"></a>Azure Stack Module 1.6.0

## <a name="requirements"></a>要件:
サポートされている Azure Stack の最小バージョンは 1811 です。

注:以前のバージョンを使用している場合は、バージョン 1.6.0 をインストールしてください

## <a name="install"></a>インストール
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.6.0
```

## <a name="release-notes"></a>リリース ノート
* 1811 更新プログラムでサポートされています
* Azs.Compute.Admin モジュール
    * New-DataDiskObject の Azs プレフィックスが見つからない問題を修正し、今後の廃止の警告と共にエイリアスを追加しました。
* Azs.Update.Admin モジュール
    * Install-AzsUpdate の前に Test-AzureStack を実行することを勧める警告を追加しました
* Azs.Fabric.Admin
    * 新しいコマンドレット (機能は Azure Stack 1811 以降によってサポートされています)
        * Get-AzsDrive
        * Get-AzsVolume
        * Get-AzsStorageSubSystem
    * 非推奨
        * Get-AzsInfrastructureVolume は、コマンドレット Get-AzsVolume のエイリアスになりました
* Azs.InfrastructureInsights.Admin
    *  新しいコマンドレット Repair-AzsAlert を追加しました
* Azs.Storage.Admin
    * 既定のクォータ値が使用されないバグを修正
* Azs.Subscriptions.Admin モジュール
    * New-AddonPlanDefinitionObject の Azs プレフィックスが見つからない問題を修正し、今後の廃止の警告と共にエイリアスを追加しました。
