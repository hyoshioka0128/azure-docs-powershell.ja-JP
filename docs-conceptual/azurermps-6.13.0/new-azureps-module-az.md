---
title: Azure PowerShell Az モジュールの概要
description: AzureRM モジュールに代わる新しい Azure PowerShell Az モジュールの概要。
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217543"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a><span data-ttu-id="ff16c-103">新しい Azure PowerShell Az モジュールの概要</span><span class="sxs-lookup"><span data-stu-id="ff16c-103">Introducing the new Azure PowerShell Az module</span></span>

<span data-ttu-id="ff16c-104">2018 年 11 月以降、Azure PowerShell `Az` モジュールが完全なパブリック プレビューとして提供されます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-104">Starting in November 2018, the Azure PowerShell `Az` module is available for full public preview.</span></span>
<span data-ttu-id="ff16c-105">Az では、コマンドの短縮と安定性の向上が実現し、Windows、macOS、および Linux がサポートされます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-105">Az offers shorter commands, improved stability, and supports Windows, macOS, and Linux.</span></span> <span data-ttu-id="ff16c-106">また、機能パリティと、AzureRM からの簡単な移行パスも提供されます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-106">Az also offers feature parity and an easy migration path from AzureRM.</span></span>

<span data-ttu-id="ff16c-107">Az では .NET Standard ライブラリが使用されます。つまり、PowerShell 5.x と PowerShell 6.x で実行できます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-107">Az uses the .NET Standard library, which means it runs on PowerShell 5.x and PowerShell 6.x.</span></span>
<span data-ttu-id="ff16c-108">PowerShell 6.x は Linux、macOS、および Windows で実行できるため、Az はすべてのプラットフォームで利用可能です。</span><span class="sxs-lookup"><span data-stu-id="ff16c-108">Since PowerShell 6.x can run on Linux, macOS, and Windows, that means Az is available for all platforms.</span></span>
<span data-ttu-id="ff16c-109">.NET Standard を使用すると Azure PowerShell のコード ベースを統合でき、ユーザーへの影響を最小限に抑えることができます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-109">Using .NET Standard allows us to unify the code base of Azure PowerShell with minimal impact on users.</span></span>

<span data-ttu-id="ff16c-110">Az は新しいモジュールであるため、バージョンがリセットされます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-110">Az is a new module, so the version has been reset.</span></span> <span data-ttu-id="ff16c-111">最初の安定版リリースが 1.0 になりますが、モジュールが AzureRm との機能パリティを持つのは 2018 年 11 月からです。</span><span class="sxs-lookup"><span data-stu-id="ff16c-111">The first stable release will be 1.0, but the module has feature parity with AzureRm as of November 2018.</span></span>

## <a name="upgrade-to-az"></a><span data-ttu-id="ff16c-112">Az にアップグレードする</span><span class="sxs-lookup"><span data-stu-id="ff16c-112">Upgrade to Az</span></span>

<span data-ttu-id="ff16c-113">新しい `Az` モジュールにアップグレードすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ff16c-113">It's recommended that users upgrade to the new `Az` module.</span></span> <span data-ttu-id="ff16c-114">そのためには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="ff16c-114">To do so:</span></span>

* [<span data-ttu-id="ff16c-115">Azure PowerShell AzureRM モジュールをアンインストールする</span><span class="sxs-lookup"><span data-stu-id="ff16c-115">Uninstall the Azure PowerShell AzureRM module</span></span>](/powershell/azure/uninstall-azurerm-ps)
* [<span data-ttu-id="ff16c-116">Azure PowerShell Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="ff16c-116">Install the Azure PowerShell Az module</span></span>](/powershell/azure/install-az-ps)
* <span data-ttu-id="ff16c-117">`Enable-AzureRMAlias` を使用して AzureRM の互換モードを有効にし、新しいコマンド セットに慣れる</span><span class="sxs-lookup"><span data-stu-id="ff16c-117">Enable compatibility mode for AzureRM with `Enable-AzureRMAlias` while you become familiar with the new command set.</span></span>

## <a name="migrate-existing-scripts-to-az"></a><span data-ttu-id="ff16c-118">Az に既存のスクリプトを移行する</span><span class="sxs-lookup"><span data-stu-id="ff16c-118">Migrate existing scripts to Az</span></span>

<span data-ttu-id="ff16c-119">主要な更新プログラムの適用には手間取る可能性があります。</span><span class="sxs-lookup"><span data-stu-id="ff16c-119">Major updates can be inconvenient.</span></span> <span data-ttu-id="ff16c-120">ただし、`Az` モジュールには、新しい構文への更新に取り組みながら、既存のスクリプトを使用できるようにする互換モードがあります。</span><span class="sxs-lookup"><span data-stu-id="ff16c-120">However, the `Az` module has a compatibility mode to help you use existing scripts while you work on updates to the new syntax.</span></span> <span data-ttu-id="ff16c-121">`AzureRM` 互換モードを有効にするには、`Enable-AzureRmAlias` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="ff16c-121">Use the `Enable-AzureRmAlias` cmdlet to enable the `AzureRM` compatibility mode.</span></span> <span data-ttu-id="ff16c-122">このコマンドレットで、新しい `Az` コマンドレット名の別名として `AzureRM` コマンドレット名を定義できます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-122">This cmdlet defines `AzureRM` cmdlet names as aliases for the new `Az` cmdlet names.</span></span>

<span data-ttu-id="ff16c-123">新しいコマンドレット名は、覚えやすいように設計されています。</span><span class="sxs-lookup"><span data-stu-id="ff16c-123">The new cmdlet names have been designed to be easy to learn.</span></span> <span data-ttu-id="ff16c-124">コマンドレット名では `AzureRm` や `Azure` を使用する代わりに、`Az` を使用します。</span><span class="sxs-lookup"><span data-stu-id="ff16c-124">Instead of using `AzureRm` or `Azure` in cmdlet names, use `Az`.</span></span> <span data-ttu-id="ff16c-125">たとえば、古いコマンド `New-AzureRmVm` は `New-AzVm` になりました。</span><span class="sxs-lookup"><span data-stu-id="ff16c-125">For example, the old command `New-AzureRmVm` has become `New-AzVm`.</span></span>

<span data-ttu-id="ff16c-126">移行プロセスの詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff16c-126">For a full description of the migration process, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>

## <a name="the-future-of-support-for-azurerm"></a><span data-ttu-id="ff16c-127">今後の AzureRM のサポート</span><span class="sxs-lookup"><span data-stu-id="ff16c-127">The future of support for AzureRM</span></span>

<span data-ttu-id="ff16c-128">`Az` バージョン 1.0 が 2018 年の 12 月にリリースされると、既存の `AzureRM` モジュールは新しいコマンドレットまたは機能を受け入れなくなります。</span><span class="sxs-lookup"><span data-stu-id="ff16c-128">The existing `AzureRM` module will no longer receive new cmdlets or features when `Az` version 1.0 is released in December 2018.</span></span> <span data-ttu-id="ff16c-129">ただし、`AzureRM` は引き続き正式に維持され、バグの修正プログラムを取得できます。</span><span class="sxs-lookup"><span data-stu-id="ff16c-129">However, `AzureRM` is still officially maintained and will get bug fixes.</span></span> <span data-ttu-id="ff16c-130">Azure の最新のサービスと機能に対応するには、`Az` モジュールに切り替える必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff16c-130">To keep up with the latest Azure services and features, you should switch to the `Az` module.</span></span>