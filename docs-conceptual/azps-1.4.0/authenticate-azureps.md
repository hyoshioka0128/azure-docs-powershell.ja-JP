---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/20/2019
ms.openlocfilehash: 897bc20721305c03a0545bc236fa91292861ef1e
ms.sourcegitcommit: 18de3041f9084f60424ccbd1d004da761277a304
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/01/2019
ms.locfileid: "57016471"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="f2219-103">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="f2219-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="f2219-104">Azure PowerShell では、複数の認証方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="f2219-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="f2219-105">[Azure Cloud Shell](/azure/cloud-shell/overview) を使用すると自動的にログインできるため、最も簡単に作業を開始できます。</span><span class="sxs-lookup"><span data-stu-id="f2219-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="f2219-106">ローカル インストールを利用すると、ブラウザーから対話形式でサインインできます。</span><span class="sxs-lookup"><span data-stu-id="f2219-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="f2219-107">自動化のスクリプトを記述するとき、必要なアクセス許可で[サービス プリンシパル](create-azure-service-principal-azureps.md)を使用する方法が推奨されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="f2219-108">ユース ケースに対して可能な限りサインイン アクセス許可を制限することで、Azure リソースのセキュリティを維持できます。</span><span class="sxs-lookup"><span data-stu-id="f2219-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="f2219-109">サインイン後、コマンドが既定のサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="f2219-110">セッションのアクティブ サブスクリプションを変更するには、[Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="f2219-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="f2219-111">Azure PowerShell でログインするときに使用される既定のサブスクリプションを変更するには、[Set-AzDefault](/powershell/module/az.accounts/set-azdefault) を使用します。</span><span class="sxs-lookup"><span data-stu-id="f2219-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="f2219-112">サインインしたままであれば、資格情報は複数の PowerShell セッション間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="f2219-113">詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2219-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="f2219-114">対話操作でサインインする</span><span class="sxs-lookup"><span data-stu-id="f2219-114">Sign in interactively</span></span>

<span data-ttu-id="f2219-115">対話形式でサインインするには、[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="f2219-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="f2219-116">このコマンドレットを実行すると、トークン文字列が表示されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="f2219-117">サインインするには、この文字列をコピーし、ブラウザーの https://microsoft.com/devicelogin に貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="f2219-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="f2219-118">Azure に接続するために PowerShell セッションが認証されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="f2219-119">ユーザー名とパスワードの資格情報による承認は、Active Directory 認証の実装の変更とセキュリティ上の懸念から、Azure PowerShell では削除されました。</span><span class="sxs-lookup"><span data-stu-id="f2219-119">Username/password credential authorization has been removed in Azure PowerShell due to changes in Active Directory authorization implementations and security concerns.</span></span>
> <span data-ttu-id="f2219-120">資格情報による承認を使用して自動化を行う場合は、代わりに[サービス プリンシパルを作成](create-azure-service-principal-azureps.md)してください。</span><span class="sxs-lookup"><span data-stu-id="f2219-120">If you use credential authorization for automation purposes, instead [create a service principal](create-azure-service-principal-azureps.md).</span></span>

## <a name="sign-in-with-a-service-principal-a-namesp-signin"></a><span data-ttu-id="f2219-121">サービス プリンシパルを使用してサインインする <a name="sp-signin"/></span><span class="sxs-lookup"><span data-stu-id="f2219-121">Sign in with a service principal <a name="sp-signin"/></span></span>

<span data-ttu-id="f2219-122">サービス プリンシパルは、非対話型の Azure アカウントです。</span><span class="sxs-lookup"><span data-stu-id="f2219-122">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="f2219-123">他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-123">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="f2219-124">サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-124">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="f2219-125">Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2219-125">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="f2219-126">サービス プリンシパルを使用してサインインするには、`Connect-AzAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="f2219-126">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="f2219-127">サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="f2219-127">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="f2219-128">サービス プリンシパルを使用してサインインする方法は、パスワードベースの認証用と証明書ベースの認証用のどちらに構成されているかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="f2219-128">How you sign in with a service principal will depend on whether it's configured for password-based or certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="f2219-129">パスワードベースの認証</span><span class="sxs-lookup"><span data-stu-id="f2219-129">Password-based authentication</span></span>

<span data-ttu-id="f2219-130">サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="f2219-130">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="f2219-131">このコマンドレットによって、ユーザー名とパスワードの入力を求めるプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-131">This cmdlet will present a prompt for a username and password.</span></span> <span data-ttu-id="f2219-132">ユーザー名にはサービス プリンシパル ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="f2219-132">Use the service principal ID for the username.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $pscredential -TenantId $tenantId
```

<span data-ttu-id="f2219-133">自動化のシナリオでは、ユーザー名とセキュリティで保護された文字列から資格情報を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2219-133">For automation scenarios, you need to create credentials from a user name and secure string:</span></span>

```azurepowershell-interactive
$passwd = ConvertTo-SecureString <use a secure password here> -AsPlainText -Force
$pscredential = New-Object System.Management.Automation.PSCredential('service principal name/id', $passwd)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -TenantId $tenantId
```

<span data-ttu-id="f2219-134">サービス プリンシパルへの接続を自動化する場合は、必ず適切なパスワード保存プラクティスを使用してください。</span><span class="sxs-lookup"><span data-stu-id="f2219-134">Make sure that you use good password storage practices when automating service principal connections.</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="f2219-135">証明書ベースの認証</span><span class="sxs-lookup"><span data-stu-id="f2219-135">Certificate-based authentication</span></span>

<span data-ttu-id="f2219-136">証明書ベースの認証では、Azure PowerShell で、証明書の拇印に基づいてローカル証明書ストアから情報を取得できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2219-136">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>
```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -TenantId $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="f2219-137">PowerShell 5 では、[PKI](/powershell/module/pkiclient) モジュールを使用して、証明書ストアを管理および検査できます。</span><span class="sxs-lookup"><span data-stu-id="f2219-137">In PowerShell 5, the certificate store can be managed and inspected with the [PKI](/powershell/module/pkiclient) module.</span></span> <span data-ttu-id="f2219-138">PowerShell 6 の場合は、プロセスがさらに複雑になります。</span><span class="sxs-lookup"><span data-stu-id="f2219-138">For PowerShell 6, the process is more complicated.</span></span> <span data-ttu-id="f2219-139">次のスクリプトでは、PowerShell からアクセスできる証明書ストアに、既存の証明書をインポートする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="f2219-139">The following scripts show you how to import an existing certificate into the certificate store accessible by PowerShell.</span></span>

#### <a name="import-a-certificate-in-powershell-5"></a><span data-ttu-id="f2219-140">PowerShell 5 で証明書をインポートする</span><span class="sxs-lookup"><span data-stu-id="f2219-140">Import a certificate in PowerShell 5</span></span>

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-6"></a><span data-ttu-id="f2219-141">PowerShell 6 で証明書をインポートする</span><span class="sxs-lookup"><span data-stu-id="f2219-141">Import a certificate in PowerShell 6</span></span>

```azurepowershell-interactive
# Import a PFX
$storeName = [System.Security.Cryptography.X509Certificates.StoreName]::My 
$storeLocation = [System.Security.Cryptography.X509Certificates.StoreLocation]::CurrentUser 
$store = [System.Security.Cryptography.X509Certificates.X509Store]::new($storeName, $storeLocation) 
$certPath = <path to certificate>
$credentials = Get-Credential -Message "Provide PFX private key password"
$flag = [System.Security.Cryptography.X509Certificates.X509KeyStorageFlags]::Exportable 
$certificate = [System.Security.Cryptography.X509Certificates.X509Certificate2]::new($certPath, $credentials.Password, $flag) 
$store.Open([System.Security.Cryptography.X509Certificates.OpenFlags]::ReadWrite) 
$store.Add($Certificate) 
$store.Close()
```

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="f2219-142">マネージド ID を使用したサインイン</span><span class="sxs-lookup"><span data-stu-id="f2219-142">Sign in using a managed identity</span></span> 

<span data-ttu-id="f2219-143">マネージド ID は Azure Active Directory の機能です。</span><span class="sxs-lookup"><span data-stu-id="f2219-143">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="f2219-144">マネージド ID は、Azure で実行されるリソースに割り当てられたサービス プリンシパルです。</span><span class="sxs-lookup"><span data-stu-id="f2219-144">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="f2219-145">サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="f2219-145">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="f2219-146">マネージド ID は、Azure クラウドで実行されているリソースでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="f2219-146">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="f2219-147">Azure リソースのマネージド ID の詳細については、「[Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2219-147">To learn more about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="f2219-148">既定ではないテナントで、あるいはクラウド ソリューション プロバイダー (CSP) としてサインインする</span><span class="sxs-lookup"><span data-stu-id="f2219-148">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="f2219-149">アカウントが複数のテナントに関連付けられている場合、接続時に `-TenantId` パラメーターを使用することがサインインで要求されます。</span><span class="sxs-lookup"><span data-stu-id="f2219-149">If your account is associated with more than one tenant, sign-in requires the use of the `-TenantId` parameter when connecting.</span></span> <span data-ttu-id="f2219-150">このパラメーターは他のあらゆるサインイン メソッドで動作します。</span><span class="sxs-lookup"><span data-stu-id="f2219-150">This parameter will work with any other sign-in method.</span></span> <span data-ttu-id="f2219-151">ログイン時、テナントの Azure オブジェクト ID (テナント ID) またはテナントの完全修飾ドメイン名がこのパラメーター値になります。</span><span class="sxs-lookup"><span data-stu-id="f2219-151">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="f2219-152">[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) の場合、`-TenantId` 値はテナント ID にすることが**必要**となります。</span><span class="sxs-lookup"><span data-stu-id="f2219-152">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/), the `-TenantId` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="f2219-153">別のクラウドにサインインする</span><span class="sxs-lookup"><span data-stu-id="f2219-153">Sign in to another Cloud</span></span>

<span data-ttu-id="f2219-154">Azure クラウド サービスでは、リージョンのデータ処理の法律に準拠した環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="f2219-154">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="f2219-155">リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="f2219-155">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="f2219-156">たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。</span><span class="sxs-lookup"><span data-stu-id="f2219-156">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="f2219-157">次のコマンドでは、使用可能な環境の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f2219-157">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```
