---
title: Azure コンテキストとサインイン資格情報
description: 複数の PowerShell セッション間で Azure の資格情報や他の情報を再利用する方法について説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.openlocfilehash: c79d1d634d5b76b2c6ab6b6ab309c2d49f9f7678
ms.sourcegitcommit: 10ec909100a70acec94d42f6084e7bf0342c6854
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "83630930"
---
# <a name="azure-powershell-context-objects"></a><span data-ttu-id="4adc5-103">Azure PowerShell コンテキスト オブジェクト</span><span class="sxs-lookup"><span data-stu-id="4adc5-103">Azure PowerShell context objects</span></span>

<span data-ttu-id="4adc5-104">Azure PowerShell は、_Azure PowerShell コンテキスト オブジェクト_ (Azure コンテキスト) を使用して、サブスクリプションと認証情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-104">Azure PowerShell uses _Azure PowerShell context objects_ (Azure contexts) to hold subscription and authentication information.</span></span> <span data-ttu-id="4adc5-105">複数のサブスクリプションがある場合は、Azure コンテキストを使用して、Azure PowerShell コマンドレットを実行するサブスクリプションを選択できます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-105">If you have more than one subscription, Azure contexts let you select the subscription to run Azure PowerShell cmdlets on.</span></span> <span data-ttu-id="4adc5-106">Azure コンテキストは、複数の PowerShell セッションにわたってサインイン情報を格納し、バックグラウンド タスクを実行するためにも使用されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-106">Azure contexts are also used to store sign-in information across multiple PowerShell sessions and run background tasks.</span></span>

<span data-ttu-id="4adc5-107">この記事では、サブスクリプションやアカウントの管理ではなく、Azure コンテキストの管理について説明します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-107">This article covers managing Azure contexts, not the management of subscriptions or accounts.</span></span> <span data-ttu-id="4adc5-108">ユーザー、サブスクリプション、テナント、またはその他のアカウント情報を管理する方法については、[Azure Active Directory](/azure/active-directory) のドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-108">If you're looking to manage users, subscriptions, tenants, or other account information, see the [Azure Active Directory](/azure/active-directory) documentation.</span></span> <span data-ttu-id="4adc5-109">コンテキストを使用してバックグラウンド タスクまたは並列タスクを実行する方法については、Azure コンテキストに慣れた後に [PowerShell ジョブでの Azure PowerShell コマンドレットの使用](using-psjobs.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-109">To learn about using contexts for running background or parallel tasks, see [Use Azure PowerShell cmdlets in PowerShell jobs](using-psjobs.md) after becoming familiar with Azure contexts.</span></span>

## <a name="overview-of-azure-context-objects"></a><span data-ttu-id="4adc5-110">Azure コンテキスト オブジェクトの概要</span><span class="sxs-lookup"><span data-stu-id="4adc5-110">Overview of Azure context objects</span></span>

<span data-ttu-id="4adc5-111">Azure コンテキストは、コマンドの実行対象のアクティブなサブスクリプションと、Azure クラウドに接続するために必要な認証情報を表す PowerShell オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="4adc5-111">Azure contexts are PowerShell objects representing your active subscription to run commands against, and the authentication information needed to connect to an Azure cloud.</span></span> <span data-ttu-id="4adc5-112">Azure コンテキストを使用すると、サブスクリプションを切り替えるたびに、Azure PowerShell でアカウントを再認証する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="4adc5-112">With Azure contexts, Azure PowerShell doesn't need to reauthenticate your account each time you switch subscriptions.</span></span> <span data-ttu-id="4adc5-113">Azure コンテキストは、次のもので構成されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-113">An Azure context consists of:</span></span>

* <span data-ttu-id="4adc5-114">[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) を使用して Azure にサインインするために使用された_アカウント_。</span><span class="sxs-lookup"><span data-stu-id="4adc5-114">The _account_ that was used to sign in to Azure with [Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount).</span></span> <span data-ttu-id="4adc5-115">Azure コンテキストでは、アカウントの観点からは、ユーザー、アプリケーション ID、およびサービス プリンシパルが同じものとして扱われます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-115">Azure contexts treat users, application IDs, and service principals the same from an account perspective.</span></span>
* <span data-ttu-id="4adc5-116">_テナント_に関連付けられたアクティブな_サブスクリプション_ (Azure リソースを作成および実行するための Microsoft とのサービス契約)。</span><span class="sxs-lookup"><span data-stu-id="4adc5-116">The active _subscription_, a service agreement with Microsoft to create and run Azure resources, which are associated with a _tenant_.</span></span> <span data-ttu-id="4adc5-117">多くの場合、テナントは、ドキュメント内で、または Active Directory を使用する場合に_組織_と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-117">Tenants are often referred to as _organizations_ in documentation or when working with Active Directory.</span></span>
* <span data-ttu-id="4adc5-118">_トークン キャッシュ_ (Azure クラウドへアクセスするための格納された認証トークン) への参照。</span><span class="sxs-lookup"><span data-stu-id="4adc5-118">A reference to a _token cache_, a stored authentication token for accessing an Azure cloud.</span></span> <span data-ttu-id="4adc5-119">このトークンの格納場所と保持期間は[コンテキスト自動保存設定](#save-azure-contexts-across-powershell-sessions)によって決定されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-119">Where this token is stored and how long it persists for is determined by the [context autosave settings](#save-azure-contexts-across-powershell-sessions).</span></span>

<span data-ttu-id="4adc5-120">これらの用語の詳細については、[Azure Active Directory の用語](/azure/active-directory/fundamentals/active-directory-whatis#terminology)に関するページをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-120">For more information on these terms, see [Azure Active Directory Terminology](/azure/active-directory/fundamentals/active-directory-whatis#terminology).</span></span> <span data-ttu-id="4adc5-121">Azure コンテキストによって使用される認証トークンは、永続セッションの一部である他の保存されたトークンと同じです。</span><span class="sxs-lookup"><span data-stu-id="4adc5-121">Authentication tokens used by Azure contexts are the same as other stored tokens that are part of a persistent session.</span></span> 

<span data-ttu-id="4adc5-122">`Connect-AzAccount` を使用してサインインすると、既定のサブスクリプションに対して少なくとも 1 つの Azure コンテキストが作成されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-122">When you sign in with `Connect-AzAccount`, at least one Azure context is created for your default subscription.</span></span> <span data-ttu-id="4adc5-123">`Connect-AzAccount` によって返されるオブジェクトは、残りの PowerShell セッションで使用される既定の Azure コンテキストです。</span><span class="sxs-lookup"><span data-stu-id="4adc5-123">The object returned by `Connect-AzAccount` is the default Azure context used for the rest of the PowerShell session.</span></span>

## <a name="get-azure-contexts"></a><span data-ttu-id="4adc5-124">Azure コンテキストを取得する</span><span class="sxs-lookup"><span data-stu-id="4adc5-124">Get Azure contexts</span></span>

<span data-ttu-id="4adc5-125">[Get-AzContext](/powershell/module/az.accounts/get-azcontext) コマンドレットを使用すると、使用可能な Azure コンテキストが取得されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-125">Available Azure contexts are retrieved with the [Get-AzContext](/powershell/module/az.accounts/get-azcontext) cmdlet.</span></span> <span data-ttu-id="4adc5-126">`-ListAvailable` を使用して使用可能なすべてのコンテキストを一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-126">List all of the available contexts with `-ListAvailable`:</span></span>

```azurepowershell-interactive
Get-AzContext -ListAvailable
```

<span data-ttu-id="4adc5-127">または、名前を指定してコンテキストを取得します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-127">Or get a context by name:</span></span>

```azurepowershell-interactive
$context = Get-AzContext -Name "mycontext"
```

<span data-ttu-id="4adc5-128">コンテキスト名は、関連付けられたサブスクリプションの名前とは異なる場合があります。</span><span class="sxs-lookup"><span data-stu-id="4adc5-128">Context names may be different from the name of the associated subscription.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4adc5-129">使用可能な Azure コンテキストが必ずしも使用可能なサブスクリプションであるとは__限りません__。</span><span class="sxs-lookup"><span data-stu-id="4adc5-129">The available Azure contexts __aren't__ always your available subscriptions.</span></span> <span data-ttu-id="4adc5-130">Azure コンテキストはローカルに保存された情報のみを表します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-130">Azure contexts only represent locally-stored information.</span></span> <span data-ttu-id="4adc5-131">[Get-AzSubscription](/powershell/module/Az.Accounts/Get-AzSubscription?view=azps-1.8.0) コマンドレットを使用すると、サブスクリプションを取得できます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-131">You can get your subscriptions with the [Get-AzSubscription](/powershell/module/Az.Accounts/Get-AzSubscription?view=azps-1.8.0) cmdlet.</span></span>

## <a name="create-a-new-azure-context-from-subscription-information"></a><span data-ttu-id="4adc5-132">サブスクリプション情報から新しい Azure コンテキストを作成する</span><span class="sxs-lookup"><span data-stu-id="4adc5-132">Create a new Azure context from subscription information</span></span>

<span data-ttu-id="4adc5-133">[Set-AzContext](/powershell/module/Az.Accounts/Set-AzContext) コマンドレットを使用して、新しい Azure コンテキストの作成と、アクティブ コンテキストとしての設定の両方を行います。</span><span class="sxs-lookup"><span data-stu-id="4adc5-133">The [Set-AzContext](/powershell/module/Az.Accounts/Set-AzContext) cmdlet is used to both create new Azure contexts and set them as the active context.</span></span>
<span data-ttu-id="4adc5-134">新しい Azure コンテキストを作成する最も簡単な方法は、既存のサブスクリプション情報を使用することです。</span><span class="sxs-lookup"><span data-stu-id="4adc5-134">The easiest way to create a new Azure context is to use existing subscription information.</span></span> <span data-ttu-id="4adc5-135">このコマンドレットは、`Get-AzSubscription` からの出力オブジェクトをパイプ値として受け取り、新しい Azure コンテキストを作成します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-135">The cmdlet is designed to take the output object from `Get-AzSubscription` as a piped value and configure a new Azure context:</span></span>

```azurepowershell-interactive
Get-AzSubscription -SubscriptionName 'MySubscriptionName' | Set-AzContext -Name 'MyContextName'
```

<span data-ttu-id="4adc5-136">または、サブスクリプション名または ID と必要に応じてテナント ID を指定します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-136">Or give the subscription name or ID and the tenant ID if necessary:</span></span>

```azurepowershell-interactive
Set-AzContext -Name 'MyContextName' -Subscription 'MySubscriptionName' -Tenant '.......'
```

<span data-ttu-id="4adc5-137">`-Name` 引数を省略すると、サブスクリプションの名前と ID が `Subscription Name (subscription-id)` の形式でコンテキスト名として使用されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-137">If the `-Name` argument is omitted, then the subscription's name and ID are used as the context name in the format `Subscription Name (subscription-id)`.</span></span>

## <a name="change-the-active-azure-context"></a><span data-ttu-id="4adc5-138">アクティブな Azure コンテキストを変更する</span><span class="sxs-lookup"><span data-stu-id="4adc5-138">Change the active Azure context</span></span>

<span data-ttu-id="4adc5-139">アクティブな Azure コンテキストを変更するには、`Set-AzContext` と [Select-AzContext](/powershell/module/az.accounts/set-azcontext) の両方を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-139">Both `Set-AzContext` and [Select-AzContext](/powershell/module/az.accounts/set-azcontext) can be used to change the active Azure context.</span></span> <span data-ttu-id="4adc5-140">[新しい Azure コンテキストの作成](#create-a-new-azure-context-from-subscription-information)に関するセクションで説明されているように、`Set-AzContext` を使用すると、サブスクリプションに対して新しい Azure コンテキストが作成され (存在しない場合)、それをアクティブ コンテキストとして使用するように切り替えられます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-140">As described in [Create a new Azure context](#create-a-new-azure-context-from-subscription-information), `Set-AzContext` creates a new Azure context for a subscription if one doesn't exist, and then switches to use that context as the active one.</span></span>

<span data-ttu-id="4adc5-141">`Select-AzContext` は、既存の Azure コンテキストでのみ使用されることが想定されており、`Set-AzContext -Context` と同じように動作しますが、パイプを使用するように設計されています。</span><span class="sxs-lookup"><span data-stu-id="4adc5-141">`Select-AzContext` is meant to be used with existing Azure contexts only and works similarly to using `Set-AzContext -Context`, but is designed for use with piping:</span></span>

```azurepowershell-interactive
Set-AzContext -Context $(Get-AzContext -Name "mycontext") # Set a context with an inline Azure context object
Get-AzContext -Name "mycontext" | Select-AzContext # Set a context with a piped Azure context object
```

<span data-ttu-id="4adc5-142">Azure PowerShell の他の多くのアカウントおよびコンテキスト管理コマンドと同様に、`Set-AzContext` と `Select-AzContext` では、コンテキストがアクティブになる期間を制御できるように `-Scope` 引数がサポートされています。</span><span class="sxs-lookup"><span data-stu-id="4adc5-142">Like many other account and context management commands in Azure PowerShell, `Set-AzContext` and `Select-AzContext` support the `-Scope` argument so that you can control how long the context is active.</span></span> <span data-ttu-id="4adc5-143">`-Scope` では、既定値を変更せずに、1 つのセッションのアクティブなコンテキストを変更できます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-143">`-Scope` lets you change a single session's active context without changing the default:</span></span>

```azurepowershell-interactive
Get-AzContext -Name "mycontext" | Select-AzContext -Scope Process
```

<span data-ttu-id="4adc5-144">PowerShell セッション全体のコンテキストを切り替えないようにするために、すべての PowerShell コマンドは `-AzContext` 引数を使用して、指定のコンテキストに対して実行できます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-144">To avoid switching contexts for a whole PowerShell session, all Azure PowerShell commands can be run against a given context with the `-AzContext` argument:</span></span>

```azurepowershell-interactive
$context = Get-AzContext -Name "mycontext"
New-AzVM -Name ExampleVM -AzContext $context
```

<span data-ttu-id="4adc5-145">Azure PowerShell コマンドレットでのコンテキストのもう 1 つの主な用途は、バックグラウンド コマンドを実行することです。</span><span class="sxs-lookup"><span data-stu-id="4adc5-145">The other main use of contexts with Azure PowerShell cmdlets is to run background commands.</span></span> <span data-ttu-id="4adc5-146">Azure PowerShell を使用した PowerShell ジョブの実行の詳細については、[PowerShell ジョブでの Azure PowerShell コマンドレットの実行](using-psjobs.md)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-146">To learn more about running PowerShell Jobs using Azure PowerShell, see [Run Azure PowerShell cmdlets in PowerShell Jobs](using-psjobs.md).</span></span>

## <a name="save-azure-contexts-across-powershell-sessions"></a><span data-ttu-id="4adc5-147">PowerShell セッション間での Azure コンテキストの保存</span><span class="sxs-lookup"><span data-stu-id="4adc5-147">Save Azure contexts across PowerShell sessions</span></span>

<span data-ttu-id="4adc5-148">既定では、Azure コンテキストは、PowerShell セッション間で使用するために保存されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-148">By default, Azure contexts are saved for use between PowerShell sessions.</span></span> <span data-ttu-id="4adc5-149">この動作は、次の方法で変更します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-149">You change this behavior in the following ways:</span></span>

* <span data-ttu-id="4adc5-150">`Connect-AzAccount` で `-Scope Process` を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="4adc5-150">Sign in using `-Scope Process` with `Connect-AzAccount`.</span></span>

  ```azurepowershell
  Connect-AzAccount -Scope Process
  ```

  <span data-ttu-id="4adc5-151">このサインインの一部として返される Azure コンテキストは、現在のセッションで_のみ_有効で、Azure PowerShell コンテキストの自動保存の設定に関係なく、自動的には保存されません。</span><span class="sxs-lookup"><span data-stu-id="4adc5-151">The Azure context returned as part of this sign in is valid for the current session _only_ and will not be automatically saved, regardless of the Azure PowerShell context autosave setting.</span></span>
* <span data-ttu-id="4adc5-152">[Disable-AzContextAutosave](/powershell/module/az.accounts/disable-azcontextautosave) コマンドレットを使用して、AzurePowershell のコンテキストの自動保存を無効にします。</span><span class="sxs-lookup"><span data-stu-id="4adc5-152">Disable AzurePowershell's context autosave with the [Disable-AzContextAutosave](/powershell/module/az.accounts/disable-azcontextautosave) cmdlet.</span></span>
  <span data-ttu-id="4adc5-153">コンテキストの自動保存を無効にしても、格納されているトークンはクリア__されません__。</span><span class="sxs-lookup"><span data-stu-id="4adc5-153">Disabling context autosave __doesn't__ clear any stored tokens.</span></span> <span data-ttu-id="4adc5-154">保存されている Azure コンテキスト情報をクリアする方法については、[Azure コンテキストと資格情報の削除](#remove-azure-contexts-and-stored-credentials)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-154">To learn how to clear stored Azure context information, see [Remove Azure contexts and credentials](#remove-azure-contexts-and-stored-credentials).</span></span>
* <span data-ttu-id="4adc5-155">Azure コンテキストの自動保存を明示的に有効にするには、[Enable-AzContextAutosave](/powershell/module/az.accounts/enable-azcontextautosave) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-155">Explicitly enable Azure context autosave can be enabled with the [Enable-AzContextAutosave](/powershell/module/az.accounts/enable-azcontextautosave) cmdlet.</span></span> <span data-ttu-id="4adc5-156">自動保存が有効になっていると、ユーザーのすべてのコンテキストは、後の PowerShell セッション用にローカルに保存されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-156">With autosave enabled, all of a user's contexts are stored locally for later PowerShell sessions.</span></span>
* <span data-ttu-id="4adc5-157">今後の PowerShell セッションで使用するために [Save-AzContext](/powershell/module/az.accounts/save-azcontext) を使用してコンテキストを手動で保存します。保存したコンテキストは、[Import-AzContext](/powershell/module/az.accounts/import-azcontext) を使用して読み込むことができます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-157">Manually save contexts with [Save-AzContext](/powershell/module/az.accounts/save-azcontext) to be used in future PowerShell sessions, where they can be loaded with [Import-AzContext](/powershell/module/az.accounts/import-azcontext):</span></span>

  ```azurepowershell
  Save-AzContext -Path current-context.json # Save the current context
  Save-AzContext -Profile $profileObject -Path other-context.json # Save a context object
  Import-AzContext -Path other-context.json # Load the context from a file and set it to the current context
  ```

> [!WARNING]
> <span data-ttu-id="4adc5-158">コンテキストの自動保存を無効にしても、保存されていた保存済みのコンテキスト情報はクリア__されません__。</span><span class="sxs-lookup"><span data-stu-id="4adc5-158">Disabling context autosave __doesn't__ clear any stored context information that was saved.</span></span> <span data-ttu-id="4adc5-159">保存されている情報を削除するには、[Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-159">To remove stored information, use the [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext) cmdlet.</span></span> <span data-ttu-id="4adc5-160">保存済みコンテキストの削除の詳細については、[コンテキストと資格情報の削除](#remove-azure-contexts-and-stored-credentials)に関する記事を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-160">For more on removing saved contexts, see [Remove contexts and credentials](#remove-azure-contexts-and-stored-credentials).</span></span>

<span data-ttu-id="4adc5-161">これらの各コマンドでは、`-Scope` パラメーターがサポートされています。これは、`Process` の値を取り、現在実行中のプロセスのみに適用することができます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-161">Each of these commands supports the `-Scope` parameter, which can take a value of `Process` to only apply to the current running process.</span></span> <span data-ttu-id="4adc5-162">たとえば、新しく作成されたコンテキストが PowerShell セッションを終了した後に保存されないようにするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4adc5-162">For example, to ensure that newly created contexts aren't saved after exiting a PowerShell session:</span></span>

```azurepowershell-interactive
Disable-AzContextAutosave -Scope Process
$context2 = Set-AzContext -Subscription "sub-id" -Tenant "other-tenant"
```

<span data-ttu-id="4adc5-163">コンテキスト情報とトークンは、Windows 上の `$env:USERPROFILE\.Azure` ディレクトリおよび他のプラットフォーム上の `$HOME/.Azure` に格納されます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-163">Context information and tokens are stored in the `$env:USERPROFILE\.Azure` directory on Windows, and on `$HOME/.Azure` on other platforms.</span></span> <span data-ttu-id="4adc5-164">サブスクリプション ID やテナント ID などの機密情報が、ログまたは保存されたコンテキストなどにより、まだ保存された情報に公開されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4adc5-164">Sensitive information such as subscription IDs and tenant IDs may still be exposed in stored information, through logs or saved contexts.</span></span> <span data-ttu-id="4adc5-165">保存されている情報をクリアする方法については、[コンテキストと資格情報の削除](#remove-azure-contexts-and-stored-credentials)に関するセクションを参照してください。</span><span class="sxs-lookup"><span data-stu-id="4adc5-165">To learn how to clear stored information, see the [Remove contexts and credentials](#remove-azure-contexts-and-stored-credentials) section.</span></span>

## <a name="remove-azure-contexts-and-stored-credentials"></a><span data-ttu-id="4adc5-166">Azure コンテキストと保存されている資格情報の削除</span><span class="sxs-lookup"><span data-stu-id="4adc5-166">Remove Azure contexts and stored credentials</span></span>

<span data-ttu-id="4adc5-167">Azure コンテキストと資格情報をクリアするには、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="4adc5-167">To clear Azure contexts and credentials:</span></span>

* <span data-ttu-id="4adc5-168">[Disconnect-AzAccount](/powershell/module/az.accounts/disconnect-azaccount) を使用してアカウントからサインアウトします。</span><span class="sxs-lookup"><span data-stu-id="4adc5-168">Sign out of an account with [Disconnect-AzAccount](/powershell/module/az.accounts/disconnect-azaccount).</span></span>
  <span data-ttu-id="4adc5-169">アカウントまたはコンテキストにより、任意のアカウントからサインアウトできます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-169">You can sign out of any account either by account or context:</span></span>

  ```azurepowershell-interactive
  Disconnect-AzAccount # Disconnect active account 
  Disconnect-AzAccount -Username "user@contoso.com" # Disconnect by account name

  Disconnect-AzAccount -ContextName "subscription2" # Disconnect by context name
  Disconnect-AzAccount -AzureContext $contextObject # Disconnect using context object information
  ```

  <span data-ttu-id="4adc5-170">切断すると、保存されている認証トークンが必ず削除され、切断されたユーザーまたはコンテキストに関連付けられている保存済みのコンテキストがクリアされます。</span><span class="sxs-lookup"><span data-stu-id="4adc5-170">Disconnecting always removes stored authentication tokens and clears saved contexts associated with the disconnected user or context.</span></span>
* <span data-ttu-id="4adc5-171">[Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext) を使用します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-171">Use [Clear-AzContext](/powershell/module/az.accounts/Clear-AzContext).</span></span> <span data-ttu-id="4adc5-172">このコマンドレットは、保存されているコンテキストと認証トークンを常に削除することが保証されており、さらにユーザーをサインアウトします。</span><span class="sxs-lookup"><span data-stu-id="4adc5-172">This cmdlet is guaranteed to always remove stored contexts and authentication tokens, and will also sign you out.</span></span>
* <span data-ttu-id="4adc5-173">[Remove-AzContext](/powershell/module/az.accounts/remove-azcontext) を使用してコンテキストを削除します。</span><span class="sxs-lookup"><span data-stu-id="4adc5-173">Remove a context with [Remove-AzContext](/powershell/module/az.accounts/remove-azcontext):</span></span>
  
  ```azurepowershell-interactive
  Remove-AzContext -Name "mycontext" # Remove by name
  Get-AzContext -Name "mycontext" | Remove-AzContext # Remove by piping Azure context object
  ```

  <span data-ttu-id="4adc5-174">アクティブなコンテキストを削除すると、Azure から切断され、`Connect-AzAccount` で再認証する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4adc5-174">If you remove the active context, you will be disconnected from Azure and need to reauthenticate with `Connect-AzAccount`.</span></span>

## <a name="see-also"></a><span data-ttu-id="4adc5-175">参照</span><span class="sxs-lookup"><span data-stu-id="4adc5-175">See also</span></span>

* [<span data-ttu-id="4adc5-176">PowerShell ジョブで Azure PowerShell コマンドレットを実行する</span><span class="sxs-lookup"><span data-stu-id="4adc5-176">Run Azure PowerShell cmdlets in PowerShell Jobs</span></span>](using-psjobs.md)
* [<span data-ttu-id="4adc5-177">Azure Active Directory 用語集</span><span class="sxs-lookup"><span data-stu-id="4adc5-177">Azure Active Directory Terminology</span></span>](/azure/active-directory/fundamentals/active-directory-whatis#terminology)
* [<span data-ttu-id="4adc5-178">Az.Accounts リファレンス</span><span class="sxs-lookup"><span data-stu-id="4adc5-178">Az.Accounts reference</span></span>](/powershell/module/az.accounts)
