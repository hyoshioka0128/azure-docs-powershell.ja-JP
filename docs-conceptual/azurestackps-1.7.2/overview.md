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
# <a name="azure-stack-module-172"></a><span data-ttu-id="0cc9d-103">Azure Stack Module 1.7.2</span><span class="sxs-lookup"><span data-stu-id="0cc9d-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="0cc9d-104">要件:</span><span class="sxs-lookup"><span data-stu-id="0cc9d-104">Requirements:</span></span>

<span data-ttu-id="0cc9d-105">サポートされている Azure Stack の最小バージョンは 1904 です。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="0cc9d-106">注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install-powershell-for-azure-stack"></a><span data-ttu-id="0cc9d-107">PowerShell for Azure Stack をインストールする</span><span class="sxs-lookup"><span data-stu-id="0cc9d-107">Install PowerShell for Azure Stack</span></span>

<span data-ttu-id="0cc9d-108">インストールには 3 つの手順があります:</span><span class="sxs-lookup"><span data-stu-id="0cc9d-108">Installation has three steps:</span></span>

1. <span data-ttu-id="0cc9d-109">Azure Stack のバージョンに応じて Azure Stack PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="0cc9d-109">Install Azure Stack PowerShell depending on your version of Azure Stack</span></span>
2. <span data-ttu-id="0cc9d-110">追加のストレージ機能を有効にする</span><span class="sxs-lookup"><span data-stu-id="0cc9d-110">Enable additional storage features</span></span>
3. <span data-ttu-id="0cc9d-111">PowerShell のインストールを確認する</span><span class="sxs-lookup"><span data-stu-id="0cc9d-111">Confirm the installation of PowerShell</span></span>

### <a name="install-azure-stack-powershell"></a><span data-ttu-id="0cc9d-112">Azure Stack PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="0cc9d-112">Install Azure Stack PowerShell</span></span>

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

### <a name="enable-additional-storage-features"></a><span data-ttu-id="0cc9d-113">追加のストレージ機能を有効にする</span><span class="sxs-lookup"><span data-stu-id="0cc9d-113">Enable additional storage features</span></span>

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

## <a name="release-notes"></a><span data-ttu-id="0cc9d-114">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="0cc9d-114">Release Notes</span></span>

* <span data-ttu-id="0cc9d-115">1904 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="0cc9d-115">Supported with 1904 update</span></span>
* <span data-ttu-id="0cc9d-116">これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-116">This a breaking change release.</span></span> <span data-ttu-id="0cc9d-117">重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-117">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="0cc9d-118">Azs.Backup.Admin モジュール \* 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-118">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="0cc9d-119">対称キーのサポートは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-119">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="0cc9d-120">Azs.Fabric.Admin モジュール       \* 非推奨           \* Get-AzsInfrastructureVolume が非推奨となったため、新しいコマンドレット Get-AzsVolume を提供           \* Get-AzsStorageSystem が非推奨となったため、新しいコマンドレット Get-AzsStorageSubSystem を提供           \* Get-AzsStoragePool が非推奨となったため、StorageSubSystem オブジェクトに容量のプロパティが含まれる</span><span class="sxs-lookup"><span data-stu-id="0cc9d-120">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="0cc9d-121">Azs.Compute.Admin モジュール           \* バグの修正:Add-AzsPlatformImage、Get-AzsPlatformImage :成功パスでのみ ConvertTo-PlatformImageObject を呼び出します。           \* バグの修正:Add-AzsVmExtension、Get-AzsVmExtension :成功パスでのみ ConvertTo-VmExtensionObject を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-121">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="0cc9d-122">Azs.Storage.Admin モジュール           \* バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="0cc9d-122">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
