---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 80c59a10666c6e3a01e6c33716fce40094fb14be
ms.sourcegitcommit: c6fd0e490fa0e33b8b768b679682a47d8faae1cf
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/16/2019
ms.locfileid: "54342067"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="25b0a-103">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="25b0a-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="25b0a-104">Azure PowerShell では、複数の認証方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="25b0a-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="25b0a-105">[Azure Cloud Shell](/azure/cloud-shell/overview) を使用すると自動的にログインできるため、最も簡単に作業を開始できます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="25b0a-106">ローカル インストールを利用すると、ブラウザーから対話形式でサインインできます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="25b0a-107">自動化のスクリプトを記述するとき、必要なアクセス許可で[サービス プリンシパル](create-azure-service-principal-azureps.md)を使用する方法が推奨されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="25b0a-108">ユース ケースに対して可能な限りサインイン アクセス許可を制限することで、Azure リソースのセキュリティを維持できます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="25b0a-109">サインイン後、コマンドが既定のサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="25b0a-110">セッションのアクティブ サブスクリプションを変更するには、[Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="25b0a-111">Azure PowerShell でログインするときに使用される既定のサブスクリプションを変更するには、[Set-AzDefault](/powershell/module/az.accounts/set-azdefault) を使用します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="25b0a-112">サインインしたままであれば、資格情報は複数の PowerShell セッション間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="25b0a-113">詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25b0a-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="25b0a-114">対話操作でサインインする</span><span class="sxs-lookup"><span data-stu-id="25b0a-114">Sign in interactively</span></span>

<span data-ttu-id="25b0a-115">対話形式でサインインするには、[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="25b0a-116">このコマンドレットを実行すると、トークン文字列が表示されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="25b0a-117">サインインするには、この文字列をコピーし、ブラウザーの https://microsoft.com/devicelogin に貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="25b0a-118">Azure に接続するために PowerShell セッションが認証されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

## <a name="sign-in-with-credentials"></a><span data-ttu-id="25b0a-119">資格情報でサインインする</span><span class="sxs-lookup"><span data-stu-id="25b0a-119">Sign in with credentials</span></span>

<span data-ttu-id="25b0a-120">Azure への接続が認められた `PSCredential` オブジェクトでサインインすることもできます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-120">You can also sign in with a `PSCredential` object authorized to connect to Azure.</span></span>
<span data-ttu-id="25b0a-121">資格情報オブジェクトを取得する最も簡単な方法は [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential) コマンドレットを使用することです。</span><span class="sxs-lookup"><span data-stu-id="25b0a-121">The easiest way to get a credential object is with the [Get-Credential](/powershell/module/Microsoft.PowerShell.Security/Get-Credential) cmdlet.</span></span> <span data-ttu-id="25b0a-122">このコマンドレットを実行すると、ユーザー名/パスワードの資格情報ペアが求められます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-122">When run, this cmdlet will prompt you for a username/password credential pair.</span></span>

> [!Note]
> <span data-ttu-id="25b0a-123">この方法は、Microsoft アカウント、または 2 要素認証が有効になっているアカウントでは機能しません。</span><span class="sxs-lookup"><span data-stu-id="25b0a-123">This approach doesn't work with Microsoft accounts or accounts that have two-factor authentication enabled.</span></span>

```azurepowershell-interactive
$creds = Get-Credential
Connect-AzAccount -Credential $creds
```

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="25b0a-124">サービス プリンシパルを使ってサインインする</span><span class="sxs-lookup"><span data-stu-id="25b0a-124">Sign in with a service principal</span></span>

<span data-ttu-id="25b0a-125">サービス プリンシパルは、非対話型の Azure アカウントです。</span><span class="sxs-lookup"><span data-stu-id="25b0a-125">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="25b0a-126">他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-126">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="25b0a-127">サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-127">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="25b0a-128">Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25b0a-128">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="25b0a-129">サービス プリンシパルを使用してサインインするには、`Connect-AzAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-129">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="25b0a-130">サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="25b0a-130">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="25b0a-131">サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-131">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="25b0a-132">このコマンドレットでは、サービス プリンシパルのユーザー ID とパスワードの入力を求められます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-132">This cmdlet will present a prompt for the service principal user ID and password.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="25b0a-133">マネージド ID を使用したサインイン</span><span class="sxs-lookup"><span data-stu-id="25b0a-133">Sign in using a managed identity</span></span> 

<span data-ttu-id="25b0a-134">マネージド ID は Azure Active Directory の機能です。</span><span class="sxs-lookup"><span data-stu-id="25b0a-134">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="25b0a-135">マネージド ID は、Azure で実行されるリソースに割り当てられたサービス プリンシパルです。</span><span class="sxs-lookup"><span data-stu-id="25b0a-135">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="25b0a-136">サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-136">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="25b0a-137">マネージド ID は、Azure クラウドで実行されているリソースでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-137">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="25b0a-138">Azure リソースのマネージド ID の詳細については、「[Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="25b0a-138">To learn more about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="25b0a-139">既定ではないテナントで、あるいはクラウド ソリューション プロバイダー (CSP) としてサインインする</span><span class="sxs-lookup"><span data-stu-id="25b0a-139">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="25b0a-140">アカウントが複数のテナントに関連付けられている場合、接続時に `-TenantId` パラメーターを使用することがサインインで要求されます。</span><span class="sxs-lookup"><span data-stu-id="25b0a-140">If your account is associated with more than one tenant, sign-in requires the use of the `-TenantId` parameter when connecting.</span></span> <span data-ttu-id="25b0a-141">このパラメーターは他のあらゆるサインイン メソッドで動作します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-141">This parameter will work with any other sign-in method.</span></span> <span data-ttu-id="25b0a-142">ログイン時、テナントの Azure オブジェクト ID (テナント ID) またはテナントの完全修飾ドメイン名がこのパラメーター値になります。</span><span class="sxs-lookup"><span data-stu-id="25b0a-142">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="25b0a-143">[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) の場合、`-TenantId` 値はテナント ID にすることが**必要**となります。</span><span class="sxs-lookup"><span data-stu-id="25b0a-143">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), the `-TenantId` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="25b0a-144">別のクラウドにサインインする</span><span class="sxs-lookup"><span data-stu-id="25b0a-144">Sign in to another Cloud</span></span>

<span data-ttu-id="25b0a-145">Azure クラウド サービスでは、リージョンのデータ処理の法律に準拠した環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-145">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="25b0a-146">リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-146">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="25b0a-147">たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-147">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="25b0a-148">次のコマンドでは、使用可能な環境の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="25b0a-148">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```