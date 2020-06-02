---
title: MSI を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用せずに MSI を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/22/2019
ms.openlocfilehash: 227c525d0625522c277d026ff10ae5a1cdcaedbe
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2020
ms.locfileid: "84121383"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a>MSI を使用した Windows への Azure PowerShell のインストール

この記事では、MSI インストーラーを使って Windows に Azure PowerShell をインストールする方法について説明します。 MSI インストーラーは、PowerShell ギャラリーがファイアウォールによってブロックされる可能性がある環境や、オフライン インストーラーが必要な環境向けに用意されています。 Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。 PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-az-ps.md)」を参照してください。

## <a name="requirements"></a>必要条件

Windows 上の MSI インストーラーは、PowerShell 5.1 のみを対象とした Azure PowerShell のインストール用に設計されています。 Windows 以外のプラットフォームまたはそれ以降のバージョンの PowerShell でのインストールの場合は、[PowerShellGet を使用してインストール](install-az-ps.md)してください。 PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
$PSVersionTable.PSVersion
```

PowerShell 5.1 で Azure PowerShell を使用するには、次の手順に従います。

1. 必要に応じて [Windows PowerShell 5.1](/powershell/scripting/windows-powershell/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。 Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。
2. [.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。

## <a name="install-or-update-on-windows-using-the-msi-package"></a>MSI パッケージを使って Windows でインストールまたは更新する

Azure PowerShell 用の MSI パッケージは [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v2.8.0-October2019) から入手できます。 MSI を使用して以前のバージョンの Azure PowerShell がインストールされている場合は、インストーラーによって自動的に削除されます。 MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。

Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzAccount
```

> [!NOTE]
> モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。 モジュールが構造化されているため、これには最大 1 分かかることがあります。

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。

## <a name="provide-feedback"></a>フィードバックの提供

Azure PowerShell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。 コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。 Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。
