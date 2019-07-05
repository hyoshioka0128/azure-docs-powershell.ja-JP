---
title: PowerShell セッション間で Azure の資格情報を保持する
description: 複数の PowerShell セッション間で Azure の資格情報や他の情報を再利用する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 02b8090aa1868f24445ddff3a95c0d0c376e2cb8
ms.sourcegitcommit: a4e527d3deba004007cfa22fa536e8255dd23b37
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "67516931"
---
# <a name="persist-azure-user-credentials-across-powershell-sessions"></a><span data-ttu-id="4003e-103">PowerShell セッション間で Azure のユーザー資格情報を保持する</span><span class="sxs-lookup"><span data-stu-id="4003e-103">Persist Azure user credentials across PowerShell sessions</span></span>

<span data-ttu-id="4003e-104">Azure PowerShell では、**Azure Context Autosave** と呼ばれる機能を提供しています。その機能は以下のとおりです。</span><span class="sxs-lookup"><span data-stu-id="4003e-104">Azure PowerShell offers a feature called **Azure Context Autosave**, which gives the following features:</span></span>

- <span data-ttu-id="4003e-105">新しい PowerShell セッションで再利用するためにサインイン情報を保持する。</span><span class="sxs-lookup"><span data-stu-id="4003e-105">Retention of sign-in information for reuse in new PowerShell sessions.</span></span>
- <span data-ttu-id="4003e-106">実行時間の長いコマンドレットを実行する場合にバックグラウンド タスクを使いやすくする。</span><span class="sxs-lookup"><span data-stu-id="4003e-106">Easier use of background tasks for executing long-running cmdlets.</span></span>
- <span data-ttu-id="4003e-107">個別のサインインを使用せずにアカウント、サブスクリプション、環境を切り替える。</span><span class="sxs-lookup"><span data-stu-id="4003e-107">Switch between accounts, subscriptions, and environments without a separate sign-in.</span></span>
- <span data-ttu-id="4003e-108">同一の PowerShell セッションから、異なる資格情報やサブスクリプションを同時に使用してタスクを実行する。</span><span class="sxs-lookup"><span data-stu-id="4003e-108">Execution of tasks using different credentials and subscriptions, simultaneously, from the same PowerShell session.</span></span>

## <a name="azure-contexts-defined"></a><span data-ttu-id="4003e-109">Azure コンテキストの定義</span><span class="sxs-lookup"><span data-stu-id="4003e-109">Azure contexts defined</span></span>

<span data-ttu-id="4003e-110">"*Azure コンテキスト*" とは、Azure PowerShell コマンドレットの対象を定義する一連の情報です。</span><span class="sxs-lookup"><span data-stu-id="4003e-110">An *Azure context* is a set of information that defines the target of Azure PowerShell cmdlets.</span></span> <span data-ttu-id="4003e-111">このコンテキストは、次の 5 つの要素で構成されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-111">The context consists of five parts:</span></span>

- <span data-ttu-id="4003e-112">"*アカウント*" - Azure との通信の認証に使用されるユーザー名またはサービス プリンシパル。</span><span class="sxs-lookup"><span data-stu-id="4003e-112">An *Account* - the UserName or Service Principal used to authenticate communications with Azure</span></span>
- <span data-ttu-id="4003e-113">"*サブスクリプション*" - 処理対象のリソースを含む Azure サブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="4003e-113">A *Subscription* - The Azure Subscription with the Resources being acted upon.</span></span>
- <span data-ttu-id="4003e-114">"*テナント*" - サブスクリプションを含む Azure Active Directory テナント。</span><span class="sxs-lookup"><span data-stu-id="4003e-114">A *Tenant* - The Azure Active Directory tenant that contains your subscription.</span></span> <span data-ttu-id="4003e-115">テナントは、サービス プリンシパル認証にとってより重要になります。</span><span class="sxs-lookup"><span data-stu-id="4003e-115">Tenants are more important to ServicePrincipal authentication.</span></span>
- <span data-ttu-id="4003e-116">"*環境*" - 対象となる特定の Azure クラウド (通常は Azure グローバル クラウド)。</span><span class="sxs-lookup"><span data-stu-id="4003e-116">An *Environment* - The particular Azure Cloud being targeted, usually the Azure global Cloud.</span></span>
  <span data-ttu-id="4003e-117">ただし、環境設定では、国内、政府、オンプレミス (Azure Stack) クラウドも対象にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4003e-117">However, the environment setting allows you to target National, Government, and on-premises (Azure Stack) clouds as well.</span></span>
- <span data-ttu-id="4003e-118">"*資格情報*" - 本人確認と Azure のリソースへのアクセスの承認のために Azure で使用される情報</span><span class="sxs-lookup"><span data-stu-id="4003e-118">*Credentials* - The information used by Azure to verify your identity and confirm your authorization to access resources in Azure</span></span>

<span data-ttu-id="4003e-119">Azure PowerShell の最新バージョンでは、新しい PowerShell セッションを開くたびに Azure コンテキストを自動的に保存できます。</span><span class="sxs-lookup"><span data-stu-id="4003e-119">With the latest version of Azure PowerShell, Azure Contexts can automatically be saved whenever opening a new PowerShell session.</span></span>

## <a name="automatically-save-the-context-for-the-next-sign-in"></a><span data-ttu-id="4003e-120">次回サインインのためのコンテキストの自動保存</span><span class="sxs-lookup"><span data-stu-id="4003e-120">Automatically save the context for the next sign-in</span></span>

<span data-ttu-id="4003e-121">Azure PowerShell では、セッション間で自動的にコンテキスト情報が保持されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-121">Azure PowerShell retains your context information automatically between sessions.</span></span> <span data-ttu-id="4003e-122">コンテキストと資格情報を記憶しないように PowerShell を設定するには、`Disable-AzContextAutoSave` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-122">To set PowerShell to forget your context and credentials, use `Disable-AzContextAutoSave`.</span></span> <span data-ttu-id="4003e-123">コンテキストの保存を無効にすると、PowerShell セッションを開くたびに Azure へのサインインが必要になります。</span><span class="sxs-lookup"><span data-stu-id="4003e-123">With context saving disabled, you'll need to sign in to Azure every time you open a PowerShell session.</span></span>

<span data-ttu-id="4003e-124">PowerShell セッションが終了した後に Azure PowerShell がコンテキストを記憶できるようにするには、`Enable-AzContextAutosave` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-124">To allow Azure PowerShell to remember your context after the PowerShell session is closed, use `Enable-AzContextAutosave`.</span></span> <span data-ttu-id="4003e-125">コンテキストと資格情報は、ユーザー ディレクトリの特殊な隠しフォルダー (Windows では `$env:USERPROFILE\.Azure`、その他のプラットフォームでは `$HOME/.Azure`) に自動的に保存されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-125">Context and credential information are automatically saved in a special hidden folder in your user directory (`$env:USERPROFILE\.Azure` on Windows, and `$HOME/.Azure` on other platforms).</span></span> <span data-ttu-id="4003e-126">新しい PowerShell セッションそれぞれで、最後のセッションで使用されたコンテキストが対象となります。</span><span class="sxs-lookup"><span data-stu-id="4003e-126">Each new PowerShell session targets the context used in your last session.</span></span>

<span data-ttu-id="4003e-127">Azure コンテキストを管理できるコマンドレットを使用すると、きめ細かな制御も可能になります。</span><span class="sxs-lookup"><span data-stu-id="4003e-127">The cmdlets that allow you to manage Azure contexts also allow you fine grained control.</span></span> <span data-ttu-id="4003e-128">変更を現在の PowerShell セッションのみ (`Process` スコープ) とすべての PowerShell セッション (`CurrentUser` スコープ) のどちらに適用するかを制御できます。</span><span class="sxs-lookup"><span data-stu-id="4003e-128">If you want changes to apply only to the current PowerShell session (`Process` scope) or every PowerShell session (`CurrentUser` scope).</span></span> <span data-ttu-id="4003e-129">これらのオプションについては、「[コンテキスト スコープの使用](#using-context-scopes)」で詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="4003e-129">These options are discussed in more detail in [Using Context Scopes](#using-context-scopes).</span></span>

## <a name="running-azure-powershell-cmdlets-as-background-jobs"></a><span data-ttu-id="4003e-130">バックグラウンド ジョブとしての Azure PowerShell コマンドレットの実行</span><span class="sxs-lookup"><span data-stu-id="4003e-130">Running Azure PowerShell cmdlets as background jobs</span></span>

<span data-ttu-id="4003e-131">**Azure Context Autosave** 機能を使用すると、コンテキストを PowerShell のバックグラウンド ジョブと共有することもできます。</span><span class="sxs-lookup"><span data-stu-id="4003e-131">The **Azure Context Autosave** feature also allows you to share you context with PowerShell background jobs.</span></span> <span data-ttu-id="4003e-132">PowerShell を使用すると、実行時間の長いタスクをバックグラウンド ジョブとして開始および監視できます。タスクが完了するのを待つ必要はありません。</span><span class="sxs-lookup"><span data-stu-id="4003e-132">PowerShell allows you to start and monitor long-executing tasks as background jobs without having to wait for the tasks to complete.</span></span> <span data-ttu-id="4003e-133">資格情報をバックグラウンド ジョブと共有するには、次の 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="4003e-133">You can share credentials with background jobs in two different ways:</span></span>

- <span data-ttu-id="4003e-134">コンテキストを引数として渡す</span><span class="sxs-lookup"><span data-stu-id="4003e-134">Passing the context as an argument</span></span>

  <span data-ttu-id="4003e-135">ほとんどの AzureRM コマンドレットでは、コンテキストをパラメーターとしてコマンドレットに渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="4003e-135">Most AzureRM cmdlets allow you to pass the context as a parameter to the cmdlet.</span></span> <span data-ttu-id="4003e-136">次の例に示すように、バックグラウンド ジョブにコンテキストを渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="4003e-136">You can pass a context to a background job as shown in the following example:</span></span>

  ```powershell-interactive
  PS C:\> $job = Start-Job { param ($ctx) New-AzVm -AzureRmContext $ctx [... Additional parameters ...]} -ArgumentList (Get-AzContext)
  ```

- <span data-ttu-id="4003e-137">自動保存を有効にした状態で既定のコンテキストを使用する</span><span class="sxs-lookup"><span data-stu-id="4003e-137">Using the default context with Autosave enabled</span></span>

  <span data-ttu-id="4003e-138">**Context Autosave** を有効にした場合、バックグラウンド ジョブは、既定で保存されているコンテキストを自動的に使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-138">If you have enabled **Context Autosave**, background jobs automatically use the default saved context.</span></span>

  ```powershell-interactive
  PS C:\> $job = Start-Job { New-AzVm [... Additional parameters ...]}
  ```

<span data-ttu-id="4003e-139">バックグラウンド タスクの結果を知っておく必要がある場合は、`Get-Job` を使用してジョブの状態を確認し、`Wait-Job` を使用してジョブの完了を待ちます。</span><span class="sxs-lookup"><span data-stu-id="4003e-139">When you need to know the outcome of the background task, use `Get-Job` to check the job status and `Wait-Job` to wait for the Job to complete.</span></span> <span data-ttu-id="4003e-140">バックグラウンド ジョブの出力をキャプチャまたは表示するには、`Receive-Job` を使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-140">Use `Receive-Job` to capture or display the output of the background job.</span></span> <span data-ttu-id="4003e-141">詳細については、「[about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4003e-141">For more information, see [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="creating-selecting-renaming-and-removing-contexts"></a><span data-ttu-id="4003e-142">コンテキストの作成、選択、名前変更、削除</span><span class="sxs-lookup"><span data-stu-id="4003e-142">Creating, selecting, renaming, and removing contexts</span></span>

<span data-ttu-id="4003e-143">コンテキストを作成するには、Azure にサインインしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4003e-143">To create a context, you must be signed in to Azure.</span></span> <span data-ttu-id="4003e-144">`Connect-AzAccount` コマンドレット (またはそのエイリアス `Login-AzAccount`) は、Azure PowerShell コマンドレットで使用される既定のコンテキストを設定し、資格情報で許可されているテナントまたはサブスクリプションへのアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="4003e-144">The `Connect-AzAccount` cmdlet (or its alias, `Login-AzAccount`) sets the default context used by Azure PowerShell cmdlets, and allows you to access any tenants or subscriptions allowed by your credentials.</span></span>

<span data-ttu-id="4003e-145">サインイン後に新しいコンテキストを追加するには、`Set-AzContext` (またはそのエイリアス `Select-AzSubscription`) を使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-145">To add a new context after sign-in, use `Set-AzContext` (or its alias, `Select-AzSubscription`).</span></span>

```azurepowershell-interactive
PS C:\> Set-AzContext -Subscription "Contoso Subscription 1" -Name "Contoso1"
```

<span data-ttu-id="4003e-146">前の例では、現在の資格情報を使用して、"Contoso Subscription 1" を対象とした新しいコンテキストを追加します。</span><span class="sxs-lookup"><span data-stu-id="4003e-146">The previous example adds a new context targeting 'Contoso Subscription 1' using your current credentials.</span></span> <span data-ttu-id="4003e-147">新しいコンテキストの名前は "Contoso1" です。</span><span class="sxs-lookup"><span data-stu-id="4003e-147">The new context is named 'Contoso1'.</span></span> <span data-ttu-id="4003e-148">コンテキストに名前を指定しない場合は、アカウント ID とサブスクリプション ID を使用した既定の名前が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-148">If you don't provide a name for the context, a default name, using the account ID and subscription ID is used.</span></span>

<span data-ttu-id="4003e-149">既存のコンテキストの名前を変更するには、`Rename-AzContext` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-149">To rename an existing context, use the `Rename-AzContext` cmdlet.</span></span> <span data-ttu-id="4003e-150">例:</span><span class="sxs-lookup"><span data-stu-id="4003e-150">For example:</span></span>

```azurepowershell-interactive
PS C:\> Rename-AzContext '[user1@contoso.org; 123456-7890-1234-564321]` 'Contoso2'
```

<span data-ttu-id="4003e-151">この例では、自動的に `[user1@contoso.org; 123456-7890-1234-564321]` という名前の付いたコンテキストの名前を簡単な名前 "Contoso2" に変更します。</span><span class="sxs-lookup"><span data-stu-id="4003e-151">This example renames the context with automatic name `[user1@contoso.org; 123456-7890-1234-564321]` to the simple name 'Contoso2'.</span></span> <span data-ttu-id="4003e-152">コンテキストを管理するコマンドレットではタブ補完も使用されているため、コンテキストをすばやく選択できます。</span><span class="sxs-lookup"><span data-stu-id="4003e-152">Cmdlets that manage contexts also use tab completion, allowing you to quickly select the context.</span></span>

<span data-ttu-id="4003e-153">最後に、コンテキストを削除するには、`Remove-AzContext` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-153">Finally, to remove a context, use the `Remove-AzContext` cmdlet.</span></span>  <span data-ttu-id="4003e-154">例:</span><span class="sxs-lookup"><span data-stu-id="4003e-154">For example:</span></span>

```azurepowershell-interactive
PS C:\> Remove-AzContext Contoso2
```

<span data-ttu-id="4003e-155">"Contoso2" という名前のコンテキストは記憶されません。</span><span class="sxs-lookup"><span data-stu-id="4003e-155">Forgets the context that was named 'Contoso2'.</span></span> <span data-ttu-id="4003e-156">`Set-AzContext` を使用して、このコンテキストを再作成できます</span><span class="sxs-lookup"><span data-stu-id="4003e-156">You can recreate this context using `Set-AzContext`</span></span>

## <a name="removing-credentials"></a><span data-ttu-id="4003e-157">資格情報の削除</span><span class="sxs-lookup"><span data-stu-id="4003e-157">Removing credentials</span></span>

<span data-ttu-id="4003e-158">`Disconnect-AzAccount` (別名 `Logout-AzAccount`) を使用して、ユーザーまたはサービス プリンシパルの資格情報と関連付けられたコンテキストをすべて削除できます。</span><span class="sxs-lookup"><span data-stu-id="4003e-158">You can remove all credentials and associated contexts for a user or service principal using `Disconnect-AzAccount` (also known as `Logout-AzAccount`).</span></span> <span data-ttu-id="4003e-159">`Disconnect-AzAccount` コマンドレットをパラメーターを指定せずに実行すると、現在のコンテキストのユーザーまたはサービス プリンシパルに関連付けられた資格情報とコンテキストがすべて削除されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-159">When executed without parameters, the `Disconnect-AzAccount` cmdlet removes all credentials and contexts associated with the User or Service Principal in the current context.</span></span> <span data-ttu-id="4003e-160">特定のプリンシパルを対象とするために、ユーザー名、サービス プリンシパル名、またはコンテキストを渡すこともできます。</span><span class="sxs-lookup"><span data-stu-id="4003e-160">You may pass in a Username, Service Principal Name, or context to target a particular principal.</span></span>

```azurepowershell-interactive
Disconnect-AzAccount user1@contoso.org
```

## <a name="using-context-scopes"></a><span data-ttu-id="4003e-161">コンテキスト スコープの使用</span><span class="sxs-lookup"><span data-stu-id="4003e-161">Using context scopes</span></span>

<span data-ttu-id="4003e-162">場合によっては、他のセッションに影響を与えることなく、PowerShell セッションでコンテキストを選択、変更、または削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="4003e-162">Occasionally, you may want to select, change, or remove a context in a PowerShell session without impacting other sessions.</span></span> <span data-ttu-id="4003e-163">コンテキストのコマンドレットの既定の動作を変更するには、`Scope` パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-163">To change the default behavior of context cmdlets, use the `Scope` parameter.</span></span> <span data-ttu-id="4003e-164">`Process` スコープは、現在のセッションのみに適用されるようにすることで、既定の動作をオーバーライドします。</span><span class="sxs-lookup"><span data-stu-id="4003e-164">The `Process` scope overrides the default behavior by making it apply only for the current session.</span></span> <span data-ttu-id="4003e-165">逆に、`CurrentUser` スコープは、現在のセッションだけでなく、すべてのセッションのコンテキストを変更します。</span><span class="sxs-lookup"><span data-stu-id="4003e-165">Conversely `CurrentUser` scope changes the context in all sessions, instead of just the current session.</span></span>

<span data-ttu-id="4003e-166">たとえば、他のウィンドウに影響を与えることなく現在の PowerShell セッションの既定のコンテキストを変更したり、次にセッションを開いたときに使用されるコンテキストを変更したりするには、次を使用します。</span><span class="sxs-lookup"><span data-stu-id="4003e-166">As an example, to change the default context in the current PowerShell session without impacting other windows, or the context used the next time a session is opened, use:</span></span>

```azurepowershell-interactive
PS C:\> Select-AzContext Contoso1 -Scope Process
```

## <a name="how-the-context-autosave-setting-is-remembered"></a><span data-ttu-id="4003e-167">コンテキストの自動保存設定を記憶する方法</span><span class="sxs-lookup"><span data-stu-id="4003e-167">How the context autosave setting is remembered</span></span>

<span data-ttu-id="4003e-168">コンテキストの自動保存設定は、ユーザーの Azure PowerShell ディレクトリ (Windows では `$env:USERPROFILE\.Azure`、その他のプラットフォームでは `$HOME/.Azure`) に保存されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-168">The context AutoSave setting is saved to the user Azure PowerShell directory (`$env:USERPROFILE\.Azure` on Windows, and `$HOME/.Azure` on other platforms).</span></span> <span data-ttu-id="4003e-169">コンピューター アカウントの中には、このディレクトリにアクセスできないものがあります。</span><span class="sxs-lookup"><span data-stu-id="4003e-169">Some kinds of computer accounts may not have access to this directory.</span></span> <span data-ttu-id="4003e-170">このようなシナリオでは、環境変数を使用できます。</span><span class="sxs-lookup"><span data-stu-id="4003e-170">For such scenarios, you can use the environment variable</span></span>

```azurepowershell-interactive
$env:AzureRmContextAutoSave="true" | "false"
```

<span data-ttu-id="4003e-171">"true" に設定すると、コンテキストは自動的に保存されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-171">When set to 'true', the context is automatically saved.</span></span> <span data-ttu-id="4003e-172">"false" に設定した場合、コンテキストは保存されません。</span><span class="sxs-lookup"><span data-stu-id="4003e-172">If set to 'false', the context isn't saved.</span></span>

## <a name="context-management-cmdlets"></a><span data-ttu-id="4003e-173">コンテキスト管理コマンドレット</span><span class="sxs-lookup"><span data-stu-id="4003e-173">Context management cmdlets</span></span>

- <span data-ttu-id="4003e-174">[Enable-AzContextAutosave][enable] - PowerShell セッション間でのコンテキストの保存を許可します。</span><span class="sxs-lookup"><span data-stu-id="4003e-174">[Enable-AzContextAutosave][enable] - Allow saving the context between powershell sessions.</span></span>
  <span data-ttu-id="4003e-175">変更するとグローバル コンテキストが変更されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-175">Any changes alter the global context.</span></span>
- <span data-ttu-id="4003e-176">[Disable-AzContextAutosave][disable] - コンテキストの自動保存をオフにします。</span><span class="sxs-lookup"><span data-stu-id="4003e-176">[Disable-AzContextAutosave][disable] - Turn off autosaving the context.</span></span> <span data-ttu-id="4003e-177">新しい PowerShell セッションごとに再度サインインが必要になります。</span><span class="sxs-lookup"><span data-stu-id="4003e-177">Each new PowerShell session is required to sign in again.</span></span>
- <span data-ttu-id="4003e-178">[Select-AzContext][select] - コンテキストを既定値として選択します。</span><span class="sxs-lookup"><span data-stu-id="4003e-178">[Select-AzContext][select] - Select a context as the default.</span></span> <span data-ttu-id="4003e-179">すべてのコマンドレットで、認証にこのコンテキストの資格情報が使用されます。</span><span class="sxs-lookup"><span data-stu-id="4003e-179">All cmdlets use the credentials in this context for authentication.</span></span>
- <span data-ttu-id="4003e-180">[Disconnect-AzAccount][remove-cred] - アカウントに関連付けられた資格情報とコンテキストをすべて削除します。</span><span class="sxs-lookup"><span data-stu-id="4003e-180">[Disconnect-AzAccount][remove-cred] - Remove all credentials and contexts associated with an account.</span></span>
- <span data-ttu-id="4003e-181">[Remove-AzContext][remove-context] - 名前付きコンテキストを削除します。</span><span class="sxs-lookup"><span data-stu-id="4003e-181">[Remove-AzContext][remove-context] - Remove a named context.</span></span>
- <span data-ttu-id="4003e-182">[Rename-AzContext][rename] - 既存のコンテキストの名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="4003e-182">[Rename-AzContext][rename] - Rename an existing context.</span></span>
- <span data-ttu-id="4003e-183">[Add-AzAccount][login] - サインインのスコープをプロセスまたは現在のユーザーにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="4003e-183">[Add-AzAccount][login] - Allow scoping of the sign-in to the process or the current user.</span></span>
  <span data-ttu-id="4003e-184">認証後に既定のコンテキストに名前を付けることができます。</span><span class="sxs-lookup"><span data-stu-id="4003e-184">Allow naming the default context after authentication.</span></span>
- <span data-ttu-id="4003e-185">[Import-AzContext][import] - サインインのスコープをプロセスまたは現在のユーザーにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="4003e-185">[Import-AzContext][import] - Allow scoping of the sign-in to the process or the current user.</span></span>
- <span data-ttu-id="4003e-186">[Set-AzContext][set-context] - 既存の名前付きコンテキストの選択と、プロセスまたは現在のユーザーへのスコープの変更を許可します。</span><span class="sxs-lookup"><span data-stu-id="4003e-186">[Set-AzContext][set-context] - Allow selection of existing named contexts, and scope changes to the process or current user.</span></span>

<!-- Hyperlinks -->
[enable]: /powershell/module/az.accounts/Enable-AzureRmContextAutosave
[disable]: /powershell/module/az.accounts/Disable-AzContextAutosave
[select]: /powershell/module/az.accounts/Select-AzContext
[remove-cred]: /powershell/module/az.accounts/Disconnect-AzAccount
[remove-context]: /powershell/module/az.accounts/Remove-AzContext
[rename]: /powershell/module/az.accounts/Rename-AzContext

<!-- Updated cmdlets -->
[login]: /powershell/module/az.accounts/Connect-AzAccount
[import]:  /powershell/module/az.accounts/Import-AzContext
[set-context]: /powershell/module/az.accounts/Set-AzContext
