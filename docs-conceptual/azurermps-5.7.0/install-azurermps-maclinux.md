---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 47611281f67d68c9fc2686e0c6156b060a225158
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51275760"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS または Linux で Azure PowerShell をインストールする

Windows 以外のプラットフォームについては、PowerShell Core v6 で Azure PowerShell を実行できます。 このバージョンの PowerShell は、.NET Core をサポートするプラットフォームで使用できるように構築されています。 これらのプラットフォームで使用するために、Azure PowerShell の特別な .NET Core バージョンが提供されています。

> [!NOTE]
> 現時点では、PowerShell Core v6 と Azure PowerShell for .NET Core はどちらもベータ版で提供されており、
> これらの製品のサポートには制限があります。 問題やバグを見つけた場合は、GitHub で問題を登録してください。
>
> * [PowerShell Core v6 の問題](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell の問題](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core"></a>PowerShell Core をインストールする

PowerShell Core のインストール手順は、macOS とほとんどの Linux ディストリビューションで異なります。
詳細な手順については、次の記事をご覧ください。

* [macOS で PowerShell Core をインストールする](/powershell/scripting/setup/installing-powershell-core-on-macos)
* [Linux で PowerShell Core をインストールする](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Azure PowerShell for .NET Core をインストールする

PowerShell Core には、インストール済みの PowerShellGet モジュールが付属しています。 PowerShell のモジュールをインストールするには、昇格された特権が必要であるため、スーパーユーザーとしてセッションを開始する必要があります。

```bash
sudo pwsh
```

Azure PowerShell をインストールするには、次のコマンドを実行します。

```powershell-interactive
Install-Module AzureRM.NetCore
```

> [!IMPORTANT]
> 他の記事で詳述されている `AzureRM` モジュールは、.NET Core 用に構築されておらず、PowerShell Core では動作しません。 `AzureRM` と `AzureRM.NetCore` では、同じコマンドレット名を使用します。唯一の違いは、ロールアップ モジュールの名前と対象とする .NET バージョンです。

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

## <a name="sign-in"></a>[サインイン]

Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、PowerShell セッションに `AzureRM.Netcore` を読み込み、Azure の資格情報でサインインする必要があります。 モジュールのインポートには、昇格された特権は__不要__です。

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM.Netcore
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 `AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。
macOS と Linux では、`$Profile` 環境変数を使用してプロファイルを操作する必要があります。 Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。

## <a name="available-cmdlets"></a>利用可能なコマンドレット

.NET Core 向けの Azure PowerShell モジュールはまだ開発途中です。 これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。 AzureRM.Netcore モジュールには次の関数が実装されています。

* アカウント管理
  * Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでサインインする
  * Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む
* 環境
  * すぐに使えるさまざまな Microsoft Azure 環境を取得する
  * カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する
* Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット
  * 仮想マシン
  * App Service (Websites)
  * SQL Database
  * Storage
  * ネットワーク

## <a name="next-steps"></a>次の手順

Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。
