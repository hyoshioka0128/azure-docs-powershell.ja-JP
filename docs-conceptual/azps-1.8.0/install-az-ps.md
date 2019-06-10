---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: d99265c7f156622d876d700106e2b06dd729e8b8
ms.sourcegitcommit: 020c69430358b13cbd99fedd5d56607c9b10047b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/29/2019
ms.locfileid: "66365742"
---
# <a name="install-the-azure-powershell-module"></a>Azure PowerShell モジュールのインストール

この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法を説明します。 これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。 Az モジュールについては、現在他のインストール方法はサポートされていません。

## <a name="requirements"></a>必要条件

Azure PowerShell は、Windows 上の PowerShell 5.1 以降、またはすべてのプラットフォーム上の PowerShell Core 6.x 以降で動作します。 PowerShell がインストールされているかどうか、または macOS または Linux かどうか不明な場合な場合は、[最新バージョンの PowerShell Core をインストール](/powershell/scripting/install/installing-powershell#powershell-core)してください。

PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
$PSVersionTable.PSVersion
```

Windows 上の PowerShell 5.1 で Azure PowerShell を実行するには、次の手順に従います。

1. 必要に応じて [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。 Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。
2. [.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。

PowerShell Core を使用する場合、Azure PowerShell にその他の要件はありません。

## <a name="install-the-azure-powershell-module"></a>Azure PowerShell モジュールのインストール

> [!IMPORTANT]
>
> AzureRM と Az の両方のモジュールを同時にインストールすることができます。 両方のモジュールをインストールした場合は、__別名を有効にしない__でください。
> 別名を有効にすると、AzureRM コマンドレットと Az コマンドの別名との間に競合が発生して、予期しない動作が起こる可能性があります。
> Az モジュールをインストールする前に、AzureRM をアンインストールすることをお勧めします。 AzureRM のアンインストールや別名の有効化はいつでもできます。 AzureRM コマンドの別名の詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。
> アンインストールの手順については、「[AzureRM モジュールをアンインストールする](uninstall-az-ps.md#uninstall-the-azurerm-module)」を参照してください。 

グローバル スコープでモジュールをインストールするには、PowerShell ギャラリーからモジュールをインストールするための、昇格された特権が必要です。 Azure PowerShell をインストールするには、管理者特権セッション (Windows の場合は [管理者として実行]、macOS または Linux の場合はスーパーユーザー権限) で、次のコマンドを実行します。

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

管理者特権へのアクセス許可がない場合は、`-Scope` 引数を追加することで、現在のユーザーに対してインストールできます。

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。 これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。

## <a name="sign-in"></a>サインイン

Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
>
> モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。 モジュールが構造化されているため、これには数秒かかることがあります。

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。

## <a name="update-the-azure-powershell-module"></a>Azure PowerShell モジュールの更新

Az モジュールのパッケージ方法のために、[Update-Module](/powershell/module/powershellget/update-module) コマンドではインストールは適切に更新されません。 Az は技術的にはメタモジュールであり、Azure サービスを操作するためのコマンドレットを含むすべてのサブモジュールが含まれています。 つまり、Azure PowerShell モジュールを更新するには、__更新__するだけではなく__再インストール__する必要があります。 これはインストールと同じ方法で行いますが、`-Force` 引数を追加する必要がある場合があります。

```powershell
Install-Module -Name Az -AllowClobber -Force
```

これによりインストールされているモジュールを上書きできますが、システム上には以前のバージョンがそのまま残っていることがあります。
以前のバージョンの Azure PowerShell をシステムから削除する方法については、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-az-ps.md)」をご覧ください。

## <a name="use-multiple-versions-of-azure-powershell"></a>複数のバージョンの Azure PowerShell の使用

複数のバージョンの Azure PowerShell をインストールできます。 複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。

特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` 引数を使用できます。

```powershell-interactive
# Install Az version 0.7.0
Install-Module -Name Az -RequiredVersion 0.7.0 
# Load Az version 0.7.0
Import-Module -Name Az -RequiredVersion 0.7.0
```

複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。

## <a name="provide-feedback"></a>フィードバックの提供

Azure Powershell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。
コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。
Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。
