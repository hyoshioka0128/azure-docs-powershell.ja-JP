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
ms.openlocfilehash: 7e728a31578989d8ce5e200491111ed9e11acba1
ms.sourcegitcommit: 5a5b6dd216d5f805204244146cf6f88ad2f34fb4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/19/2018
ms.locfileid: "36238004"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="df0cd-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="df0cd-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="df0cd-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="df0cd-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="df0cd-105">これは、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで使用することも、ローカル コンピューターにインストールして PowerShell セッションで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="df0cd-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="df0cd-106">Azure PowerShell は、[Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで実行するか、所有するコンピューターに[インストール](install-azurerm-ps.md)します。</span><span class="sxs-lookup"><span data-stu-id="df0cd-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="df0cd-107">実際に使う際には、[概要](get-started-azureps.md)の記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="df0cd-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="df0cd-108">最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="df0cd-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="df0cd-109">Azure PowerShell の基本的な使い方については、次のサンプルが参考になります。</span><span class="sxs-lookup"><span data-stu-id="df0cd-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="df0cd-110">Linux virtual machines</span><span class="sxs-lookup"><span data-stu-id="df0cd-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="df0cd-111">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="df0cd-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="df0cd-112">Web Apps</span><span class="sxs-lookup"><span data-stu-id="df0cd-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="df0cd-113">SQL Database</span><span class="sxs-lookup"><span data-stu-id="df0cd-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

> [!NOTE]
> <span data-ttu-id="df0cd-114">変換できないクラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="df0cd-114">If you have deployments that use the classic deployment model that cannot be converted, you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="df0cd-115">詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="df0cd-115">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

### <a name="need-help-with-powershell"></a><span data-ttu-id="df0cd-116">PowerShell について不明点がある場合</span><span class="sxs-lookup"><span data-stu-id="df0cd-116">Need help with PowerShell?</span></span>

<span data-ttu-id="df0cd-117">PowerShell についてまだよく知らない方は、PowerShell の概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="df0cd-117">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span>

* [<span data-ttu-id="df0cd-118">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="df0cd-118">Installing PowerShell</span></span>](/powershell/scripting/installing-windows-powershell)
* [<span data-ttu-id="df0cd-119">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="df0cd-119">Scripting with PowerShell</span></span>](/powershell/scripting/scripting-with-windows-powershell)

<span data-ttu-id="df0cd-120">また、「[PowerShell Basics: (Part 1) Getting Started with PowerShell (PowerShell の基礎: (パート 1) PowerShell の基本)](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)」のビデオもご覧ください。</span><span class="sxs-lookup"><span data-stu-id="df0cd-120">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="df0cd-121">または、Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)に関するクラスにご参加ください。</span><span class="sxs-lookup"><span data-stu-id="df0cd-121">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="df0cd-122">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="df0cd-122">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="df0cd-123">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="df0cd-123">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="df0cd-124">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="df0cd-124">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="df0cd-125">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="df0cd-125">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="df0cd-126">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="df0cd-126">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)