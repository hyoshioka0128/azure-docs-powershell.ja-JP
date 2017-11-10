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
# <a name="azure-stack-powershell"></a>Azure Stack PowerShell

Azure Stack には、次の 2 つの PowerShell モジュールが必要です。  

1. Azure Stack 対応の **AzureRM** モジュール。API バージョン **2017-03-09-profile** のプロファイルをインストールすることで利用できます。 このプロファイルを使ってインストールされたコマンドレットを使用できるのは Azure Stack のオペレーターとユーザーです。

2. 最新バージョンは、**1.2.11** インストールの **AzureStack** モジュールです。 このモジュールを使ってインストールされたコマンドレットを使用できるのは Azure Stack のオペレーターだけです。 オペレーターは、このモジュールによって得られる PowerShell コマンドレットを使って、プランやサービス、クォータの管理などの操作を実行できます。 このモジュールで利用できる PowerShell コマンドレットについては、[AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.11#azurerm.azurestackadmin) と [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.11#azurerm.azurestackstorage) のリファレンス コンテンツをご覧ください。

## <a name="next-steps"></a>次のステップ

* [PowerShell for Azure Stack のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [PowerShell を Azure Stack で使用するための構成](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
