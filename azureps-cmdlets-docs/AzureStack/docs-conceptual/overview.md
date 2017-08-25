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
ms.openlocfilehash: 2a03697e0f3e80d63c48f2dc5615f6c99b9ef716
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <a name="azure-stack-powershell"></a><span data-ttu-id="1066d-103">Azure Stack PowerShell</span><span class="sxs-lookup"><span data-stu-id="1066d-103">Azure Stack PowerShell</span></span> 

<span data-ttu-id="1066d-104">Azure Stack には、次の 2 つの PowerShell モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="1066d-104">Azure Stack requires the following two PowerShell modules:</span></span>  

1. <span data-ttu-id="1066d-105">Azure Stack 対応の **AzureRM** モジュール。API バージョン **2017-03-09-profile** のプロファイルをインストールすることで利用できます。</span><span class="sxs-lookup"><span data-stu-id="1066d-105">The Azure Stack compatible **AzureRM** module which is available by installing the **2017-03-09-profile** API Version Profile.</span></span> <span data-ttu-id="1066d-106">このプロファイルを使ってインストールされたコマンドレットは、Azure Stack のクラウド管理者とテナントが利用できます。</span><span class="sxs-lookup"><span data-stu-id="1066d-106">The cmdlets installed by using this profile can be used by the Azure Stack cloud administrators and the tenants.</span></span> <span data-ttu-id="1066d-107">このプロファイルで利用できる PowerShell コマンドレットについては、[1.2.9 バージョンの AzureRM](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9) モジュールに関する PowerShell リファレンス コンテンツをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1066d-107">To learn about the PowerShell cmdlets that are available in this profile, see the PowerShell reference content for the [1.2.9 version of AzureRM](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9) module.</span></span>  

2. <span data-ttu-id="1066d-108">**1.2.9** バージョンの **AzureStack** モジュール。</span><span class="sxs-lookup"><span data-stu-id="1066d-108">The **1.2.9** version of the **AzureStack** module.</span></span> <span data-ttu-id="1066d-109">このモジュールを使ってインストールされたコマンドレットを使用できるのは Azure Stack のクラウド管理者だけです。</span><span class="sxs-lookup"><span data-stu-id="1066d-109">The cmdlets installed by using this module can be used by Azure Stack cloud administrators only.</span></span> <span data-ttu-id="1066d-110">管理者は、このモジュールによって得られる PowerShell コマンドレットを使って、プランやサービス、クォータの管理などの操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="1066d-110">Administrator can perform operations such as manage offers, plans, services, quotas, etc. by using the PowerShell cmdlets provided by this module.</span></span> <span data-ttu-id="1066d-111">このモジュールで利用できる PowerShell コマンドレットについては、[AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) と [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage) のリファレンス コンテンツをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1066d-111">To learn about the PowerShell cmdlets available in this module, see the [AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) and [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage) Reference content.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1066d-112">次のステップ</span><span class="sxs-lookup"><span data-stu-id="1066d-112">Next Steps</span></span>

* [<span data-ttu-id="1066d-113">PowerShell for Azure Stack のインストール</span><span class="sxs-lookup"><span data-stu-id="1066d-113">Install PowerShell for Azure Stack</span></span>](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [<span data-ttu-id="1066d-114">PowerShell を Azure Stack で使用するための構成</span><span class="sxs-lookup"><span data-stu-id="1066d-114">Configure PowerShell for use with Azure Stack</span></span>](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)


