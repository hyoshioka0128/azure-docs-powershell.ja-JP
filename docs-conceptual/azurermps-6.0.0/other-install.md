---
title: Azure PowerShell のその他のインストール方法 | Microsoft Docs
description: MSI パッケージまたは Web Platform Installer を使って Azure PowerShell をインストールする方法について説明します。
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: fd5263a327fa8e4b70418bf6fa7702d8c5383733
ms.sourcegitcommit: 37bfbf11fd0967a8e7977c692ab829d286baf88a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/08/2018
---
# <a name="other-installation-methods"></a>その他のインストール方法

Azure PowerShell には、複数のインストール方法があります。 その中でも、PowerShell ギャラリーに対して PowerShellGet を使う方法をお勧めします。 それ以外にも、Web Platform Installer (WebPI) を使うか、GitHub から入手した MSI ファイルを使って Windows に Azure PowerShell をインストールすることができます。 Azure PowerShell は Docker コンテナーにインストールすることもできます。

## <a name="install-on-windows-using-the-web-platform-installer"></a>Web Platform Installer を使って Windows にインストールする

WebPI から最新の Azure PowerShell をインストールする方法は、以前のバージョンと同じです。
[Azure PowerShell WebPI パッケージ](http://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。

> [!NOTE]
> 以前に PowerShell ギャラリーから Azure モジュールをインストールしている場合は、これらのモジュールは自動的に削除されます。 これによって、インストールされる Azure PowerShell のバージョンが 1 つに限定されるため、環境の複雑化を防ぐことができます。 ただし場合によっては、同時に複数のバージョンをインストールしなければならないケースもあります。
>
> PowerShell ギャラリー モジュールでは、`$env:ProgramFiles\WindowsPowerShell\Modules` にモジュールがインストールされます。 一方、WebPI インストーラーでは、Azure モジュールは `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\` にインストールされます。
>
> インストール中にエラーが発生した場合は、`$env:ProgramFiles\WindowsPowerShell\Modules` フォルダーから Azure* フォルダーを手動で削除したうえで、もう一度インストールを試みてください。

インストールが完了したら、Azure PowerShell コマンドレットを含むディレクトリが `$env:PSModulePath` の設定に含まれている必要があります。 Azure PowerShell が適切にインストールされているかどうかは、次のコマンドを使って確認できます。

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> WebPI からのインストール時に発生する可能性のある問題が確認されています。 システムの更新やその他のインストールでコンピューターの再起動が必要になった場合、Azure PowerShell のインストール パスが `$env:PSModulePath` の更新に含まれない場合があります。

インストール後にコマンドレットを読み込んだり実行したりしようとすると、次のエラー メッセージが表示されることがあります。

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

このエラーは、コンピューターを再起動するか、完全修飾パスを使ってモジュールをインポートすることで修正できます。 例: 

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-on-windows-using-the-msi-package"></a>MSI パッケージを使って Windows にインストールする

Azure PowerShell は、[GitHub](https://aka.ms/azps-release) から MSI ファイルを使ってインストールすることができます。 以前のバージョンの Azure モジュールをインストール済みである場合、それらのモジュールはインストーラーによって自動的に削除されます。 MSI パッケージでは、モジュールが `$env:ProgramFiles\WindowsPowerShell\Modules` にインストールされますが、バージョンごとのフォルダーは作成されません。

## <a name="install-in-a-docker-container"></a>Docker コンテナーにインストールする

Microsoft では、Azure PowerShell が事前構成されている Docker イメージを保持しています。

`docker run` でコンテナーを実行します。

```powershell
docker run azuresdk/azure-powershell
```

また Microsoft では、PowerShell Core コンテナーとしてコマンドレットのサブセットを保持しています。

Mac/Linux の場合、`latest` イメージを使用します。

```bash
docker run azuresdk/azure-powershell-core:latest
```

Windows の場合、`nanoserver` イメージを使用します。

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

Azure PowerShell が [PowerShell ギャラリー](https://www.powershellgallery.com/)から `Install-Module` によってイメージにインストールされます。
