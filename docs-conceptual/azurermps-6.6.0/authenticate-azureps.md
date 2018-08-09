---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、サービス プリンシパルまたは MSI を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 20194ac2282d602ba61bf130791edac9f4ffae6c
ms.sourcegitcommit: afae9f2f091b21ed07d5aec1c249cf859a8b89a4
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/09/2018
ms.locfileid: "39653867"
---
# <a name="sign-in-with-azure-powershell"></a><span data-ttu-id="d2cf3-103">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="d2cf3-103">Sign in with Azure PowerShell</span></span>

<span data-ttu-id="d2cf3-104">Azure PowerShell は、複数の認証方法をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-104">Azure PowerShell supports multiple authentication methods.</span></span> <span data-ttu-id="d2cf3-105">最も簡単に始められるのは、コマンド ラインから対話形式でサインインする方法です。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-105">The simplest way to get started is to sign in interactively at the command line.</span></span>

## <a name="sign-in-interactively"></a><span data-ttu-id="d2cf3-106">対話操作でサインインする</span><span class="sxs-lookup"><span data-stu-id="d2cf3-106">Sign in interactively</span></span>

<span data-ttu-id="d2cf3-107">対話操作でサインインするには、[Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-107">To sign in interactively, use the [Connect-AzureRmAccount](/powershell/module/azurerm.profile/connect-azurermaccount) cmdlet.</span></span>

```azurepowershell
Connect-AzureRmAccount
```

<span data-ttu-id="d2cf3-108">このコマンドレットを実行すると、ダイアログ ボックスが表示され、Azure アカウントに関連付けられている電子メール アドレスとパスワードを入力するように求められます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-108">When run, this cmdlet will bring up a dialog box prompting you for your email address and password associated with your Azure account.</span></span> <span data-ttu-id="d2cf3-109">認証すると、現在の PowerShell セッションに対してこの情報が保存され、ダイアログは閉じます。これで、すべての Azure PowerShell コマンドレットにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-109">When you authenticate, that information is saved for the current PowerShell session, the dialog is closed, and you have access to all of the Azure PowerShell cmdlets.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="d2cf3-110">Azure PowerShell 6.3.0 の時点で、Windows にサインインしたままである限り、資格情報は複数の PowerShell セッション間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-110">As of Azure PowerShell 6.3.0, your credentials are shared among multiple PowerShell sessions as long as you remain signed in to Windows.</span></span> <span data-ttu-id="d2cf3-111">詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-111">For more information, see the article on [Persistent Credentials](context-persistence.md).</span></span>

## <a name="sign-in-with-a-service-principal"></a><span data-ttu-id="d2cf3-112">サービス プリンシパルを使ってサインインする</span><span class="sxs-lookup"><span data-stu-id="d2cf3-112">Sign in with a service principal</span></span>

<span data-ttu-id="d2cf3-113">サービス プリンシパルは、リソースの操作に使用できる非対話型のアカウントを作成する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-113">Service principals provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="d2cf3-114">サービス プリンシパルは、Azure Active Directory を使用してルールを適用できるユーザー アカウントに似ています。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-114">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span> <span data-ttu-id="d2cf3-115">サービス プリンシパルに最低限必要なアクセス許可だけを付与することによって、自動化スクリプトをより安全にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-115">By granting the minimum permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

<span data-ttu-id="d2cf3-116">Azure PowerShell で使用するサービス プリンシパルを作成する必要がある場合は、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-116">If you need to create a service principal for use with Azure PowerShell, see [Create an Azure service principal with Azure PowerShell](create-azure-service-principal-azureps.md).</span></span>

<span data-ttu-id="d2cf3-117">サービス プリンシパルを使用してサインインするには、`Connect-AzureRmAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-117">To sign in with a service principal, use the `-ServicePrincipal` argument with the `Connect-AzureRmAccount` cmdlet.</span></span> <span data-ttu-id="d2cf3-118">サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-118">You will also need the service princpal's application ID, sign-in credentials, and the tenant ID associate with the service principal.</span></span> <span data-ttu-id="d2cf3-119">サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-119">In order to get the service principal's credentials as the appropriate object, use the [Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) cmdlet.</span></span> <span data-ttu-id="d2cf3-120">このコマンドレットにより、サービス プリンシパル ユーザー ID とパスワードを入力するダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-120">This cmdlet will display a dialog box to enter the service principal user ID and password into.</span></span>

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-vm-managed-service-identity"></a><span data-ttu-id="d2cf3-121">Azure VM マネージド サービス ID を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="d2cf3-121">Sign in using an Azure VM Managed Service Identity</span></span>

<span data-ttu-id="d2cf3-122">管理対象サービス ID (MSI) は、Azure Active Directory のプレビュー機能です。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-122">Managed Service Identity (MSI) is a preview feature of Azure Active Directory.</span></span> <span data-ttu-id="d2cf3-123">サインインに MSI サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-123">You can use an MSI service principal for sign-in, and acquire an app-only access token to access other resources.</span></span> <span data-ttu-id="d2cf3-124">MSI は、Azure クラウドで実行されている仮想マシンでのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-124">MSI is only available on virtual machines running in an Azure cloud.</span></span>

<span data-ttu-id="d2cf3-125">MSI の詳細については、「[How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition (サインインとトークン取得に Azure VM の管理対象サービス ID (MSI) を使用する方法)](/azure/active-directory/msi-how-to-get-access-token-using-msi)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-125">For more information about MSI, see [How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition](/azure/active-directory/msi-how-to-get-access-token-using-msi).</span></span>

## <a name="sign-in-to-another-cloud"></a><span data-ttu-id="d2cf3-126">別のクラウドにサインインする</span><span class="sxs-lookup"><span data-stu-id="d2cf3-126">Sign in to another Cloud</span></span>

<span data-ttu-id="d2cf3-127">Azure クラウド サービスでは、さまざまなリージョンのデータ処理規制に準拠したさまざまな環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-127">Azure cloud services provide different environments that adhere to the data-handling regulations of various regions.</span></span> <span data-ttu-id="d2cf3-128">Azure アカウントがこれらのリージョンのいずれかに関連付けられたクラウド内にある場合は、サインイン時に環境を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-128">If your Azure account is in a cloud associated with one of these regions, you need to specify the environment when you sign in.</span></span> <span data-ttu-id="d2cf3-129">たとえば、アカウントが中国のクラウド内にある場合、次のコマンドを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-129">For example, if you account is in the China cloud you sign on using the following command:</span></span>

```azurepowershell-interactive
Connect-AzureRmAccount -Environment AzureChinaCloud
```

<span data-ttu-id="d2cf3-130">使用可能な環境の一覧を取得するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-130">Use the following command to get a list of available environments:</span></span>

```azurepowershell-interactive
Get-AzureRmEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="d2cf3-131">Azure ロールベース アクセスの管理についての詳細情報</span><span class="sxs-lookup"><span data-stu-id="d2cf3-131">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="d2cf3-132">Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2cf3-132">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="d2cf3-133">ロール管理を目的とした Azure PowerShell のコマンドレット:</span><span class="sxs-lookup"><span data-stu-id="d2cf3-133">Azure PowerShell cmdlets for role management:</span></span>

* [<span data-ttu-id="d2cf3-134">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d2cf3-134">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="d2cf3-135">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2cf3-135">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="d2cf3-136">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d2cf3-136">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="d2cf3-137">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2cf3-137">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="d2cf3-138">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="d2cf3-138">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="d2cf3-139">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2cf3-139">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="d2cf3-140">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="d2cf3-140">Set-AzureRmRoleDefinition</span></span>](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
