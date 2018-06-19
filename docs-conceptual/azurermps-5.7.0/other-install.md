---
title: Azure PowerShell のその他のインストール方法
description: MSI パッケージまたは Web Platform Installer を使って Azure PowerShell をインストールする方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323273"
---
# <a name="other-installation-methods"></a>その他のインストール方法

この記事では、MSI または Web Platform Installer (WebPI) を使って Azure PowerShell をインストールする方法について説明します。 Docker コンテナー内から Azure PowerShell を実行することもできます。 これらのインストール方法は、システムで必要とされる場合にのみ使用してください。 通常、Azure PowerShell は、PowerShellGet を使用してインストールすることをお勧めします。 PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。

Linux または macOS 環境でのインストールについては、「[macOS または Linux で Azure PowerShell をインストールする](install-azurermps-maclinux.md)」を参照してください。

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a>Web Platform Installer を使って Windows でインストールまたは更新する

WebPI から最新の Azure PowerShell をインストールする方法は、以前のバージョンと同じです。
[Azure PowerShell WebPI パッケージ](http://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。

> [!NOTE]
> 以前に PowerShell ギャラリーから Azure モジュールをインストールしている場合は、これらのモジュールは自動的に削除されます。 これによって、インストールされる Azure PowerShell のバージョンが 1 つに限定されるため、環境の複雑化を防ぐことができます。 ただし場合によっては、同時に複数のバージョンをインストールしなければならないケースもあります。
>
> PowerShell ギャラリー モジュールでは、`$env:ProgramFiles\WindowsPowerShell\Modules` にモジュールがインストールされます。 一方、WebPI インストーラーでは、Azure モジュールは `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\` にインストールされます。
>
> インストール中にエラーが発生した場合は、ご自身の `$env:ProgramFiles\WindowsPowerShell\Modules` フォルダーから `Azure*` フォルダーを手動で削除したうえで、もう一度インストールを試みてください。

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

このエラーは、コンピューターを再起動するか、完全修飾パスを使ってモジュールをインポートすることで修正できます。

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a>MSI パッケージを使って Windows でインストールまたは更新する

Azure PowerShell は、[GitHub](https://aka.ms/azps-release) から MSI ファイルを使ってインストールすることができます。 以前のバージョンの Azure モジュールをインストール済みである場合、それらのモジュールはインストーラーによって自動的に削除されます。 MSI パッケージでは、モジュールが `$env:ProgramFiles\WindowsPowerShell\Modules` にインストールされますが、バージョンごとのフォルダーは作成されません。

## <a name="run-in-a-docker-container"></a>Docker コンテナーでの実行

Microsoft では、Azure PowerShell が事前構成されている一連の Docker イメージを保持しています。 使用できるコンテナーは 2 種類あります。Windows 上で従来の PowerShell を実行しているコンテナーと、Windows または Linux のいずれかの上で PowerShell Core を実行しているコンテナーです。

| 環境 | Docker イメージ |
|-------------|--------------|
| Windows 上の PowerShell | [azuresdk/azure-powershell](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| Windows 上の PowerShell Core | [azuresdk/azure-powershell-core:nanoserver](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| Linux 上の PowerShell Core | [azuresdk/azure-powershell-core:latest](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。 たとえば、Linux コンテナー上で PowerShell Core を実行するには、次を使用します。

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> Docker で Windows コンテナーを実行するには、お使いのホスト OS が Windows でなければなりません。また、Windows コンテナーを実行するように Docker が設定されている必要があります。 Docker での Windows 環境と Linux 環境の切り替えについては、[Windows コンテナーと Linux コンテナーの切り替え](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)に関する Docker のドキュメントをご覧ください。