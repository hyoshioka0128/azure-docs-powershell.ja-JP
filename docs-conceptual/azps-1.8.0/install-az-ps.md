---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 8e63e3efb2671eef435498063010d5704c793060
ms.sourcegitcommit: a261efc84dedfd829c0613cf62f8fcf3aa62adb8
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/06/2019
ms.locfileid: "68807504"
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

> [!WARNING]
> Windows 用の PowerShell 5.1 で AzureRM と Az の両方のモジュールを同時にインストールすることは__できません__。 AzureRM をシステムで引き続き使用できるようにしておく必要がある場合は、PowerShell Core 6.x 以降用の Az モジュールをインストールします。 そのためには、[PowerShell Core 6.x 以降をインストール](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows)してから、PowerShell Core ターミナルで以下の手順に従ってください。

推奨されるインストール方法として、アクティブ ユーザーにのみインストールします。

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

システム上のすべてのユーザーに対してインストールする場合は、管理者特権が必要です。 管理者特権での PowerShell セッションから、管理者として実行するか、macOS または Linux 上で `sudo` コマンドを使用して実行します。

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope AllUsers
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

## <a name="troubleshooting"></a>トラブルシューティング

ここでは、Azure PowerShell モジュールのインストール時に発生する一般的な問題をいくつか示します。 ここに示されていない問題が発生した場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)してください。

### <a name="proxy-blocks-connection"></a>プロキシによる接続のブロック

PowerShell ギャラリーにアクセスできないことを示すエラーが `Install-Module` から発生した場合は、プロキシの内側にいる可能性があります。 さまざまなオペレーティング システムにシステム全体のプロキシを構成するためのさまざまな要件がありますが、ここではそれについて詳しく説明しません。 プロキシ設定とお使いの OS 用に構成する方法については、システム管理者に問い合わせてください。

PowerShell 自体は、このプロキシを自動的に使用するように構成されていない場合があります。 PowerShell 5.1 以降は、次のコマンドで PowerShell セッションに使用するプロキシを構成します。

```powershell
(New-Object System.Net.WebClient).Proxy.Credentials = `
  [System.Net.CredentialCache]::DefaultNetworkCredentials
```

オペレーティング システムの資格情報が正しく構成されている場合は、これにより PowerShell 要求がプロキシ経由でルーティングされます。
この設定をセッション間で保持するためには、このコマンドを [PowerShell プロファイル](/powershell/module/microsoft.powershell.core/about/about_profiles)に追加します。

パッケージをインストールするためには、プロキシで次のアドレスへの HTTPS 接続を許可する必要があります。

* `https://www.powershellgallery.com`

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
