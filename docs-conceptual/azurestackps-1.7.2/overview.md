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
ms.openlocfilehash: 1b3d707e862dd0c21e9e6b0a89f429ff21b1a99d
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "68861340"
---
# <a name="azure-stack-module-172"></a><span data-ttu-id="4a26e-103">Azure Stack Module 1.7.2</span><span class="sxs-lookup"><span data-stu-id="4a26e-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="4a26e-104">要件:</span><span class="sxs-lookup"><span data-stu-id="4a26e-104">Requirements:</span></span>

<span data-ttu-id="4a26e-105">サポートされている Azure Stack の最小バージョンは 1904 です。</span><span class="sxs-lookup"><span data-stu-id="4a26e-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="4a26e-106">注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a26e-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="4a26e-107">インストール</span><span class="sxs-lookup"><span data-stu-id="4a26e-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a><span data-ttu-id="4a26e-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="4a26e-108">Release Notes</span></span>

* <span data-ttu-id="4a26e-109">1904 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="4a26e-109">Supported with 1904 update</span></span>
* <span data-ttu-id="4a26e-110">これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="4a26e-110">This a breaking change release.</span></span> <span data-ttu-id="4a26e-111">重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a26e-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="4a26e-112">重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。</span><span class="sxs-lookup"><span data-stu-id="4a26e-112">Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="4a26e-113">対称キーのサポートは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="4a26e-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="4a26e-114">重大な変更について詳しくは、 https://aka.ms/azspshmigration170 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a26e-114">For details on the breaking changes, refer to https://aka.ms/azspshmigration170</span></span>
* <span data-ttu-id="4a26e-115">Azs.Storage.Admin モジュール</span><span class="sxs-lookup"><span data-stu-id="4a26e-115">Azs.Storage.Admin Module</span></span> 
* <span data-ttu-id="4a26e-116">バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4a26e-116">Bug fix - New Storage Quota uses defaults if none provided.</span></span>
