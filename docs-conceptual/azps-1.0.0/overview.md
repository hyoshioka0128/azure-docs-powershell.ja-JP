---
title: Azure PowerShell の概要
description: Azure PowerShell Az モジュールの概要と、インストールして使い始める方法に関する情報。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 10/29/2018
ms.openlocfilehash: 7982e122d49db4d558648231d1ab8bfeed80be2d
ms.sourcegitcommit: 4acddc7026522c4fe39de2c4424917d88ee01b7e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/21/2018
ms.locfileid: "53736462"
---
# <a name="overview-of-azure-powershell"></a><span data-ttu-id="7fc16-103">Azure PowerShell の概要</span><span class="sxs-lookup"><span data-stu-id="7fc16-103">Overview of Azure PowerShell</span></span>

<span data-ttu-id="7fc16-104">Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="7fc16-104">Azure PowerShell provides a set of cmdlets that use the [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) model for managing your Azure resources.</span></span> <span data-ttu-id="7fc16-105">Azure PowerShell では .NET Standard が使用されているので、Windows、macOS、Linux で使用できます。</span><span class="sxs-lookup"><span data-stu-id="7fc16-105">Azure PowerShell uses .NET Standard, making it available for Windows, macOS, and Linux.</span></span>
<span data-ttu-id="7fc16-106">Azure PowerShell は、Azure Cloud Shell から利用することもできます。</span><span class="sxs-lookup"><span data-stu-id="7fc16-106">Azure PowerShell is also available from Azure Cloud Shell.</span></span>

<span data-ttu-id="7fc16-107">Azure PowerShell は、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで実行するか、[ローカルにインストール](install-az-ps.md)します。</span><span class="sxs-lookup"><span data-stu-id="7fc16-107">Use [Azure Cloud Shell](/azure/cloud-shell/overview) to run Azure PowerShell in your browser, or [install locally](install-az-ps.md).</span></span> <span data-ttu-id="7fc16-108">Azure PowerShell の基礎を学び、Azure を使い始めるには、[概要](get-started-azureps.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-108">Check out the [Get Started](get-started-azureps.md) article to learn the Azure PowerShell basics and get started with Azure.</span></span>

<span data-ttu-id="7fc16-109">Azure PowerShell の最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-109">For information about the latest Azure PowerShell release, see the [release notes](release-notes-azureps.md).</span></span>

## <a name="about-the-new-az-module"></a><span data-ttu-id="7fc16-110">新しい Az モジュールについて</span><span class="sxs-lookup"><span data-stu-id="7fc16-110">About the new Az module</span></span>

<span data-ttu-id="7fc16-111">このドキュメントでは、Azure PowerShell の新しい Az モジュールについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7fc16-111">This documentation describes the new Az module for Azure PowerShell.</span></span> <span data-ttu-id="7fc16-112">この新しいモジュールは、.NET Standard で一から作成されています。</span><span class="sxs-lookup"><span data-stu-id="7fc16-112">This new module is written from the ground up in .NET Standard.</span></span> <span data-ttu-id="7fc16-113">.NET Standard の使用により、Azure PowerShell は Windows 上の PowerShell 5.x または任意のプラットフォーム上の PowerShell 6 で実行できます。</span><span class="sxs-lookup"><span data-stu-id="7fc16-113">Using .NET Standard allows Azure PowerShell to run under PowerShell 5.x on Windows or PowerShell 6 on any platform.</span></span> <span data-ttu-id="7fc16-114">PowerShell を使用して Azure を操作するときに、Az モジュールが使用されるようになりました。</span><span class="sxs-lookup"><span data-stu-id="7fc16-114">The Az module is now the intended way to interact with Azure through PowerShell.</span></span>
<span data-ttu-id="7fc16-115">AzureRM はバグの修正プログラムを引き続き取得できますが、新機能は追加されなくなります。</span><span class="sxs-lookup"><span data-stu-id="7fc16-115">AzureRM will continue to get bug fixes, but no longer receive new features.</span></span>

<span data-ttu-id="7fc16-116">コマンド名の変更や、AzureRM のメンテナンス プランなど、新しいモジュールの詳細については、[Azure PowerShell Az モジュールの概要](new-azureps-module-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-116">Learn the full details about the new module, including how commands have been renamed and the maintenance plans for AzureRM, in the [Introducing the Azure PowerShell Az module](new-azureps-module-az.md).</span></span> <span data-ttu-id="7fc16-117">新しいモジュールをすぐに使い始める場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-117">If you want to get started with using the new module right away, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

<span data-ttu-id="7fc16-118">[AzureRM のドキュメント](/powershell/azure/azurerm)も利用できます。</span><span class="sxs-lookup"><span data-stu-id="7fc16-118">The [AzureRM documentation](/powershell/azure/azurerm) is also available.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="7fc16-119">新しいモジュールのコマンドレット名を反映するために、Azure のドキュメントを更新中ですが、記事で AzureRM コマンドが引き続き使用されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="7fc16-119">While the Azure documentation is being updated to reflect the new module cmdlet names, articles may still use the AzureRM commands.</span></span> <span data-ttu-id="7fc16-120">Az モジュールをインストールしたら、`Enable-AzureRmAlias` を使用して、AzureRM コマンドレットのエイリアスを有効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7fc16-120">After installing the Az module, it's recommended that you enable the AzureRM cmdlet aliases with `Enable-AzureRmAlias`.</span></span> <span data-ttu-id="7fc16-121">詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-121">See the [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md) article for more details.</span></span>

## <a name="common-scenarios"></a><span data-ttu-id="7fc16-122">一般的なシナリオ</span><span class="sxs-lookup"><span data-stu-id="7fc16-122">Common scenarios</span></span>

<span data-ttu-id="7fc16-123">Azure PowerShell の基本的な使い方については、次のサンプルが参考になります。</span><span class="sxs-lookup"><span data-stu-id="7fc16-123">The following samples can help you learn how to perform common scenarios with Azure PowerShell:</span></span>

* [<span data-ttu-id="7fc16-124">Linux virtual machines</span><span class="sxs-lookup"><span data-stu-id="7fc16-124">Linux Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="7fc16-125">Windows Virtual Machines</span><span class="sxs-lookup"><span data-stu-id="7fc16-125">Windows Virtual Machines</span></span>](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="7fc16-126">Web Apps</span><span class="sxs-lookup"><span data-stu-id="7fc16-126">Web Apps</span></span>](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [<span data-ttu-id="7fc16-127">SQL Database</span><span class="sxs-lookup"><span data-stu-id="7fc16-127">SQL Databases</span></span>](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="learn-powershell-basics"></a><span data-ttu-id="7fc16-128">PowerShell の基礎を学ぶ</span><span class="sxs-lookup"><span data-stu-id="7fc16-128">Learn PowerShell basics</span></span>

<span data-ttu-id="7fc16-129">PowerShell について初めて学ぶ場合は、概要に関するページからご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-129">If you're unfamiliar with PowerShell, an introduction may be helpful.</span></span>

* [<span data-ttu-id="7fc16-130">PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="7fc16-130">Installing PowerShell</span></span>](/powershell/scripting/setup/installing-windows-powershell)
* [<span data-ttu-id="7fc16-131">PowerShell を使用したスクリプト</span><span class="sxs-lookup"><span data-stu-id="7fc16-131">Scripting with PowerShell</span></span>](/powershell/scripting/powershell-scripting)

<span data-ttu-id="7fc16-132">次のビデオをご覧いただくこともできます。[PowerShell の基礎: (パート 1) PowerShell の概要](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)。</span><span class="sxs-lookup"><span data-stu-id="7fc16-132">You can also watch this video: [PowerShell Basics: (Part 1) Getting Started with PowerShell](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1).</span></span>

<span data-ttu-id="7fc16-133">または、Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)に関するクラスにご参加ください。</span><span class="sxs-lookup"><span data-stu-id="7fc16-133">Or attend the Microsoft Virtual Academy's [Getting Started with PowerShell Jumpstart](https://mva.microsoft.com/liveevents/powershell-jumpstart).</span></span>

## <a name="build-your-skills-with-microsoft-learn"></a><span data-ttu-id="7fc16-134">Microsoft Learn でスキルを身に付ける</span><span class="sxs-lookup"><span data-stu-id="7fc16-134">Build your skills with Microsoft Learn</span></span>

- [<span data-ttu-id="7fc16-135">PowerShell でスクリプトを使用した Azure タスクの自動化</span><span class="sxs-lookup"><span data-stu-id="7fc16-135">Automate Azure tasks using scripts with PowerShell</span></span>](/learn/modules/automate-azure-tasks-with-powershell/)
- [<span data-ttu-id="7fc16-136">対話型学習の詳細...</span><span class="sxs-lookup"><span data-stu-id="7fc16-136">More interactive learning...</span></span>](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a><span data-ttu-id="7fc16-137">その他の Azure PowerShell モジュール</span><span class="sxs-lookup"><span data-stu-id="7fc16-137">Other Azure PowerShell modules</span></span>

* [<span data-ttu-id="7fc16-138">Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="7fc16-138">Azure Active Directory</span></span>](/powershell/azure/active-directory/)
* [<span data-ttu-id="7fc16-139">Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7fc16-139">Azure Information Protection</span></span>](/powershell/azure/aip/)
* [<span data-ttu-id="7fc16-140">Azure Service Fabric</span><span class="sxs-lookup"><span data-stu-id="7fc16-140">Azure Service Fabric</span></span>](/powershell/azure/service-fabric/)
* [<span data-ttu-id="7fc16-141">Azure ElasticDB</span><span class="sxs-lookup"><span data-stu-id="7fc16-141">Azure ElasticDB</span></span>](/powershell/azure/elasticdbjobs/)
