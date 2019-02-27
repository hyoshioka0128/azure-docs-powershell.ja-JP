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
ms.openlocfilehash: af34497f243ce8f4f718e88312f6ad54eb6ad848
ms.sourcegitcommit: 993db64e68b222acbcfdeef2e81eb3316b160858
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/14/2019
ms.locfileid: "56240533"
---
# <a name="azure-stack-module-170"></a>Azure Stack Module 1.7.0

## <a name="requirements"></a>要件:
サポートされている Azure Stack の最小バージョンは 1901 です。

注:以前のバージョンを使用している場合は、バージョン 1.7.0 をインストールしてください

## <a name="install"></a>Install
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.0
```
## <a name="release-notes"></a>リリース ノート
* 1901 更新プログラムでサポートされています
* これは重大な変更のリリースです。 重大な変更について詳しくは、 https://aka.ms/azspshmigration170 を参照してください。
* Azs.Backup.Admin モジュール * 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。 対称キーのサポートは非推奨となりました。
* Azs.Fabric.Admin モジュール       * 非推奨           * Get-AzsInfrastructureVolume が非推奨となったため、新しいコマンドレット Get-AzsVolume を提供           * Get-AzsStorageSystem が非推奨となったため、新しいコマンドレット Get-AzsStorageSubSystem を提供           * Get-AzsStoragePool が非推奨となったため、StorageSubSystem オブジェクトに容量のプロパティが含まれる
* Azs.Compute.Admin モジュール           * バグの修正:Add-AzsPlatformImage、Get-AzsPlatformImage :成功パスでのみ ConvertTo-PlatformImageObject を呼び出します。           * バグの修正:Add-AzsVmExtension、Get-AzsVmExtension :成功パスでのみ ConvertTo-VmExtensionObject を呼び出します。
* Azs.Storage.Admin モジュール           * バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。

