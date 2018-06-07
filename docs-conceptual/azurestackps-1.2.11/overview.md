---
title: Azure Stack PowerShell の概要 | Microsoft Docs
description: Azure Stack PowerShell のインストールと構成について概説します。
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
ms.openlocfilehash: 3f55ff613004f0726e20255126b29bf7f64662b8
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34820203"
---
# <a name="azure-stack-powershell"></a><span data-ttu-id="25f19-103">Azure Stack PowerShell</span><span class="sxs-lookup"><span data-stu-id="25f19-103">Azure Stack PowerShell</span></span>

<span data-ttu-id="25f19-104">Azure Stack には、次の 2 つの PowerShell モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="25f19-104">Azure Stack requires the following two PowerShell modules:</span></span>  

1. <span data-ttu-id="25f19-105">Azure Stack 対応の **AzureRM** モジュール。API バージョン **2017-03-09-profile** のプロファイルをインストールすることで利用できます。</span><span class="sxs-lookup"><span data-stu-id="25f19-105">The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile.</span></span> <span data-ttu-id="25f19-106">このプロファイルを使ってインストールされたコマンドレットを使用できるのは Azure Stack のオペレーターとユーザーです。</span><span class="sxs-lookup"><span data-stu-id="25f19-106">The cmdlets installed by using this profile can be used by Azure Stack operators and users.</span></span>

2. <span data-ttu-id="25f19-107">最新バージョンは、**1.2.11** インストールの **AzureStack** モジュールです。</span><span class="sxs-lookup"><span data-stu-id="25f19-107">The most current version is the **1.2.11** install of the **AzureStack** module.</span></span> <span data-ttu-id="25f19-108">このモジュールを使ってインストールされたコマンドレットを使用できるのは Azure Stack のオペレーターだけです。</span><span class="sxs-lookup"><span data-stu-id="25f19-108">The cmdlets installed by using this module can be used by Azure Stack operators only.</span></span> <span data-ttu-id="25f19-109">オペレーターは、このモジュールによって得られる PowerShell コマンドレットを使って、プランやサービス、クォータの管理などの操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="25f19-109">Operators can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module.</span></span> <span data-ttu-id="25f19-110">このモジュールで利用できる PowerShell コマンドレットについては、[AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) と [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) のリファレンス コンテンツをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="25f19-110">To learn about the PowerShell cmdlets available in this module, see the [AzureStackAdmin](https://docs.microsoft.com/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) and [AzureStackStorage](https://docs.microsoft.com/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) Reference content.</span></span>

## <a name="next-steps"></a><span data-ttu-id="25f19-111">次の手順</span><span class="sxs-lookup"><span data-stu-id="25f19-111">Next Steps</span></span>

* [<span data-ttu-id="25f19-112">PowerShell for Azure Stack のインストール</span><span class="sxs-lookup"><span data-stu-id="25f19-112">Install PowerShell for Azure Stack</span></span>](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [<span data-ttu-id="25f19-113">PowerShell を Azure Stack で使用するための構成</span><span class="sxs-lookup"><span data-stu-id="25f19-113">Configure PowerShell for use with Azure Stack</span></span>](https://docs.microsoft.com/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
