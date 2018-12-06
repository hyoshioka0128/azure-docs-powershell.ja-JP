---
title: Azure PowerShell で Azure サービス プリンシパルを作成する
description: Azure PowerShell でアプリまたはサービスのサービス プリンシパルを作成する方法について説明します。
keywords: Azure PowerShell, Azure Active Directory, Azure Active Directory, AD, RBAC
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 2db1ada32e5a9285c27ec3f569b622c9c33a06b0
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "52826631"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a>Azure PowerShell で Azure サービス プリンシパルを作成する

Azure PowerShell を使ってアプリまたはサービスを管理する場合、その実行には、自分の資格情報ではなく、Azure Active Directory (AAD) のサービス プリンシパルを使用する必要があります。 この記事では、Azure PowerShell でセキュリティ プリンシパルを作成する手順を紹介します。

> [!NOTE]
> Azure Portal からサービス プリンシパルを作成することもできます。 詳細については、「[リソースにアクセスできる Azure Active Directory アプリケーションとサービス プリンシパルをポータルで作成する](/azure/azure-resource-manager/resource-group-create-service-principal-portal)」を参照してください。

## <a name="what-is-a-service-principal"></a>"サービス プリンシパル" とは

Azure サービス プリンシパルは、ユーザーによって作成されたアプリやサービス、オートメーション ツールが特定の Azure リソースにアクセスする際に使うセキュリティ ID です。 アクセス許可が厳しく管理された、特定のロールが与えられた "ユーザー ID" (ユーザー名とパスワードまたは証明書) と考えてください。 一般的なユーザー ID とは異なり、サービス プリンシパルで行うタスクは制限する必要があります。 管理タスクを実行するために必要な最小限のアクセス許可レベルだけを与えるようにすれば、セキュリティは向上します。

## <a name="verify-your-own-permission-level"></a>自分のアクセス許可レベルの確認

まず、Azure Active Directory と Azure サブスクリプションの両方で適切なアクセス許可を持っている必要があります。 Active Directory でアプリを作成し、サービス プリンシパルにロールを割り当てることができる必要があります。

自分のアカウントに適切なアクセス許可があるかどうかを確認する最も簡単な方法は、ポータルを使用することです。 [ポータルでの必要なアクセス許可のチェック](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions)に関するページをご覧ください。

## <a name="create-a-service-principal-for-your-app"></a>アプリのサービス プリンシパルを作成する

サービス プリンシパルは、Azure アカウントへのサインイン後に作成することができます。 デプロイされているアプリを識別する手段が必要です。次のいずれかの方法があります。

* デプロイされているアプリの一意の名前 (次の例の "MyDemoWebApp" など)
* アプリケーション ID (デプロイされているアプリやサービス、オブジェクトに関連付けられている一意の GUID)

### <a name="get-information-about-your-application"></a>アプリケーションに関する情報を取得する

アプリケーションに関する情報は、`Get-AzureRmADApplication` コマンドレットを使って取得できます。

```azurepowershell-interactive
Get-AzureRmADApplication -DisplayNameStartWith MyDemoWebApp
```

```output
DisplayName             : MyDemoWebApp
ObjectId                : 775f64cd-0ec8-4b9b-b69a-8b8946022d9f
IdentifierUris          : {http://MyDemoWebApp}
HomePage                : http://www.contoso.com
Type                    : Application
ApplicationId           : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
AvailableToOtherTenants : False
AppPermissions          :
ReplyUrls               : {}
```

### <a name="create-a-service-principal-for-your-application"></a>アプリケーションのサービス プリンシパルを作成する

サービス プリンシパルは、`New-AzureRmADServicePrincipal` コマンドレットを使って作成します。

```azurepowershell-interactive
$servicePrincipal = New-AzureRmADServicePrincipal -ApplicationId 00c01aaa-1603-49fc-b6df-b78c4e5138b4
```

```output
Secret                : System.Security.SecureString
ServicePrincipalNames : {00c01aaa-1603-49fc-b6df-b78c4e5138b4, http://MyDemoWebApp}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
AdfsId                :
Type                  : ServicePrincipal
```

ここから、Connect-AzureRmAccount で $servicePrincipal.Secret プロパティを直接使用する (次の「サービス プリンシパルを使ってサインインする」を参照) か、後で使用できるようにこの SecureString をプレーンテキストに変換することができます。

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($servicePrincipal.Secret)
$password = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
[Runtime.InteropServices.Marshal]::ZeroFreeBSTR($BSTR)
```

### <a name="sign-in-using-the-service-principal"></a>サービス プリンシパルを使ってサインインする

指定した "*アプリ ID*" と自動生成された "*パスワード*" を使って、アプリの新しいサービス プリンシパルとしてサインインできるようになりました。 サービス プリンシパルのテナント ID も必要です。 テナント ID は、個人用の資格情報で Azure にサインインすると表示されます。 サービス プリンシパルを使用してサインインするには、次のコマンドを使用します。

```azurepowershell-interactive
$cred = New-Object System.Management.Automation.PSCredential ("00c01aaa-1603-49fc-b6df-b78c4e5138b4", $servicePrincipal.Secret)
Connect-AzureRmAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

サインインに成功すると、次のような出力が表示されます。

```output
Environment           : AzureCloud
Account               : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
SubscriptionId        :
SubscriptionName      :
CurrentStorageAccount :
```

お疲れさまでした。 これらの資格情報を使ってアプリを実行することができます。 次に、サービス プリンシパルのアクセス許可を調整する必要があります。

## <a name="managing-roles"></a>ロールの管理

> [!NOTE]
> Azure のロールベースのアクセス制御 (RBAC) は、ユーザー プリンシパルとサービス プリンシパルのロールを定義して管理するためのモデルです。 ロールに関連付けられる一連のアクセス許可によって、プリンシパルが各種の操作 (読み取り、アクセス、書き込み、または管理) を実行できるリソースが決まります。 RBAC とロールについて詳しくは、[RBAC のための組み込みロール](/azure/active-directory/role-based-access-built-in-roles)に関するページをご覧ください。

Azure PowerShell には、ロールの割り当て管理を目的とした次のコマンドレットが用意されています。

* [Get-AzureRmRoleAssignment](/powershell/module/azurerm.resources/get-azurermroleassignment)
* [New-AzureRmRoleAssignment](/powershell/module/azurerm.resources/new-azurermroleassignment)
* [Remove-AzureRmRoleAssignment](/powershell/module/azurerm.resources/remove-azurermroleassignment)

サービス プリンシパルの既定のロールは**共同作成者**です。 このロールは、広範なアクセス許可が与えられていることから、Azure サービスに対するアプリの対話の範囲によっては最適とは言えない場合もあります。
読み取り専用のアプリであれば、より制限の厳しい**閲覧者**ロールの方が適しています。 Azure Portal でロールごとのアクセス許可について詳しい情報を確認したり、カスタム ロールを作成したりすることができます。

この例では、先ほどの例に**閲覧者**ロールを追加し、**共同作成者**ロールを削除しています。

```azurepowershell-interactive
New-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Reader
```

```output
RoleAssignmentId   : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG/providers/Microsoft.Authorization/roleAssignments/818892f2-d075-46a1-a3a2-3a4e1a12fcd5
Scope              : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG
DisplayName        : MyDemoWebApp
SignInName         :
RoleDefinitionName : Reader
RoleDefinitionId   : b24988ac-6180-42a0-ab88-20f7382dd24c
ObjectId           : 698138e7-d7b6-4738-a866-b4e3081a69e4
ObjectType         : ServicePrincipal
```

```azurepowershell-interactive
Remove-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4 -RoleDefinitionName Contributor
```

現在割り当てられているロールを表示するには、次のコマンドレットを使用します。

```azurepowershell-interactive
Get-AzureRmRoleAssignment -ResourceGroupName myRG -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
```

```output
RoleAssignmentId   : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG/providers/Microsoft.Authorization/roleAssignments/0906bbd8-9982-4c03-8dae-aeaae8b13f9e
Scope              : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myRG
DisplayName        : MyDemoWebApp
SignInName         :
RoleDefinitionName : Reader
RoleDefinitionId   : acdd72a7-3385-48ef-bd42-f606fba81ae7
ObjectId           : 698138e7-d7b6-4738-a866-b4e3081a69e4
ObjectType         : ServicePrincipal
```

その他、ロールの管理を目的として次の Azure PowerShell コマンドレットが用意されています。

* [Get-AzureRmRoleDefinition](/powershell/module/azurerm.resources/Get-AzureRmRoleDefinition)
* [New-AzureRmRoleDefinition](/powershell/module/azurerm.resources/New-AzureRmRoleDefinition)
* [Remove-AzureRmRoleDefinition](/powershell/module/azurerm.resources/Remove-AzureRmRoleDefinition)
* [Set-AzureRmRoleDefinition](/powershell/module/azurerm.resources/Set-AzureRmRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a>セキュリティ プリンシパルの資格情報を変更する

セキュリティ上、アクセス許可の確認とパスワードの更新を定期的に行うことが大切です。 必要に応じて、アプリの変更に合わせてセキュリティ資格情報を適宜更新することもできます。 たとえばサービス プリンシパルのパスワードは、新しいパスワードを作成して古いパスワードを削除することで変更できます。

### <a name="add-a-new-password-for-the-service-principal"></a>サービス プリンシパルの新しいパスワードを追加する

```azurepowershell-interactive
New-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
Secret    : System.Security.SecureString
StartDate : 11/16/2018 12:38:23 AM
EndDate   : 11/16/2019 12:38:23 AM
KeyId     : 6f801c3e-6fcd-42b9-be8e-320b17ba1d36
Type      : Password
```

### <a name="get-a-list-of-credentials-for-the-service-principal"></a>サービス プリンシパルの一連の資格情報を取得する

```azurepowershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a>サービス プリンシパルから古いパスワードを削除する

```azurepowershell-interactive
Remove-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a>サービス プリンシパルの一連の資格情報を確認する

```azurepowershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-information-about-the-service-principal"></a>サービス プリンシパルに関する情報を取得する

```azurepowershell-interactive
$svcprincipal = Get-AzureRmADServicePrincipal -ObjectId 698138e7-d7b6-4738-a866-b4e3081a69e4
$svcprincipal | Select-Object *
```

```output
ServicePrincipalNames : {http://MyDemoWebApp, 00c01aaa-1603-49fc-b6df-b78c4e5138b4}
ApplicationId         : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
DisplayName           : MyDemoWebApp
Id                    : 698138e7-d7b6-4738-a866-b4e3081a69e4
Type                  : ServicePrincipal
```
