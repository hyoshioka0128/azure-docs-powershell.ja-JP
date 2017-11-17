---
title: "Azure Stack PowerShell の概要 | Microsoft Docs"
description: "Azure Stack PowerShell のインストールと構成について概説します。"
author: SnehaGunda
manager: Byronr
ms.product: azure-stack
ms.service: powershell
ms.devlang: powershell
ms.topic: reference
ms.author: sngun
ms.manager: byronr
ms.openlocfilehash: 49980b361c580a1a00f07c2002241e71f2c0b654
ms.sourcegitcommit: df44d5d9874b55455ec745f1846e06a4b3266d13
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2017
---
# <a name="azure-stack-powershell"></a><span data-ttu-id="08ea6-103">Azure Stack PowerShell</span><span class="sxs-lookup"><span data-stu-id="08ea6-103">Azure Stack PowerShell</span></span>

<span data-ttu-id="08ea6-104">Azure Stack には、次の 2 つの PowerShell モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="08ea6-104">Azure Stack requires the following two PowerShell modules:</span></span>  

1. <span data-ttu-id="08ea6-105">Azure Stack 対応の **AzureRM** モジュール。API バージョン **2017-03-09-profile** のプロファイルをインストールすることで利用できます。</span><span class="sxs-lookup"><span data-stu-id="08ea6-105">The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile.</span></span> <span data-ttu-id="08ea6-106">このプロファイルを使ってインストールされたコマンドレットを使用できるのは Azure Stack のオペレーターとユーザーです。</span><span class="sxs-lookup"><span data-stu-id="08ea6-106">The cmdlets installed by using this profile can be used by Azure Stack operators and users.</span></span>

2. <span data-ttu-id="08ea6-107">最新バージョンは、**1.2.11** インストールの **AzureStack** モジュールです。</span><span class="sxs-lookup"><span data-stu-id="08ea6-107">The most current version is the **1.2.11** install of the **AzureStack** module.</span></span> <span data-ttu-id="08ea6-108">このモジュールを使ってインストールされたコマンドレットを使用できるのは Azure Stack のオペレーターだけです。</span><span class="sxs-lookup"><span data-stu-id="08ea6-108">The cmdlets installed by using this module can be used by Azure Stack operators only.</span></span> <span data-ttu-id="08ea6-109">オペレーターは、このモジュールによって得られる PowerShell コマンドレットを使って、プランやサービス、クォータの管理などの操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="08ea6-109">Operators can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module.</span></span> <span data-ttu-id="08ea6-110">このモジュールで利用できる PowerShell コマンドレットについては、[AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) と [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) のリファレンス コンテンツをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="08ea6-110">To learn about the PowerShell cmdlets available in this module, see the [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) and [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) Reference content.</span></span>

## <a name="next-steps"></a><span data-ttu-id="08ea6-111">次のステップ</span><span class="sxs-lookup"><span data-stu-id="08ea6-111">Next Steps</span></span>

* [<span data-ttu-id="08ea6-112">PowerShell for Azure Stack のインストール</span><span class="sxs-lookup"><span data-stu-id="08ea6-112">Install PowerShell for Azure Stack</span></span>](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [<span data-ttu-id="08ea6-113">PowerShell を Azure Stack で使用するための構成</span><span class="sxs-lookup"><span data-stu-id="08ea6-113">Configure PowerShell for use with Azure Stack</span></span>](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
