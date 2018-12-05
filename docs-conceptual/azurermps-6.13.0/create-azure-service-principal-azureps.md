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
ms.sourcegitcommit: 558436c824d9b59731aa9b963cdc8df4dea932e7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "52587807"
---
# <a name="create-an-azure-service-principal-with-azure-powershell"></a><span data-ttu-id="4293d-104">Azure PowerShell で Azure サービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="4293d-104">Create an Azure service principal with Azure PowerShell</span></span>

<span data-ttu-id="4293d-105">Azure PowerShell を使ってアプリまたはサービスを管理する場合、その実行には、自分の資格情報ではなく、Azure Active Directory (AAD) のサービス プリンシパルを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4293d-105">If you plan to manage your app or service with Azure PowerShell, you should run it under an Azure Active Directory (AAD) service principal, rather than your own credentials.</span></span> <span data-ttu-id="4293d-106">この記事では、Azure PowerShell でセキュリティ プリンシパルを作成する手順を紹介します。</span><span class="sxs-lookup"><span data-stu-id="4293d-106">This article steps you through creating a security principal with Azure PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="4293d-107">Azure Portal からサービス プリンシパルを作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="4293d-107">You can also create a service principal through the Azure portal.</span></span> <span data-ttu-id="4293d-108">詳細については、「[リソースにアクセスできる Azure Active Directory アプリケーションとサービス プリンシパルをポータルで作成する](/azure/azure-resource-manager/resource-group-create-service-principal-portal)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4293d-108">Read [Use portal to create Active Directory application and service principal that can access resources](/azure/azure-resource-manager/resource-group-create-service-principal-portal) for more details.</span></span>

## <a name="what-is-a-service-principal"></a><span data-ttu-id="4293d-109">"サービス プリンシパル" とは</span><span class="sxs-lookup"><span data-stu-id="4293d-109">What is a 'service principal'?</span></span>

<span data-ttu-id="4293d-110">Azure サービス プリンシパルは、ユーザーによって作成されたアプリやサービス、オートメーション ツールが特定の Azure リソースにアクセスする際に使うセキュリティ ID です。</span><span class="sxs-lookup"><span data-stu-id="4293d-110">An Azure service principal is a security identity used by user-created apps, services, and automation tools to access specific Azure resources.</span></span> <span data-ttu-id="4293d-111">アクセス許可が厳しく管理された、特定のロールが与えられた "ユーザー ID" (ユーザー名とパスワードまたは証明書) と考えてください。</span><span class="sxs-lookup"><span data-stu-id="4293d-111">Think of it as a 'user identity' (username and password or certificate) with a specific role, and tightly controlled permissions.</span></span> <span data-ttu-id="4293d-112">一般的なユーザー ID とは異なり、サービス プリンシパルで行うタスクは制限する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4293d-112">A service principal should only need to do specific things, unlike a general user identity.</span></span> <span data-ttu-id="4293d-113">管理タスクを実行するために必要な最小限のアクセス許可レベルだけを与えるようにすれば、セキュリティは向上します。</span><span class="sxs-lookup"><span data-stu-id="4293d-113">It improves security if you only grant it the minimum permissions level needed to perform its management tasks.</span></span>

## <a name="verify-your-own-permission-level"></a><span data-ttu-id="4293d-114">自分のアクセス許可レベルの確認</span><span class="sxs-lookup"><span data-stu-id="4293d-114">Verify your own permission level</span></span>

<span data-ttu-id="4293d-115">まず、Azure Active Directory と Azure サブスクリプションの両方で適切なアクセス許可を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4293d-115">First, you must have sufficient permissions in both your Azure Active Directory and your Azure subscription.</span></span> <span data-ttu-id="4293d-116">Active Directory でアプリを作成し、サービス プリンシパルにロールを割り当てることができる必要があります。</span><span class="sxs-lookup"><span data-stu-id="4293d-116">You must be able to create an app in the Active Directory and assign a role to the service principal.</span></span>

<span data-ttu-id="4293d-117">自分のアカウントに適切なアクセス許可があるかどうかを確認する最も簡単な方法は、ポータルを使用することです。</span><span class="sxs-lookup"><span data-stu-id="4293d-117">The easiest way to check whether your account has the right permissions is through the portal.</span></span> <span data-ttu-id="4293d-118">[ポータルでの必要なアクセス許可のチェック](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4293d-118">See [Check required permission in portal](/azure/azure-resource-manager/resource-group-create-service-principal-portal#required-permissions).</span></span>

## <a name="create-a-service-principal-for-your-app"></a><span data-ttu-id="4293d-119">アプリのサービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="4293d-119">Create a service principal for your app</span></span>

<span data-ttu-id="4293d-120">サービス プリンシパルは、Azure アカウントへのサインイン後に作成することができます。</span><span class="sxs-lookup"><span data-stu-id="4293d-120">Once signed in to your Azure account, you can create the service principal.</span></span> <span data-ttu-id="4293d-121">デプロイされているアプリを識別する手段が必要です。次のいずれかの方法があります。</span><span class="sxs-lookup"><span data-stu-id="4293d-121">You must have one of the following ways to identify your deployed app:</span></span>

* <span data-ttu-id="4293d-122">デプロイされているアプリの一意の名前 (次の例の "MyDemoWebApp" など)</span><span class="sxs-lookup"><span data-stu-id="4293d-122">The unique name of your deployed app, such as "MyDemoWebApp" in the following examples, or</span></span>
* <span data-ttu-id="4293d-123">アプリケーション ID (デプロイされているアプリやサービス、オブジェクトに関連付けられている一意の GUID)</span><span class="sxs-lookup"><span data-stu-id="4293d-123">the Application ID, the unique GUID associated with your deployed app, service, or object</span></span>

### <a name="get-information-about-your-application"></a><span data-ttu-id="4293d-124">アプリケーションに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="4293d-124">Get information about your application</span></span>

<span data-ttu-id="4293d-125">アプリケーションに関する情報は、`Get-AzureRmADApplication` コマンドレットを使って取得できます。</span><span class="sxs-lookup"><span data-stu-id="4293d-125">The `Get-AzureRmADApplication` cmdlet can be used to get information about your application.</span></span>

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

### <a name="create-a-service-principal-for-your-application"></a><span data-ttu-id="4293d-126">アプリケーションのサービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="4293d-126">Create a service principal for your application</span></span>

<span data-ttu-id="4293d-127">サービス プリンシパルは、`New-AzureRmADServicePrincipal` コマンドレットを使って作成します。</span><span class="sxs-lookup"><span data-stu-id="4293d-127">The `New-AzureRmADServicePrincipal` cmdlet is used to create the service principal.</span></span>

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

<span data-ttu-id="4293d-128">ここから、Connect-AzureRmAccount で $servicePrincipal.Secret プロパティを直接使用する (次の「サービス プリンシパルを使ってサインインする」を参照) か、後で使用できるようにこの SecureString をプレーンテキストに変換することができます。</span><span class="sxs-lookup"><span data-stu-id="4293d-128">From here, you can either directly use the $servicePrincipal.Secret property in Connect-AzureRmAccount (see "Sign in using the service principal" below), or you can convert this SecureString to a plain text string for later usage:</span></span>

```azurepowershell-interactive
$BSTR = [System.Runtime.InteropServices.Marshal]::SecureStringToBSTR($servicePrincipal.Secret)
$password = [System.Runtime.InteropServices.Marshal]::PtrToStringAuto($BSTR)
[Runtime.InteropServices.Marshal]::ZeroFreeBSTR($BSTR)
```

### <a name="sign-in-using-the-service-principal"></a><span data-ttu-id="4293d-129">サービス プリンシパルを使ってサインインする</span><span class="sxs-lookup"><span data-stu-id="4293d-129">Sign in using the service principal</span></span>

<span data-ttu-id="4293d-130">指定した "*アプリ ID*" と自動生成された "*パスワード*" を使って、アプリの新しいサービス プリンシパルとしてサインインできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="4293d-130">You can now sign in as the new service principal for your app using the *appId* you provided and *password* that was automatically generated.</span></span> <span data-ttu-id="4293d-131">サービス プリンシパルのテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="4293d-131">You also need the Tenant ID for the service principal.</span></span> <span data-ttu-id="4293d-132">テナント ID は、個人用の資格情報で Azure にサインインすると表示されます。</span><span class="sxs-lookup"><span data-stu-id="4293d-132">Your Tenant ID is displayed when you sign into Azure with your personal credentials.</span></span> <span data-ttu-id="4293d-133">サービス プリンシパルを使用してサインインするには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="4293d-133">To sign in with a service principal, use the following commands:</span></span>

```azurepowershell-interactive
$cred = New-Object System.Management.Automation.PSCredential ("00c01aaa-1603-49fc-b6df-b78c4e5138b4", $servicePrincipal.Secret)
Connect-AzureRmAccount -Credential $cred -ServicePrincipal -TenantId XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
```

<span data-ttu-id="4293d-134">サインインに成功すると、次のような出力が表示されます。</span><span class="sxs-lookup"><span data-stu-id="4293d-134">After a successful sign-in you see output like:</span></span>

```output
Environment           : AzureCloud
Account               : 00c01aaa-1603-49fc-b6df-b78c4e5138b4
TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
SubscriptionId        :
SubscriptionName      :
CurrentStorageAccount :
```

<span data-ttu-id="4293d-135">お疲れさまでした。</span><span class="sxs-lookup"><span data-stu-id="4293d-135">Congratulations!</span></span> <span data-ttu-id="4293d-136">これらの資格情報を使ってアプリを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="4293d-136">You can use these credentials to run your app.</span></span> <span data-ttu-id="4293d-137">次に、サービス プリンシパルのアクセス許可を調整する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4293d-137">Next, you need to adjust the permissions of the service principal.</span></span>

## <a name="managing-roles"></a><span data-ttu-id="4293d-138">ロールの管理</span><span class="sxs-lookup"><span data-stu-id="4293d-138">Managing roles</span></span>

> [!NOTE]
> <span data-ttu-id="4293d-139">Azure のロールベースのアクセス制御 (RBAC) は、ユーザー プリンシパルとサービス プリンシパルのロールを定義して管理するためのモデルです。</span><span class="sxs-lookup"><span data-stu-id="4293d-139">Azure Role-Based Access Control (RBAC) is a model for defining and managing roles for user and service principals.</span></span> <span data-ttu-id="4293d-140">ロールに関連付けられる一連のアクセス許可によって、プリンシパルが各種の操作 (読み取り、アクセス、書き込み、または管理) を実行できるリソースが決まります。</span><span class="sxs-lookup"><span data-stu-id="4293d-140">Roles have sets of permissions associated with them, which determine the resources a principal can read, access, write, or manage.</span></span> <span data-ttu-id="4293d-141">RBAC とロールについて詳しくは、[RBAC のための組み込みロール](/azure/active-directory/role-based-access-built-in-roles)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4293d-141">For more information on RBAC and roles, see [RBAC: Built-in roles](/azure/active-directory/role-based-access-built-in-roles).</span></span>

<span data-ttu-id="4293d-142">Azure PowerShell には、ロールの割り当て管理を目的とした次のコマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="4293d-142">Azure PowerShell provides the following cmdlets to manage role assignments:</span></span>

* [<span data-ttu-id="4293d-143">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4293d-143">Get-AzureRmRoleAssignment</span></span>](/powershell/module/azurerm.resources/get-azurermroleassignment)
* [<span data-ttu-id="4293d-144">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4293d-144">New-AzureRmRoleAssignment</span></span>](/powershell/module/azurerm.resources/new-azurermroleassignment)
* [<span data-ttu-id="4293d-145">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4293d-145">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/azurerm.resources/remove-azurermroleassignment)

<span data-ttu-id="4293d-146">サービス プリンシパルの既定のロールは**共同作成者**です。</span><span class="sxs-lookup"><span data-stu-id="4293d-146">The default role for a service principal is **Contributor**.</span></span> <span data-ttu-id="4293d-147">このロールは、広範なアクセス許可が与えられていることから、Azure サービスに対するアプリの対話の範囲によっては最適とは言えない場合もあります。</span><span class="sxs-lookup"><span data-stu-id="4293d-147">It may not be the best choice depending on the scope of your app's interactions with Azure services, given its broad permissions.</span></span>
<span data-ttu-id="4293d-148">読み取り専用のアプリであれば、より制限の厳しい**閲覧者**ロールの方が適しています。</span><span class="sxs-lookup"><span data-stu-id="4293d-148">The **Reader** role is more restrictive and can be a good choice for read-only apps.</span></span> <span data-ttu-id="4293d-149">Azure Portal でロールごとのアクセス許可について詳しい情報を確認したり、カスタム ロールを作成したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="4293d-149">You can view details on role-specific permissions or create custom ones through the Azure portal.</span></span>

<span data-ttu-id="4293d-150">この例では、先ほどの例に**閲覧者**ロールを追加し、**共同作成者**ロールを削除しています。</span><span class="sxs-lookup"><span data-stu-id="4293d-150">In this example, we add the **Reader** role to our prior example, and delete the **Contributor** one:</span></span>

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

<span data-ttu-id="4293d-151">現在割り当てられているロールを表示するには、次のコマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="4293d-151">To view the current roles assigned:</span></span>

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

<span data-ttu-id="4293d-152">その他、ロールの管理を目的として次の Azure PowerShell コマンドレットが用意されています。</span><span class="sxs-lookup"><span data-stu-id="4293d-152">Other Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="4293d-153">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4293d-153">Get-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="4293d-154">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4293d-154">New-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="4293d-155">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4293d-155">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="4293d-156">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="4293d-156">Set-AzureRmRoleDefinition</span></span>](/powershell/module/azurerm.resources/Set-AzureRmRoleDefinition)

## <a name="change-the-credentials-of-the-security-principal"></a><span data-ttu-id="4293d-157">セキュリティ プリンシパルの資格情報を変更する</span><span class="sxs-lookup"><span data-stu-id="4293d-157">Change the credentials of the security principal</span></span>

<span data-ttu-id="4293d-158">セキュリティ上、アクセス許可の確認とパスワードの更新を定期的に行うことが大切です。</span><span class="sxs-lookup"><span data-stu-id="4293d-158">It's a good security practice to review the permissions and update the password regularly.</span></span> <span data-ttu-id="4293d-159">必要に応じて、アプリの変更に合わせてセキュリティ資格情報を適宜更新することもできます。</span><span class="sxs-lookup"><span data-stu-id="4293d-159">You may also want to manage and modify the security credentials as your app changes.</span></span> <span data-ttu-id="4293d-160">たとえばサービス プリンシパルのパスワードは、新しいパスワードを作成して古いパスワードを削除することで変更できます。</span><span class="sxs-lookup"><span data-stu-id="4293d-160">For example, we can change the password of the service principal by creating a new password and removing the old one.</span></span>

### <a name="add-a-new-password-for-the-service-principal"></a><span data-ttu-id="4293d-161">サービス プリンシパルの新しいパスワードを追加する</span><span class="sxs-lookup"><span data-stu-id="4293d-161">Add a new password for the service principal</span></span>

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

### <a name="get-a-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="4293d-162">サービス プリンシパルの一連の資格情報を取得する</span><span class="sxs-lookup"><span data-stu-id="4293d-162">Get a list of credentials for the service principal</span></span>

```azurepowershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
5/5/2016 4:55:27 PM 5/5/2017 4:55:27 PM ca9d4846-4972-4c70-b6f5-a4effa60b9bc Password
```

### <a name="remove-the-old-password-from-the-service-principal"></a><span data-ttu-id="4293d-163">サービス プリンシパルから古いパスワードを削除する</span><span class="sxs-lookup"><span data-stu-id="4293d-163">Remove the old password from the service principal</span></span>

```azurepowershell-interactive
Remove-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp -KeyId ca9d4846-4972-4c70-b6f5-a4effa60b9bc
```

```output
Confirm
Are you sure you want to remove credential with keyId '6f801c3e-6fcd-42b9-be8e-320b17ba1d36' for
service principal objectId '698138e7-d7b6-4738-a866-b4e3081a69e4'.
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

### <a name="verify-the-list-of-credentials-for-the-service-principal"></a><span data-ttu-id="4293d-164">サービス プリンシパルの一連の資格情報を確認する</span><span class="sxs-lookup"><span data-stu-id="4293d-164">Verify the list of credentials for the service principal</span></span>

```azurepowershell-interactive
Get-AzureRmADSpCredential -ServicePrincipalName http://MyDemoWebApp
```

```output
StartDate           EndDate             KeyId                                Type
---------           -------             -----                                ----
3/8/2017 5:58:24 PM 3/8/2018 5:58:24 PM 6f801c3e-6fcd-42b9-be8e-320b17ba1d36 Password
```

### <a name="get-information-about-the-service-principal"></a><span data-ttu-id="4293d-165">サービス プリンシパルに関する情報を取得する</span><span class="sxs-lookup"><span data-stu-id="4293d-165">Get information about the service principal</span></span>

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
