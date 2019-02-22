---
title: Azure PowerShell の概要 | Microsoft Docs
description: Azure PowerShell について概説すると共に、インストールと構成に関するページへのリンクを紹介します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 08/31/2017
ms.openlocfilehash: 5ee8572ccb8e9fc2de11c2253a1815a666e038a7
ms.sourcegitcommit: 2054a8f74cd9bf5a50ea7fdfddccaa632c842934
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/12/2019
ms.locfileid: "56153584"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="43111-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="43111-103">Overview of Azure PowerShell</span></span>

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

<span data-ttu-id="43111-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="43111-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="43111-105">これは、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで使用することも、ローカル コンピューターにインストールして PowerShell セッションで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="43111-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="43111-106">Azure PowerShell は、[Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで実行するか、所有するコンピューターに[インストール](install-azurerm-ps.md)します。</span><span class="sxs-lookup"><span data-stu-id="43111-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="43111-107">実際に使う際には、[概要](get-started-azureps.md)の記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="43111-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="43111-108">最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="43111-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="43111-109">Azure PowerShell の基本的な使い方については、次のサンプルが参考になります。</span><span class="sxs-lookup"><span data-stu-id="43111-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="43111-110">Linux virtual machines</span><span class="sxs-lookup"><span data-stu-id="43111-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="43111-111">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="43111-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="43111-112">Web Apps</span><span class="sxs-lookup"><span data-stu-id="43111-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="43111-113">SQL Database</span><span class="sxs-lookup"><span data-stu-id="43111-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="43111-114">PowerShell の基礎を学ぶ</span><span class="sxs-lookup"><span data-stu-id="43111-114">Learn PowerShell basics</span></span>

<span data-ttu-id="43111-115">PowerShell についてまだよく知らない方は、PowerShell の概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="43111-115">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span>

* [<span data-ttu-id="43111-116">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="43111-116">Installing PowerShell</span></span>](/powershell/scripting/installing-windows-powershell)
* [<span data-ttu-id="43111-117">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="43111-117">Scripting with PowerShell</span></span>](/powershell/scripting/scripting-with-windows-powershell)

<span data-ttu-id="43111-118">次のビデオをご覧いただくこともできます。[PowerShell の基礎: (パート 1) PowerShell の概要](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)。</span><span class="sxs-lookup"><span data-stu-id="43111-118">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="43111-119">または、Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)に関するクラスにご参加ください。</span><span class="sxs-lookup"><span data-stu-id="43111-119">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="43111-120">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="43111-120">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="43111-121">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="43111-121">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="43111-122">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="43111-122">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="43111-123">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="43111-123">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="43111-124">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="43111-124">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
