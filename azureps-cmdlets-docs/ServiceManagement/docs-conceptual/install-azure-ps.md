---
title: "Azure PowerShell Service Management モジュールのインストールと構成 | Microsoft Docs"
description: "初めて使う Azure PowerShell をインストールして構成する方法について説明します。"
services: azure
author: sdwheeler
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/06/2017
ms.openlocfilehash: c51c727c1cb022eca59f819c7f24d8e058c677da
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <a name="installing-the-azure-powershell-service-management-module"></a>Azure PowerShell Service Management モジュールのインストール

Azure PowerShell は、[PowerShell ギャラリー](https://www.powershellgallery.com/)からインストールすることをお勧めします。

## <a name="step-1-install-powershellget"></a>手順 1: PowerShellGet をインストールする

PowerShell ギャラリーからソフトウェアをインストールするには、PowerShellGet モジュールが必要です。 PowerShellGet のバージョンが適切であるかなど、システム要件を満たしていることを確認してください。 ご使用のシステムに PowerShellGet がインストールされているかどうかを確認するには、次のコマンドを実行します。

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

次のような出力結果が表示されます。

```
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

PowerShellGet がインストールされていない場合は、「[PowerShellGet の入手方法](install-azurerm-ps.md#how-to-get-powershellget)」をご覧ください。

## <a name="step-2-install-azure-powershell"></a>手順 2: Azure PowerShell をインストールする

Windows PowerShell コンソールから管理者として次のコマンドを実行します。

```powershell
Install-Module Azure
```

Azure モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。 AzureRM モジュールをインストールすると、まだインストールしていない他の Azure モジュールが PowerShell ギャラリーからダウンロードされてインストールされます。

Azure Service Management モジュールでは、Azure PowerShell Resource Manager モジュールと共通の依存コンポーネントが使用されます。 Azure PowerShell Resource Manager モジュールがインストール済みである場合は、インストール コマンドに `-AllowClobber` パラメーターを追加する必要があります。 これにより、共通する既存の依存コンポーネントが更新されます。 このパラメーターを指定しないと、モジュールのインストールは失敗します。

```powershell
Install-Module Azure -AllowClobber
```

このモジュールのインストール後、次のコマンドを実行することでモジュールをインポートすることができます。

```powershell
Import-Module Azure
```

## <a name="to-use-the-cmdlets"></a>コマンドレットを使用するには

Azure Service Management コマンドレットを使うにはまず、Azure アカウントにログオンする必要があります。 アカウントにログオンするには、次のコマンドを実行します。

```powershell
Add-AzureAccount
```

Azure にログインすると、指定されたセッションのコンテキストが Azure PowerShell によって作成されます。 コンテキストには、そのセッション内のすべてのコマンドレットで使われる Azure PowerShell 環境、アカウント、テナント、サブスクリプションが保持されています。 これで以下のモジュールを使う準備が整いました。

## <a name="azure-service-management-cmdlets"></a>Azure Service Management のコマンドレット

Azure PowerShell モジュールは頻繁に更新されます。 コマンドレットのオンライン ヘルプに、ご利用のモジュールに存在しないコマンドレットやパラメーターの記述が見つかった場合は、最新バージョンのモジュールをダウンロードしてインストールしてください。 ご利用のモジュールのバージョンを調べるには、「`(Get-Module Azure).Version`」と入力します。

Azure における定型的なタスクを自動化する際に利用できるサンプル スクリプトについては、[Microsoft Azure スクリプト センター](http://www.windowsazure.com/documentation/scripts/)をご覧ください。

Windows PowerShell のインストール、学習、使用、カスタマイズ全般については、「[Windows PowerShell を使用したスクリプト](http://go.microsoft.com/fwlink/p/?linkid=320210)」を参照してください。
