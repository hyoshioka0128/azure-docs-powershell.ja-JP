---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに MSI を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: b442da364a01cd6022c14cbb32a9b633676ca8c7
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "52828860"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a>MSI を使用した Windows への Azure PowerShell のインストール

この記事では、MSI インストーラーを使って Windows に Azure PowerShell をインストールする方法について説明します。  
これらのインストール方法は、システムで必要とされる場合にのみ使用してください。 Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。 PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。

> [!NOTE]
> Azure PowerShell 6.x 以降のバージョンでは、Web Platform Installer によるインストール方法は使用できなくなりました。 Web Platform Installer を使用する必要がある場合は、代わりに MSI の使用を検討するか、以前のバージョンの Azure PowerShell をインストールしてください。

Linux または macOS 環境でのインストールについては、「[macOS または Linux で Azure PowerShell をインストールする](install-azurermps-maclinux.md)」を参照してください。

## <a name="install-or-update-on-windows-using-the-msi-package"></a>MSI パッケージを使って Windows でインストールまたは更新する

Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/latest) から MSI ファイルを使ってインストールすることができます。 以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。 MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。 `AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。

> [!NOTE]
> Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。

Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
>
> モジュールの自動読み込みを無効にしている場合は、`Import-Module AzureRM` を使用してモジュールを手動でインポートする必要があります。 モジュールが構造化されているため、これには数秒かかることがあります。

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。
