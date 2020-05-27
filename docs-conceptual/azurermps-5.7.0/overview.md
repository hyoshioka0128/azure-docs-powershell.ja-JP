---
title: Azure PowerShell の概要 | Microsoft Docs
description: Azure PowerShell について概説すると共に、インストールと構成に関するページへのリンクを紹介します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/31/2017
ms.openlocfilehash: 97afd1d9f7792540e94d79023c0450b192cb2fb8
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83384862"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="0caf0-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="0caf0-103">Overview of Azure PowerShell</span></span>

[!INCLUDE[az-replacing-azurerm.md](../includes/az-replacing-azurerm.md)]

<span data-ttu-id="0caf0-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="0caf0-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="0caf0-105">これは、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで使用することも、ローカル コンピューターにインストールして PowerShell セッションで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="0caf0-105">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span>

<span data-ttu-id="0caf0-106">Azure PowerShell は、[Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで実行するか、所有するコンピューターに[インストール](install-azurerm-ps.md)します。</span><span class="sxs-lookup"><span data-stu-id="0caf0-106">Use the [Cloud Shell](/azure/cloud-shell/overview) to run the Azure PowerShell in your browser, or [install](install-azurerm-ps.md) it on own computer.</span></span> <span data-ttu-id="0caf0-107">実際に使う際には、[概要](get-started-azureps.md)の記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="0caf0-107">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="0caf0-108">最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0caf0-108">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="0caf0-109">Azure PowerShell の基本的な使い方については、次のサンプルが参考になります。</span><span class="sxs-lookup"><span data-stu-id="0caf0-109">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="0caf0-110">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="0caf0-110">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="0caf0-111">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="0caf0-111">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="0caf0-112">Web Apps</span><span class="sxs-lookup"><span data-stu-id="0caf0-112">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="0caf0-113">SQL Database</span><span class="sxs-lookup"><span data-stu-id="0caf0-113">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="0caf0-114">PowerShell の基礎を学ぶ</span><span class="sxs-lookup"><span data-stu-id="0caf0-114">Learn PowerShell basics</span></span>

<span data-ttu-id="0caf0-115">PowerShell についてまだよく知らない方は、PowerShell の概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="0caf0-115">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span>

* [<span data-ttu-id="0caf0-116">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="0caf0-116">Installing PowerShell</span></span>](/powershell/scripting/installing-windows-powershell)
* [<span data-ttu-id="0caf0-117">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="0caf0-117">Scripting with PowerShell</span></span>](/powershell/scripting/scripting-with-windows-powershell)

<span data-ttu-id="0caf0-118">次のビデオをご覧いただくこともできます。[PowerShell の基礎: (パート 1) PowerShell の概要](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)。</span><span class="sxs-lookup"><span data-stu-id="0caf0-118">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="0caf0-119">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="0caf0-119">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="0caf0-120">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="0caf0-120">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="0caf0-121">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="0caf0-121">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="0caf0-122">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="0caf0-122">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="0caf0-123">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="0caf0-123">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
