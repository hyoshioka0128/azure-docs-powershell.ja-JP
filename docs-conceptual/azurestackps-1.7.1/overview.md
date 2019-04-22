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
ms.sourcegitcommit: ae4540a90508db73335a54408dfd6cdf3712a1e9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/18/2019
ms.locfileid: "58808062"
---
# <a name="azure-stack-module-171"></a><span data-ttu-id="7b895-103">Azure Stack Module 1.7.1</span><span class="sxs-lookup"><span data-stu-id="7b895-103">Azure Stack Module 1.7.1</span></span>

## <a name="requirements"></a><span data-ttu-id="7b895-104">要件:</span><span class="sxs-lookup"><span data-stu-id="7b895-104">Requirements:</span></span>

<span data-ttu-id="7b895-105">サポートされている Azure Stack の最小バージョンは 1901 です。</span><span class="sxs-lookup"><span data-stu-id="7b895-105">Minimum supported Azure Stack version is 1901.</span></span>

<span data-ttu-id="7b895-106">注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b895-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="7b895-107">Install</span><span class="sxs-lookup"><span data-stu-id="7b895-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.4.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.1
```

## <a name="release-notes"></a><span data-ttu-id="7b895-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="7b895-108">Release Notes</span></span>

* <span data-ttu-id="7b895-109">1901 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="7b895-109">Supported with 1901 update</span></span>
* <span data-ttu-id="7b895-110">これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="7b895-110">This a breaking change release.</span></span> <span data-ttu-id="7b895-111">重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7b895-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="7b895-112">Azs.Backup.Admin モジュール \* 重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。</span><span class="sxs-lookup"><span data-stu-id="7b895-112">Azs.Backup.Admin Module \* Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="7b895-113">対称キーのサポートは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="7b895-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="7b895-114">Azs.Fabric.Admin モジュール       \* 非推奨           \* Get-AzsInfrastructureVolume が非推奨となったため、新しいコマンドレット Get-AzsVolume を提供           \* Get-AzsStorageSystem が非推奨となったため、新しいコマンドレット Get-AzsStorageSubSystem を提供           \* Get-AzsStoragePool が非推奨となったため、StorageSubSystem オブジェクトに容量のプロパティが含まれる</span><span class="sxs-lookup"><span data-stu-id="7b895-114">Azs.Fabric.Admin Module       \* Deprecation           \* Get-AzsInfrastructureVolume has been deprecated, we provide new cmdlet Get-AzsVolume           \* Get-AzsStorageSystem has been deprecated, we provide new cmdlet Get-AzsStorageSubSystem           \* Get-AzsStoragePool has been deprecated, the StorageSubSystem object has the capacity property</span></span>
* <span data-ttu-id="7b895-115">Azs.Compute.Admin モジュール           \* バグの修正:Add-AzsPlatformImage、Get-AzsPlatformImage :成功パスでのみ ConvertTo-PlatformImageObject を呼び出します。           \* バグの修正:Add-AzsVmExtension、Get-AzsVmExtension :成功パスでのみ ConvertTo-VmExtensionObject を呼び出します。</span><span class="sxs-lookup"><span data-stu-id="7b895-115">Azs.Compute.Admin Module           \* BugFix: Add-AzsPlatformImage, Get-AzsPlatformImage : Calling ConvertTo-PlatformImageObject only in the success path           \* BugFix: Add-AzsVmExtension, Get-AzsVmExtension : Calling ConvertTo-VmExtensionObject only in the success path</span></span>
* <span data-ttu-id="7b895-116">Azs.Storage.Admin モジュール           \* バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="7b895-116">Azs.Storage.Admin Module           \* Bug fix - New Storage Quota uses defaults if none provided.'</span></span>
