---
title: Azure PowerShell による Azure サブスクリプションの管理
description: Azure PowerShell による Azure サブスクリプションの管理
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 02/04/2019
ms.openlocfilehash: 778fdb463a42b609d3a94c910a2c0f9553ef4eb9
ms.sourcegitcommit: 0c012450805bef75472f48c74fe488baf6ba53bb
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/04/2019
ms.locfileid: "66498394"
---
# <a name="use-multiple-azure-subscriptions"></a><span data-ttu-id="2d036-103">複数の Azure サブスクリプションの使用</span><span class="sxs-lookup"><span data-stu-id="2d036-103">Use multiple Azure subscriptions</span></span>

<span data-ttu-id="2d036-104">ほとんどの Azure ユーザーは、サブスクリプションを 1 つしか持っていません。</span><span class="sxs-lookup"><span data-stu-id="2d036-104">Most Azure users will only ever have a single subscription.</span></span> <span data-ttu-id="2d036-105">ただし、複数の組織に属している場合や、組織がグループ間で特定のリソースへのアクセスを分けている場合、Azure に複数のサブスクリプションを持っていることがあります。</span><span class="sxs-lookup"><span data-stu-id="2d036-105">However, if you are part of more than one organization or your organization has divided up access to certain resources across groupings, you may have multiple subscriptions within Azure.</span></span> <span data-ttu-id="2d036-106">CLI では、サブスクリプションをグローバルに選択することも、コマンドごとに選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="2d036-106">The CLI supports selecting a subscription both globally and per command.</span></span>

<span data-ttu-id="2d036-107">サブスクリプション、請求、およびコスト管理の詳細については、[課金とコスト管理に関するドキュメント](/azure/billing/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2d036-107">For detailed information on subscriptions, billing, and cost management, see the [billing and cost management documentation](/azure/billing/).</span></span>

## <a name="tenants-users-and-subscriptions"></a><span data-ttu-id="2d036-108">テナント、ユーザー、サブスクリプション</span><span class="sxs-lookup"><span data-stu-id="2d036-108">Tenants, users, and subscriptions</span></span>

<span data-ttu-id="2d036-109">Azure におけるテナント、ユーザー、サブスクリプションが混同されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="2d036-109">You might have some confusion over the difference between tenants, users, and subscriptions within Azure.</span></span> <span data-ttu-id="2d036-110">"_テナント_" とは、組織全体を含む Azure Active Directory エンティティです。</span><span class="sxs-lookup"><span data-stu-id="2d036-110">A _tenant_ is the Azure Active Directory entity that encompasses a whole organization.</span></span> <span data-ttu-id="2d036-111">このテナントは、少なくとも 1 つの "_サブスクリプション_" を持ち、少なくとも 1 人の "_ユーザー_" が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2d036-111">This tenant has at least one _subscription_ and _user_.</span></span> <span data-ttu-id="2d036-112">ユーザーとは個人であり、1 つのテナント (ユーザーが属している組織) にのみ関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2d036-112">A user is an individual and is associated with only one tenant, the organization that they belong to.</span></span> <span data-ttu-id="2d036-113">ユーザーは、Azure にサインインしてリソースを作成、管理、および使用するアカウントです。</span><span class="sxs-lookup"><span data-stu-id="2d036-113">Users are those accounts that sign in to Azure to create, manage, and use resources.</span></span>
<span data-ttu-id="2d036-114">1 人のユーザーが複数の "_サブスクリプション_" にアクセスできる場合があります。サブスクリプションとは、Azure をはじめとするクラウド サービスを使用するための Microsoft との契約です。</span><span class="sxs-lookup"><span data-stu-id="2d036-114">A user may have access to multiple _subscriptions_, which are the agreements with Microsoft to use cloud services, including Azure.</span></span> <span data-ttu-id="2d036-115">各リソースは、サブスクリプションに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2d036-115">Every resource is associated with a subscription.</span></span>

<span data-ttu-id="2d036-116">テナント、ユーザー、サブスクリプションの違いの詳細については、[Azure クラウド用語集](/azure/azure-glossary-cloud-terminology)のページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2d036-116">To learn more about the differences between tenants, users, and subscriptions, see the [Azure cloud terminology dictionary](/azure/azure-glossary-cloud-terminology).</span></span>  <span data-ttu-id="2d036-117">Azure Active Directory テナントに新しいサブスクリプションを追加する方法については、「[Azure サブスクリプションを Azure Active Directory に追加する方法](/azure/active-directory/active-directory-how-subscriptions-associated-directory)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2d036-117">To learn how to add a new subscription to your Azure Active Directory tenant, see [How to add an Azure subscription to Azure Active Directory](/azure/active-directory/active-directory-how-subscriptions-associated-directory).</span></span>
<span data-ttu-id="2d036-118">特定のテナントにサインインする方法を確認するには、[Azure PowerShell を使用したサインイン](/powershell/azure/authenticate-azureps)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="2d036-118">To learn how to sign in to a specific tenant, see [Sign in with Azure PowerShell](/powershell/azure/authenticate-azureps).</span></span>

## <a name="change-the-active-subscription"></a><span data-ttu-id="2d036-119">アクティブなサブスクリプションを変更する</span><span class="sxs-lookup"><span data-stu-id="2d036-119">Change the active subscription</span></span>

<span data-ttu-id="2d036-120">Azure PowerShell でサブスクリプションのリソースにアクセスするには、現在の Azure セッションに関連付けられているサブスクリプションを変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d036-120">In Azure PowerShell, accessing the resources for a subscription requires changing the subscription associated with your current Azure session.</span></span>
<span data-ttu-id="2d036-121">これは、アクティブなセッションのコンテキスト、どのテナント、サブスクリプション、およびユーザーに対してコマンドレットを実行するかについての情報を変更することによって実行します。</span><span class="sxs-lookup"><span data-stu-id="2d036-121">This is done by modifying the active session context, the information about which tenant, subscription, and user cmdlets should be run against.</span></span>
<span data-ttu-id="2d036-122">サブスクリプションを変更するには、まず Azure PowerShell コンテキスト オブジェクトを [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) で取得し、次に、現在のコンテキストを [Set-AzContext](/powershell/module/az.accounts/set-azcontext) で変更する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d036-122">In order to change subscriptions, an Azure PowerShell Context object first needs to be retrieved with [Get-AzSubscription](/powershell/module/az.accounts/get-azsubscription) and then the current context changed with [Set-AzContext](/powershell/module/az.accounts/set-azcontext).</span></span>

<span data-ttu-id="2d036-123">次の例は、現在アクティブなテナントでサブスクリプションを取得し、アクティブなセッションとして設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2d036-123">The next example shows how to get a subscription in the currently active tenant, and set it as the active session:</span></span>

```powershell-interactive
$context = Get-AzSubscription -SubscriptionId ...
Set-AzContext $context
```

<span data-ttu-id="2d036-124">コンテキストの保存方法や複数のサブスクリプションすばやく簡単に切り替えて操作する方法など、Azure PowerShell コンテキストの詳細については、[Azure PowerShell コンテキストでの資格情報の保持](context-persistence.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d036-124">To learn more about Azure PowerShell contexts, including how to save them and quickly switch between them for working with multiple subscriptions easily, see [Persist credentials with Azure PowerShell contexts](context-persistence.md).</span></span>