---
title: Azure コンテキストとサインイン資格情報
description: 複数の PowerShell セッション間で Azure の資格情報や他の情報を再利用する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.openlocfilehash: 72d1b07bb2c66f80ea6f5d37ef7012d0d0a5bbbc
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "72791470"
---
# <a name="azure-powershell-context-objects"></a>Azure PowerShell コンテキスト オブジェクト

Azure PowerShell は、_Azure PowerShell コンテキスト オブジェクト_ (Azure コンテキスト) を使用して、サブスクリプションと認証情報を保持します。 複数のサブスクリプションがある場合は、Azure コンテキストを使用して、Azure PowerShell コマンドレットを実行するサブスクリプションを選択できます。 Azure コンテキストは、複数の PowerShell セッションにわたってサインイン情報を格納し、バックグラウンド タスクを実行するためにも使用されます。

この記事では、サブスクリプションやアカウントの管理ではなく、Azure コンテキストの管理について説明します。 ユーザー、サブスクリプション、テナント、またはその他のアカウント情報を管理する方法については、[Azure Active Directory](/azure/active-directory) のドキュメントを参照してください。 コンテキストを使用してバックグラウンド タスクまたは並列タスクを実行する方法については、Azure コンテキストに慣れた後に [PowerShell ジョブでの Azure PowerShell コマンドレットの使用](using-psjobs.md)に関するページを参照してください。

## <a name="overview-of-azure-context-objects"></a>Azure コンテキスト オブジェクトの概要

Azure コンテキストは、コマンドの実行対象のアクティブなサブスクリプションと、Azure クラウドに接続するために必要な認証情報を表す PowerShell オブジェクトです。 Azure コンテキストを使用すると、サブスクリプションを切り替えるたびに、Azure PowerShell でアカウントを再認証する必要はありません。 Azure コンテキストは、次のもので構成されます。

* [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) を使用して Azure にサインインするために使用された_アカウント_。 Azure コンテキストでは、アカウントの観点からは、ユーザー、アプリケーション ID、およびサービス プリンシパルが同じものとして扱われます。
* _テナント_に関連付けられたアクティブな_サブスクリプション_ (Azure リソースを作成および実行するための Microsoft とのサービス契約)。 多くの場合、テナントは、ドキュメント内で、または Active Directory を使用する場合に_組織_と呼ばれます。
* _トークン キャッシュ_ (Azure クラウドへアクセスするための格納された認証トークン) への参照。 このトークンの格納場所と保持期間は[コンテキスト自動保存設定](#save-azure-contexts-across-powershell-sessions)によって決定されます。

これらの用語の詳細については、[Azure Active Directory の用語](/azure/active-directory/fundamentals/active-directory-whatis#terminology)に関するページをご覧ください。 Azure コンテキストによって使用される認証トークンは、永続セッションの一部である他の保存されたトークンと同じです。 

`Connect-AzAccount` を使用してサインインすると、既定のサブスクリプションに対して少なくとも 1 つの Azure コンテキストが作成されます。 `Connect-AzAccount` によって返されるオブジェクトは、残りの PowerShell セッションで使用される既定の Azure コンテキストです。

## <a name="get-azure-contexts"></a>Azure コンテキストを取得する

[Get-AzContext](/powershell/module/az.accounts/get-azcontext) コマンドレットを使用すると、使用可能な Azure コンテキストが取得されます。 `-ListAvailable` を使用して使用可能なすべてのコンテキストを一覧表示します。

```azurepowershell-interactive
Get-AzContext -ListAvailable
```

または、名前を指定してコンテキストを取得します。

```azurepowershell-interactive
$context = Get-Context -Name "mycontext"
```

コンテキスト名は、関連付けられたサブスクリプションの名前とは異なる場合があります。

> [!IMPORTANT]
> 使用可能な Azure コンテキストが必ずしも使用可能なサブスクリプションであるとは__限りません__。 Azure コンテキストはローカルに保存された情報のみを表します。 [Get-AzSubscription](/powershell/module/Az.Accounts/Get-AzSubscription?view=azps-1.8.0) コマンドレットを使用すると、サブスクリプションを取得できます。

## <a name="create-a-new-azure-context-from-subscription-information"></a>サブスクリプション情報から新しい Azure コンテキストを作成する

[Set-AzContext](/powershell/module/Az.Accounts/Set-AzContext) コマンドレットを使用して、新しい Azure コンテキストの作成と、アクティブ コンテキストとしての設定の両方を行います。
新しい Azure コンテキストを作成する最も簡単な方法は、既存のサブスクリプション情報を使用することです。 このコマンドレットは、`Get-AzSubscription` からの出力オブジェクトをパイプ値として受け取り、新しい Azure コンテキストを作成します。

```azurepowershell-interactive
Get-AzSubscription -SubscriptionName 'MySubscriptionName' | Set-AzContext -Name 'MyContextName'
```

または、サブスクリプション名または ID と必要に応じてテナント ID を指定します。

```azurepowershell-interactive
Set-AzContext -Name 'MyContextName' -Subscription 'MySubscriptionName' -Tenant '.......'
```

`-Name` 引数を省略すると、サブスクリプションの名前と ID が `Subscription Name (subscription-id)` の形式でコンテキスト名として使用されます。

## <a name="change-the-active-azure-context"></a>アクティブな Azure コンテキストを変更する

アクティブな Azure コンテキストを変更するには、`Set-AzContext` と [Select-AzContext](/powershell/module/az.accounts/set-azcontext) の両方を使用できます。 [新しい Azure コンテキストの作成](#create-a-new-azure-context-from-subscription-information)に関するセクションで説明されているように、`Set-AzContext` を使用すると、サブスクリプションに対して新しい Azure コンテキストが作成され (存在しない場合)、それをアクティブ コンテキストとして使用するように切り替えられます。

`Select-AzContext` は、既存の Azure コンテキストでのみ使用されることが想定されており、`Set-AzContext -Context` と同じように動作しますが、パイプを使用するように設計されています。

```azurepowershell-interactive
Set-AzContext -Context $(Get-AzContext -Name "mycontext") # Set a context with an inline Azure context object
Get-AzContext -Name "mycontext" | Select-AzContext # Set a context with a piped Azure context object
```

Azure PowerShell の他の多くのアカウントおよびコンテキスト管理コマンドと同様に、`Set-AzContext` と `Select-AzContext` では、コンテキストがアクティブになる期間を制御できるように `-Scope` 引数がサポートされています。 `-Scope` では、既定値を変更せずに、1 つのセッションのアクティブなコンテキストを変更できます。

```azurepowershell-interactive
Get-AzContext -Name "mycontext" | Select-AzContext -Scope Process
```

PowerShell セッション全体のコンテキストを切り替えないようにするために、すべての PowerShell コマンドは `-AzContext` 引数を使用して、指定のコンテキストに対して実行できます。

```azurepowershell-interactive
$context = Get-AzContext -Name "mycontext"
New-AzVM -Name ExampleVM -AzContext $context
```

Azure PowerShell コマンドレットでのコンテキストのもう 1 つの主な用途は、バックグラウンド コマンドを実行することです。 Azure PowerShell を使用した PowerShell ジョブの実行の詳細については、[PowerShell ジョブでの Azure PowerShell コマンドレットの実行](using-psjobs.md)に関する記事を参照してください。

## <a name="save-azure-contexts-across-powershell-sessions"></a>PowerShell セッション間での Azure コンテキストの保存

既定では、Azure コンテキストは、PowerShell セッション間で使用するために保存されます。 この動作は、次の方法で変更します。

* `Connect-AzAccount` で `-Scope Process` を使用してサインインします。

  ```azurepowershell
  Connect-AzAccount -Scope Process
  ```

  このサインインの一部として返される Azure コンテキストは、現在のセッションで_のみ_有効で、Azure PowerShell コンテキストの自動保存の設定に関係なく、自動的には保存されません。
* [Disable-AzContextAutosave](/powershell/module/az.accounts/disable-azcontextautosave) コマンドレットを使用して、AzurePowershell のコンテキストの自動保存を無効にします。
  コンテキストの自動保存を無効にしても、格納されているトークンはクリア__されません__。 保存されている Azure コンテキスト情報をクリアする方法については、[Azure コンテキストと資格情報の削除](#remove-azure-contexts-and-stored-credentials)に関する記事を参照してください。
* Azure コンテキストの自動保存を明示的に有効にするには、[Enable-AzContextAutosave](/powershell/module/az.accounts/enable-azcontextautosave) コマンドレットを使用します。 自動保存が有効になっていると、ユーザーのすべてのコンテキストは、後の PowerShell セッション用にローカルに保存されます。
* 今後の PowerShell セッションで使用するために [Save-AzContext](/powershell/module/az.accounts/save-azcontext) を使用してコンテキストを手動で保存します。保存したコンテキストは、[Import-AzContext](/powershell/module/az.accounts/import-azcontext) を使用して読み込むことができます。

  ```azurepowershell
  Save-AzContext -Path current-context.json # Save the current context
  Save-AzContext -Profile $profileObject -Path other-context.json # Save a context object
  Import-AzContext -Path other-context.json # Load the context from a file and set it to the current context
  ```

> [!WARNING]
> コンテキストの自動保存を無効にしても、保存されていた保存済みのコンテキスト情報はクリア__されません__。 保存されている情報を削除するには、[Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext) コマンドレットを使用します。 保存済みコンテキストの削除の詳細については、[コンテキストと資格情報の削除](#remove-azure-contexts-and-stored-credentials)に関する記事を参照してください。

これらの各コマンドでは、`-Scope` パラメーターがサポートされています。これは、`Process` の値を取り、現在実行中のプロセスのみに適用することができます。 たとえば、新しく作成されたコンテキストが PowerShell セッションを終了した後に保存されないようにするには、次のようにします。

```azurepowershell-interactive
Disable-AzContextAutosave -Scope Process
$context2 = Set-AzContext -Subscription "sub-id" -Tenant "other-tenant"
```

コンテキスト情報とトークンは、Windows 上の `$env:USERPROFILE\.Azure` ディレクトリおよび他のプラットフォーム上の `$HOME/.Azure` に格納されます。 サブスクリプション ID やテナント ID などの機密情報が、ログまたは保存されたコンテキストなどにより、まだ保存された情報に公開されている場合があります。 保存されている情報をクリアする方法については、[コンテキストと資格情報の削除](#remove-azure-contexts-and-stored-credentials)に関するセクションを参照してください。

## <a name="remove-azure-contexts-and-stored-credentials"></a>Azure コンテキストと保存されている資格情報の削除

Azure コンテキストと資格情報をクリアするには、次のようにします。

* [Disconnect-AzAccount](/powershell/module/az.accounts/disconnect-azaccount) を使用してアカウントからサインアウトします。
  アカウントまたはコンテキストにより、任意のアカウントからサインアウトできます。

  ```azurepowershell-interactive
  Disconnect-AzAccount # Disconnect active account 
  Disconnect-AzAccount -Username "user@contoso.com" # Disconnect by account name

  Disconnect-AzAccount -ContextName "subscription2" # Disconnect by context name
  Disconnect-AzAccount -AzureContext $contextObject # Disconnect using context object information
  ```

  切断すると、保存されている認証トークンが必ず削除され、切断されたユーザーまたはコンテキストに関連付けられている保存済みのコンテキストがクリアされます。
* [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext) を使用します。 このコマンドレットは、保存されているコンテキストと認証トークンを常に削除することが保証されており、さらにユーザーをサインアウトします。
* [Remove-AzContext](/powershell/module/az.accounts/remove-azcontext) を使用してコンテキストを削除します。
  
  ```azurepowershell-interactive
  Remove-AzContext -Name "mycontext" # Remove by name
  Get-AzContext -Name "mycontext" | Remove-AzContext # Remove by piping Azure context object
  ```

  アクティブなコンテキストを削除すると、Azure から切断され、`Connect-AzAccount` で再認証する必要があります。

## <a name="see-also"></a>参照

* [PowerShell ジョブで Azure PowerShell コマンドレットを実行する](using-psjobs.md)
* [Azure Active Directory 用語集](/azure/active-directory/fundamentals/active-directory-whatis#terminology)
* [Az.Accounts リファレンス](/powershell/module/az.accounts)
