---
title: Azure PowerShell で Azure サービス プリンシパルを使用する
description: Azure PowerShell でサービス プリンシパルを作成および使用する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 04/23/2019
ms.openlocfilehash: 1980600207cbd65abb8b0bc1afcdc65fbcfd0dc2
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498779"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="6664d-103">Azure PowerShell で Azure サービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="6664d-103">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="6664d-104">Azure サービスを使用する自動化ツールのアクセス許可は、常に制限されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6664d-104">Automated tools that use Azure services should always have restricted permissions.</span></span> <span data-ttu-id="6664d-105">完全な特権を持つユーザーとしてアプリケーションをサインインさせる代わりに、Azure にはサービス プリンシパルが用意されています。</span><span class="sxs-lookup"><span data-stu-id="6664d-105">Instead of having applications sign in as a fully privileged user, Azure offers service principals.</span></span>

<span data-ttu-id="6664d-106">Azure サービス プリンシパルは、Azure リソースにアクセスするアプリケーション、ホステッド サービス、および自動化ツールで使用するために作成される ID です。</span><span class="sxs-lookup"><span data-stu-id="6664d-106">An Azure service principal is an identity created for use with applications, hosted services, and automated tools to access Azure resources.</span></span> <span data-ttu-id="6664d-107">このアクセスはサービス プリンシパルに割り当てられているロールによって制限されるため、どのリソースに、どのレベルでアクセスできるかを制御することができます。</span><span class="sxs-lookup"><span data-stu-id="6664d-107">This access is restricted by the roles assigned to the service principal, giving you control over which resources can be accessed and at which level.</span></span> <span data-ttu-id="6664d-108">セキュリティ上の理由から、自動化ツールにはユーザー ID でのログインを許可するのではなく、常にサービス プリンシパルを使用することを推奨します。</span><span class="sxs-lookup"><span data-stu-id="6664d-108">For security reasons, it's always recommended to use service principals with automated tools rather than allowing them to log in with a user identity.</span></span>

<span data-ttu-id="6664d-109">この記事では、Azure PowerShell を使用して、サービス プリンシパルの作成、情報取得、およびリセットを行うための手順について説明します。</span><span class="sxs-lookup"><span data-stu-id="6664d-109">This article shows you the steps for creating, getting information about, and resetting a service principal with Azure PowerShell.</span></span>

## <a name="create-a-service-principal"></a><span data-ttu-id="6664d-110">サービス プリンシパルの作成</span><span class="sxs-lookup"><span data-stu-id="6664d-110">Create a service principal</span></span>

<span data-ttu-id="6664d-111">[New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal) コマンドレットを使用してサービス プリンシパルを作成します。</span><span class="sxs-lookup"><span data-stu-id="6664d-111">Create a service principal with the [New-AzADServicePrincipal](/powershell/module/Az.Resources/New-AzADServicePrincipal) cmdlet.</span></span> <span data-ttu-id="6664d-112">サービス プリンシパルを作成する際に、サービス プリンシパルが使用するサインイン認証の種類を選択します。</span><span class="sxs-lookup"><span data-stu-id="6664d-112">When creating a service principal, you choose the type of sign-in authentication it uses.</span></span>

> [!NOTE]
>
> <span data-ttu-id="6664d-113">ご利用のアカウントにサービス プリンシパルを作成するためのアクセス許可がない場合は、`New-AzADServicePrincipal` から "この操作を完了するのに十分な特権がありません" というエラー メッセージが返されます。</span><span class="sxs-lookup"><span data-stu-id="6664d-113">If your account doesn't have permission to create a service principal, `New-AzADServicePrincipal` will return an error message containing "Insufficient privileges to complete the operation."</span></span> <span data-ttu-id="6664d-114">サービス プリンシパルを作成するには、Azure Active Directory 管理者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6664d-114">Contact your Azure Active Directory admin to create a service principal.</span></span>

<span data-ttu-id="6664d-115">サービス プリンシパルで使用できる認証には、パスワードベースの認証と証明書ベースの認証の 2 種類があります。</span><span class="sxs-lookup"><span data-stu-id="6664d-115">There are two types of authentication available for service principals: Password-based authentication, and certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="6664d-116">パスワードベースの認証</span><span class="sxs-lookup"><span data-stu-id="6664d-116">Password-based authentication</span></span>

<span data-ttu-id="6664d-117">パスワード ベースの認証では、他の認証パラメーターは使用せず、自動的に作成されるランダム パスワードを使用します。</span><span class="sxs-lookup"><span data-stu-id="6664d-117">Without any other authentication parameters, password-based authentication is used and a random password created for you.</span></span> <span data-ttu-id="6664d-118">パスワード ベースの認証を使用する場合は、次の方法をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6664d-118">If you want password-based authentication, this method is recommended.</span></span>

```azurepowershell-interactive
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName
```

<span data-ttu-id="6664d-119">返されるオブジェクトには、`Secret` メンバーが含まれています。これは生成されたパスワードを格納している `SecureString` です。</span><span class="sxs-lookup"><span data-stu-id="6664d-119">The returned object contains the `Secret` member, which is a `SecureString` containing the generated password.</span></span> <span data-ttu-id="6664d-120">サービス プリンシパルで認証するためには、この値を必ず安全な場所に保存してください。</span><span class="sxs-lookup"><span data-stu-id="6664d-120">Make sure that you store this value somewhere secure to authenticate with the service principal.</span></span> <span data-ttu-id="6664d-121">この値は、コンソール出力には表示され__ません__。</span><span class="sxs-lookup"><span data-stu-id="6664d-121">Its value __won't__ be displayed in the console output.</span></span> <span data-ttu-id="6664d-122">パスワードを紛失した場合は、[サービス プリンシパルの資格情報をリセット](#reset-credentials)します。</span><span class="sxs-lookup"><span data-stu-id="6664d-122">If you lose the password, [reset the service principal credentials](#reset-credentials).</span></span> 

<span data-ttu-id="6664d-123">ユーザー指定のパスワードの場合、`-PasswordCredential` 引数は `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential` オブジェクトを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6664d-123">For user-supplied passwords, the `-PasswordCredential` argument takes `Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential` objects.</span></span> <span data-ttu-id="6664d-124">これらのオブジェクトは有効な `StartDate` と`EndDate` を持ち、プレーンテキストの `Password` を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6664d-124">These objects must have a valid `StartDate` and `EndDate`, and take a plaintext `Password`.</span></span> <span data-ttu-id="6664d-125">パスワードを作成する際は、必ず [Azure Active Directory のパスワードの規則と制約事項](/azure/active-directory/active-directory-passwords-policy)に従ってください。</span><span class="sxs-lookup"><span data-stu-id="6664d-125">When creating a password, make sure you follow the [Azure Active Directory password rules and restrictions](/azure/active-directory/active-directory-passwords-policy).</span></span> <span data-ttu-id="6664d-126">脆弱なパスワードを使用したり、パスワードを再利用したりしないでください。</span><span class="sxs-lookup"><span data-stu-id="6664d-126">Don't use a weak password or reuse a password.</span></span>

```azurepowershell-interactive
Import-Module Az.Resources # Imports the PSADPasswordCredential object
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADPasswordCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; Password=<Choose a strong password>}
$sp = New-AzAdServicePrincipal -DisplayName ServicePrincipalName -PasswordCredential $credentials
```

<span data-ttu-id="6664d-127">`New-AzADServicePrincipal` から返されるオブジェクトには `Id` メンバーと `DisplayName` メンバーが含まれ、そのどちらもサービス プリンシパルでのサインインに使用できます。</span><span class="sxs-lookup"><span data-stu-id="6664d-127">The object returned from `New-AzADServicePrincipal` contains the `Id` and `DisplayName` members, either of which can be used for sign in with the service principal.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="6664d-128">サービス プリンシパルを使用してサインインするには、サービス プリンシパルを作成したテナントの ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="6664d-128">Signing in with a service principal requires the tenant ID which the service principal was created under.</span></span> <span data-ttu-id="6664d-129">サービス プリンシパルの作成時にアクティブなテナントを取得するには、サービス プリンシパルの作成__直後に__、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="6664d-129">To get the active tenant when the service principal was created, run the following command __immediately after__ service principal creation:</span></span>
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

### <a name="certificate-based-authentication"></a><span data-ttu-id="6664d-130">証明書ベースの認証</span><span class="sxs-lookup"><span data-stu-id="6664d-130">Certificate-based authentication</span></span>

<span data-ttu-id="6664d-131">証明書ベースの認証を使用するサービス プリンシパルは、`-CertValue` パラメーターを使用して作成します。</span><span class="sxs-lookup"><span data-stu-id="6664d-131">Service principals using certificate-based authentication are created with the `-CertValue` parameter.</span></span> <span data-ttu-id="6664d-132">このパラメーターは、公開証明書の Base64 でエンコードされた ASCII 文字列を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6664d-132">This parameter takes a base64-encoded ASCII string of the public certificate.</span></span> <span data-ttu-id="6664d-133">これは、PEM ファイル、あるいはテキスト エンコードされた CRT または CER で表されます。</span><span class="sxs-lookup"><span data-stu-id="6664d-133">This is represented by a PEM file, or a text-encoded CRT or CER.</span></span> <span data-ttu-id="6664d-134">公開証明書のバイナリ エンコーディングはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6664d-134">Binary encodings of the public certificate aren't supported.</span></span> <span data-ttu-id="6664d-135">この手順では、既に証明書を使用できるようになっていることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="6664d-135">These instructions assume that you already have a certificate available.</span></span>

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -CertValue $cert
```

<span data-ttu-id="6664d-136">また、`-KeyCredential` パラメーターを使用することもできます。これは `PSADKeyCredential` オブジェクトを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6664d-136">You can also use the `-KeyCredential` parameter, which takes `PSADKeyCredential` objects.</span></span> <span data-ttu-id="6664d-137">これらのオブジェクトは、有効な `StartDate` と `EndDate` を持ち、`CertValue` メンバーが公開証明書の Base64 でエンコードされた ASCII 文字列に設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6664d-137">These objects must have a valid `StartDate`, `EndDate`, and have the `CertValue` member set to a base64-encoded ASCII string of the public certificate.</span></span>

```azurepowershell-interactive
$cert = <public certificate as base64-encoded string>
$credentials = New-Object Microsoft.Azure.Commands.ActiveDirectory.PSADKeyCredential -Property @{ StartDate=Get-Date; EndDate=Get-Date -Year 2024; KeyId=New-Guid; CertValue=$cert}
$sp = New-AzADServicePrincipal -DisplayName ServicePrincipalName -KeyCredential $credentials
```

<span data-ttu-id="6664d-138">`New-AzADServicePrincipal` から返されるオブジェクトには `Id` メンバーと `DisplayName` メンバーが含まれ、そのどちらもサービス プリンシパルでのサインインに使用できます。</span><span class="sxs-lookup"><span data-stu-id="6664d-138">The object returned from `New-AzADServicePrincipal` contains the `Id` and `DisplayName` members, either of which can be used for sign in with the service principal.</span></span> <span data-ttu-id="6664d-139">サービス プリンシパルを使用してサインインするクライアントには、証明書の秘密キーへのアクセス権も必要です。</span><span class="sxs-lookup"><span data-stu-id="6664d-139">Clients which sign in with the service principal also need access to the certificate's private key.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="6664d-140">サービス プリンシパルを使用してサインインするには、サービス プリンシパルを作成したテナントの ID が必要です。</span><span class="sxs-lookup"><span data-stu-id="6664d-140">Signing in with a service principal requires the tenant ID which the service principal was created under.</span></span> <span data-ttu-id="6664d-141">サービス プリンシパルの作成時にアクティブなテナントを取得するには、サービス プリンシパルの作成__直後に__、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="6664d-141">To get the active tenant when the service principal was created, run the following command __immediately after__ service principal creation:</span></span>
>
> ```azurepowershell-interactive
> (Get-AzContext).Tenant.Id
> ```

## <a name="get-an-existing-service-principal"></a><span data-ttu-id="6664d-142">既存のサービス プリンシパルの取得</span><span class="sxs-lookup"><span data-stu-id="6664d-142">Get an existing service principal</span></span>

<span data-ttu-id="6664d-143">[Get AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal) を使用すると、現在アクティブなテナントのサービス プリンシパル一覧を取得できます。</span><span class="sxs-lookup"><span data-stu-id="6664d-143">A list of service principals for the currently active tenant can be retrieved with [Get-AzADServicePrincipal](/powershell/module/az.resources/get-azadserviceprincipal).</span></span> <span data-ttu-id="6664d-144">既定では、このコマンドによってテナント内の__すべての__サービス プリンシパルが返されるため、大規模な組織の場合は、結果が返されるまでに長時間を要することがあります。</span><span class="sxs-lookup"><span data-stu-id="6664d-144">By default this command returns __all__ service principals in a tenant, so for large organizations, it may take a long time to return results.</span></span> <span data-ttu-id="6664d-145">代わりに、オプションのサーバー側フィルター処理引数のいずれかを使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="6664d-145">Instead, using one of the optional server-side filtering arguments is recommended:</span></span>

* <span data-ttu-id="6664d-146">`-DisplayNameBeginsWith` は、指定した値に一致する "_プレフィックス_" を持つサービス プリンシパルを要求します。</span><span class="sxs-lookup"><span data-stu-id="6664d-146">`-DisplayNameBeginsWith` requests service principals that have a _prefix_ that match the provided value.</span></span> <span data-ttu-id="6664d-147">サービス プリンシパルの表示名は、作成時に `-DisplayName` で設定した値です。</span><span class="sxs-lookup"><span data-stu-id="6664d-147">The display name of a service principal is the value set with `-DisplayName` during creation.</span></span>
* <span data-ttu-id="6664d-148">`-DisplayName` は、サービス プリンシパル名に "_正確に一致するもの_" を要求します。</span><span class="sxs-lookup"><span data-stu-id="6664d-148">`-DisplayName` requests an _exact match_ of a service principal name.</span></span>

## <a name="manage-service-principal-roles"></a><span data-ttu-id="6664d-149">サービス プリンシパル ロールを管理する</span><span class="sxs-lookup"><span data-stu-id="6664d-149">Manage service principal roles</span></span>

<span data-ttu-id="6664d-150">Azure PowerShell には、ロールの割り当てを管理するための、次のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="6664d-150">Azure PowerShell has the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="6664d-151">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6664d-151">Get-AzRoleAssignment</span></span>](/powershell/module/az.resources/get-azroleassignment)
* [<span data-ttu-id="6664d-152">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6664d-152">New-AzRoleAssignment</span></span>](/powershell/module/az.resources/new-azroleassignment)
* [<span data-ttu-id="6664d-153">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="6664d-153">Remove-AzRoleAssignment</span></span>](/powershell/module/az.resources/remove-azroleassignment)

<span data-ttu-id="6664d-154">サービス プリンシパルの既定のロールは**共同作成者**です。</span><span class="sxs-lookup"><span data-stu-id="6664d-154">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="6664d-155">このロールには、Azure アカウントの読み取りと書き込みを行うための完全なアクセス許可が付与されます。</span><span class="sxs-lookup"><span data-stu-id="6664d-155">This role has full permissions to read and write to an Azure account.</span></span> <span data-ttu-id="6664d-156">**閲覧者**ロールは制限がより厳しく、読み取り専用アクセスが提供されます。</span><span class="sxs-lookup"><span data-stu-id="6664d-156">The **Reader** role is more restrictive, with read-only access.</span></span>  <span data-ttu-id="6664d-157">ロールベースのアクセス制御 (RBAC) とロールの詳細については、[RBAC の組み込みのロール](/azure/active-directory/role-based-access-built-in-roles)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="6664d-157">For more information on Role-Based Access Control (RBAC) and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="6664d-158">この例では、**閲覧者**ロールを追加し、**共同作成者**ロールを削除します。</span><span class="sxs-lookup"><span data-stu-id="6664d-158">This example adds the **Reader** role and removes the **Contributor** one:</span></span>

```azurepowershell-interactive
New-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Reader"
Remove-AzRoleAssignment -ApplicationId <service principal application ID> -RoleDefinitionName "Contributor"
```

> [!IMPORTANT]
> <span data-ttu-id="6664d-159">ロールの割り当てコマンドレットは、サービス プリンシパル オブジェクト ID を受け取りません。</span><span class="sxs-lookup"><span data-stu-id="6664d-159">Role assignment cmdlets don't take the service principal object ID.</span></span> <span data-ttu-id="6664d-160">これらは、作成時に生成され、関連付けられているアプリケーション ID を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6664d-160">They take the associated application ID, which is generated at creation time.</span></span> <span data-ttu-id="6664d-161">サービス プリンシパルのアプリケーション ID を取得するには、`Get-AzADServicePrincipal` を使用します。</span><span class="sxs-lookup"><span data-stu-id="6664d-161">To get the application ID for a service principal, use `Get-AzADServicePrincipal`.</span></span>

> [!NOTE]
> <span data-ttu-id="6664d-162">ロールを割り当てるためのアクセス許可がアカウントにない場合は、アカウントに "'Microsoft.Authorization/roleAssignments/write' のアクションを実行するためのアクセス権限がありません" というエラー メッセージが表示されます。ロールを管理するには、Azure Active Directory 管理者にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="6664d-162">If your account doesn't have permission to assign a role, you see an error message that your account "does not have authorization to perform action 'Microsoft.Authorization/roleAssignments/write'." Contact your Azure Active Directory admin to manage roles.</span></span>

<span data-ttu-id="6664d-163">ロールを追加しても、以前に割り当てられたアクセス許可は制限され "_ません_"。</span><span class="sxs-lookup"><span data-stu-id="6664d-163">Adding a role _doesn't_ restrict previously assigned permissions.</span></span> <span data-ttu-id="6664d-164">サービス プリンシパルのアクセス許可を制限するときは、__共同作成者__ロールを削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6664d-164">When restricting a service principal's permissions, the __Contributor__ role should be removed.</span></span>

<span data-ttu-id="6664d-165">変更を確認するには、割り当てられているロールの一覧を表示します。</span><span class="sxs-lookup"><span data-stu-id="6664d-165">The changes can be verified by listing the assigned roles:</span></span>

```azurepowershell-interactive
Get-AzRoleAssignment -ServicePrincipalName ServicePrincipalName
```

## <a name="sign-in-using-a-service-principal"></a><span data-ttu-id="6664d-166">サービス プリンシパルを使用したサインイン</span><span class="sxs-lookup"><span data-stu-id="6664d-166">Sign in using a service principal</span></span>

<span data-ttu-id="6664d-167">サインインして、新しいサービス プリンシパルの資格情報とアクセス許可をテストします。</span><span class="sxs-lookup"><span data-stu-id="6664d-167">Test the new service principal's credentials and permissions by signing in.</span></span> <span data-ttu-id="6664d-168">サービス プリンシパルでサインインするには、サービス プリンシパルに関連付けられている `applicationId` 値、およびサービス プリンシパルを作成したテナントが必要です。</span><span class="sxs-lookup"><span data-stu-id="6664d-168">To sign in with a service principal, you need the `applicationId` value associated with it, and the tenant it was created under.</span></span>

<span data-ttu-id="6664d-169">パスワードを使用してサービス プリンシパルでサインインするには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="6664d-169">To sign in with a service principal using a password:</span></span>

```azurepowershell-interactive
# Use the application ID as the username, and the secret as password
$credentials = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $credentials -Tenant <tenant ID> 
```

<span data-ttu-id="6664d-170">証明書ベースの認証では、Azure PowerShell で、証明書の拇印に基づいてローカル証明書ストアから情報を取得できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="6664d-170">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -TenantId $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="6664d-171">PowerShell がアクセスできる資格情報ストアに証明書をインポートする手順については、「[Sign in with Azure PowerShell (Azure PowerShell を使用してサインインする)](authenticate-azureps.md#sp-signin)」を参照してください</span><span class="sxs-lookup"><span data-stu-id="6664d-171">For instructions on importing a certificate into a credential store accessible by PowerShell, see [Sign in with Azure PowerShell](authenticate-azureps.md#sp-signin)</span></span>

## <a name="reset-credentials"></a><span data-ttu-id="6664d-172">資格情報をリセットする</span><span class="sxs-lookup"><span data-stu-id="6664d-172">Reset credentials</span></span>

<span data-ttu-id="6664d-173">サービス プリンシパルの資格情報を忘れた場合は、[New-AzADSpCredential](/module/az.resources/new-azadspcredential) を使用して新しい資格情報を追加します。</span><span class="sxs-lookup"><span data-stu-id="6664d-173">If you forget the credentials for a service principal, use [New-AzADSpCredential](/module/az.resources/new-azadspcredential) to add a new credential.</span></span> <span data-ttu-id="6664d-174">このコマンドレットは、`New-AzADServicePrincipal` と同じ資格情報の引数と型を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="6664d-174">This cmdlet takes the same credential arguments and types as `New-AzADServicePrincipal`.</span></span> <span data-ttu-id="6664d-175">資格情報の引数を指定しない場合、ランダムなパスワードを持つ新しい `PasswordCredential` が作成されます。</span><span class="sxs-lookup"><span data-stu-id="6664d-175">Without any credential arguments, a new `PasswordCredential` with a random password is created.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="6664d-176">新しい資格情報を割り当てる前に、既存の資格情報を使用したサインインを防ぐために、既存の資格情報を削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6664d-176">Before assigning any new credentials, you may want to remove existing credentials to prevent sign in with them.</span></span> <span data-ttu-id="6664d-177">これを行うには、[Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="6664d-177">To do so, use the [Remove-AzADSpCredential](/powershell/module/az.resources/remove-azadspcredential) cmdlet:</span></span>
>
> ```azurepowershell-interactive
> Remove-AzADSpCredential -DisplayName ServicePrincipalName
> ```

```azurepowershell-interactive
$newCredential = New-AzADSpCredential -ServicePrincipalName ServicePrincipalName
```
