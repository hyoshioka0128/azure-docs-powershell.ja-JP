---
title: "Azure PowerShell でのログイン"
description: "Azure PowerShell でのログイン"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 1af5aeffb8e87e916df3e2440a84805935136c0f
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2017
---
# <a name="log-in-with-azure-powershell"></a><span data-ttu-id="c068e-103">Azure PowerShell でのログイン</span><span class="sxs-lookup"><span data-stu-id="c068e-103">Log in with Azure PowerShell</span></span>

<span data-ttu-id="c068e-104">Azure PowerShell は、複数のログイン方法をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="c068e-104">Azure PowerShell supports multiple login methods.</span></span> <span data-ttu-id="c068e-105">最も簡単に始められるのは、コマンド ラインから対話形式でログインする方法です。</span><span class="sxs-lookup"><span data-stu-id="c068e-105">The simplest way to get started is to log in interactively at the command line.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="c068e-106">対話形式でのログイン</span><span class="sxs-lookup"><span data-stu-id="c068e-106">Interactive log in</span></span>

1. <span data-ttu-id="c068e-107">「 `Login-AzureRmAccount`」と入力します。</span><span class="sxs-lookup"><span data-stu-id="c068e-107">Type `Login-AzureRmAccount`.</span></span> <span data-ttu-id="c068e-108">Azure の資格情報の入力を求めるダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="c068e-108">You will get dialog box asking for your Azure credentials.</span></span>

2. <span data-ttu-id="c068e-109">アカウントに関連付けられている電子メール アドレスとパスワードを入力します。</span><span class="sxs-lookup"><span data-stu-id="c068e-109">Type the email address and password associated with your account.</span></span> <span data-ttu-id="c068e-110">Azure により資格情報が認証および保存され、ウィンドウが閉じます。</span><span class="sxs-lookup"><span data-stu-id="c068e-110">Azure authenticates and saves the credential information, and then closes the window.</span></span>

## <a name="log-in-with-a-service-principal"></a><span data-ttu-id="c068e-111">サービス プリンシパルによるログイン</span><span class="sxs-lookup"><span data-stu-id="c068e-111">Log in with a service principal</span></span>

<span data-ttu-id="c068e-112">サービス プリンシパルは、リソースの操作に使用できる非対話型のアカウントを作成する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="c068e-112">Service principals provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="c068e-113">サービス プリンシパルは、Azure Active Directory を使用してルールを適用できるユーザー アカウントに似ています。</span><span class="sxs-lookup"><span data-stu-id="c068e-113">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span> <span data-ttu-id="c068e-114">サービス プリンシパルに最低限必要なアクセス許可だけを付与することによって、自動化スクリプトをより安全にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c068e-114">By granting the minimum permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

1. <span data-ttu-id="c068e-115">まだサービス プリンシパルがない場合は、サービス プリンシパルを[作成](create-azure-service-principal-azureps.md)します。</span><span class="sxs-lookup"><span data-stu-id="c068e-115">If you don't already have a service principal, [create one](create-azure-service-principal-azureps.md).</span></span>

2. <span data-ttu-id="c068e-116">サービス プリンシパルを使用してログインします。</span><span class="sxs-lookup"><span data-stu-id="c068e-116">Log in with the service principal.</span></span>

    ```powershell
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    <span data-ttu-id="c068e-117">テナント ID を取得するには、対話形式でログインし、サブスクリプションから TenantId を取得します。</span><span class="sxs-lookup"><span data-stu-id="c068e-117">To get your TenantId, log in interactively and then get the TenantId from your subscription.</span></span>

    ```powershell
    Get-AzureRmSubscription
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :
    ```

### <a name="log-in-using-an-azure-vm-managed-service-identity"></a><span data-ttu-id="c068e-118">Azure VM の管理対象サービス ID を使用したログイン</span><span class="sxs-lookup"><span data-stu-id="c068e-118">Log in using an Azure VM Managed Service Identity</span></span>

<span data-ttu-id="c068e-119">管理対象サービス ID (MSI) は、Azure Active Directory のプレビュー機能です。</span><span class="sxs-lookup"><span data-stu-id="c068e-119">Managed Service Identity (MSI) is a preview feature of Azure Active Directory.</span></span> <span data-ttu-id="c068e-120">サインインに MSI サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="c068e-120">You can use an MSI service principal for sign-in, and acquire an app-only access token to access other resources.</span></span>

<span data-ttu-id="c068e-121">MSI の詳細については、「[How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition (サインインとトークン取得に Azure VM の管理対象サービス ID (MSI) を使用する方法)](/azure/active-directory/msi-how-to-get-access-token-using-msi)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c068e-121">For more information about MSI, see [How to use an Azure VM Managed Service Identity (MSI) for sign-in and token acquisition](/azure/active-directory/msi-how-to-get-access-token-using-msi).</span></span>

## <a name="log-in-to-another-cloud"></a><span data-ttu-id="c068e-122">別のクラウドにログインする</span><span class="sxs-lookup"><span data-stu-id="c068e-122">Log in to another Cloud</span></span>

<span data-ttu-id="c068e-123">Azure Cloud Services では、さまざまな政府機関から発せられるデータ処理規制に準拠したさまざまな環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="c068e-123">Azure cloud services provide different environments that adhere to the data-handling regulations of various governments.</span></span> <span data-ttu-id="c068e-124">Azure アカウントが政府機関のクラウド内にある場合は、サインイン時に環境を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c068e-124">If your Azure account is in one the government clouds, you need to specify the environment when you sign in.</span></span> <span data-ttu-id="c068e-125">たとえば、アカウントが中国のクラウド内にある場合、次のコマンドを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="c068e-125">For example, if you account is in the China cloud you sign on using the following command:</span></span>

```powershell
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

<span data-ttu-id="c068e-126">使用可能な環境の一覧を取得するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="c068e-126">Use the following command to get a list of available environments:</span></span>

```powershell
Get-AzureRmEnvironment | Select-Object Name
```

```
Name
----
AzureCloud
AzureChinaCloud
AzureUSGovernment
AzureGermanCloud
```

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="c068e-127">Azure ロールベース アクセスの管理についての詳細情報</span><span class="sxs-lookup"><span data-stu-id="c068e-127">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="c068e-128">Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c068e-128">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="c068e-129">ロール管理を目的とした Azure PowerShell のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="c068e-129">Azure PowerShell cmdlets for role management</span></span>

* [<span data-ttu-id="c068e-130">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c068e-130">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="c068e-131">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c068e-131">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="c068e-132">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c068e-132">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="c068e-133">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c068e-133">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="c068e-134">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="c068e-134">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="c068e-135">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c068e-135">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="c068e-136">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="c068e-136">Set-AzureRmRoleDefinition</span></span>](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
