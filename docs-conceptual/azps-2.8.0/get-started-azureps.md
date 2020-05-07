---
title: Azure PowerShell の使用に関するページ
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 01/17/2020
ms.openlocfilehash: 718f0dc0f1ef9b0c2aa3d0630ca099fa5cec7ec0
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "76256838"
---
# <a name="get-started-with-azure-powershell"></a>Azure PowerShell の使用に関するページ

Azure PowerShell は、コマンド ラインから Azure リソースを管理できるように設計されています。 Azure Resource Manager モデルを使用する自動化ツールをビルドする場合に Azure PowerShell を使用します。
[Azure Cloud Shell](/azure/cloud-shell/overview) を使ってブラウザーで試してみるか、ローカル コンピューターにインストールします。

この記事では、Azure PowerShell の基本的な使い方と、主要な概念について説明します。

## <a name="install-or-run-in-azure-cloud-shell"></a>Azure Cloud Shell でのインストールまたは実行

Azure PowerShell の使用を開始する最も簡単な方法として、Azure Cloud Shell 環境でこれを試してみます。
Cloud Shell を起動して実行する方法については、「[Azure Cloud Shell の PowerShell のクイックスタート](/azure/cloud-shell/quickstart-powershell)」をご覧ください。
Cloud Shell では Linux コンテナー上で PowerShell 6 が実行されるため、Windows 固有の機能は利用できません。

Azure PowerShell をローカル コンピューターにインストールする準備ができたら、「[Install the Azure PowerShell module (Azure PowerShell モジュールのインストール)](install-az-ps.md)」の手順に従います。

## <a name="sign-in-to-azure"></a>Azure へのサインイン

`Connect-AzAccount` コマンドレットを使って対話形式でサインインします。 Cloud Shell を使用する場合は、次の手順をスキップします。Azure Cloud Shell セッションは、Cloud Shell セッションを起動した環境、サブスクリプション、およびテナント用に既に認証されています。

```azurepowershell-interactive
Connect-AzAccount
```

米国以外のリージョンの場合、`-Environment` パラメーターを使ってサインインします。 [Get AzEnvironment](/powershell/module/Az.Accounts/Get-AzEnvironment) コマンドレットを使って、リージョンの環境の名前を取得します。 たとえば、Azure China 21Vianet にサインインするには、以下を使用します。

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

PowerShell 5.1 環境では、サインイン ダイアログが表示され、Azure アカウントのユーザー名とパスワードを入力できます。 それ以外のすべてのバージョンの PowerShell では、[https://microsoft.com/devicelogin ] で使用するトークンが提供されます。
お使いのブラウザーでこのページを開いてトークンを入力し、Azure アカウントの資格情報でサインインし、Azure PowerShell を承認します。

サインインすると、どの Azure サブスクリプションがアクティブになっているかを示す情報が表示されます。 アカウントに複数の Azure サブスクリプションがあり、別のサブスクリプションを選択する場合は、使用可能なサブスクリプションを [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) コマンドレットで取得し、サブスクリプション ID を指定して [Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを実行します。
Azure PowerShell による Azure サブスクリプションの管理の詳細については、「[複数の Azure サブスクリプションの使用](manage-subscriptions-azureps.md)」を参照してください。

サインインしたら、Azure PowerShell コマンドレットを使ってサブスクリプションのリソースにアクセスし、管理できます。 サインイン プロセスと、認証方法の詳細については、「[Sign in with Azure PowerShell (Azure PowerShell を使用してサインインする)](authenticate-azureps.md)」を参照してください。

## <a name="find-commands"></a>コマンドを見つける

Azure PowerShell コマンドレットは、PowerShell の標準的な名前付け規則 (`VERB-NOUN`) に従っています。 動詞はアクションを説明し (例: `New`、`Get`、`Set`、`Remove`)、名詞はリソースの種類を説明します (例: `AzVM`、`AzKeyVaultCertificate`、`AzFirewall`、`AzVirtualNetworkGateway`)。 Azure PowerShell では名詞は常にプレフィックス `Az` で始まります。 標準的な動詞の完全な一覧については、「[Approved verbs for PowerShell Command (PowerShell コマンドの承認された動詞)](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)」を参照してください。

使用できる名詞、動詞、および Azure PowerShell モジュールを知ることは、[Get-Command](/powershell/module/microsoft.powershell.core/get-command) コマンドレットを使ったコマンドの検索に役立ちます。 たとえば、動詞 `Get` を使用したすべての VM 関連のコマンドを見つけるには、以下を使用します。

```powershell-interactive
Get-Command -Verb Get -Noun AzVM* -Module Az.Compute
```

一般的なコマンドを簡単に見つけられるように、この表にはリソースの種類、対応する Azure PowerShell モジュール、および `Get-Command` と共に使用する名詞プレフィックスが示されています。

| リソースの種類 | Azure PowerShell モジュール | 名詞プレフィックス |
|---------------|-------------------------|----------------|
| [リソース グループ](/azure/azure-resource-manager/resource-group-overview) | [Az.Resources](/powershell/module/az.resources#resources) | `AzResourceGroup` |
| [仮想マシン](/azure/virtual-machines) | [Az.Compute](/powershell/module/az.compute#virtual_machines) | `AzVM` |
| [ストレージ アカウント](/azure/storage/common/storage-introduction) | [Az.Storage](/powershell/module/az.storage/) | `AzStorageAccount` |
| [Key Vault](/azure/key-vault/key-vault-whatis) | [Az.KeyVault](/powershell/module/az.keyvault) | `AzKeyVault` |
| [Web アプリケーション](/azure/app-service) | [Az.Websites](/powershell/module/az.websites) | `AzWebApp` |
| [SQL データベース](/azure/sql-database) | [Az.Sql](/powershell/module/az.sql) | `AzSqlDatabase` |

Azure PowerShell のモジュールの完全な一覧については、GitHub でホストされている [Azure PowerShell モジュールの一覧](https://github.com/Azure/azure-powershell/blob/master/documentation/azure-powershell-modules.md)をご覧ください。

## <a name="learn-azure-powershell-basics-with-quickstarts-and-tutorials"></a>クイックスタートとチュートリアルを利用して Azure PowerShell の基本について学習する

Azure PowerShell の使用を開始するには、仮想マシンの設定方法、またはそれらにクエリを実行する方法を説明した詳細なチュートリアルをお試しください。

> [!div class="nextstepaction"]
> [Azure PowerShell を使用した仮想マシンの作成](azureps-vm-tutorial.yml)

その他の一般的な Azure サービス用の Azure PowerShell クイックスタートもあります。

* [ストレージ アカウントの作成](/azure/storage/common/storage-quickstart-create-account?tabs=azure-powershell)
* [Azure Blob Storage との間でのオブジェクトの転送に関するページ](/azure/storage/blobs/storage-quickstart-blobs-powershell)
* [Azure Key Vault からのシークレットの作成と取得に関するページ](/azure/key-vault/quick-create-powershell)
* [Azure SQL データベースとファイアウォールの作成に関するページ](/azure/sql-database/scripts/sql-database-create-and-configure-database-powershell)
* [Azure Container Instances でのコンテナーの実行に関するページ](/azure/container-instances/container-instances-quickstart-powershell)
* [仮想マシン スケール セット (VMSS) の作成に関するページ](/azure/virtual-machine-scale-sets/quick-create-powershell)
* [Standard ロード バランサ―の作成に関するページ](/azure/load-balancer/quickstart-create-standard-load-balancer-powershell)

## <a name="next-steps"></a>次のステップ

* [Azure PowerShell を使用してサインインする](authenticate-azureps.md)
* [Azure PowerShell による Azure サブスクリプションの管理](manage-subscriptions-azureps.md)
* [Azure PowerShell でサービス プリンシパルを作成する](create-azure-service-principal-azureps.md)
* コミュニティに質問する:
  * [MSDN の Azure フォーラム](https://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [Stack Overflow](https://go.microsoft.com/fwlink/?LinkId=320213)
