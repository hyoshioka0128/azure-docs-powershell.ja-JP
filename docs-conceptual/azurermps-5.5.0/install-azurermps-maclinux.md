---
title: "macOS および Linux での Azure PowerShell のインストールおよび構成 | Microsoft Docs"
description: "macOS および Linux で初めて使う Azure PowerShell をインストールして構成する方法について説明します。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/12/2018
ms.openlocfilehash: 64a86dfd4af7f3f0a91501e9a096ff190f7100cb
ms.sourcegitcommit: 5fe9a579d2e0d1cb5a05aadaeba5db784f1b18fa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/28/2018
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a>macOS および Linux での Azure PowerShell のインストールおよび構成

PowerShell Core v6 と Azure PowerShell を Windows 以外のプラットフォームにもインストールできるようになりました。
Azure PowerShell を macOS や Linux にインストールするプロセスは Windows の場合とほぼ同じですが、最初に PowerShell Core v6 をインストールする必要があります。

> [!NOTE]

> 現時点では、PowerShell Core v6 と Azure PowerShell for .NET Core はどちらもベータ版で提供されており、
> これらの製品のサポートには制限があります。 問題やバグを見つけた場合は、GitHub に問題を登録してください。
>
> * [PowerShell Core v6 の問題](https://github.com/PowerShell/PowerShell/issues)
> * [Azure PowerShell の問題](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-core-v6"></a>手順 1: PowerShell Core v6 をインストールする

PowerShell Core v6 をインストールするプロセスは、インストール先のオペレーティング システムによって異なります。
PowerShell Core v6 は Windows にインストールすることもできますが、この記事では、macOS および Linux へのインストールについて説明します。 Azure PowerShell を Windows で使用する場合は、Windows 向けの[インストール](./install-azurerm-ps.md) ガイドをご覧ください。

Linux または macOS への **PowerShell Core v6** のインストールは、Linux ディストリビューションまたは OS バージョンによって異なります。
詳細な手順については、次の記事をご覧ください。

- [macOS および Linux への PowerShell Core のインストール](/powershell/scripting/setup/installing-powershell-core-on-macos-and-linux)

## <a name="step-2-install-azure-powershell-for-net-core"></a>手順 2: Azure PowerShell for .NET Core をインストールする

PowerShell Core v6 には、インストール済みの PowerShellGet モジュールが付属しています。 これにより、PowerShell ギャラリーで公開されている任意のモジュールを簡単にインストールできます。 Azure PowerShell をインストールするには、新しい PowerShell セッションを開き、次のコマンドを実行します。

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a>手順 3: AzureRM.Netcore モジュールを読み込む

モジュールは、インストール後、PowerShell セッションに読み込む必要があります。 モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

インポートが完了したら、次のコマンドを使って Azure へのサインインを試みることで、新しくインストールしたモジュールをテストすることができます。

```powershell
Login-AzureRMAccount
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
