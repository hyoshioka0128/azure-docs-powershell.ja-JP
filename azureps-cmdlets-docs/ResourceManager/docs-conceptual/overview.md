---
title: "Azure PowerShell の概要 | Microsoft Docs"
description: "Azure PowerShell について概説すると共に、インストールと構成に関するページへのリンクを紹介します。"
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 07/26/2017
ms.openlocfilehash: 02bfc15fec83ed4078d9a054b450c5a3cd66b8e2
ms.sourcegitcommit: db5c50de90764a9bdc7c1f1dbca3aed5bfeb05fa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2017
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="402e8-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="402e8-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="402e8-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="402e8-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span>

<span data-ttu-id="402e8-105">ご利用のシステムで Azure PowerShell を使用するための準備については、[インストール](install-azurerm-ps.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="402e8-105">Review the [Install](install-azurerm-ps.md) article to get Azure PowerShell up and running on your system.</span></span> <span data-ttu-id="402e8-106">実際に使う際には、[概要](get-started-azureps.md)の記事をお読みください。</span><span class="sxs-lookup"><span data-stu-id="402e8-106">Then read the [Get Started](get-started-azureps.md) article to begin using it.</span></span> <span data-ttu-id="402e8-107">最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="402e8-107">For information about the latest release, see the [release notes](release-notes-azureps.md).</span></span>

<span data-ttu-id="402e8-108">Azure PowerShell の基本的な使い方については、次のサンプルが参考になります。</span><span class="sxs-lookup"><span data-stu-id="402e8-108">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="402e8-109">Linux 仮想マシン</span><span class="sxs-lookup"><span data-stu-id="402e8-109">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="402e8-110">Windows 仮想マシン</span><span class="sxs-lookup"><span data-stu-id="402e8-110">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="402e8-111">Web Apps</span><span class="sxs-lookup"><span data-stu-id="402e8-111">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="402e8-112">SQL Database</span><span class="sxs-lookup"><span data-stu-id="402e8-112">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

> [!NOTE]<span data-ttu-id="402e8-113"> > 変換できないクラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。</span><span class="sxs-lookup"><span data-stu-id="402e8-113"> > If you have deployments that use the classic deployment model that cannot be converted, you can install the Service Management version of Azure PowerShell.</span></span> <span data-ttu-id="402e8-114">詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="402e8-114">For more information, see [Install the Azure PowerShell Service Management module](/powershell/azure/servicemanagement/install-azure-ps).</span></span>

### <a name="need-help-with-powershell"></a><span data-ttu-id="402e8-115">PowerShell について不明点がある場合</span><span class="sxs-lookup"><span data-stu-id="402e8-115">Need help with PowerShell?</span></span>

<span data-ttu-id="402e8-116">PowerShell についてまだよく知らない方は、PowerShell の概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="402e8-116">If you are unfamiliar with PowerShell, you may find an introduction to PowerShell helpful.</span></span>

* [<span data-ttu-id="402e8-117">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="402e8-117">Installing PowerShell</span></span>](/powershell/scripting/installing-windows-powershell)
* [<span data-ttu-id="402e8-118">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="402e8-118">Scripting with PowerShell</span></span>](/powershell/scripting/scripting-with-windows-powershell)

<span data-ttu-id="402e8-119">また、「[PowerShell Basics: (Part 1) Getting Started with PowerShell (PowerShell の基礎: (パート 1) PowerShell の基本)](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)」のビデオもご覧ください。</span><span class="sxs-lookup"><span data-stu-id="402e8-119">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="402e8-120">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="402e8-120">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="402e8-121">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="402e8-121">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="402e8-122">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="402e8-122">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="402e8-123">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="402e8-123">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="402e8-124">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="402e8-124">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
