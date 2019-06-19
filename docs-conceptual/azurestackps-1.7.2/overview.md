---
title: Azure Stack 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack 管理の PowerShell の概要と、インストールおよび構成の手順。
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/06/2019
ms.openlocfilehash: b77e09f6fcd5b7752af9f51a42d357db4f1b13db
ms.sourcegitcommit: febbbd3f75c8dd1a296281d265289f015b6cb537
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/12/2019
ms.locfileid: "67037674"
---
# <a name="azure-stack-module-172"></a>Azure Stack Module 1.7.2

## <a name="requirements"></a>要件:

サポートされている Azure Stack の最小バージョンは 1904 です。

注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。

## <a name="install"></a>Install

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a>リリース ノート

* 1904 更新プログラムでサポートされています
* これは重大な変更のリリースです。 重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。
* 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。 対称キーのサポートは非推奨となりました。
* 重大な変更について詳しくは、 https://aka.ms/azspshmigration170 を参照してください。
* Azs.Storage.Admin モジュール 
* バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。
