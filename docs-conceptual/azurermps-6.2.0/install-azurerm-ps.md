---
title: PowerShellGet を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/31/2018
ms.openlocfilehash: 9b7046157e32a5c8473210e9840f9ae1b2f45902
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323103"
---
# <a name="install-azure-powershell-with-powershellget"></a>PowerShellGet を使用して Azure PowerShell をインストールする

この記事では、PowerShellGet を使用して、Windows 環境に Azure PowerShell モジュールをインストールする手順について説明します。  Azure PowerShell をインストールする場合は、この方法をお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、「[その他のインストール方法](other-install.md)」を参照してください。

macOS または Linux で Azure PowerShell を使用する場合は、「[macOS および Linux での Azure PowerShell のインストールおよび構成](install-azurermps-maclinux.md)」をご覧ください。

## <a name="system-requirements"></a>システム要件

Azure PowerShell バージョン 6.1.0 には、PowerShell バージョン 5.0 (以降) が必要です。 PowerShell 5.0 へのアップグレードについては、[既存の Windows PowerShell のアップグレード](/powershell/scripting/setup/installing-windows-powershell?view=powershell-6#upgrading-existing-windows-powershell)に関するページを参照してください。

PowerShellGet は、PowerShell 5.0 に自動的に追加されます。

## <a name="install-or-update-the-azure-powershell-module"></a>Azure PowerShell モジュールをインストールまたは更新する

Azure PowerShell を PowerShell ギャラリーからインストールするためには、昇格された特権が必要です。 管理者特権の PowerShell セッションから次のコマンドを実行します。

```powershell
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

> [!IMPORTANT]
> このコマンドにより、お使いのシステム上の Azure PowerShell の既存のインストールすべてが更新されます。 複数のバージョンをインストールする必要がある場合は、FAQ の「[複数のバージョンの Azure PowerShell をインストールできますか](#multiple-versions)」の回答を参照してください。

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとして構成されていません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、"Yes" または "Yes to All" と回答します。

> [!NOTE]
> ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。

AzureRM モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。 AzureRM モジュールをインストールすると、まだインストールしていない Azure PowerShell モジュールが PowerShell ギャラリーからダウンロードされます。

## <a name="load-the-azure-powershell-module"></a>Azure PowerShell モジュールを読み込む

モジュールは、インストール後、PowerShell セッションに読み込む必要があります。 これは通常の (管理者特権ではない) PowerShell セッションで実行する必要があります。 モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。

```powershell
Import-Module -Name AzureRM
```

## <a name="reporting-issues-and-feedback"></a>問題とフィードバックの報告

ツールにバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。 コマンド ラインからフィードバックを送るには、`Send-Feedback` コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell の使用について詳しくは、次の記事をご覧ください。

* [Azure PowerShell の概要](get-started-azureps.md)

## <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a id="helpmechoose"></a>Azure PowerShell のバージョンを確認するには、どうすればよいですか。

Azure PowerShell は、できるだけ早く最新バージョンにアップグレードすることをお勧めしますが、いくつかのバージョンがサポートされています。 インストールされている Azure PowerShell のバージョンを確認するには、コマンド ラインから `Get-Module AzureRM` を実行します。

```powershell
Get-Module AzureRM -ListAvailable | Select-Object -Property Name,Version,Path
```

### <a name="can-i-use-azure-powershell-for-azure-classic-deployments"></a>Azure クラシックのデプロイに Azure PowerShell を使用できますか。

クラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。 詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。 Azure と AzureRM のモジュールは、依存するコンポーネントが共通しています。 Azure と AzureRM の両方のモジュールを使用する場合は、各パッケージの同じバージョンをインストールする必要があります。

### <a name="a-namemultiple-versionscan-i-install-multiple-versions-of-azure-powershell"></a><a name="multiple-versions"/>複数のバージョンの Azure PowerShell をインストールできますか。

PowerShellGet を使用したインストールのみが、複数のバージョンのインストールに対応しています。 複数のバージョンをインストールするには、`-RequiredVersion` パラメーターを `Install-Module` コマンドレットに追加します。 たとえば、バージョン 6.1.0 と 1.2.9 の両方をインストールするには、次を実行します。

```powershell
Install-Module -Name AzureRM -RequiredVersion 6.1.0
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

PowerShell セッションに読み込むことができるモジュールのバージョンは 1 つだけです。 特定のバージョンの Azure PowerShell モジュールをインポートするには、新しい PowerShell ウィンドウを開いて `Import-Module` を実行する必要があります。

```powershell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

> [!NOTE]
> 共存インストールでの使用が想定された最初のモジュール バージョンは、バージョン 2.1.0 とバージョン 1.2.6 です。 以前のバージョンの Azure PowerShell を読み込むと、互換性のないバージョンの **AzureRM.Profile** モジュールが読み込まれます。 このため、コマンドレットでは、コマンドレットを実行するたびにログインを要求されます。
