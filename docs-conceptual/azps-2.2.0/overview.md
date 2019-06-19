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
ms.openlocfilehash: 710decaf8fcc0ba57e1e978a665474047393adc7
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498660"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="a9a4e-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="a9a4e-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="a9a4e-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="a9a4e-105">Azure PowerShell では .NET Standard が使用されているので、Windows、macOS、Linux で使用できます。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="a9a4e-106">Azure PowerShell は、Azure Cloud Shell 上で利用することもできます。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-106">Azure PowerShell is also available on Azure Cloud Shell.</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="a9a4e-107">新しい Az モジュールについて</span><span class="sxs-lookup"><span data-stu-id="a9a4e-107">About the new Az module</span></span>

<span data-ttu-id="a9a4e-108">このドキュメントでは、Azure PowerShell の新しい Az モジュールについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-108">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="a9a4e-109">この新しいモジュールは、.NET Standard で一から作成されています。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-109">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="a9a4e-110">.NET Standard の使用により、Azure PowerShell は Windows 上の PowerShell 5.1 または任意のプラットフォーム上の PowerShell Core 6.x 以降で実行できます。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-110">Using .NET Standard allows Azure PowerShell to run under PowerShell 5.1 on Windows or PowerShell Core 6.x and later on any platform.</span></span> <span data-ttu-id="a9a4e-111">PowerShell を使用して Azure を操作するときに、Az モジュールが使用されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-111">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="a9a4e-112">AzureRM はバグの修正プログラムを引き続き取得できますが、新機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-112">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="a9a4e-113">コマンド名の変更や、AzureRM のメンテナンス プランなど、新しいモジュールの詳細については、[Azure PowerShell Az モジュールの概要](new-azureps-module-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-113">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="a9a4e-114">新しいモジュールをすぐに使い始める場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-114">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="a9a4e-115">[AzureRM のドキュメント](/powershell/azure/azurerm)も利用できます。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-115">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="a9a4e-116">新しいモジュールのコマンドレット名を反映するために、Azure のドキュメントを更新中ですが、記事で AzureRM コマンドが引き続き使用されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-116">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="a9a4e-117">Az モジュールをインストールしたら、`Enable-AzureRmAlias` を使用して、AzureRM コマンドレットのエイリアスを有効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-117">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="a9a4e-118">詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-118">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="run-or-install"></a><span data-ttu-id="a9a4e-119">実行またはインストール</span><span class="sxs-lookup"><span data-stu-id="a9a4e-119">Run or install</span></span>

<span data-ttu-id="a9a4e-120">Azure PowerShell は、Windows 上の PowerShell 5.1 以降に、または任意のプラットフォーム上の PowerShell Core 6.x 以降にインストールでき、Azure Cloud Shell で実行できます。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-120">You can install Azure PowerShell on PowerShell 5.1 or higher on Windows, PowerShell Core 6.x and later on any platform, or run in Azure Cloud Shell.</span></span>

* <span data-ttu-id="a9a4e-121">Azure Cloud Shell を使用したブラウザーでの実行方法については、「[Azure Cloud Shell の PowerShell のクイックスタート](/azure/cloud-shell/quickstart-powershell)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-121">To run in your browser with Azure Cloud Shell, see [Quickstart for PowerShell in Azure Cloud Shell](/azure/cloud-shell/quickstart-powershell).</span></span>
* <span data-ttu-id="a9a4e-122">お使いのシステムに Azure PowerShell をインストールするには、「[Azure PowerShell のインストール](install-az-ps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-122">To install Azure PowerShell on your system, see [Install Azure PowerShell](install-az-ps.md).</span></span>

<span data-ttu-id="a9a4e-123">Azure PowerShell の最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-123">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="get-started"></a><span data-ttu-id="a9a4e-124">作業の開始</span><span class="sxs-lookup"><span data-stu-id="a9a4e-124">Get Started</span></span>

<span data-ttu-id="a9a4e-125">Azure PowerShell の基礎を学ぶには、[Azure PowerShell の使用に関するページ](get-started-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-125">Read the [Get Started with Azure PowerShell](get-started-azureps.md) article to learn the Azure PowerShell basics.</span></span> <span data-ttu-id="a9a4e-126">PowerShell について初めて学ぶ場合は、概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-126">If you're not familiar with PowerShell, an introduction might be helpful:</span></span>

* [<span data-ttu-id="a9a4e-127">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="a9a4e-127">Install PowerShell</span></span>](/powershell/scripting/install/installing-powershell)
* [<span data-ttu-id="a9a4e-128">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="a9a4e-128">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)
* [<span data-ttu-id="a9a4e-129">PowerShell の基礎: (パート 1) PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="a9a4e-129">PowerShell Basics: (Part 1) Getting Started with PowerShell</span></span>](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)
* <span data-ttu-id="a9a4e-130">Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)</span><span class="sxs-lookup"><span data-stu-id="a9a4e-130">Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart)</span></span>

<span data-ttu-id="a9a4e-131">次のサンプルは、Azure の一般的な使用法の理解に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a9a4e-131">The following samples can help you with some common uses of Azure:</span></span>

* [<span data-ttu-id="a9a4e-132">Linux Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="a9a4e-132">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a9a4e-133">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="a9a4e-133">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a9a4e-134">Web Apps</span><span class="sxs-lookup"><span data-stu-id="a9a4e-134">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="a9a4e-135">SQL Database</span><span class="sxs-lookup"><span data-stu-id="a9a4e-135">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="a9a4e-136">Microsoft Learn でスキルを身に付ける</span><span class="sxs-lookup"><span data-stu-id="a9a4e-136">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="a9a4e-137">PowerShell でスクリプトを使用した Azure タスクの自動化</span><span class="sxs-lookup"><span data-stu-id="a9a4e-137">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="a9a4e-138">対話型学習の詳細...</span><span class="sxs-lookup"><span data-stu-id="a9a4e-138">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="a9a4e-139">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="a9a4e-139">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="a9a4e-140">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="a9a4e-140">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="a9a4e-141">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="a9a4e-141">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="a9a4e-142">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="a9a4e-142">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)