---
title: Azure Stack Hub 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack Hub 管理の PowerShell の概要と、インストールおよび構成の手順。
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 04/16/2020
ms.openlocfilehash: fd1f2a3778e348ba41b46acb4bdce19e18a7f4ec
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "81524967"
---
# <a name="azure-stack-hub-module-200"></a>Azure Stack Hub モジュール 2.0.0

## <a name="requirements"></a>要件:

サポートされている Azure Stack Hub の最小バージョンは 2002 です。

注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。

## <a name="install"></a>インストール

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue
Get-Module -Name Az.* -ListAvailable | Uninstall-Module -Force -Verbose -ErrorAction Continue

Install-Module -Name Az.BootStrapper -Force -AllowPrerelease

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 2.0.0-preview -AllowPrerelease
```


## <a name="release-notes"></a>リリース ノート

* 2002 更新プログラムでサポートされています。  

  Azure Stack Hub 2.0.0 は破壊的変更を伴うリリースです。 このモジュールは、AzureRM モジュールではなく Az モジュールを使用します。 移行ガイドと、破壊的変更の一覧については、「[Azure Stack Hub での AzureRM から Azure PowerShell Az への移行](https://aka.ms/AA7qsji)」を参照してください。
