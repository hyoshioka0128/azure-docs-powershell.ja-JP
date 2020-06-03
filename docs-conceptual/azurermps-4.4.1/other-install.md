---
title: Azure PowerShell のその他のインストール方法 | Microsoft Docs
description: MSI パッケージまたは Web Platform Installer を使って Azure PowerShell をインストールする方法について説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 3f8963c98b26f971c1259dc89d5da1f35ce3015a
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386699"
---
# <a name="other-installation-methods"></a>その他のインストール方法

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

Azure PowerShell には、複数のインストール方法があります。 その中でも、PowerShell ギャラリーに対して PowerShellGet を使う方法をお勧めします。 それ以外にも、Web Platform Installer (WebPI) を使うか、GitHub から入手した MSI ファイルを使って Windows に Azure PowerShell をインストールすることができます。

## <a name="install-on-windows-using-the-web-platform-installer"></a>Web Platform Installer を使って Windows にインストールする

WebPI から最新の Azure PowerShell をインストールする方法は、以前のバージョンと同じです。
[Azure PowerShell WebPI パッケージ](https://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。

> [!NOTE]
> 以前に PowerShell ギャラリーから Azure モジュールをインストールしている場合は、これらのモジュールは自動的に削除されます。 これによって、インストールされる Azure PowerShell のバージョンが 1 つに限定されるため、環境の複雑化を防ぐことができます。 ただし場合によっては、同時に複数のバージョンをインストールしなければならないケースもあります。
>
> PowerShell ギャラリー モジュールでは、`$env:ProgramFiles\WindowsPowerShell\Modules` にモジュールがインストールされます。 一方、WebPI インストーラーでは、Azure モジュールは `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\` にインストールされます。
>
> インストール中にエラーが発生した場合は、`$env:ProgramFiles\WindowsPowerShell\Modules` フォルダーから Azure\* フォルダーを手動で削除したうえで、もう一度インストールを試みてください。

インストールが完了したら、Azure PowerShell コマンドレットを含むディレクトリが `$env:PSModulePath` の設定に含まれている必要があります。 Azure PowerShell が適切にインストールされているかどうかは、次のコマンドを使って確認できます。

```powershell-interactive
# To make sure the Azure PowerShell module is available after you install
Get-InstalledModule -Name AzureRM -AllVersions | Select-Object Name, Version, Path
```

> [!NOTE]
> WebPI からのインストール時に発生する可能性のある問題が確認されています。 システムの更新やその他のインストールでコンピューターの再起動が必要になった場合、Azure PowerShell のインストール パスが `$env:PSModulePath` の更新に含まれない場合があります。

インストール後にコマンドレットを読み込んだり実行したりしようとすると、次のエラー メッセージが表示されることがあります。

```output
PS C:\> Login-AzureRmAccount
Login-AzureRmAccount : The term 'Login-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Login-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Login-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

このエラーは、コンピューターを再起動するか、完全修飾パスを使ってモジュールをインポートすることで修正できます。 次に例を示します。

```powershell-interactive
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-on-windows-using-the-msi-package"></a>MSI パッケージを使って Windows にインストールする

Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/latest) から MSI ファイルを使ってインストールすることができます。 以前のバージョンの Azure モジュールをインストール済みである場合、それらのモジュールはインストーラーによって自動的に削除されます。 MSI パッケージでは、モジュールが `$env:ProgramFiles\WindowsPowerShell\Modules` にインストールされますが、バージョンごとのフォルダーは作成されません。

