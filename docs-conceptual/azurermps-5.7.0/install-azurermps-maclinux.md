---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323256"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a>macOS または Linux で Azure PowerShell をインストールする

Windows 以外のプラットフォームについては、PowerShell Core v6 上で Azure PowerShell を実行できます。 この製品は、.NET Core 用に構築されており、.Net Core ランタイムをサポートするすべてのプラットフォームで実行できます。Windows 用に .NET Framework 上に構築される標準の Azure PowerShell ではありません。

> [!NOTE]
> 現時点では、PowerShell Core v6 と Azure PowerShell for .NET Core はどちらもベータ版で提供されており、
> これらの製品のサポートには制限があります。 問題やバグを見つけた場合は、GitHub で問題を登録してください。
>
> * [PowerShell Core v6 の問題](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell の問題](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a>PowerShell Core v6 をインストールする

Linux または macOS への PowerShell Core v6 のインストールは、Linux ディストリビューションまたは OS バージョンによって異なります。
詳細な手順については、次の記事をご覧ください。

- [macOS で PowerShell Core をインストールする](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [Linux で PowerShell Core をインストールする](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a>Azure PowerShell for .NET Core をインストールする

PowerShell Core v6 には、インストール済みの PowerShellGet モジュールが付属しています。 これにより、PowerShell ギャラリーで公開されている任意のモジュールを簡単にインストールできます。 Azure PowerShell をインストールするには、新しい PowerShell セッションを開き、次のコマンドを実行します。

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a>AzureRM.Netcore モジュールを読み込む

モジュールは、インストール後、PowerShell セッションに読み込む必要があります。 モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

インポートが完了したら、次のコマンドを使って Azure へのサインインを試みることで、新しくインストールしたモジュールをテストすることができます。

```powershell
Connect-AzureRmAccount
```

上記のコマンドを実行すると、`https://aka.ms/devicelogin` に移動して指定されたコードを入力するよう求められます。

## <a name="available-cmdlets"></a>利用可能なコマンドレット

.NET Standard 向けの Azure PowerShell モジュールはまだ開発途中です。 これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。 AzureRM.Netcore モジュールには次の関数が実装されています。

* アカウント管理
  - Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでログインする
  - Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む
* 環境
  - すぐに使えるさまざまな Microsoft Azure 環境を取得する
  - カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する
* Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット
  - 仮想マシン
  - App Service (Websites)
  - SQL Database
  - Storage
  - ネットワーク

## <a name="next-steps"></a>次の手順

Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。
