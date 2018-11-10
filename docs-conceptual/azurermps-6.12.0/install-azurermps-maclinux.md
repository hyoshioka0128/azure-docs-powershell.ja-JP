---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/05/2018
ms.openlocfilehash: f60ea1c608be4b1c8319d53303713ba039276abc
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51273805"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS または Linux で Azure PowerShell をインストールする

Windows 以外のプラットフォームについては、PowerShell Core v6 で Azure PowerShell を実行できます。 このバージョンの PowerShell は、.NET Core をサポートするプラットフォームで使用できるように構築されています。 これらのプラットフォームで使用するために、Azure PowerShell の .NET Standard バージョンが提供されています。

> [!NOTE]
> 現時点では、Azure PowerShell for .NET Standard はベータ版で提供されています。
> 問題やバグを見つけた場合は、GitHub で問題を登録してください。
>
> * [Azure PowerShell の問題](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>PowerShell Core をインストールする

PowerShell Core のインストール手順は、macOS とほとんどの Linux ディストリビューションで異なります。
詳細な手順については、次の記事をご覧ください。

* [macOS で PowerShell Core をインストールする](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Linux で PowerShell Core をインストールする](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-standard"></a>Azure PowerShell for .NET Standard をインストールする

> [!IMPORTANT]
> 他の記事で詳述されている `AzureRM` モジュールは、PowerShell Core では動作しません。
> PowerShell Core で Azure PowerShell の機能を使用するには、`Az` モジュールをインストールする必要があります。

PowerShell Core には、インストール済みの PowerShellGet モジュールが付属しています。 次のコマンドを使用して PowerShell を起動します。

```bash
pwsh
```

Azure PowerShell をインストールするには、次のコマンドを実行します。

```powershell-interactive
Install-Module Az
```

> [!NOTE]
> モジュールをインストールするときにアクセス許可エラーが発生した場合は、スーパーユーザー モードで PowerShell を実行して、モジュールをインストールしなければならない可能性があります。
>
> ```bash
> sudo pwsh
> ```

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

## <a name="enable-aliases"></a>エイリアスを有効にする

既存の `AzureRM` モジュールとの互換性のために、新しい `Az` モジュールでは、`AzureRM` コマンドレット用に下位互換性のあるエイリアスを作成することができます。 初めてモジュールを使用する前に、次のコマンドでこれらのエイリアスを設定します。

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Enable AzureRM aliases for the user
Enable-AzureRmAlias -Scope CurrentUser
```

これにより現在のユーザーに対してのみエイリアスが設定されます。 エイリアスを設定する際に `-Scope` に指定できる他の値については、コマンドレットのヘルプを確認してください。

> [!NOTE]
> パスの場所に関するエラーが発生した場合は、それがお使いのローカル システムに存在することを確認します。 `CurrentUser` スコープの場合、このエラーは、`bash` で次のコマンドを実行することで解決できます。
>
> ```bash
> mkdir -p $HOME/.config/powershell
> ```

## <a name="sign-in"></a>[サインイン]

Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、PowerShell セッションに `Az` を読み込み、Azure の資格情報でサインインする必要があります。 モジュールのインポートには、昇格された特権は__不要__です。

```powershell-interactive
# Import the module into the PowerShell session
Import-Module Az
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 `Az` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。
macOS と Linux では、`$Profile` 環境変数を使用してプロファイルを操作する必要があります。 Azure サインインをセッション間で維持する方法については、「[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)」を参照してください。

## <a name="next-steps"></a>次の手順

Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。
