---
title: Docker コンテナー内での Azure PowerShell の実行
description: Docker コンテナー内で Azure PowerShell を実行する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 656c58fbb7cafb539736a0083d6aed1f46b7b98d
ms.sourcegitcommit: cb1fd248920d7efca67bd6c738a3b47206df7890
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2018
ms.locfileid: "39024938"
---
# <a name="run-azure-powershell-in-a-docker-container"></a>Docker コンテナー内での Azure PowerShell の実行

Azure PowerShell で事前構成されている一連の Docker イメージがあります。 使用できるコンテナーは 2 種類あります。Windows 上で従来の PowerShell を実行しているコンテナーと、Windows または Linux 上で PowerShell Core を実行しているコンテナーです。

| 環境 | Docker イメージ |
|-------------|--------------|
| Windows 上の PowerShell | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| Windows 上の PowerShell Core | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| Linux 上の PowerShell Core | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。 たとえば、Linux コンテナー上で PowerShell Core を実行するには、次を使用します。

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Docker で Windows コンテナーを実行するには、お使いのホスト OS が Windows でなければなりません。また、Windows コンテナーを実行するように Docker が設定されている必要があります。 Docker での Windows 環境と Linux 環境の切り替えについては、[Windows コンテナーと Linux コンテナーの切り替え](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)に関する Docker のドキュメントをご覧ください。

## <a name="use-a-powershell-core-container"></a>PowerShell Core コンテナーを使用する

PowerShell Core コンテナーには PowerShell Core v6 が付属し、`AzureRM.NetCore` モジュールがプレインストールされています。 [Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。

```powershell
Import-Module AzureRM.NetCore
Connect-AzureRmAccount
```

## <a name="use-the-windows-container-with-powershell"></a>PowerShell で Windows コンテナーを使用する

Windows コンテナーには、`AzureRM` モジュールがプレインストールされています。 [Import-Module](/powershell/module/microsoft.powershell.core/import-module) コマンドレットを実行し、Azure アカウントでサインインします。

```powershell
Import-Module AzureRM
Connect-AzureRmAccount
```