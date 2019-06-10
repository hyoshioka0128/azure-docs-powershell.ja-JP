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
ms.openlocfilehash: af0343e5ad92fa7f2b5c10e3e67cb7e10feb81c6
ms.sourcegitcommit: 0fdccb57a356b6e7c35a77b1f76e01fb96ef582b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/17/2019
ms.locfileid: "65855790"
---
# <a name="azure-stack-module-172"></a>Azure Stack Module 1.7.2

## <a name="requirements"></a>要件:

サポートされている Azure Stack の最小バージョンは 1904 です。

注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。

## <a name="install-powershell-for-azure-stack"></a>PowerShell for Azure Stack をインストールする

インストールには 3 つの手順があります:

1. Azure Stack のバージョンに応じて Azure Stack PowerShell をインストールする
2. 追加のストレージ機能を有効にする
3. PowerShell のインストールを確認する

### <a name="install-azure-stack-powershell"></a>Azure Stack PowerShell のインストール

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install the AzureRM.BootStrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRM.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Get-AzureRmProfile -Update
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

### <a name="enable-additional-storage-features"></a>追加のストレージ機能を有効にする

```
# Install the Azure.Storage module version 4.5.0
Install-Module -Name Azure.Storage -RequiredVersion 4.5.0 -Force -AllowClobber

# Install the AzureRm.Storage module version 5.0.4
Install-Module -Name AzureRM.Storage -RequiredVersion 5.0.4 -Force -AllowClobber

# Remove incompatible storage module installed by AzureRM.Storage
Uninstall-Module Azure.Storage -RequiredVersion 4.6.1 -Force

# Load the modules explicitly specifying the versions
Import-Module -Name Azure.Storage -RequiredVersion 4.5.0
Import-Module -Name AzureRM.Storage -RequiredVersion 5.0.4
```

## <a name="release-notes"></a>リリース ノート

* 1904 更新プログラムでサポートされています
* これは重大な変更のリリースです。 重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。
* Azs.Backup.Admin モジュール * 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。 対称キーのサポートは非推奨となりました。
* Azs.Fabric.Admin モジュール       * 非推奨           * Get-AzsInfrastructureVolume が非推奨となったため、新しいコマンドレット Get-AzsVolume を提供           * Get-AzsStorageSystem が非推奨となったため、新しいコマンドレット Get-AzsStorageSubSystem を提供           * Get-AzsStoragePool が非推奨となったため、StorageSubSystem オブジェクトに容量のプロパティが含まれる
* Azs.Compute.Admin モジュール           * バグの修正:Add-AzsPlatformImage、Get-AzsPlatformImage :成功パスでのみ ConvertTo-PlatformImageObject を呼び出します。           * バグの修正:Add-AzsVmExtension、Get-AzsVmExtension :成功パスでのみ ConvertTo-VmExtensionObject を呼び出します。
* Azs.Storage.Admin モジュール           * バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。
