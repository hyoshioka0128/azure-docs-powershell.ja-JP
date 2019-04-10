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
ms.openlocfilehash: 6568dc4e6c51e8f250aad2c4dd765c065fe6a8bf
ms.sourcegitcommit: d3069aba7d1ac248aff755e4b21533af1f73251d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/02/2019
ms.locfileid: "58808062"
---
# <a name="azure-stack-module-171"></a>Azure Stack Module 1.7.1

## <a name="requirements"></a>要件:

サポートされている Azure Stack の最小バージョンは 1901 です。

注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。

## <a name="install"></a>Install

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.1
```

## <a name="release-notes"></a>リリース ノート

* 1901 更新プログラムでサポートされています
* これは重大な変更のリリースです。 重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。
* Azs.Backup.Admin モジュール * 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。 対称キーのサポートは非推奨となりました。
* Azs.Fabric.Admin モジュール       * 非推奨           * Get-AzsInfrastructureVolume が非推奨となったため、新しいコマンドレット Get-AzsVolume を提供           * Get-AzsStorageSystem が非推奨となったため、新しいコマンドレット Get-AzsStorageSubSystem を提供           * Get-AzsStoragePool が非推奨となったため、StorageSubSystem オブジェクトに容量のプロパティが含まれる
* Azs.Compute.Admin モジュール           * バグの修正:Add-AzsPlatformImage、Get-AzsPlatformImage :成功パスでのみ ConvertTo-PlatformImageObject を呼び出します。           * バグの修正:Add-AzsVmExtension、Get-AzsVmExtension :成功パスでのみ ConvertTo-VmExtensionObject を呼び出します。
* Azs.Storage.Admin モジュール           * バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。
