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
ms.openlocfilehash: f6d249ca5bb09c4fe8445ba5b339ffa6012815ed
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <a name="log-in-with-azure-powershell"></a><span data-ttu-id="e0693-103">Azure PowerShell でのログイン</span><span class="sxs-lookup"><span data-stu-id="e0693-103">Log in with Azure PowerShell</span></span>

<span data-ttu-id="e0693-104">Azure PowerShell は、複数のログイン方法をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="e0693-104">Azure PowerShell supports multiple login methods.</span></span> <span data-ttu-id="e0693-105">最も簡単に始められるのは、コマンド ラインから対話形式でログインする方法です。</span><span class="sxs-lookup"><span data-stu-id="e0693-105">The simplest way to get started is to log in interactively at the command line.</span></span>

## <a name="interactive-log-in"></a><span data-ttu-id="e0693-106">対話形式でのログイン</span><span class="sxs-lookup"><span data-stu-id="e0693-106">Interactive log in</span></span>

1. <span data-ttu-id="e0693-107">「 `Login-AzureRmAccount`」と入力します。</span><span class="sxs-lookup"><span data-stu-id="e0693-107">Type `Login-AzureRmAccount`.</span></span> <span data-ttu-id="e0693-108">Azure の資格情報の入力を求めるダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e0693-108">You will get dialog box asking for your Azure credentials.</span></span>

2. <span data-ttu-id="e0693-109">アカウントに関連付けられている電子メール アドレスとパスワードを入力します。</span><span class="sxs-lookup"><span data-stu-id="e0693-109">Type the email address and password associated with your account.</span></span> <span data-ttu-id="e0693-110">Azure により資格情報が認証および保存され、ウィンドウが閉じます。</span><span class="sxs-lookup"><span data-stu-id="e0693-110">Azure authenticates and saves the credential information, and then closes the window.</span></span>

## <a name="log-in-with-a-service-principal"></a><span data-ttu-id="e0693-111">サービス プリンシパルによるログイン</span><span class="sxs-lookup"><span data-stu-id="e0693-111">Log in with a service principal</span></span>

<span data-ttu-id="e0693-112">サービス プリンシパルは、リソースの操作に使用できる非対話型のアカウントを作成する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="e0693-112">Service principals provide a way for you to create non-interactive accounts that you can use to manipulate resources.</span></span> <span data-ttu-id="e0693-113">サービス プリンシパルは、Azure Active Directory を使用してルールを適用できるユーザー アカウントに似ています。</span><span class="sxs-lookup"><span data-stu-id="e0693-113">Service principals are like user accounts to which you can apply rules using Azure Active Directory.</span></span> <span data-ttu-id="e0693-114">サービス プリンシパルに最低限必要なアクセス許可だけを付与することによって、自動化スクリプトをより安全にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e0693-114">By granting the minimum permissions needed to a service principal, you can ensure your automation scripts are even more secure.</span></span>

1. <span data-ttu-id="e0693-115">まだサービス プリンシパルがない場合は、サービス プリンシパルを[作成](create-azure-service-principal-azureps.md)します。</span><span class="sxs-lookup"><span data-stu-id="e0693-115">If you don't already have a service principal, [create one](create-azure-service-principal-azureps.md).</span></span>

2. <span data-ttu-id="e0693-116">サービス プリンシパルを使用してログインします。</span><span class="sxs-lookup"><span data-stu-id="e0693-116">Log in with the service principal.</span></span>

    ```powershell
    Login-AzureRmAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
    ```

    <span data-ttu-id="e0693-117">テナント ID を取得するには、対話形式でログインし、サブスクリプションから TenantId を取得します。</span><span class="sxs-lookup"><span data-stu-id="e0693-117">To get your TenantId, log in interactively and then get the TenantId from your subscription.</span></span>

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

## <a name="log-in-to-another-cloud"></a><span data-ttu-id="e0693-118">別のクラウドにログインする</span><span class="sxs-lookup"><span data-stu-id="e0693-118">Log in to another Cloud</span></span>

<span data-ttu-id="e0693-119">Azure Cloud Services では、さまざまな政府機関から発せられるデータ処理規制に準拠したさまざまな環境を提供します。</span><span class="sxs-lookup"><span data-stu-id="e0693-119">Azure cloud services provide different environments that adhere to the data-handling regulations of various governments.</span></span> <span data-ttu-id="e0693-120">Azure アカウントが政府機関のクラウド内にある場合は、サインイン時に環境を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e0693-120">If your Azure account is in one the government clouds, you need to specify the environment when you sign in.</span></span> <span data-ttu-id="e0693-121">たとえば、アカウントが中国のクラウド内にある場合、次のコマンドを使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="e0693-121">For example, if you account is in the China cloud you sign on using the following command:</span></span>

```powershell
Login-AzureRmAccount -EnvironmentName AzureChinaCloud
```

<span data-ttu-id="e0693-122">使用可能な環境の一覧を取得するには、次のコマンドを使用します。</span><span class="sxs-lookup"><span data-stu-id="e0693-122">Use the following command to get a list of available environments:</span></span>

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

## <a name="learn-more-about-managing-azure-role-based-access"></a><span data-ttu-id="e0693-123">Azure ロールベース アクセスの管理についての詳細情報</span><span class="sxs-lookup"><span data-stu-id="e0693-123">Learn more about managing Azure role-based access</span></span>

<span data-ttu-id="e0693-124">Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0693-124">For more information about authentication and subscription management in Azure, see [Manage Accounts, Subscriptions, and Administrative Roles](/azure/active-directory/role-based-access-control-configure).</span></span>

<span data-ttu-id="e0693-125">ロール管理を目的とした Azure PowerShell のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="e0693-125">Azure PowerShell cmdlets for role management</span></span>

* [<span data-ttu-id="e0693-126">Get-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e0693-126">Get-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleAssignment)
* [<span data-ttu-id="e0693-127">Get-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0693-127">Get-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Get-AzureRmRoleDefinition)
* [<span data-ttu-id="e0693-128">New-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e0693-128">New-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleAssignment)
* [<span data-ttu-id="e0693-129">New-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0693-129">New-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/New-AzureRmRoleDefinition)
* [<span data-ttu-id="e0693-130">Remove-AzureRmRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e0693-130">Remove-AzureRmRoleAssignment</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleAssignment)
* [<span data-ttu-id="e0693-131">Remove-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0693-131">Remove-AzureRmRoleDefinition</span></span>](/powershell/module/AzureRM.Resources/Remove-AzureRmRoleDefinition)
* [<span data-ttu-id="e0693-132">Set-AzureRmRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e0693-132">Set-AzureRmRoleDefinition</span></span>](/powershell/moduel/AzureRM.Resources/Set-AzureRmRoleDefinition)
