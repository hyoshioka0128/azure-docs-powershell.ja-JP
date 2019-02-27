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
# <a name="azure-stack-module-170"></a><span data-ttu-id="efa0e-103">Azure Stack Module 1.7.0</span><span class="sxs-lookup"><span data-stu-id="efa0e-103">Azure Stack Module 1.7.0</span></span>

## <a name="requirements"></a><span data-ttu-id="efa0e-104">要件:</span><span class="sxs-lookup"><span data-stu-id="efa0e-104">Requirements:</span></span>
<span data-ttu-id="efa0e-105">サポートされている Azure Stack の最小バージョンは 1901 です。</span><span class="sxs-lookup"><span data-stu-id="efa0e-105">Minimum supported Azure Stack version is 1901.</span></span>

<span data-ttu-id="efa0e-106">注:以前のバージョンを使用している場合は、バージョン 1.7.0 をインストールしてください</span><span class="sxs-lookup"><span data-stu-id="efa0e-106">Note: If you are using an earlier version install version 1.7.0</span></span>

## <a name="install"></a><span data-ttu-id="efa0e-107">Install</span><span class="sxs-lookup"><span data-stu-id="efa0e-107">Install</span></span>
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
## <a name="release-notes"></a><span data-ttu-id="efa0e-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="efa0e-108">Release Notes</span></span>
* <span data-ttu-id="efa0e-109">1901 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="efa0e-109">Supported with 1901 update</span></span>
* <span data-ttu-id="efa0e-110">これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="efa0e-110">This a breaking change release.</span></span> <span data-ttu-id="efa0e-111">重大な変更について詳しくは、 https://aka.ms/azspshmigration170 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="efa0e-111">For details on the breaking changes, refer to https://aka.ms/azspshmigration170</span></span>
* <span data-ttu-id="efa0e-112">Azs.Backup.Admin モジュール \* 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。</span><span class="sxs-lookup"><span data-stu-id="efa0e-112">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="efa0e-113">対称キーのサポートは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="efa0e-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="efa0e-114">Azs.Fabric.Admin モジュール       \* 非推奨           \* Get-AzsInfrastructureVolume が非推奨となったため、新しいコマンドレット Get-AzsVolume を提供           \* Get-AzsStorageSystem が非推奨となったため、新しいコマンドレット Get-AzsStorageSubSystem を提供           \* Get-AzsStoragePool が非推奨となったため、StorageSubSystem オブジェクトに容量のプロパティが含まれる</span><span class="sxs-lookup"><span data-stu-id="efa0e-114">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="efa0e-115">Azs.Compute.Admin モジュール           \* バグの修正:Add-AzsPlatformImage、Get-AzsPlatformImage :成功パスでのみ ConvertTo-PlatformImageObject を呼び出します。           \* バグの修正:Add-AzsVmExtension、Get-AzsVmExtension :成功パスでのみ ConvertTo-VmExtensionObject を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="efa0e-115">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="efa0e-116">Azs.Storage.Admin モジュール           \* バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="efa0e-116">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>

