---
title: PowerShell セッション間でのユーザー ログインの保持
description: この記事では、複数の PowerShell セッション間で資格情報やその他のユーザー情報を再利用できるようにする、Azure PowerShell の新機能について説明します。
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/31/2017
ms.openlocfilehash: 4b2b3b690a8c5d6951b24d49091154c6fb479fe3
ms.sourcegitcommit: 5f0013981fcea1d689649b9a2b2ffe84ae842e56
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2018
---
# <a name="persisting-user-logins-across-powershell-sessions"></a>PowerShell セッション間でのユーザー ログインの保持

Azure PowerShell の 2017 年 9 月のリリースでは、Azure Resource Manager のコマンドレットに新機能として **Azure Context Autosave** が導入されました。 この機能により、次のように、いくつかの新しいユーザー シナリオが可能になります。

- 新しい PowerShell セッションで再利用するためにログイン情報を保持する。
- 実行時間の長いコマンドレットを実行する場合にバックグラウンド タスクを使いやすくする。
- 個別のログインを使用せずにアカウント、サブスクリプション、環境を切り替える。
- 同一の PowerShell セッションから、異なる資格情報やサブスクリプションを同時に使用してタスクを実行する。

## <a name="azure-contexts-defined"></a>Azure コンテキストの定義

"*Azure コンテキスト*" とは、Azure PowerShell コマンドレットの対象を定義する一連の情報です。 このコンテキストは、次の 5 つの要素で構成されます。

- "*アカウント*" - Azure との通信の認証に使用されるユーザー名またはサービス プリンシパル。
- "*サブスクリプション*" - 処理対象のリソースを含む Azure サブスクリプション。
- "*テナント*" - サブスクリプションを含む Azure Active Directory テナント。 テナントは、サービス プリンシパル認証にとってより重要になります。
- "*環境*" - 対象となる特定の Azure クラウド (通常は Azure グローバル クラウド)。
  ただし、環境設定では、国内、政府、オンプレミス (Azure Stack) クラウドも対象にすることができます。
- "*資格情報*" - 本人確認と Azure のリソースへのアクセスの承認のために Azure で使用される情報。

以前のリリースでは、新しい PowerShell セッションを開くたびに Azure コンテキストを作成する必要がありました。 Azure PowerShell v4.4.0 以降では、新しい PowerShell セッションを開くとすぐに Azure コンテキストの自動保存と再利用を有効にすることができます。

## <a name="automatically-saving-the-context-for-the-next-login"></a>次回ログインのためのコンテキストの自動保存

既定では、Azure PowerShell は PowerShell セッションを終了するたびにコンテキスト情報を破棄します。

PowerShell セッションが終了した後に Azure PowerShell がコンテキストを記憶できるようにするには、`Enable-AzureRmContextAutosave` を使用します。 コンテキストと資格情報は、ユーザー ディレクトリの特殊な隠しフォルダー (`%AppData%\Roaming\Windows Azure PowerShell`) に自動的に保存されます。
その後、新しい PowerShell セッションそれぞれで、最後のセッションで使用されたコンテキストが対象となります。

コンテキストと資格情報を記憶しないように PowerShell を設定するには、`Disable-AzureRmContextAutoSave` を使用します。 PowerShell セッションを開くたびに Azure へのログインが必要になります。

Azure コンテキストを管理できるコマンドレットを使用すると、きめ細かな制御も可能になります。 変更を現在の PowerShell セッションのみ (`Process` スコープ) とすべての PowerShell セッション (`CurrentUser` スコープ) のどちらに適用するかを制御できます。 これらのオプションについては、「[コンテキスト スコープの使用](#Using-Context-Scopes)」で詳しく説明します。

## <a name="running-azure-powershell-cmdlets-as-background-jobs"></a>バックグラウンド ジョブとしての Azure PowerShell コマンドレットの実行

**Azure Context Autosave** 機能を使用すると、コンテキストを PowerShell のバックグラウンド ジョブと共有することもできます。 PowerShell を使用すると、実行時間の長いタスクをバックグラウンド ジョブとして開始および監視できます。タスクが完了するのを待つ必要はありません。 資格情報をバックグラウンド ジョブと共有するには、次の 2 つの方法があります。

- コンテキストを引数として渡す

  ほとんどの AzureRM コマンドレットでは、コンテキストをパラメーターとしてコマンドレットに渡すことができます。 次の例に示すように、バックグラウンド ジョブにコンテキストを渡すことができます。

  ```powershell
  PS C:\> $job = Start-Job { param ($ctx) New-AzureRmVm -AzureRmContext $ctx [... Additional parameters ...]} -ArgumentList (Get-AzureRmContext)
  ```

- 自動保存を有効にした状態で既定のコンテキストを使用する

  **Context Autosave** を有効にした場合、バックグラウンド ジョブは、既定で保存されているコンテキストを自動的に使用します。

  ```powershell
  PS C:\> $job = Start-Job { New-AzureRmVm [... Additional parameters ...]}
  ```

バックグラウンド タスクの結果を知っておく必要がある場合は、`Get-Job` を使用してジョブの状態を確認し、`Wait-Job` を使用してジョブの完了を待ちます。 バックグラウンド ジョブの出力をキャプチャまたは表示するには、`Receive-Job` を使用します。 詳細については、「[about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs)」を参照してください。

## <a name="creating-selecting-renaming-and-removing-contexts"></a>コンテキストの作成、選択、名前変更、削除

コンテキストを作成するには、Azure にログインしている必要があります。 `Connect-AzureRmAccount` コマンドレット (またはそのエイリアス `Login-AzureRmAccount`) は、後続の Azure PowerShell コマンドレットで使用される既定のコンテキストを設定し、ログイン資格情報で許可されているテナントまたはサブスクリプションへのアクセスを許可します。

ログイン後に新しいコンテキストを追加するには、`Set-AzureRmContext` (またはそのエイリアス `Select-AzureRmSubscription`) を使用します。

```powershell
PS C:\> Set-AzureRMContext -Subscription "Contoso Subscription 1" -Name "Contoso1"
```

前の例では、現在の資格情報を使用して、"Contoso Subscription 1" を対象とした新しいコンテキストを追加します。 新しいコンテキストの名前は "Contoso1" です。 コンテキストに名前を指定しない場合は、アカウント ID とサブスクリプション ID を使用した既定の名前が使用されます。

既存のコンテキストの名前を変更するには、`Rename-AzureRmContext` コマンドレットを使用します。 例: 

```powershell
PS C:\> Rename-AzureRmContext '[user1@contoso.org; 123456-7890-1234-564321]` 'Contoso2'
```

この例では、自動的に `[user1@contoso.org; 123456-7890-1234-564321]` という名前の付いたコンテキストの名前を簡単な名前 "Contoso2" に変更します。 コンテキストを管理するコマンドレットではタブ補完も使用されているため、コンテキストをすばやく選択できます。

最後に、コンテキストを削除するには、`Remove-AzureRmContext` コマンドレットを使用します。  例: 

```powershell
PS C:\> Remove-AzureRmContext Contoso2
```

"Contoso2" という名前のコンテキストは記憶されません。 その後、`Set-AzureRmContext` を使用して、このコンテキストを再作成できます。

## <a name="removing-credentials"></a>資格情報の削除

`Remove-AzureRmAccount` (別名 `Logout-AzureRmAccount`) を使用して、ユーザーまたはサービス プリンシパルの資格情報と関連付けられたコンテキストをすべて削除できます。 `Remove-AzureRmAccount` コマンドレットをパラメーターを指定せずに実行すると、現在のコンテキストのユーザーまたはサービス プリンシパルに関連付けられた資格情報とコンテキストがすべて削除されます。 特定のプリンシパルを対象とするために、ユーザー名、サービス プリンシパル名、またはコンテキストを渡すこともできます。

```powershell
Remove-AzureRmAccount user1@contoso.org
```

## <a name="using-context-scopes"></a>コンテキスト スコープの使用

場合によっては、他のセッションに影響を与えることなく、PowerShell セッションでコンテキストを選択、変更、または削除することもできます。 コンテキストのコマンドレットの既定の動作を変更するには、`Scope` パラメーターを使用します。 `Process` スコープは、現在のセッションのみに適用されるようにすることで、既定の動作を無視します。 逆に、`CurrentUser` スコープは、現在のセッションだけでなく、すべてのセッションのコンテキストを変更します。

たとえば、他のウィンドウに影響を与えることなく現在の PowerShell セッションの既定のコンテキストを変更したり、次にセッションを開いたときに使用されるコンテキストを変更したりするには、次を使用します。

```powershell
PS C:\> Select-AzureRmContext Contoso1 -Scope Process
```

## <a name="how-the-context-autosave-setting-is-remembered"></a>コンテキストの自動保存設定を記憶する方法

コンテキストの自動保存設定は、ユーザーの Azure PowerShell ディレクトリ (`%AppData%\Roaming\Windows Azure PowerShell`) に保存されます。 コンピューター アカウントの中には、このディレクトリにアクセスできないものがあります。 このようなシナリオでは、環境変数を使用できます。

```powershell
$env:AzureRmContextAutoSave="true" | "false"
```

"true" に設定した場合、コンテキストは自動的に保存されます。 "false" に設定した場合、コンテキストは保存されません。

## <a name="changes-to-the-azurermprofile-module"></a>AzureRM.Profile モジュールの変更点

コンテキスト管理用の新しいコマンドレット

- [Enable-AzureRmContextAutosave][enable] - PowerShell セッション間でのコンテキストの保存を許可します。
  変更するとグローバル コンテキストが変更されます。
- [Disable-AzureRmContextAutosave][disable] - コンテキストの自動保存をオフにします。 新しい PowerShell セッションごとに再度ログインが必要になります。
- [Select-AzureRmContext][select] - コンテキストを既定値として選択します。 後続のすべてのコマンドレットでは、認証にこのコンテキストの資格情報が使用されます。
- [Remove-AzureRmAccount][remove-cred] - アカウントに関連付けられた資格情報とコンテキストをすべて削除します。
- [Remove-AzureRmContext][remove-context] - 名前付きコンテキストを削除します。
- [Rename-AzureRmContext][rename] - 既存のコンテキストの名前を変更します。

既存のプロファイル コマンドレットの変更

- [Add-AzureRmAccount][login] - ログインのスコープをプロセスまたは現在のユーザーにすることを許可します。
  ログイン後に既定のコンテキストに名前を付けることができます。
- [Import-AzureRmContext][import] - ログインのスコープをプロセスまたは現在のユーザーにすることを許可します。
- [Set-AzureRmContext][set-context] - 既存の名前付きコンテキストの選択と、プロセスまたは現在のユーザーへのスコープの変更を許可します。

<!-- Hyperlinks -->
[enable]: /powershell/module/azurerm.profile/Enable-AzureRmContextAutosave
[disable]: /powershell/module/azurerm.profile/Disable-AzureRmContextAutosave
[select]: /powershell/module/azurerm.profile/Select-AzureRmContext
[remove-cred]: /powershell/module/azurerm.profile/Remove-AzureRmAccount
[remove-context]: /powershell/module/azurerm.profile/Remove-AzureRmContext
[rename]: /powershell/module/azurerm.profile/Rename-AzureRmContext

<!-- Updated cmdlets -->
[login]: /powershell/module/azurerm.profile/Add-AzureRmAccount
[import]: /powershell/module/azurerm.profile/Import-AzureRmAccount
[set-context]: /powershell/module/azurerm.profile/Import-AzureRmContext
