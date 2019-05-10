---
title: Azure PowerShell Az モジュールの概要
description: AzureRM モジュールに代わる新しい Azure PowerShell Az モジュールの概要。
ms.date: 12/13/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 10665a72bc7dcae8ecf36b5ef4e2ab285a0e78b7
ms.sourcegitcommit: accff0c2cd6035fcda2d917f6051a5b509eb6255
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "65048701"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="fbdcd-103">新しい Azure PowerShell Az モジュールの概要</span><span class="sxs-lookup"><span data-stu-id="fbdcd-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="fbdcd-104">2018 年 12 月から、Azure PowerShell Az モジュールが一般公開リリースされました。このモジュールは、Azure の操作を目的とする PowerShell モジュールです。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-104">Starting in December 2018, the Azure PowerShell Az module is in general release and now the intended PowerShell module for interacting with Azure.</span></span> <span data-ttu-id="fbdcd-105">Az で、コマンドの短縮、安定性の向上、およびクロスプラットフォームのサポートが実現します。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-105">Az offers shorter commands, improved stability, and cross-platform support.</span></span> <span data-ttu-id="fbdcd-106">また、機能パリティと、AzureRM からの簡単な移行パスも提供されます。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="fbdcd-107">Az では .NET Standard ライブラリが使用されます。つまり、PowerShell 5 と PowerShell 6 上で実行できます。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-107">Az uses the .NET Standard library, which means it runs on PowerShell 5 and PowerShell 6.</span></span>
<span data-ttu-id="fbdcd-108">PowerShell 6 は Linux、macOS、および Windows 上で実行できるため、Azure PowerShell はすべてのプラットフォームで利用できるようになりました。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-108">Since PowerShell 6 can run on Linux, macOS, and Windows, Azure PowerShell is now available for all platforms.</span></span>
<span data-ttu-id="fbdcd-109">.NET Standard を使用すると Azure PowerShell のコード ベースを統合でき、ユーザーへの影響を最小限に抑えることができます。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="fbdcd-110">Az は新しいモジュールであるため、バージョンが 1.0.0 にリセットされます。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-110">Az is a new module, so the version has been reset to 1.0.0.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="fbdcd-111">Az にアップグレードする</span><span class="sxs-lookup"><span data-stu-id="fbdcd-111">Upgrade to Az</span></span>

<span data-ttu-id="fbdcd-112">すべてのユーザーを新しい Az モジュールにアップグレードすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-112">It's recommended that all users upgrade to the new Az module.</span></span> <span data-ttu-id="fbdcd-113">そのためには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-113">To do so:</span></span>

* <span data-ttu-id="fbdcd-114">__推奨__:[Azure PowerShell AzureRM モジュールをアンインストールする](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span><span class="sxs-lookup"><span data-stu-id="fbdcd-114">__RECOMMENDED__: [Uninstall the Azure PowerShell AzureRM module](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)</span></span>
* [<span data-ttu-id="fbdcd-115">Azure PowerShell Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="fbdcd-115">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="fbdcd-116">新しいコマンド セットについて理解を深めながら、`Enable-AzureRMAlias` を使用して AzureRM コマンドレットのエイリアスを互換モードで追加できるようにします。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-116">Enable compatibility mode to add aliases for AzureRM cmdlets with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span> <span data-ttu-id="fbdcd-117">AzureRM がインストールされていない場合は、別名の有効化__のみ__を行います。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-117">__Only__ enable aliases if you do not have AzureRM installed.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="fbdcd-118">Az に既存のスクリプトを移行する</span><span class="sxs-lookup"><span data-stu-id="fbdcd-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="fbdcd-119">主要な更新プログラムの適用には手間取る可能性があります。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="fbdcd-120">ただし、Az モジュールには、新しい構文への更新に取り組みながら、既存のスクリプトを使用できるようにする互換モードがあります。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-120">However, the Az module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="fbdcd-121">AzureRM 互換モードを有効にするには、`Enable-AzureRmAlias` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-121">Use the `Enable-AzureRmAlias` cmdlet to enable the AzureRM compatibility mode.</span></span> <span data-ttu-id="fbdcd-122">このコマンドレットで、新しい Az コマンドレット名の別名として AzureRM コマンドレット名を定義できます。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-122">This cmdlet defines AzureRM cmdlet names as aliases for the new Az cmdlet names.</span></span>

<span data-ttu-id="fbdcd-123">新しいコマンドレット名は、覚えやすいように設計されています。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="fbdcd-124">コマンドレット名では `AzureRm` や `Azure` を使用する代わりに、`Az` を使用します。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="fbdcd-125">たとえば、古いコマンド `New-AzureRMVm` は `New-AzVm` になりました。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-125">For example, the old command `New-AzureRMVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="fbdcd-126">移行プロセスの詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="fbdcd-127">今後の AzureRM のサポート</span><span class="sxs-lookup"><span data-stu-id="fbdcd-127">The future of support for AzureRM</span></span>

<span data-ttu-id="fbdcd-128">既存の AzureRM モジュールは、新しいコマンドレットや機能を受け入れなくなります。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-128">The existing AzureRM module will no longer receive new cmdlets or features.</span></span> <span data-ttu-id="fbdcd-129">ただし、AzureRM は 2020 年 12 月まで引き続き正式に維持され、バグの修正プログラムを取得できます。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-129">However, AzureRM is still officially maintained and will get bug fixes up through December 2020.</span></span> <span data-ttu-id="fbdcd-130">Azure の最新のサービスと機能に対応するには、Az モジュールに切り替えてください。</span><span class="sxs-lookup"><span data-stu-id="fbdcd-130">To keep up with the latest Azure services and features, switch to the Az module.</span></span>
