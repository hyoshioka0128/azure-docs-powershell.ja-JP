---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: c57ba563b5a4d4d19944fe8eca2cb4244ee5ed9e
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34819713"
---
# <a name="release-notes"></a><span data-ttu-id="63255-103">リリース ノート</span><span class="sxs-lookup"><span data-stu-id="63255-103">Release notes</span></span>

<span data-ttu-id="63255-104">これは Azure PowerShell の今回のリリースで行われた変更の一覧です。</span><span class="sxs-lookup"><span data-stu-id="63255-104">This is a list of changes made to Azure PowerShell in this release.</span></span>

## <a name="version-129"></a><span data-ttu-id="63255-105">バージョン 1.2.9</span><span class="sxs-lookup"><span data-stu-id="63255-105">Version 1.2.9</span></span>

<span data-ttu-id="63255-106">このリリースの変更</span><span class="sxs-lookup"><span data-stu-id="63255-106">Changes This Release</span></span>

* <span data-ttu-id="63255-107">AzureRm.AzureStackAdmin モジュール</span><span class="sxs-lookup"><span data-stu-id="63255-107">AzureRm.AzureStackAdmin Module</span></span>
    + <span data-ttu-id="63255-108">管理者の Azure Resource Manager とテナントの Azure Resource Manager の分割に対応するために Add-AzureRmResourceProviderRegistration コマンドレットを変更しました。</span><span class="sxs-lookup"><span data-stu-id="63255-108">Changes in the Add-AzureRmResourceProviderRegistration cmdlet for the support of Admin Azure resource manager and tenant azure resource manager split.</span></span> <span data-ttu-id="63255-109">新しいパラメーター (-ResourceManagerType) を追加しました。</span><span class="sxs-lookup"><span data-stu-id="63255-109">A new parameter -ResourceManagerType has been added.</span></span>
    + <span data-ttu-id="63255-110">各コマンドレットから -AdminUri、-ApiVersion、-SubscriptionId、-Token の各パラメーターを削除しました。</span><span class="sxs-lookup"><span data-stu-id="63255-110">Removal of the parameters -AdminUri, -ApiVersion, -SubscriptionId and -Token from each cmdlets.</span></span> <span data-ttu-id="63255-111">これらのパラメーターが非推奨となる予定であると、かねてからお伝えしてきましたが、今回でそれらが削除されたことになります。</span><span class="sxs-lookup"><span data-stu-id="63255-111">We have been printing warnings that these parameters will be deprecated and now they got removed.</span></span>
* <span data-ttu-id="63255-112">AzureStackStorage モジュール</span><span class="sxs-lookup"><span data-stu-id="63255-112">AzureStackStorage module</span></span>
    + <span data-ttu-id="63255-113">コンテナーの移行のシナリオに対応するために新しいコマンドレットを追加しました。</span><span class="sxs-lookup"><span data-stu-id="63255-113">Added new cmdlets to support container migration scenarios.</span></span>
    + <span data-ttu-id="63255-114">内部コンポーネントと基になる機能を参照するコマンドレットを削除しました。</span><span class="sxs-lookup"><span data-stu-id="63255-114">Removed cmdlets referring to internal components and underlying features.</span></span>
* <span data-ttu-id="63255-115">AzureRM.BootStrapper</span><span class="sxs-lookup"><span data-stu-id="63255-115">AzureRM.BootStrapper</span></span>
    + <span data-ttu-id="63255-116">バージョン プロファイルを使って Azure PowerShell コマンドレットのバージョンを管理する新しいモジュールを作成しました。</span><span class="sxs-lookup"><span data-stu-id="63255-116">Created new module to manage versions of Azure PowerShell cmdlets through the use of version profiles</span></span>