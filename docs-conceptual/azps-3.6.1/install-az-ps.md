---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/26/2020
ms.openlocfilehash: 7a25270566f5e856ee44c4c191a47a3e7334508b
ms.sourcegitcommit: f6fa6543be1e0f6330b1598f01528b2928cc426c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2020
ms.locfileid: "79110985"
---
# <a name="install-azure-powershell"></a>Azure PowerShell をインストールする

この記事では、PowerShellGet を使用して Azure PowerShell モジュールをインストールする方法について説明します。 これらの手順は、Windows、macOS、および Linux プラットフォーム上で使用できます。

Azure PowerShell は Azure [Cloud Shell](/azure/cloud-shell/overview) でも利用でき、現在は [Docker イメージ](azureps-in-docker.md)にプレインストールされています。

## <a name="requirements"></a>必要条件

Azure PowerShell は、Windows 上の PowerShell 5.1 以降、またはすべてのプラットフォーム上の PowerShell Core 6.x 以降で動作します。 お使いのオペレーティング システムで利用できる[最新バージョンの PowerShell Core](/powershell/scripting/install/installing-powershell#powershell-core) をインストールする必要があります。 PowerShell Core 上で実行する場合、Azure PowerShell にその他の要件はありません。

PowerShell のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
$PSVersionTable.PSVersion
```

Windows 上の PowerShell 5.1 で Azure PowerShell を使用するには、次の手順に従います。

1. 必要に応じて [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。 Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。
2. [.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。
3. 最新バージョンの PowerShellGet がインストールされていることを確認します。 `Update-Module PowerShellGet -Force` を実行します。

## <a name="install-the-azure-powershell-module"></a>Azure PowerShell モジュールのインストール

推奨されるインストール方法は、PowerShellGet コマンドレットを使用することです。 この方法は、Windows、macOS、Linux プラットフォーム上で同じように利用できます。 PowerShell セッションから次のコマンドを実行します。

```powershell-interactive
Install-Module -Name Az -AllowClobber
```

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the `Set-PSRepository` cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

Az モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。 これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。

> [!WARNING]
> Windows 用の PowerShell 5.1 に対して AzureRM と Az の両方のモジュールを同時にインストールすることはサポートされていません。 AzureRM をシステムで引き続き使用できるようにしておく必要がある場合は、PowerShell Core 6.x 以降用の Az モジュールをインストールします。

まず、[PowerShell Core 6.x 以降をインストールします](/powershell/scripting/install/installing-powershell-core-on-windows)。

次に、PowerShell Core セッションから、現在のユーザーに対してのみ Az モジュールをインストールします。 これが推奨されるインストール範囲です。

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope CurrentUser
```

システム上のすべてのユーザーに対してモジュールをインストールするには、管理者特権が必要です。 Windows で **[管理者として実行]** を使用するか、macOS または Linux 上で `sudo` コマンドを使用して、PowerShell セッションを開始します。

```powershell-interactive
Install-Module -Name Az -AllowClobber -Scope AllUsers
```

## <a name="install-offline"></a>オフラインでインストールする

環境によっては、PowerShell ギャラリーに接続できない場合があります。 そのような場合でも、次のいずれかの方法を使用してオフラインでインストールできます。

* モジュールをネットワーク内の別の場所にダウンロードし、それをインストール ソースとして使用します。
  これにより、1 台のサーバーまたはファイル共有に PowerShell モジュールをキャッシュして、任意の接続されていないシステムに PowerShellGet でデプロイすることができます。 ローカル リポジトリを設定して、切断されたシステムにインストールする方法については、「[ローカルの PowerShellGet リポジトリの操作](/powershell/scripting/gallery/how-to/working-with-local-psrepositories)」で説明されています。
* ネットワークに接続されているコンピューターに [Azure PowerShell MSI をダウンロード](install-az-ps-msi.md)し、PowerShell ギャラリーにアクセスできないシステムにインストーラーをコピーします。 MSI インストーラーは、Windows 上の PowerShell 5.1 でのみ動作することに注意してください。
* モジュールを [Save-Module](/powershell/module/PowershellGet/Save-Module) を使用してファイル共有に保存するか、別のソースに保存して他のコンピューターに手動でコピーします。

  ```powershell-interactive
  Save-Module -Name Az -Path '\\server\share\PowerShell\modules' -Force
  ```

## <a name="troubleshooting"></a>トラブルシューティング

ここでは、Azure PowerShell モジュールのインストール時に発生する一般的な問題をいくつか示します。 ここに示されていない問題が発生した場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)してください。

### <a name="proxy-blocks-connection"></a>プロキシによる接続のブロック

PowerShell ギャラリーにアクセスできないことを示すエラーが `Install-Module` から発生した場合は、プロキシの内側にいる可能性があります。 システム全体のプロキシを構成するための要件は、オペレーティング システムとネットワーク環境によってさまざまに異なります。 プロキシ設定と、ご使用の環境での構成方法については、システム管理者にお問い合わせください。

PowerShell 自体は、このプロキシを自動的に使用するように構成されていない場合があります。 PowerShell 5.1 以降では、次のコマンドを使用して、プロキシを使用するように PowerShell セッションを構成します。

```powershell
$webClient = New-Object System.Net.WebClient
$webClient.Proxy.Credentials = [System.Net.CredentialCache]::DefaultNetworkCredentials
```

オペレーティング システムの資格情報が正しく構成されている場合は、この構成により PowerShell 要求がプロキシ経由でルーティングされます。 この設定をセッション間で保持するには、このコマンドを [PowerShell プロファイル](/powershell/module/microsoft.powershell.core/about/about_profiles)に追加します。

パッケージをインストールするには、プロキシで次のアドレスへの HTTPS 接続を許可する必要があります。

* `https://www.powershellgallery.com`

## <a name="sign-in"></a>サインイン

Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。

```powershell-interactive
# Connect to Azure with a browser sign in token
Connect-AzAccount
```

> [!NOTE]
> モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートします。 モジュールが構造化されているため、これには数秒かかることがあります。

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。

## <a name="update-the-azure-powershell-module"></a>Azure PowerShell モジュールの更新

PowerShell モジュールを更新するには、モジュールのインストールに使用したのと同じ方法を使用する必要があります。 たとえば、最初に `Install-Module` を使用した場合は、[Update-Module](/powershell/module/powershellget/update-module) を使用して最新バージョンを取得する必要があります。 最初に MSI パッケージを使用した場合は、新しい MSI をダウンロードしてインストールする必要があります。

PowerShellGet コマンドレットは、MSI パッケージからインストールされたモジュールを更新できません。 MSI パッケージは、PowerShellGet を使用してインストールされたモジュールを更新しません。 PowershellGet を使用した更新で問題が発生した場合は、**更新**ではなく**再インストール**を行う必要があります。 再インストールはインストールと同じ方法で行いますが、`-Force` パラメーターを追加する必要があります。

```powershell
Install-Module -Name Az -AllowClobber -Force
```

MSI ベースのインストールとは異なり、PowerShellGet を使用してインストールまたは更新を行っても、システム上に存在する古いバージョンは削除されません。 古いバージョンの Azure PowerShell をシステムから削除する方法については、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。 MSI ベースのインストールの詳細については、「[MSI を使用して Azure PowerShell をインストールする](install-az-ps-msi.md)」を参照してください。

## <a name="use-multiple-versions-of-azure-powershell"></a>複数のバージョンの Azure PowerShell の使用

複数のバージョンの Azure PowerShell をインストールできます。 複数のバージョンの Azure PowerShell がインストールされているかどうかを確認するには、次のコマンドを使用します。

```powershell-interactive
Get-InstalledModule -Name Az -AllVersions | select Name,Version
```

Azure PowerShell のバージョンを削除するには、「[Azure PowerShell モジュールのアンインストール](uninstall-az-ps.md)」を参照してください。

複数のバージョンのモジュールがインストールされている場合は、モジュールが自動的に読み込まれ、`Import-Module` によって、既定で最新バージョンが読み込まれます。

特定のバージョンの `Az` モジュールをインストールしたり読み込んだりするには、`-RequiredVersion` パラメーターを使用できます。

```powershell-interactive
# Install Az version 3.6.1
Install-Module -Name Az -RequiredVersion 3.6.1
# Load Az version 3.6.1
Import-Module -Name Az -RequiredVersion 3.6.1
```

## <a name="provide-feedback"></a>フィードバックの提供

Azure PowerShell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。 コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。 Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。
