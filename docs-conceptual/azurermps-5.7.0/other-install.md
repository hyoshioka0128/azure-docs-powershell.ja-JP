---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 55a89861c3bcca41b940d34d945cd43690331f3e
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83385764"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a>MSI または Web Platform Installer を使用した Windows への Azure PowerShell のインストール

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

この記事では、MSI または Web Platform Installer (WebPI) を使って Windows に Azure PowerShell をインストールする方法について説明します。  
これらのインストール方法は、システムで必要とされる場合にのみ使用してください。 Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。 PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。

## <a name="install-or-update-on-windows-using-the-msi-package"></a>MSI パッケージを使って Windows でインストールまたは更新する

Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018) から MSI ファイルを使ってインストールすることができます。 以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。 MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。 `AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。

> [!NOTE]
> Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。

Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 `AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。
Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>Web Platform Installer を使って Windows でインストールまたは更新する

[Azure PowerShell WebPI パッケージ](https://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。 MSI または WebPI を使用して以前のバージョンの Azure モジュールがインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。 モジュールは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にインストールされます。 `AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。

> [!NOTE]
> Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。

Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 `AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。
Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。
