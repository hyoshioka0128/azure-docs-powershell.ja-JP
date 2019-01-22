---
title: Azure Stack 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack 管理の PowerShell の概要と、インストールおよび構成の手順。
author: bganapa
ms.author: bganapa
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 09/21/2018
ms.openlocfilehash: b0e85bec82b9b7c876b2bbf337b603c8d68cf6a3
ms.sourcegitcommit: 4e1174236796e7da929ff276addb32e42c18b707
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "54240137"
---
# <a name="azure-stack-module-160"></a><span data-ttu-id="e8343-103">Azure Stack Module 1.6.0</span><span class="sxs-lookup"><span data-stu-id="e8343-103">Azure Stack Module 1.6.0</span></span>

## <a name="requirements"></a><span data-ttu-id="e8343-104">要件:</span><span class="sxs-lookup"><span data-stu-id="e8343-104">Requirements:</span></span>
<span data-ttu-id="e8343-105">サポートされている Azure Stack の最小バージョンは 1811 です。</span><span class="sxs-lookup"><span data-stu-id="e8343-105">Minimum supported Azure Stack version is 1811.</span></span>

<span data-ttu-id="e8343-106">注:以前のバージョンを使用している場合は、バージョン 1.6.0 をインストールしてください</span><span class="sxs-lookup"><span data-stu-id="e8343-106">Note: If you are using an earlier version install version 1.6.0</span></span>

## <a name="install"></a><span data-ttu-id="e8343-107">Install</span><span class="sxs-lookup"><span data-stu-id="e8343-107">Install</span></span>
```
# Remove previous versions of AzureStack and AzureRM modules
Uninstall-Module -Name AzureRM -Force
Uninstall-Module -Name Azure.Storage -Force
Uninstall-Module -Name AzureStack -Force
Get-Module -Name "Azs*" -ListAvailable | Uninstall-Module  -Force 
Get-Module -Name "AzureRm*" -ListAvailable | Uninstall-Module  -Force

# Install the AzureRM.Bootstrapper module. Select Yes when prompted to install NuGet
Install-Module -Name AzureRm.BootStrapper

# Install and import the API Version Profile required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2018-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.6.0
```

## <a name="release-notes"></a><span data-ttu-id="e8343-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="e8343-108">Release Notes</span></span>
* <span data-ttu-id="e8343-109">1811 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="e8343-109">Supported with 1811 update</span></span>
* <span data-ttu-id="e8343-110">Azs.Compute.Admin モジュール</span><span class="sxs-lookup"><span data-stu-id="e8343-110">Azs.Compute.Admin Module</span></span>
    * <span data-ttu-id="e8343-111">New-DataDiskObject の Azs プレフィックスが見つからない問題を修正し、今後の廃止の警告と共にエイリアスを追加しました。</span><span class="sxs-lookup"><span data-stu-id="e8343-111">Fixed missing Azs prefix for New-DataDiskObject and added alias with warning of future deprecation.</span></span>
* <span data-ttu-id="e8343-112">Azs.Update.Admin モジュール</span><span class="sxs-lookup"><span data-stu-id="e8343-112">Azs.Update.Admin Module</span></span>
    * <span data-ttu-id="e8343-113">Install-AzsUpdate の前に Test-AzureStack を実行することを勧める警告を追加しました</span><span class="sxs-lookup"><span data-stu-id="e8343-113">Added a warning to recommend running Test-AzureStack before Install-AzsUpdate</span></span>
* <span data-ttu-id="e8343-114">Azs.Fabric.Admin</span><span class="sxs-lookup"><span data-stu-id="e8343-114">Azs.Fabric.Admin</span></span>
    * <span data-ttu-id="e8343-115">新しいコマンドレット (機能は Azure Stack 1811 以降によってサポートされています)</span><span class="sxs-lookup"><span data-stu-id="e8343-115">New cmdlet (The features are supported by Azure Stack 1811+)</span></span>
        * <span data-ttu-id="e8343-116">Get-AzsDrive</span><span class="sxs-lookup"><span data-stu-id="e8343-116">Get-AzsDrive</span></span>
        * <span data-ttu-id="e8343-117">Get-AzsVolume</span><span class="sxs-lookup"><span data-stu-id="e8343-117">Get-AzsVolume</span></span>
        * <span data-ttu-id="e8343-118">Get-AzsStorageSubSystem</span><span class="sxs-lookup"><span data-stu-id="e8343-118">Get-AzsStorageSubSystem</span></span>
    * <span data-ttu-id="e8343-119">非推奨</span><span class="sxs-lookup"><span data-stu-id="e8343-119">Deprecation</span></span>
        * <span data-ttu-id="e8343-120">Get-AzsInfrastructureVolume は、コマンドレット Get-AzsVolume のエイリアスになりました</span><span class="sxs-lookup"><span data-stu-id="e8343-120">Get-AzsInfrastructureVolume is an alias now to the cmdlet Get-AzsVolume</span></span>
* <span data-ttu-id="e8343-121">Azs.InfrastructureInsights.Admin</span><span class="sxs-lookup"><span data-stu-id="e8343-121">Azs.InfrastructureInsights.Admin</span></span>
    *  <span data-ttu-id="e8343-122">新しいコマンドレット Repair-AzsAlert を追加しました</span><span class="sxs-lookup"><span data-stu-id="e8343-122">Added a new cmdlet Repair-AzsAlert</span></span>
* <span data-ttu-id="e8343-123">Azs.Storage.Admin</span><span class="sxs-lookup"><span data-stu-id="e8343-123">Azs.Storage.Admin</span></span>
    * <span data-ttu-id="e8343-124">既定のクォータ値が使用されないバグを修正</span><span class="sxs-lookup"><span data-stu-id="e8343-124">Bug fix where default quota values are not being used</span></span>
* <span data-ttu-id="e8343-125">Azs.Subscriptions.Admin モジュール</span><span class="sxs-lookup"><span data-stu-id="e8343-125">Azs.Subscriptions.Admin Module</span></span>
    * <span data-ttu-id="e8343-126">New-AddonPlanDefinitionObject の Azs プレフィックスが見つからない問題を修正し、今後の廃止の警告と共にエイリアスを追加しました。</span><span class="sxs-lookup"><span data-stu-id="e8343-126">Fixed missing Azs prefix for New-AddonPlanDefinitionObject and added alias with warning of future deprecation.</span></span>
