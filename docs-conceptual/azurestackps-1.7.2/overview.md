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
# <a name="azure-stack-module-172"></a><span data-ttu-id="bee84-103">Azure Stack Module 1.7.2</span><span class="sxs-lookup"><span data-stu-id="bee84-103">Azure Stack Module 1.7.2</span></span>

## <a name="requirements"></a><span data-ttu-id="bee84-104">要件:</span><span class="sxs-lookup"><span data-stu-id="bee84-104">Requirements:</span></span>

<span data-ttu-id="bee84-105">サポートされている Azure Stack の最小バージョンは 1904 です。</span><span class="sxs-lookup"><span data-stu-id="bee84-105">Minimum supported Azure Stack version is 1904.</span></span>

<span data-ttu-id="bee84-106">注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bee84-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="bee84-107">Install</span><span class="sxs-lookup"><span data-stu-id="bee84-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Install-Module -Name AzureRM -RequiredVersion 2.5.0

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.7.2
```

## <a name="release-notes"></a><span data-ttu-id="bee84-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="bee84-108">Release Notes</span></span>

* <span data-ttu-id="bee84-109">1904 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="bee84-109">Supported with 1904 update</span></span>
* <span data-ttu-id="bee84-110">これは重大な変更のリリースです。</span><span class="sxs-lookup"><span data-stu-id="bee84-110">This a breaking change release.</span></span> <span data-ttu-id="bee84-111">重大な変更について詳しくは、<https://aka.ms/azspshmigration170> を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bee84-111">For details on the breaking changes, refer to <https://aka.ms/azspshmigration170></span></span>
* <span data-ttu-id="bee84-112">重大な変更:バックアップが証明書ベースの暗号化モードに変更されました。</span><span class="sxs-lookup"><span data-stu-id="bee84-112">Breaking change: Backup changes to cert-based encryption mode.</span></span> <span data-ttu-id="bee84-113">対称キーのサポートは非推奨となりました。</span><span class="sxs-lookup"><span data-stu-id="bee84-113">Support for symmetric keys is deprecated.</span></span>
* <span data-ttu-id="bee84-114">重大な変更について詳しくは、 https://aka.ms/azspshmigration170 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bee84-114">For details on the breaking changes, refer to https://aka.ms/azspshmigration170</span></span>
* <span data-ttu-id="bee84-115">Azs.Storage.Admin モジュール</span><span class="sxs-lookup"><span data-stu-id="bee84-115">Azs.Storage.Admin Module</span></span> 
* <span data-ttu-id="bee84-116">バグの修正 - 新しい Storage クォータでは、値が未指定の場合に既定値が使用されます。</span><span class="sxs-lookup"><span data-stu-id="bee84-116">Bug fix - New Storage Quota uses defaults if none provided.</span></span>