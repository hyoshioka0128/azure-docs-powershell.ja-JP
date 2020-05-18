---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/09/2018
ms.openlocfilehash: 464d7efa640f1d1ffd1c34bfbe6cf13cbe5202b6
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "68863235"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="00220-103">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="00220-103">Sign in with Azure PowerShell</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="00220-104">Azure PowerShell では、複数の認証方法がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="00220-104">Azure PowerShell supports several authentication methods.</span></span> <span data-ttu-id="00220-105">最も簡単に始められるのは、コマンド ラインから対話形式でサインインする方法です。</span><span class="sxs-lookup"><span data-stu-id="00220-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="00220-106">対話操作でサインインする</span><span class="sxs-lookup"><span data-stu-id="00220-106">Sign in interactively</span></span>

<span data-ttu-id="00220-107">対話操作でサインインするには、[Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="00220-107">To sign in interactively, use the [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) cmdlet.</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount
```

<span data-ttu-id="00220-108">このコマンドレットを実行すると、ダイアログ ボックスが表示され、Azure アカウントに関連付けられている電子メール アドレスとパスワードを入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="00220-108">When run, this cmdlet will bring up a dialog box prompting you for your email address and password associated with your Azure account.</span></span> <span data-ttu-id="00220-109">この認証は、現在の PowerShell セッションが終了するまで有効です。</span><span class="sxs-lookup"><span data-stu-id="00220-109">This authentication lasts for the current PowerShell session.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="00220-110">Azure PowerShell 6.3.0 の時点で、Windows にサインインしたままである限り、資格情報は複数の PowerShell セッション間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="00220-110">As of Azure PowerShell 6.3.0, your credentials are shared among multiple PowerShell sessions as long as you remain signed in to Windows.</span></span> <span data-ttu-id="00220-111">詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00220-111">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="00220-112">サービス プリンシパルを使ってサインインする</span><span class="sxs-lookup"><span data-stu-id="00220-112">Sign in with a service principal</span></span>

<span data-ttu-id="00220-113">サービス プリンシパルは、非対話型の Azure アカウントです。</span><span class="sxs-lookup"><span data-stu-id="00220-113">Service principals are non-interactive Azure accounts.</span></span> <span data-ttu-id="00220-114">他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。</span><span class="sxs-lookup"><span data-stu-id="00220-114">Like other user accounts, their permissions are managed with Azure Active Directory.</span></span> <span data-ttu-id="00220-115">サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。</span><span class="sxs-lookup"><span data-stu-id="00220-115">By granting a service principal only the permissions it needs, your automation scripts stay secure.</span></span>

<span data-ttu-id="00220-116">Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00220-116">To learn how to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="00220-117">サービス プリンシパルを使用してサインインするには、`Connect-AzureRmAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="00220-117">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzureRmAccount` cmdlet.</span></span> <span data-ttu-id="00220-118">サービス プリンシパルのサインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="00220-118">You'll also need the service principal's sign-in credentials and the tenant ID associated with the service principal.</span></span> <span data-ttu-id="00220-119">サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="00220-119">To get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="00220-120">このコマンドレットにより、サービス プリンシパル ユーザー ID とパスワードを入力するダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="00220-120">This cmdlet will display a dialog box to enter the service principal user ID and password into.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a><span data-ttu-id="00220-121">Azure マネージド サービス ID を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="00220-121">Sign in using an Azure Managed Service Identity</span></span>

<span data-ttu-id="00220-122">Azure リソースのマネージドID は、Azure Active Directory の機能です。</span><span class="sxs-lookup"><span data-stu-id="00220-122">Managed identities for Azure resources is a feature of Azure Active Directory.</span></span> <span data-ttu-id="00220-123">サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="00220-123">You can use a managed identity service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="00220-124">マネージド ID は、Azure クラウドで実行されている仮想マシンでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="00220-124">Managed identities are only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="00220-125">Azure リソースのマネージド ID の詳細については、「[How to use managed identities for Azure resources on an Azure VM to acquire an access token (Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法)](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="00220-125">For more information about managed identities for Azure resources, see [How to use managed identities for Azure resources on an Azure VM to acquire an access token](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token).</span></span>

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a><span data-ttu-id="00220-126">クラウド ソリューション プロバイダー (CSP) としてサインインする</span><span class="sxs-lookup"><span data-stu-id="00220-126">Sign in as a Cloud Solution Provider (CSP)</span></span>

<span data-ttu-id="00220-127">[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/) のサインインには、`-TenantId` を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="00220-127">A [Cloud Solution Provider (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/) sign-in requires the use of `-TenantId`.</span></span> <span data-ttu-id="00220-128">通常は、このパラメーターにはテナント ID またはドメイン名を指定できます。</span><span class="sxs-lookup"><span data-stu-id="00220-128">Normally, this parameter can be provided as either a tenant ID or a domain name.</span></span> <span data-ttu-id="00220-129">しかし、CSP のサインインの場合、**テナント ID** を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="00220-129">However, for CSP sign-in, it must be provided a **tenant ID**.</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="00220-130">別のクラウドにサインインする</span><span class="sxs-lookup"><span data-stu-id="00220-130">Sign in to another Cloud</span></span>

<span data-ttu-id="00220-131">Azure クラウド サービスでは、リージョンのデータ処理規制に準拠した環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="00220-131">Azure cloud services offer environments compliant with regional data-handling regulations.</span></span>
<span data-ttu-id="00220-132">リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。</span><span class="sxs-lookup"><span data-stu-id="00220-132">For accounts in a regional cloud, set the environment when you sign in with the `-Environment` argument.</span></span>
<span data-ttu-id="00220-133">たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。</span><span class="sxs-lookup"><span data-stu-id="00220-133">For example, if your account is in the China cloud:</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

<span data-ttu-id="00220-134">次のコマンドでは、使用可能な環境の一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="00220-134">The following command gets a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="00220-135">Azure ロールベース アクセスの管理についての詳細情報</span><span class="sxs-lookup"><span data-stu-id="00220-135">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="00220-136">Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="00220-136">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="00220-137">ロール管理を目的とした Azure PowerShell のコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="00220-137">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="00220-138">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="00220-138">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="00220-139">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="00220-139">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="00220-140">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="00220-140">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="00220-141">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="00220-141">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="00220-142">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="00220-142">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="00220-143">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="00220-143">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="00220-144">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="00220-144">Set-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Set-AzureRmRoleDefinition)
