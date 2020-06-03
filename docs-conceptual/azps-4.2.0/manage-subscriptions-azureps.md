---
title: Azure PowerShell による Azure サブスクリプションの管理
description: Azure PowerShell による Azure サブスクリプションの管理
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/04/2019
ms.openlocfilehash: 4947435259f78c10e4f67434eb62ec8d4c3c6013
ms.sourcegitcommit: cef87acc9f2a0d296bef74f526afd2e067e8146b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "84299181"
---
# <a name="use-multiple-azure-subscriptions"></a>複数の Azure サブスクリプションの使用

ほとんどの Azure ユーザーは、サブスクリプションを 1 つしか持っていません。 ただし、複数の組織に属している場合や、組織がグループ間で特定のリソースへのアクセスを分けている場合、Azure に複数のサブスクリプションを持っていることがあります。 CLI では、サブスクリプションをグローバルに選択することも、コマンドごとに選択することもできます。

サブスクリプション、請求、およびコスト管理の詳細については、[課金とコスト管理に関するドキュメント](/azure/billing/)をご覧ください。

## <a name="tenants-users-and-subscriptions"></a>テナント、ユーザー、サブスクリプション

Azure におけるテナント、ユーザー、サブスクリプションが混同されている場合があります。 "_テナント_" とは、組織全体を含む Azure Active Directory エンティティです。 このテナントは、少なくとも 1 つの "_サブスクリプション_" を持ち、少なくとも 1 人の "_ユーザー_" が含まれます。 ユーザーとは個人であり、1 つのテナント (ユーザーが属している組織) にのみ関連付けられています。 ユーザーは、Azure にサインインしてリソースを作成、管理、および使用するアカウントです。
1 人のユーザーが複数の "_サブスクリプション_" にアクセスできる場合があります。サブスクリプションとは、Azure をはじめとするクラウド サービスを使用するための Microsoft との契約です。 各リソースは、サブスクリプションに関連付けられています。

テナント、ユーザー、サブスクリプションの違いの詳細については、[Azure クラウド用語集](/azure/azure-glossary-cloud-terminology)のページをご覧ください。  Azure Active Directory テナントに新しいサブスクリプションを追加する方法については、「[Azure サブスクリプションを Azure Active Directory テナントに関連付けるまたは追加する](/azure/active-directory/active-directory-how-subscriptions-associated-directory)」をご覧ください。
特定のテナントにサインインする方法を確認するには、[Azure PowerShell を使用したサインイン](/powershell/azure/authenticate-azureps)に関するページをご覧ください。

## <a name="change-the-active-subscription"></a>アクティブなサブスクリプションを変更する

Azure PowerShell でサブスクリプションのリソースにアクセスするには、現在の Azure セッションに関連付けられているサブスクリプションを変更する必要があります。
これは、アクティブなセッションのコンテキスト、どのテナント、サブスクリプション、およびユーザーに対してコマンドレットを実行するかについての情報を変更することによって実行します。
サブスクリプションを変更するには、まず Azure PowerShell コンテキスト オブジェクトを [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) で取得し、次に、現在のコンテキストを [Set-AzContext](/powershell/module/az.accounts/set-azcontext) で変更する必要があります。

次の例は、現在アクティブなテナントでサブスクリプションを取得し、アクティブなセッションとして設定する方法を示しています。

```powershell-interactive
$context = Get-AzSubscription -SubscriptionId ...
Set-AzContext $context
```

コンテキストの保存方法や複数のサブスクリプションすばやく簡単に切り替えて操作する方法など、Azure PowerShell コンテキストの詳細については、[Azure PowerShell コンテキストでの資格情報の保持](context-persistence.md)に関するページを参照してください。
