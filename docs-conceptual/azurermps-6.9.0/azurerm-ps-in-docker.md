---
title: Docker コンテナー内での Azure PowerShell の実行
description: Docker コンテナー内で Azure PowerShell を実行する方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 0ed8f50abbcb2aa00192196f19004446dc696b5d
ms.sourcegitcommit: 19dffee617477001f98d43e39a50ce1fad087b74
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/27/2018
ms.locfileid: "47178563"
---
# <a name="run-azure-powershell-in-a-docker-container"></a>Docker コンテナー内での Azure PowerShell の実行

Microsoft では、Azure PowerShell が事前インストールされた Docker イメージを公開しています。 これらのイメージにより、Azure PowerShell を試験的に利用するか、分離環境で Azure PowerShell を実行することができます。 PowerShell Core と PowerShell 5 の両方が実行されているイメージがあります。 

| 環境 | Docker イメージ |
|-------------|--------------|
| Windows 上の PowerShell | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| Windows 上の PowerShell Core | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| Linux 上の PowerShell Core | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。 たとえば、PowerShell Core で Linux コンテナーを実行するには、次を使用します。

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
