---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/04/2019
ms.openlocfilehash: 44f5d5b44788a52db297a0d73697161eec2eedc2
ms.sourcegitcommit: 45e1823aa1a792840aa4829831b5f67a9d5d24a0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/26/2019
ms.locfileid: "74537350"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="11c1e-103">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="11c1e-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="11c1e-104">Azure PowerShell では、複数の認証方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="11c1e-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="11c1e-105">[Azure Cloud Shell](/azure/cloud-shell/overview) を使用すると自動的にログインできるため、最も簡単に作業を開始できます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-105">The easiest way to get started is with [Azure Cloud Shell](/azure/cloud-shell/overview), which automatically logs you in.</span></span> <span data-ttu-id="11c1e-106">ローカル インストールを利用すると、ブラウザーから対話形式でサインインできます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-106">With a local install, you can sign in interactively through your browser.</span></span> <span data-ttu-id="11c1e-107">自動化のスクリプトを記述するとき、必要なアクセス許可で[サービス プリンシパル](create-azure-service-principal-azureps.md)を使用する方法が推奨されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-107">When writing scripts for automation, the recommended approach is to use a [service principal](create-azure-service-principal-azureps.md) with the necessary permissions.</span></span> <span data-ttu-id="11c1e-108">ユース ケースに対して可能な限りサインイン アクセス許可を制限することで、Azure リソースのセキュリティを維持できます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-108">When you restrict sign-in permissions as much as possible for your use case, you help keep your Azure resources secure.</span></span>

<span data-ttu-id="11c1e-109">サインイン後、コマンドが既定のサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-109">After signing in, commands are run against your default subscription.</span></span> <span data-ttu-id="11c1e-110">セッションのアクティブ サブスクリプションを変更するには、[Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-110">To change your active subscription for a session, use the [Set-AzContext](/powershell/module/az.accounts/set-azcontext) cmdlet.</span></span> <span data-ttu-id="11c1e-111">Azure PowerShell でログインするときに使用される既定のサブスクリプションを変更するには、[Set-AzDefault](/powershell/module/az.accounts/set-azdefault) を使用します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-111">To change the default subscription used when logging in with Azure PowerShell, use [Set-AzDefault](/powershell/module/az.accounts/set-azdefault).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="11c1e-112">サインインしたままであれば、資格情報は複数の PowerShell セッション間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-112">Your credentials are shared among multiple PowerShell sessions as long as you remain signed in.</span></span>
> <span data-ttu-id="11c1e-113">詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11c1e-113">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="11c1e-114">対話操作でサインインする</span><span class="sxs-lookup"><span data-stu-id="11c1e-114">Sign in interactively</span></span>

<span data-ttu-id="11c1e-115">対話形式でサインインするには、[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-115">To sign in interactively, use the [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzAccount
```

<span data-ttu-id="11c1e-116">このコマンドレットを実行すると、トークン文字列が表示されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-116">When run, this cmdlet will present a token string.</span></span> <span data-ttu-id="11c1e-117">サインインするには、この文字列をコピーし、ブラウザーの https://microsoft.com/devicelogin に貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-117">To sign in, copy this string and paste it into https://microsoft.com/devicelogin in a browser.</span></span> <span data-ttu-id="11c1e-118">Azure に接続するために PowerShell セッションが認証されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-118">Your PowerShell session will be authenticated to connect to Azure.</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="11c1e-119">ユーザー名とパスワードの資格情報による承認は、Active Directory 認証の実装の変更とセキュリティ上の懸念から、Azure PowerShell では削除されました。</span><span class="sxs-lookup"><span data-stu-id="11c1e-119">Username/password credential authorization has been removed in Azure PowerShell due to changes in Active Directory authorization implementations and security concerns.</span></span>
> <span data-ttu-id="11c1e-120">資格情報による承認を使用して自動化を行う場合は、代わりに[サービス プリンシパルを作成](create-azure-service-principal-azureps.md)してください。</span><span class="sxs-lookup"><span data-stu-id="11c1e-120">If you use credential authorization for automation purposes, instead [create a service principal](create-azure-service-principal-azureps.md).</span></span>

## <a name="sign-in-with-a-service-principal-a-namesp-signin"></a><span data-ttu-id="11c1e-121">サービス プリンシパルを使用してサインインする <a name="sp-signin"/></span><span class="sxs-lookup"><span data-stu-id="11c1e-121">Sign in with a service principal <a name="sp-signin"/></span></span>

<span data-ttu-id="11c1e-122">サービス プリンシパルは、非対話型の Azure アカウントです。</span><span class="sxs-lookup"><span data-stu-id="11c1e-122">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="11c1e-123">他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-123">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="11c1e-124">サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-124">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="11c1e-125">Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11c1e-125">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="11c1e-126">サービス プリンシパルを使用してサインインするには、`Connect-AzAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-126">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzAccount` cmdlet.</span></span> <span data-ttu-id="11c1e-127">サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="11c1e-127">You'll also need the service principal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="11c1e-128">サービス プリンシパルを使用してサインインする方法は、パスワードベースの認証用と証明書ベースの認証用のどちらに構成されているかによって異なります。</span><span class="sxs-lookup"><span data-stu-id="11c1e-128">How you sign in with a service principal will depend on whether it's configured for password-based or certificate-based authentication.</span></span>

### <a name="password-based-authentication"></a><span data-ttu-id="11c1e-129">パスワードベースの認証</span><span class="sxs-lookup"><span data-stu-id="11c1e-129">Password-based authentication</span></span>

<span data-ttu-id="11c1e-130">サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-130">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="11c1e-131">このコマンドレットによって、ユーザー名とパスワードの入力を求めるプロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-131">This cmdlet will present a prompt for a username and password.</span></span> <span data-ttu-id="11c1e-132">ユーザー名にはサービス プリンシパル ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-132">Use the service principal ID for the username.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

<span data-ttu-id="11c1e-133">自動化のシナリオでは、ユーザー名とセキュリティで保護された文字列から資格情報を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="11c1e-133">For automation scenarios, you need to create credentials from a user name and secure string:</span></span>

```azurepowershell-interactive
$passwd = ConvertTo-SecureString <use a secure password here> -AsPlainText -Force
$pscredential = New-Object System.Management.Automation.PSCredential('service principal name/id', $passwd)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

<span data-ttu-id="11c1e-134">サービス プリンシパルへの接続を自動化する場合は、必ず適切なパスワード保存プラクティスを使用してください。</span><span class="sxs-lookup"><span data-stu-id="11c1e-134">Make sure that you use good password storage practices when automating service principal connections.</span></span>

### <a name="certificate-based-authentication"></a><span data-ttu-id="11c1e-135">証明書ベースの認証</span><span class="sxs-lookup"><span data-stu-id="11c1e-135">Certificate-based authentication</span></span>

<span data-ttu-id="11c1e-136">証明書ベースの認証では、Azure PowerShell で、証明書の拇印に基づいてローカル証明書ストアから情報を取得できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="11c1e-136">Certificate-based authentication requires that Azure PowerShell can retrieve information from a local certificate store based on a certificate thumbprint.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ApplicationId $appId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="11c1e-137">登録されたアプリケーションではなくサービス プリンシパルを使用する場合は、`-ServicePrincipal` 引数を追加し、`-ApplicationId` パラメーターの値としてサービス プリンシパルの ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-137">When using a service principal instead of a registered application, add the `-ServicePrincipal` argument and provide the service principal's ID as the `-ApplicationId` parameter's value.</span></span>

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -ApplicationId $servicePrincipalId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

<span data-ttu-id="11c1e-138">PowerShell 5.1 では、[PKI](/powershell/module/pkiclient) モジュールを使用して、証明書ストアを管理および検査できます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-138">In PowerShell 5.1, the certificate store can be managed and inspected with the [PKI](/powershell/module/pkiclient) module.</span></span> <span data-ttu-id="11c1e-139">PowerShell Core 6.x 以降の場合は、プロセスがさらに複雑になります。</span><span class="sxs-lookup"><span data-stu-id="11c1e-139">For PowerShell Core 6.x and later, the process is more complicated.</span></span> <span data-ttu-id="11c1e-140">次のスクリプトでは、PowerShell からアクセスできる証明書ストアに、既存の証明書をインポートする方法を示します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-140">The following scripts show you how to import an existing certificate into the certificate store accessible by PowerShell.</span></span>

#### <a name="import-a-certificate-in-powershell-51"></a><span data-ttu-id="11c1e-141">PowerShell 5.1 で証明書をインポートする</span><span class="sxs-lookup"><span data-stu-id="11c1e-141">Import a certificate in PowerShell 5.1</span></span>

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-core-6x-and-later"></a><span data-ttu-id="11c1e-142">PowerShell Core 6.x 以降で証明書をインポートする</span><span class="sxs-lookup"><span data-stu-id="11c1e-142">Import a certificate in PowerShell Core 6.x and later</span></span>

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

## <a name="sign-in-using-a-managed-identity"></a><span data-ttu-id="11c1e-143">マネージド ID を使用したサインイン</span><span class="sxs-lookup"><span data-stu-id="11c1e-143">Sign in using a managed identity</span></span>

<span data-ttu-id="11c1e-144">マネージド ID は Azure Active Directory の機能です。</span><span class="sxs-lookup"><span data-stu-id="11c1e-144">Managed identities are a feature of Azure Active Directory.</span></span> <span data-ttu-id="11c1e-145">マネージド ID は、Azure で実行されるリソースに割り当てられたサービス プリンシパルです。</span><span class="sxs-lookup"><span data-stu-id="11c1e-145">Managed identities are service principals assigned to resources that run in Azure.</span></span> <span data-ttu-id="11c1e-146">サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-146">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="11c1e-147">マネージド ID は、Azure クラウドで実行されているリソースでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-147">Managed identities are only available on resources running in an Azure cloud.</span></span>

<span data-ttu-id="11c1e-148">Azure リソースのマネージド ID の詳細については、「[Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11c1e-148">To learn more about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="11c1e-149">既定ではないテナントで、あるいはクラウド ソリューション プロバイダー (CSP) としてサインインする</span><span class="sxs-lookup"><span data-stu-id="11c1e-149">Sign in with a non-default tenant or as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="11c1e-150">アカウントが複数のテナントに関連付けられている場合、接続時に `-Tenant` パラメーターを使用することがサインインで要求されます。</span><span class="sxs-lookup"><span data-stu-id="11c1e-150">If your account is associated with more than one tenant, sign-in requires the use of the `-Tenant` parameter when connecting.</span></span> <span data-ttu-id="11c1e-151">このパラメーターはあらゆるサインイン メソッドで動作します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-151">This parameter will work with any sign-in method.</span></span> <span data-ttu-id="11c1e-152">ログイン時、テナントの Azure オブジェクト ID (テナント ID) またはテナントの完全修飾ドメイン名がこのパラメーター値になります。</span><span class="sxs-lookup"><span data-stu-id="11c1e-152">When logging in, this parameter value can either be the Azure object ID of the tenant (Tenant ID) or the fully qualified domain name of the tenant.</span></span>

<span data-ttu-id="11c1e-153">[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/) の場合、`-Tenant` 値はテナント ID にすることが**必要**となります。</span><span class="sxs-lookup"><span data-stu-id="11c1e-153">If you're a [Cloud Solution Provider (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/), the `-Tenant` value **must** be a tenant ID.</span></span>

```azurepowershell-interactive
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="11c1e-154">別のクラウドにサインインする</span><span class="sxs-lookup"><span data-stu-id="11c1e-154">Sign in to another Cloud</span></span>

<span data-ttu-id="11c1e-155">Azure クラウド サービスでは、リージョンのデータ処理の法律に準拠した環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-155">Azure cloud services offer environments compliant with regional data-handling laws.</span></span>
<span data-ttu-id="11c1e-156">リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-156">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="11c1e-157">このパラメーターはあらゆるサインイン メソッドで動作します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-157">This parameter will work with any sign-in method.</span></span> <span data-ttu-id="11c1e-158">たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-158">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

<span data-ttu-id="11c1e-159">次のコマンドでは、使用可能な環境の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="11c1e-159">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```
