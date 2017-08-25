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
# <a name="azure-stack-powershell"></a>Azure Stack PowerShell 

Azure Stack には、次の 2 つの PowerShell モジュールが必要です。  

1. Azure Stack 対応の **AzureRM** モジュール。API バージョン **2017-03-09-profile** のプロファイルをインストールすることで利用できます。 このプロファイルを使ってインストールされたコマンドレットは、Azure Stack のクラウド管理者とテナントが利用できます。 このプロファイルで利用できる PowerShell コマンドレットについては、[1.2.9 バージョンの AzureRM](https://docs.microsoft.com/en-us/powershell/azure/overview?view=azurermps-1.2.9) モジュールに関する PowerShell リファレンス コンテンツをご覧ください。  

2. **1.2.9** バージョンの **AzureStack** モジュール。 このモジュールを使ってインストールされたコマンドレットを使用できるのは Azure Stack のクラウド管理者だけです。 管理者は、このモジュールによって得られる PowerShell コマンドレットを使って、プランやサービス、クォータの管理などの操作を実行できます。 このモジュールで利用できる PowerShell コマンドレットについては、[AzureStackAdmin](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackadmin/?view=azurestackps-1.2.9#azurerm.azurestackadmin) と [AzureStackStorage](https://docs.microsoft.com/en-us/powershell/module/azurerm.azurestackstorage/?view=azurestackps-1.2.9#azurerm.azurestackstorage) のリファレンス コンテンツをご覧ください。

## <a name="next-steps"></a>次のステップ

* [PowerShell for Azure Stack のインストール](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-install?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)
* [PowerShell を Azure Stack で使用するための構成](https://docs.microsoft.com/en-us/azure/azure-stack/azure-stack-powershell-configure?view=azurestackps-1.2.9&toc=%2fpowershell%2fmodule%2ftoc.json%3fview%3dazurestackps-1.2.9&view=azurestackps-1.2.9)


