---
title: Azure Stack 管理の PowerShell の概要 | Microsoft Docs
description: Azure Stack 管理の PowerShell の概要と、インストールおよび構成の手順。
author: sijuman
ms.author: sijuman
manager: knithinc
ms.devlang: powershell
ms.topic: conceptual
ms.manager: knithinc
ms.date: 02/24/2020
ms.openlocfilehash: ec406c80de6b457f7e340a23fe8caf2ab83be46a
ms.sourcegitcommit: a6f2fc500242de6248224278d743fd09aac2fafd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2020
ms.locfileid: "78264412"
---
# <a name="azure-stack-module-180"></a><span data-ttu-id="29794-103">Azure Stack Module 1.8.0</span><span class="sxs-lookup"><span data-stu-id="29794-103">Azure Stack Module 1.8.0</span></span>

## <a name="requirements"></a><span data-ttu-id="29794-104">要件:</span><span class="sxs-lookup"><span data-stu-id="29794-104">Requirements:</span></span>

<span data-ttu-id="29794-105">サポートされている Azure Stack の最小バージョンは 1910 です。</span><span class="sxs-lookup"><span data-stu-id="29794-105">Minimum supported Azure Stack version is 1910.</span></span>

<span data-ttu-id="29794-106">注:以前のバージョンの Azure Stack については、「[Azure Stack Powershell のインストール](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="29794-106">Note: For earlier versions of Azure Stack check [Install Azure Stack Powershell](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install#install-azure-stack-powershell)</span></span>

## <a name="install"></a><span data-ttu-id="29794-107">インストール</span><span class="sxs-lookup"><span data-stu-id="29794-107">Install</span></span>

```powershell
# Remove previous versions of AzureStack and AzureRM modules
Get-Module -Name Azs.* -ListAvailable | Uninstall-Module -Force -Verbose
Get-Module -Name Azure* -ListAvailable | Uninstall-Module -Force -Verbose

# Install and import the API Version Modules required by Azure Stack into the current PowerShell session.
Use-AzureRmProfile -Profile 2019-03-01-hybrid -Force

# Install Azure Stack Admin Module
Install-Module -Name AzureStack -RequiredVersion 1.8.0
```

## <a name="release-notes"></a><span data-ttu-id="29794-108">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="29794-108">Release Notes</span></span>

* <span data-ttu-id="29794-109">1910 更新プログラムでサポートされています</span><span class="sxs-lookup"><span data-stu-id="29794-109">Supported with 1910 update</span></span>
* <span data-ttu-id="29794-110">変更内容:</span><span class="sxs-lookup"><span data-stu-id="29794-110">Changes include:</span></span>

    - <span data-ttu-id="29794-111">**新しい DRP 管理モジュール**:デプロイ リソース プロバイダー (DRP) を使用すると、Azure Stack Hub に対するリソース プロバイダーの調整されたデプロイが可能になります。</span><span class="sxs-lookup"><span data-stu-id="29794-111">**New DRP Admin module**: The Deployment Resource Provider (DRP) enables orchestrated deployments of resource providers to Azure Stack Hub.</span></span> <span data-ttu-id="29794-112">これらのコマンドを使うと、DRP とやり取りする Azure Resource Manager レイヤーとやり取りできます。</span><span class="sxs-lookup"><span data-stu-id="29794-112">These commands interact with the Azure Resource Manager layer to interact with DRP.</span></span>

    - <span data-ttu-id="29794-113">**BRP**:</span><span class="sxs-lookup"><span data-stu-id="29794-113">**BRP**:</span></span>
        - <span data-ttu-id="29794-114">Azure Stack インフラストラクチャ バックアップの 1 つのロールの復元をサポートします。</span><span class="sxs-lookup"><span data-stu-id="29794-114">Support single role restore for Azures stack infrastructure backup.</span></span>
        - <span data-ttu-id="29794-115">パラメーター `RoleName` をコマンドレット R`estore-AzsBackup` に追加します。</span><span class="sxs-lookup"><span data-stu-id="29794-115">Add parameter `RoleName` to cmdlet R`estore-AzsBackup`.</span></span>

    - <span data-ttu-id="29794-116">**FRP**:API バージョン 2019-05-01 の**ドライブ**と**ボリューム** リソースの破壊的変更。</span><span class="sxs-lookup"><span data-stu-id="29794-116">**FRP**: Breaking changes for **Drive** and **Volume** resources with API version 2019-05-01.</span></span> <span data-ttu-id="29794-117">これらの機能は Azure Stack Hub 1910 以降でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="29794-117">The features are supported by Azure Stack Hub 1910 and later:</span></span>
        - <span data-ttu-id="29794-118">ID、`Name`、`HealthStatus`、および `OperationalStatus` の値が変更されました。</span><span class="sxs-lookup"><span data-stu-id="29794-118">The value of ID, `Name`, `HealthStatus`, and `OperationalStatus` have been changed.</span></span>
        - <span data-ttu-id="29794-119">**ドライブ** リソースの新しいプロパティ `FirmwareVersion`、`IsIndicationEnabled`、`Manufacturer`、`StoragePool` がサポートされるようになりました。</span><span class="sxs-lookup"><span data-stu-id="29794-119">Supported new properties `FirmwareVersion`, `IsIndicationEnabled`, `Manufacturer`, and `StoragePool` for **Drive** resources.</span></span>
        - <span data-ttu-id="29794-120">**ドライブ** リソースのプロパティ `CanPool` および `CannotPoolReason` は廃止されました。代わりに `OperationalStatus` を使用してください。</span><span class="sxs-lookup"><span data-stu-id="29794-120">The properties `CanPool` and `CannotPoolReason` of **Drive** resources have been deprecated; use `OperationalStatus` instead.</span></span>
