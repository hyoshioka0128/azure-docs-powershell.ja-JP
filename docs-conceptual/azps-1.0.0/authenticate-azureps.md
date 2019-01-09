---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 8b085720aeabe26c1293ece193e050b31f99a693
ms.sourcegitcommit: ae81b08a45d8729fc8d40156422e3eb2e94de8c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/27/2018
ms.locfileid: "53786681"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="bf97c-103">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="bf97c-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="bf97c-104">Azure PowerShell では、複数の認証方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="bf97c-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="bf97c-105">最も簡単に始められるのは、コマンド ラインから対話形式でサインインする方法です。</span><span class="sxs-lookup"><span data-stu-id="bf97c-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="bf97c-106">対話操作でサインインする</span><span class="sxs-lookup"><span data-stu-id="bf97c-106">Sign in interactively</span></span>

<span data-ttu-id="bf97c-107">対話形式でサインインするには、[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-107">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="bf97c-108">このコマンドレットを実行すると、トークン文字列が表示されます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-108">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="bf97c-109">ログインするには、この文字列をコピーし、ブラウザーの https://microsoft.com/devicelogin に貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-109">To log in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="bf97c-110">Azure に接続するために PowerShell セッションが認証されます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-110">Your PowerShell session will then be authenticated to connect to Azure.</span></span> <span data-ttu-id="bf97c-111">この認証は、現在の PowerShell セッションが終了するまで有効です。</span><span class="sxs-lookup"><span data-stu-id="bf97c-111">This authentication lasts for the current PowerShell session.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="bf97c-112">サインインしたままであれば、資格情報は複数の PowerShell セッション間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="bf97c-113">詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf97c-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="bf97c-114">サービス プリンシパルを使ってサインインする</span><span class="sxs-lookup"><span data-stu-id="bf97c-114">Sign in with a service principal</span></span>

<span data-ttu-id="bf97c-115">サービス プリンシパルは、非対話型の Azure アカウントです。</span><span class="sxs-lookup"><span data-stu-id="bf97c-115">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="bf97c-116">他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-116">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="bf97c-117">サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-117">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="bf97c-118">Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf97c-118">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="bf97c-119">サービス プリンシパルを使用してサインインするには、`Connect-AzAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-119">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="bf97c-120">サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="bf97c-120">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="bf97c-121">サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-121">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="bf97c-122">このコマンドレットでは、サービス プリンシパルのユーザー ID とパスワードの入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-122">This cmdlet will present a prompt for the service principal user ID and password.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a><span data-ttu-id="bf97c-123">Azure マネージド サービス ID を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="bf97c-123">Sign in using an Azure Managed Service Identity</span></span>

<span data-ttu-id="bf97c-124">Azure リソースのマネージドID は、Azure Active Directory の機能です。</span><span class="sxs-lookup"><span data-stu-id="bf97c-124">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="bf97c-125">サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-125">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="bf97c-126">マネージド ID は、Azure クラウドで実行されている仮想マシンでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-126">Managed identities are only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="bf97c-127">Azure リソースのマネージド ID の詳細については、「[How to use managed identities for Azure resources on an Azure VM to acquire an access token (Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法)](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf97c-127">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="bf97c-128">クラウド ソリューション プロバイダー (CSP) としてサインインする</span><span class="sxs-lookup"><span data-stu-id="bf97c-128">Sign in as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="bf97c-129">[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) のサインインには、`-TenantId` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf97c-129">A [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) sign-in requires the use of `-TenantId`.</span></span> <span data-ttu-id="bf97c-130">通常は、このパラメーターにはテナント ID またはドメイン名を指定できます。</span><span class="sxs-lookup"><span data-stu-id="bf97c-130">Normally, this parameter can be provided as either a tenant ID or a domain name.</span></span> <span data-ttu-id="bf97c-131">しかし、CSP のサインインの場合、**テナント ID** を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="bf97c-131">However, for CSP sign-in, it must be provided a **tenant ID**.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="bf97c-132">別のクラウドにサインインする</span><span class="sxs-lookup"><span data-stu-id="bf97c-132">Sign in to another Cloud</span></span>

<span data-ttu-id="bf97c-133">Azure クラウド サービスでは、リージョンのデータ処理規制に準拠した環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-133">Azure cloud services offer environments compliant with regional data-handling regulations.</span></span>
<span data-ttu-id="bf97c-134">リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-134">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="bf97c-135">たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-135">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="bf97c-136">次のコマンドでは、使用可能な環境の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="bf97c-136">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="bf97c-137">Azure ロールベース アクセスの管理についての詳細情報</span><span class="sxs-lookup"><span data-stu-id="bf97c-137">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="bf97c-138">Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bf97c-138">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="bf97c-139">ロール管理を目的とした Azure PowerShell のコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="bf97c-139">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="bf97c-140">Get-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bf97c-140">Get-AzRoleAssignment</span></span>](/powershell/module/az.Resources/Get-azRoleAssignment)
* [<span data-ttu-id="bf97c-141">Get-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bf97c-141">Get-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Get-azRoleDefinition)
* [<span data-ttu-id="bf97c-142">New-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bf97c-142">New-AzRoleAssignment</span></span>](/powershell/module/az.Resources/New-azRoleAssignment)
* [<span data-ttu-id="bf97c-143">New-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bf97c-143">New-AzRoleDefinition</span></span>](/powershell/module/az.Resources/New-azRoleDefinition)
* [<span data-ttu-id="bf97c-144">Remove-AzRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bf97c-144">Remove-AzRoleAssignment</span></span>](/powershell/module/az.Resources/Remove-azRoleAssignment)
* [<span data-ttu-id="bf97c-145">Remove-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bf97c-145">Remove-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Remove-azRoleDefinition)
* [<span data-ttu-id="bf97c-146">Set-AzRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="bf97c-146">Set-AzRoleDefinition</span></span>](/powershell/module/az.Resources/Set-azRoleDefinition)
