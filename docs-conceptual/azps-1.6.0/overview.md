---
title: Azure PowerShell の概要
description: Azure PowerShell Az モジュールの概要と、インストールして使い始める方法に関する情報。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 01/10/2019
ms.openlocfilehash: 45ab083dd133c8c7b8dbe902484c92564bc216b9
ms.sourcegitcommit: 8f59e11e5c991543964154d63648aa1e6ae22512
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2019
ms.locfileid: "58475602"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="419ff-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="419ff-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="419ff-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="419ff-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="419ff-105">Azure PowerShell では .NET Standard が使用されているので、Windows、macOS、Linux で使用できます。</span><span class="sxs-lookup"><span data-stu-id="419ff-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="419ff-106">Azure PowerShell は、Azure Cloud Shell 上で利用することもできます。</span><span class="sxs-lookup"><span data-stu-id="419ff-106">Azure PowerShell is also available on Azure Cloud Shell.</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="419ff-107">新しい Az モジュールについて</span><span class="sxs-lookup"><span data-stu-id="419ff-107">About the new Az module</span></span>

<span data-ttu-id="419ff-108">このドキュメントでは、Azure PowerShell の新しい Az モジュールについて説明します。</span><span class="sxs-lookup"><span data-stu-id="419ff-108">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="419ff-109">この新しいモジュールは、.NET Standard で一から作成されています。</span><span class="sxs-lookup"><span data-stu-id="419ff-109">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="419ff-110">.NET Standard の使用により、Azure PowerShell は Windows 上の PowerShell 5 または任意のプラットフォーム上の PowerShell 6 で実行できます。</span><span class="sxs-lookup"><span data-stu-id="419ff-110">Using .NET Standard allows Azure PowerShell to run under PowerShell 5 on Windows or PowerShell 6 on any platform.</span></span> <span data-ttu-id="419ff-111">PowerShell を使用して Azure を操作するときに、Az モジュールが使用されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="419ff-111">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="419ff-112">AzureRM はバグの修正プログラムを引き続き取得できますが、新機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="419ff-112">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="419ff-113">コマンド名の変更や、AzureRM のメンテナンス プランなど、新しいモジュールの詳細については、[Azure PowerShell Az モジュールの概要](new-azureps-module-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-113">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="419ff-114">新しいモジュールをすぐに使い始める場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-114">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="419ff-115">[AzureRM のドキュメント](/powershell/azure/azurerm)も利用できます。</span><span class="sxs-lookup"><span data-stu-id="419ff-115">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="419ff-116">新しいモジュールのコマンドレット名を反映するために、Azure のドキュメントを更新中ですが、記事で AzureRM コマンドが引き続き使用されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="419ff-116">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="419ff-117">Az モジュールをインストールしたら、`Enable-AzureRmAlias` を使用して、AzureRM コマンドレットのエイリアスを有効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="419ff-117">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="419ff-118">詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-118">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="419ff-119">実行またはインストール</span><span class="sxs-lookup"><span data-stu-id="419ff-119">Run or install</span></span>

<span data-ttu-id="419ff-120">Azure PowerShell は、Windows 上の PowerShell 5.1 以上に、または任意のプラットフォーム上の PowerShell 6 にインストールでき、Azure Cloud Shell で実行できます。</span><span class="sxs-lookup"><span data-stu-id="419ff-120">You can install Azure PowerShell on PowerShell 5.1 or higher on Windows, PowerShell 6 on any platform, or run in Azure Cloud Shell.</span></span>

* <span data-ttu-id="419ff-121">Azure Cloud Shell を使用したブラウザーでの実行方法については、「[Azure Cloud Shell の PowerShell のクイックスタート](/azure/cloud-shell/quickstart-powershell)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-121">To run in your browser with Azure Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="419ff-122">お使いのシステムに Azure PowerShell をインストールするには、「[Azure PowerShell のインストール](install-az-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-122">To install Azure PowerShell on your system, see [Install Azure PowerShell](install-az-ps.md).</span></span>

<span data-ttu-id="419ff-123">Azure PowerShell の最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-123">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="419ff-124">作業の開始</span><span class="sxs-lookup"><span data-stu-id="419ff-124">Get Started</span></span>

<span data-ttu-id="419ff-125">Azure PowerShell の基礎を学ぶには、[Azure PowerShell の使用に関するページ](get-started-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-125">Read the [Get Started with Azure PowerShell](get-started-azureps.md) article to learn the Azure PowerShell basics.</span></span> <span data-ttu-id="419ff-126">PowerShell について初めて学ぶ場合は、概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="419ff-126">If you're not familiar with PowerShell, an introduction might be helpful:</span></span>

* [<span data-ttu-id="419ff-127">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="419ff-127">Install PowerShell</span></span>](/powershell/scripting/install/installing-powershell)
* [<span data-ttu-id="419ff-128">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="419ff-128">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)
* [<span data-ttu-id="419ff-129">PowerShell の基礎: (パート 1) PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="419ff-129">PowerShell Basics: (Part 1) Getting Started with PowerShell</span></span>](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)
* <span data-ttu-id="419ff-130">Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)</span><span class="sxs-lookup"><span data-stu-id="419ff-130">Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart)</span></span>

<span data-ttu-id="419ff-131">次のサンプルは、Azure の一般的な使用法の理解に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="419ff-131">The following samples can help you with some common uses of Azure:</span></span>

* [<span data-ttu-id="419ff-132">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="419ff-132">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="419ff-133">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="419ff-133">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="419ff-134">Web Apps</span><span class="sxs-lookup"><span data-stu-id="419ff-134">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="419ff-135">SQL Database</span><span class="sxs-lookup"><span data-stu-id="419ff-135">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="419ff-136">Microsoft Learn でスキルを身に付ける</span><span class="sxs-lookup"><span data-stu-id="419ff-136">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="419ff-137">PowerShell でスクリプトを使用した Azure タスクの自動化</span><span class="sxs-lookup"><span data-stu-id="419ff-137">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="419ff-138">対話型学習の詳細...</span><span class="sxs-lookup"><span data-stu-id="419ff-138">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="419ff-139">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="419ff-139">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="419ff-140">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="419ff-140">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="419ff-141">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="419ff-141">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="419ff-142">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="419ff-142">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)