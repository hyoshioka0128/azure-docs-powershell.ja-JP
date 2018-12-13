---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 9a93145f2abeea466a739775ca8ae7e337e78166
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217849"
---
# <a name="sign-in-with-azure-powershell"></a>Azure PowerShell を使用してサインインする

Azure PowerShell は、複数の認証方法をサポートしています。 最も簡単に始められるのは、コマンド ラインから対話形式でサインインする方法です。

## <a name="sign-in-interactively"></a>対話操作でサインインする

対話操作でサインインするには、[Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) コマンドレットを使用します。

```azurepowershell-interactive
Connect-AzureRmAccount
```

このコマンドレットを実行すると、ダイアログ ボックスが表示され、Azure アカウントに関連付けられている電子メール アドレスとパスワードを入力するように求められます。 認証すると、現在の PowerShell セッションに対してこの情報が保存され、ダイアログは閉じます。これで、すべての Azure PowerShell コマンドレットにアクセスできます。

> [!IMPORTANT]
> このサインインは、現在の PowerShell セッション "_のみ_" を対象としています。 複数のセッションにわたって認証情報を保持する場合は、[永続的な資格情報](context-persistence.md)に関する記事をご覧ください。

## <a name="sign-in-with-a-service-principal"></a>サービス プリンシパルを使ってサインインする

サービス プリンシパルは、リソースの操作に使用できる非対話型のアカウントを作成する方法を提供します。 サービス プリンシパルは、Azure Active Directory を使用してルールを適用できるユーザー アカウントに似ています。 サービス プリンシパルに最低限必要なアクセス許可だけを付与することによって、自動化スクリプトをより安全にすることができます。

Azure PowerShell で使用するサービス プリンシパルを作成する必要がある場合は、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。

サービス プリンシパルを使用してサインインするには、`Connect-AzureRmAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。 サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。 サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。 このコマンドレットにより、サービス プリンシパル ユーザー ID とパスワードを入力するダイアログ ボックスが表示されます。

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-managed-identities-for-azure-resources"></a>Azure リソースのマネージド ID を使用してサインインする

Azure リソースのマネージドID は、Azure Active Directory の機能です。 サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。 マネージド ID は、Azure クラウドで実行されている仮想マシンでのみ使用できます。

Azure リソースのマネージド ID の詳細については、「[How to use managed identities for Azure resources on an Azure VM to acquire an access token (Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法)](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。

## <a name="sign-in-to-another-cloud"></a>別のクラウドにサインインする

Azure クラウド サービスでは、さまざまなリージョンのデータ処理規制に準拠したさまざまな環境を提供します。 Azure アカウントがこれらのリージョンのいずれかに関連付けられたクラウド内にある場合は、サインイン時に環境を指定する必要があります。 たとえば、アカウントが中国のクラウド内にある場合、次のコマンドを使用してサインインします。

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

使用可能な環境の一覧を取得するには、次のコマンドを使用します。

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Azure ロールベース アクセスの管理についての詳細情報

Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。

ロール管理を目的とした Azure PowerShell のコマンドレット:

* [Get-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [Get-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [New-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleAssignment](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [Remove-AzureRmRoleDefinition](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
