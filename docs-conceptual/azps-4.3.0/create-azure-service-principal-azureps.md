---
title: Azure PowerShell で Azure サービス プリンシパルを使用する
description: Azure PowerShell でサービス プリンシパルを作成および使用する方法について説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/17/2020
ms.openlocfilehash: ebdc0783c43ccecbbeb315de5b5baebc9539b40e
ms.sourcegitcommit: 747769a143ddebff39e78c2cc62a182401adddb9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/23/2020
ms.locfileid: "85268121"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a>Azure PowerShell で Azure サービス プリンシパルを作成する

Azure サービスを使用する自動化ツールのアクセス許可は、常に制限されている必要があります。 完全な特権を持つユーザーとしてアプリケーションをサインインさせる代わりに、Azure にはサービス プリンシパルが用意されています。

Azure サービス プリンシパルは、Azure リソースにアクセスするアプリケーション、ホステッド サービス、および自動化ツールで使用するために作成される ID です。 このアクセスはサービス プリンシパルに割り当てられているロールによって制限されるため、どのリソースに、どのレベルでアクセスできるかを制御することができます。 セキュリティ上の理由から、自動化ツールにはユーザー ID でのログインを許可するのではなく、常にサービス プリンシパルを使用することを推奨します。

この記事では、Azure PowerShell を使用して、サービス プリンシパルの作成、情報取得、およびリセットを行うための手順について説明します。

## <a name="create-a-service-principal"></a>サービス プリンシパルの作成

[New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal) コマンドレットを使用してサービス プリンシパルを作成します。 サービス プリンシパルを作成する際に、サービス プリンシパルが使用するサインイン認証の種類を選択します。

> [!NOTE]
> ご利用のアカウントにサービス プリンシパルを作成するためのアクセス許可がない場合は、`New-AzADServicePrincipal` から "この操作を完了するのに十分な特権がありません" というエラー メッセージが返されます。
> サービス プリンシパルを作成するには、Azure Active Directory 管理者にお問い合わせください。

サービス プリンシパルで使用できる認証には、パスワードベースの認証と証明書ベースの認証の 2 種類があります。

### <a name="password-based-authentication"></a>パスワードベースの認証

> [!IMPORTANT]
> パスワードベースの認証サービス プリンシパルの既定ロールは**共同作成者**です。 このロールには、Azure アカウントの読み取りと書き込みを行うための完全なアクセス許可が付与されます。 ロールの割り当ての管理については、「[サービス プリンシパル ロールを管理する](#manage-service-principal-roles)」を参照してください。

パスワード ベースの認証では、他の認証パラメーターは使用せず、自動的に作成されるランダム パスワードを使用します。 パスワード ベースの認証を使用する場合は、次の方法をお勧めします。

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

返されるオブジェクトには、`Secret` メンバーが含まれています。これは生成されたパスワードを格納している `SecureString` です。 サービス プリンシパルで認証するためには、この値を必ず安全な場所に保存してください。 この値は、コンソール出力には表示され_ません_。 パスワードを紛失した場合は、[サービス プリンシパルの資格情報をリセット](#reset-credentials)します。

次のコードにより、シークレットをエクスポートできます。

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($sp.Secret)
$UnsecureSecret = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
```

ユーザー指定のパスワードの場合、`-PasswordCredential` 引数は `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential` オブジェクトを受け取ります。 これらのオブジェクトは有効な `StartDate` と`EndDate` を持ち、プレーンテキストの `Password` を受け取ります。 パスワードを作成する際は、必ず [Azure Active Directory のパスワードの規則と制約事項](/azure/active-directory/active-directory-passwords-policy)に従ってください。
脆弱なパスワードを使用したり、パスワードを再利用したりしないでください。

```azurepowershell-interactive
Import-Module -Name Az.Resources # Imports the PSADPasswordCredential object
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential -Property @{StartDate=Get-Date; EndDate=Get-Date -Year 2024; Password=<Choose a strong password>}
$sp = New-AzAdServicePrincipal -DisplayName ServicePrincipalName -PasswordCredential $credentials
```

`New-AzADServicePrincipal` から返されるオブジェクトには `Id` メンバーと `DisplayName` メンバーが含まれ、そのどちらもサービス プリンシパルでのサインインに使用できます。

> [!IMPORTANT]
> サービス プリンシパルを使用してサインインするには、サービス プリンシパルを作成したテナントの ID が必要です。 サービス プリンシパルの作成時にアクティブなテナントを取得するには、サービス プリンシパルの作成_直後に_、次のコマンドを実行します。

```azurepowershell-interactive
(Get-AzContext).Tenant.Id
```

### <a name="certificate-based-authentication"></a>証明書ベースの認証

> [!IMPORTANT]
> 証明書ベースの認証サービス プリンシパルを作成するときに割り当てられる既定のロールはありません。 ロールの割り当ての管理については、「[サービス プリンシパル ロールを管理する](#manage-service-principal-roles)」を参照してください。

証明書ベースの認証を使用するサービス プリンシパルは、`-CertValue` パラメーターを使用して作成します。 このパラメーターは、公開証明書の Base64 でエンコードされた ASCII 文字列を受け取ります。 これは、PEM ファイル、あるいはテキスト エンコードされた CRT または CER で表されます。 公開証明書のバイナリ エンコーディングはサポートされていません。 この手順では、既に証明書を使用できるようになっていることを前提としています。

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -CertValue $cert
```

また、`-KeyCredential` パラメーターを使用することもできます。これは `PSADKeyCredential` オブジェクトを受け取ります。 これらのオブジェクトは、有効な `StartDate` と `EndDate` を持ち、`CertValue` メンバーが公開証明書の Base64 でエンコードされた ASCII 文字列に設定されている必要があります。

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADKeyCredential -Property @{StartDate=Get-Date; EndDate=Get-Date -Year 2024; KeyId=New-Guid; CertValue=$cert}
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -KeyCredential $credentials
```

`New-AzADServicePrincipal` から返されるオブジェクトには `Id` メンバーと `DisplayName` メンバーが含まれ、そのどちらもサービス プリンシパルでのサインインに使用できます。 サービス プリンシパルを使用してサインインするクライアントには、証明書の秘密キーへのアクセス権も必要です。

> [!IMPORTANT]
> サービス プリンシパルを使用してサインインするには、サービス プリンシパルを作成したテナントの ID が必要です。 サービス プリンシパルの作成時にアクティブなテナントを取得するには、サービス プリンシパルの作成_直後に_、次のコマンドを実行します。

```azurepowershell-interactive
(Get-AzContext).Tenant.Id
```

## <a name="get-an-existing-service-principal"></a>既存のサービス プリンシパルの取得

[Get AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal) を使用すると、アクティブなテナントのサービス プリンシパル一覧を取得できます。 既定では、このコマンドによって、テナント内の "_すべて_" のサービス プリンシパルが返されます。 大規模な組織では、結果が返されるまでに長い時間がかかることがあります。 代わりに、オプションのサーバー側フィルター処理引数のいずれかを使用することをお勧めします。

- `-DisplayNameBeginsWith` は、指定した値に一致する "_プレフィックス_" を持つサービス プリンシパルを要求します。 サービス プリンシパルの表示名は、作成時に `-DisplayName` で設定した値です。
- `-DisplayName` は、サービス プリンシパル名に "_正確に一致するもの_" を要求します。

## <a name="manage-service-principal-roles"></a>サービス プリンシパル ロールを管理する

Azure PowerShell には、ロールの割り当てを管理するための、次のコマンドレットが用意されています。

- [Get-AzRoleAssignment](/powershell/module/az.resources/get-azroleassignment)
- [New-AzRoleAssignment](/powershell/module/az.resources/new-azroleassignment)
- [Remove-AzRoleAssignment](/powershell/module/az.resources/remove-azroleassignment)

パスワードベースの認証サービス プリンシパルの既定ロールは**共同作成者**です。 このロールには、Azure アカウントの読み取りと書き込みを行うための完全なアクセス許可が付与されます。 **閲覧者**ロールは制限がより厳しく、読み取り専用アクセスが提供されます。 ロールベースのアクセス制御 (RBAC) とロールの詳細については、[RBAC の組み込みのロール](/azure/active-directory/role-based-access-built-in-roles)に関するページをご覧ください。

この例では、**閲覧者**ロールを追加し、**共同作成者**ロールを削除します。

```azurepowershell-interactive
New-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName 'Reader'
Remove-AzRoleAssignment -ObjectId <service principal object ID> -RoleDefinitionName 'Contributor'
```

> [!IMPORTANT]
> ロールの割り当てコマンドレットは、サービス プリンシパル オブジェクト ID を受け取りません。 これらは、作成時に生成され、関連付けられているアプリケーション ID を受け取ります。 サービス プリンシパルのアプリケーション ID を取得するには、`Get-AzADServicePrincipal` を使用します。

> [!NOTE]
> ロールを割り当てるためのアクセス許可がアカウントにない場合は、アカウントに "'Microsoft.Authorization/roleAssignments/write' のアクションを実行するためのアクセス権限がありません" というエラー メッセージが表示されます。 ロールを管理するには、Azure Active Directory 管理者にお問い合わせください。

ロールを追加しても、以前に割り当てられたアクセス許可は制限され "_ません_"。 サービス プリンシパルのアクセス許可を制限するときは、**共同作成者**ロールを削除する必要があります。

変更を確認するには、割り当てられているロールの一覧を表示します。

```azurepowershell-interactive
Get-AzRoleAssignment -ServicePrincipalName ServicePrincipalName
```

## <a name="sign-in-using-a-service-principal"></a>サービス プリンシパルを使用したサインイン

サインインして、新しいサービス プリンシパルの資格情報とアクセス許可をテストします。 サービス プリンシパルでサインインするには、サービス プリンシパルに関連付けられている `applicationId` 値、およびサービス プリンシパルを作成したテナントが必要です。

パスワードを使用してサービス プリンシパルでサインインするには、次のコマンドを使用します。

```azurepowershell-interactive
# Use the application ID as the username, and the secret as password
$credentials = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $credentials -Tenant <tenant ID>
```

証明書ベースの認証では、Azure PowerShell で、証明書の拇印に基づいてローカル証明書ストアから情報を取得できる必要があります。

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -Tenant <tenant ID> -CertificateThumbprint <thumbprint>
```

PowerShell がアクセスできる資格情報ストアに証明書をインポートする手順については、「[Sign in with Azure PowerShell (Azure PowerShell を使用してサインインする)](authenticate-azureps.md#sp-signin)」を参照してください

## <a name="reset-credentials"></a>資格情報をリセットする

サービス プリンシパルの資格情報を忘れた場合は、[New-AzADSpCredential](/powershell/module/az.resources/new-azadspcredential) を使用して新しい資格情報とランダムなパスワードを追加します。 このコマンドレットでは、パスワードをリセットするときにユーザー定義の資格情報はサポートされません。

> [!IMPORTANT]
> 新しい資格情報を割り当てる前に、既存の資格情報を使用したサインインを防ぐために、既存の資格情報を削除する必要があります。 これを行うには、[Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential) コマンドレットを使用します。

```azurepowershell-interactive
Remove-AzADSpCredential -DisplayName ServicePrincipalName
```

```azurepowershell-interactive
$newCredential = New-AzADSpCredential -ServicePrincipalName ServicePrincipalName
```

## <a name="troubleshooting"></a>トラブルシューティング

エラー _"New-AzADServicePrincipal: プロパティ identifierUris に対して同じ値を持つ別のオブジェクトが既に存在します"_ を受け取った場合は、同じ名前のサービス プリンシパルがまだ存在していないことを確認してください。

```azurepowershell-interactive
Get-AzAdServicePrincipal -DisplayName ServicePrincipalName
```

既存のサービス プリンシパルがもう不要である場合は、次の例を使用して削除できます。

```azurepowershell-interactive
Remove-AzAdServicePrincipal -DisplayName ServicePrincipalName
```

このエラーは、以前に Azure Active Directory アプリケーションのサービス プリンシパルを作成した場合にも発生する可能性があります。 サービス プリンシパルを削除しても、アプリケーションは引き続き利用できます。 このアプリケーションでは、同じ名前で別のサービス プリンシパルを作成することはできません。

次の例を使用すると、同じ名前の Azure Active Directory アプリケーションが存在しないことを確認できます。

```azurepowershell-interactive
Get-AzADApplication -DisplayName ServicePrincipalName
```

同じ名前のアプリケーションが存在するが、もう必要ない場合は、次の例を使用して削除できます。

```azurepowershell-interactive
Remove-AzADApplication -DisplayName ServicePrincipalName
```

それ以外の場合は、作成しようとしている新しいサービス プリンシパルの代替名を選択します。
