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
ms.sourcegitcommit: 4c61442a2df1cee633ce93cad9f6bc793803baa2
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2020
ms.locfileid: "81524967"
---
# <a name="azure-stack-hub-module-200"></a><span data-ttu-id="e53d7-103">Azure Stack Hub モジュール 2.0.0</span><span class="sxs-lookup"><span data-stu-id="e53d7-103">Azure Stack Hub Module 2.0.0</span></span>

## <a name="requirements"></a><span data-ttu-id="e53d7-104">要件:</span><span class="sxs-lookup"><span data-stu-id="e53d7-104">Requirements:</span></span>

<span data-ttu-id="e53d7-105">サポートされている Azure Stack Hub の最小バージョンは 2002 です。</span><span class="sxs-lookup"><span data-stu-id="e53d7-105">Minimum supported Azure Stack Hub version is 2002.</span></span>

<span data-ttu-id="e53d7-106">注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e53d7-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="e53d7-107">インストール</span><span class="sxs-lookup"><span data-stu-id="e53d7-107">Install</span></span>

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


## <a name="release-notes"></a><span data-ttu-id="e53d7-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="e53d7-108">Release Notes</span></span>

* <span data-ttu-id="e53d7-109">2002 更新プログラムでサポートされています。</span><span class="sxs-lookup"><span data-stu-id="e53d7-109">Supported with 2002 update.</span></span>  

  <span data-ttu-id="e53d7-110">Azure Stack Hub 2.0.0 は破壊的変更を伴うリリースです。</span><span class="sxs-lookup"><span data-stu-id="e53d7-110">The Azure Stack Hub 2.0.0 is a breaking change.</span></span> <span data-ttu-id="e53d7-111">このモジュールは、AzureRM モジュールではなく Az モジュールを使用します。</span><span class="sxs-lookup"><span data-stu-id="e53d7-111">The module uses the Az module rather than the AzureRM module.</span></span> <span data-ttu-id="e53d7-112">移行ガイドと、破壊的変更の一覧については、「[Azure Stack Hub での AzureRM から Azure PowerShell Az への移行](https://aka.ms/AA7qsji)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e53d7-112">You can find a migration guide and a list of breaking changes in [Migrate from AzureRM to Azure PowerShell Az in Azure Stack Hub](https://aka.ms/AA7qsji).</span></span>
