---
title: PowerShell セッション間でのユーザー ログインの保持
description: この記事では、複数の PowerShell セッション間で資格情報やその他のユーザー情報を再利用できるようにする、Azure PowerShell の新機能について説明します。
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 08/31/2017
ms.openlocfilehash: 8ef20796b64b16c78a653e293a57d5e752d89710
ms.sourcegitcommit: 15bf69bf95eceb936b3a429e741add95c308826a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/28/2018
---
# <a name="persisting-user-logins-across-powershell-sessions"></a><span data-ttu-id="ddb44-103">PowerShell セッション間でのユーザー ログインの保持</span><span class="sxs-lookup"><span data-stu-id="ddb44-103">Persisting user logins across PowerShell sessions</span></span>

<span data-ttu-id="ddb44-104">Azure PowerShell の 2017 年 9 月のリリースでは、Azure Resource Manager のコマンドレットに新機能として **Azure Context Autosave** が導入されました。</span><span class="sxs-lookup"><span data-stu-id="ddb44-104">In the September 2017 release of Azure PowerShell, Azure Resource Manager cmdlets introduce a new feature, **Azure Context Autosave**.</span></span> <span data-ttu-id="ddb44-105">この機能により、次のように、いくつかの新しいユーザー シナリオが可能になります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-105">This feature enables several new user scenarios, including:</span></span>

- <span data-ttu-id="ddb44-106">新しい PowerShell セッションで再利用するためにログイン情報を保持する。</span><span class="sxs-lookup"><span data-stu-id="ddb44-106">Retention of login information for reuse in new PowerShell sessions.</span></span>
- <span data-ttu-id="ddb44-107">実行時間の長いコマンドレットを実行する場合にバックグラウンド タスクを使いやすくする。</span><span class="sxs-lookup"><span data-stu-id="ddb44-107">Easier use of background tasks for executing long-running cmdlets.</span></span>
- <span data-ttu-id="ddb44-108">個別のログインを使用せずにアカウント、サブスクリプション、環境を切り替える。</span><span class="sxs-lookup"><span data-stu-id="ddb44-108">Switch between accounts, subscriptions, and environments without a separate login.</span></span>
- <span data-ttu-id="ddb44-109">同一の PowerShell セッションから、異なる資格情報やサブスクリプションを同時に使用してタスクを実行する。</span><span class="sxs-lookup"><span data-stu-id="ddb44-109">Execution of tasks using different credentials and subscriptions, simultaneously, from the same PowerShell session.</span></span>

## <a name="azure-contexts-defined"></a><span data-ttu-id="ddb44-110">Azure コンテキストの定義</span><span class="sxs-lookup"><span data-stu-id="ddb44-110">Azure contexts defined</span></span>

<span data-ttu-id="ddb44-111">"*Azure コンテキスト*" とは、Azure PowerShell コマンドレットの対象を定義する一連の情報です。</span><span class="sxs-lookup"><span data-stu-id="ddb44-111">An *Azure context* is a set of information that defines the target of Azure PowerShell cmdlets.</span></span> <span data-ttu-id="ddb44-112">このコンテキストは、次の 5 つの要素で構成されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-112">The context consists of five parts:</span></span>

- <span data-ttu-id="ddb44-113">"*アカウント*" - Azure との通信の認証に使用されるユーザー名またはサービス プリンシパル。</span><span class="sxs-lookup"><span data-stu-id="ddb44-113">An *Account* - the UserName or Service Principal used to authenticate communications with Azure</span></span>
- <span data-ttu-id="ddb44-114">"*サブスクリプション*" - 処理対象のリソースを含む Azure サブスクリプション。</span><span class="sxs-lookup"><span data-stu-id="ddb44-114">A *Subscription* - The Azure Subscription containing the Resources being acted upon.</span></span>
- <span data-ttu-id="ddb44-115">"*テナント*" - サブスクリプションを含む Azure Active Directory テナント。</span><span class="sxs-lookup"><span data-stu-id="ddb44-115">A *Tenant* - The Azure Active Directory tenant that contains your subscription.</span></span> <span data-ttu-id="ddb44-116">テナントは、サービス プリンシパル認証にとってより重要になります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-116">Tenants are more important to ServicePrincipal authentication.</span></span>
- <span data-ttu-id="ddb44-117">"*環境*" - 対象となる特定の Azure クラウド (通常は Azure グローバル クラウド)。</span><span class="sxs-lookup"><span data-stu-id="ddb44-117">An *Environment* - The particular Azure Cloud being targeted, usually the Azure global Cloud.</span></span>
  <span data-ttu-id="ddb44-118">ただし、環境設定では、国内、政府、オンプレミス (Azure Stack) クラウドも対象にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-118">However, the environment setting allows you to target National, Government, and on-premises (Azure Stack) clouds as well.</span></span>
- <span data-ttu-id="ddb44-119">"*資格情報*" - 本人確認と Azure のリソースへのアクセスの承認のために Azure で使用される情報。</span><span class="sxs-lookup"><span data-stu-id="ddb44-119">*Credentials* - The information used by Azure to verify your identity and ensure your authorization to access resources in Azure</span></span>

<span data-ttu-id="ddb44-120">以前のリリースでは、新しい PowerShell セッションを開くたびに Azure コンテキストを作成する必要がありました。</span><span class="sxs-lookup"><span data-stu-id="ddb44-120">In previous releases, your Azure Context had to be created each time you opened a new PowerShell session.</span></span> <span data-ttu-id="ddb44-121">Azure PowerShell v4.4.0 以降では、新しい PowerShell セッションを開くとすぐに Azure コンテキストの自動保存と再利用を有効にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-121">Beginning with Azure PowerShell v4.4.0, you can enable the automatic saving and reuse of Azure Contexts whenever you open a new PowerShell session.</span></span>

## <a name="automatically-saving-the-context-for-the-next-login"></a><span data-ttu-id="ddb44-122">次回ログインのためのコンテキストの自動保存</span><span class="sxs-lookup"><span data-stu-id="ddb44-122">Automatically saving the context for the next login</span></span>

<span data-ttu-id="ddb44-123">既定では、Azure PowerShell は PowerShell セッションを終了するたびにコンテキスト情報を破棄します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-123">By default, Azure PowerShell discards your context information whenever you close the PowerShell session.</span></span>

<span data-ttu-id="ddb44-124">PowerShell セッションが終了した後に Azure PowerShell がコンテキストを記憶できるようにするには、`Enable-AzureRmContextAutosave` を使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-124">To allow Azure PowerShell to remember your context after the PowerShell session is closed, use `Enable-AzureRmContextAutosave`.</span></span> <span data-ttu-id="ddb44-125">コンテキストと資格情報は、ユーザー ディレクトリの特殊な隠しフォルダー (`%AppData%\Roaming\Windows Azure PowerShell`) に自動的に保存されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-125">Context and credential information are automatically saved in a special hidden folder in your user directory (`%AppData%\Roaming\Windows Azure PowerShell`).</span></span>
<span data-ttu-id="ddb44-126">その後、新しい PowerShell セッションそれぞれで、最後のセッションで使用されたコンテキストが対象となります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-126">Subsequently, each new PowerShell session targets the context used in your last session.</span></span>

<span data-ttu-id="ddb44-127">コンテキストと資格情報を記憶しないように PowerShell を設定するには、`Disable-AzureRmContextAutoSave` を使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-127">To set PowerShell to forget your context and credentials, use `Disable-AzureRmContextAutoSave`.</span></span> <span data-ttu-id="ddb44-128">PowerShell セッションを開くたびに Azure へのログインが必要になります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-128">You will need to log in to Azure every time you open a PowerShell session.</span></span>

<span data-ttu-id="ddb44-129">Azure コンテキストを管理できるコマンドレットを使用すると、きめ細かな制御も可能になります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-129">The cmdlets that allow you to manage Azure contexts also allow you fine grained control.</span></span> <span data-ttu-id="ddb44-130">変更を現在の PowerShell セッションのみ (`Process` スコープ) とすべての PowerShell セッション (`CurrentUser` スコープ) のどちらに適用するかを制御できます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-130">If you want changes to apply only to the current PowerShell session (`Process` scope) or every PowerShell session (`CurrentUser` scope).</span></span> <span data-ttu-id="ddb44-131">これらのオプションについては、「[コンテキスト スコープの使用](#Using-Context-Scopes)」で詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-131">These options are discussed in mode detail in [Using Context Scopes](#Using-Context-Scopes).</span></span>

## <a name="running-azure-powershell-cmdlets-as-background-jobs"></a><span data-ttu-id="ddb44-132">バックグラウンド ジョブとしての Azure PowerShell コマンドレットの実行</span><span class="sxs-lookup"><span data-stu-id="ddb44-132">Running Azure PowerShell cmdlets as background jobs</span></span>

<span data-ttu-id="ddb44-133">**Azure Context Autosave** 機能を使用すると、コンテキストを PowerShell のバックグラウンド ジョブと共有することもできます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-133">The **Azure Context Autosave** feature also allows you to share you context with PowerShell background jobs.</span></span> <span data-ttu-id="ddb44-134">PowerShell を使用すると、実行時間の長いタスクをバックグラウンド ジョブとして開始および監視できます。タスクが完了するのを待つ必要はありません。</span><span class="sxs-lookup"><span data-stu-id="ddb44-134">PowerShell allows you to start and monitor long-executing tasks as background jobs without having to wait for the tasks to complete.</span></span> <span data-ttu-id="ddb44-135">資格情報をバックグラウンド ジョブと共有するには、次の 2 つの方法があります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-135">You can share credentials with background jobs in two different ways:</span></span>

- <span data-ttu-id="ddb44-136">コンテキストを引数として渡す</span><span class="sxs-lookup"><span data-stu-id="ddb44-136">Passing the context as an argument</span></span>

  <span data-ttu-id="ddb44-137">ほとんどの AzureRM コマンドレットでは、コンテキストをパラメーターとしてコマンドレットに渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-137">Most AzureRM cmdlets allow you to pass the context as a parameter to the cmdlet.</span></span> <span data-ttu-id="ddb44-138">次の例に示すように、バックグラウンド ジョブにコンテキストを渡すことができます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-138">You can pass a context to a background job as shown in the following example:</span></span>

  ```powershell
  PS C:\> $job = Start-Job { param ($ctx) New-AzureRmVm -AzureRmContext $ctx [... Additional parameters ...]} -ArgumentList (Get-AzureRmContext)
  ```

- <span data-ttu-id="ddb44-139">自動保存を有効にした状態で既定のコンテキストを使用する</span><span class="sxs-lookup"><span data-stu-id="ddb44-139">Using the default context with Autosave enabled</span></span>

  <span data-ttu-id="ddb44-140">**Context Autosave** を有効にした場合、バックグラウンド ジョブは、既定で保存されているコンテキストを自動的に使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-140">If you have enabled **Context Autosave**, background jobs automatically use the default saved context.</span></span>

  ```powershell
  PS C:\> $job = Start-Job { New-AzureRmVm [... Additional parameters ...]}
  ```

<span data-ttu-id="ddb44-141">バックグラウンド タスクの結果を知っておく必要がある場合は、`Get-Job` を使用してジョブの状態を確認し、`Wait-Job` を使用してジョブの完了を待ちます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-141">When you need to know the outcome of the background task, use `Get-Job` to check the job status and `Wait-Job` to wait for the Job to complete.</span></span> <span data-ttu-id="ddb44-142">バックグラウンド ジョブの出力をキャプチャまたは表示するには、`Receive-Job` を使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-142">Use `Receive-Job` to capture or display the output of the background job.</span></span> <span data-ttu-id="ddb44-143">詳細については、「[about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ddb44-143">For more information, see [about_Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="creating-selecting-renaming-and-removing-contexts"></a><span data-ttu-id="ddb44-144">コンテキストの作成、選択、名前変更、削除</span><span class="sxs-lookup"><span data-stu-id="ddb44-144">Creating, selecting, renaming, and removing contexts</span></span>

<span data-ttu-id="ddb44-145">コンテキストを作成するには、Azure にログインしている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-145">To create a context, you must be logged in to Azure.</span></span> <span data-ttu-id="ddb44-146">`Add-AzureRmAccount` コマンドレット (またはそのエイリアス `Login-AzureRmAccount`) は、後続の Azure PowerShell コマンドレットで使用される既定のコンテキストを設定し、ログイン資格情報で許可されているテナントまたはサブスクリプションへのアクセスを許可します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-146">The `Add-AzureRmAccount` cmdlet (or its alias, `Login-AzureRmAccount`) sets the default context used by subsequent Azure PowerShell cmdlets, and allows you to access any tenants or subscriptions allowed by your login credentials.</span></span>

<span data-ttu-id="ddb44-147">ログイン後に新しいコンテキストを追加するには、`Set-AzureRmContext` (またはそのエイリアス `Select-AzureRmSubscription`) を使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-147">To add a new context after login, use `Set-AzureRmContext` (or its alias, `Select-AzureRmSubscription`).</span></span>

```powershell
PS C:\> Set-AzureRMContext -Subscription "Contoso Subscription 1" -Name "Contoso1"
```

<span data-ttu-id="ddb44-148">前の例では、現在の資格情報を使用して、"Contoso Subscription 1" を対象とした新しいコンテキストを追加します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-148">The previous example adds a new context targeting 'Contoso Subscription 1' using your current credentials.</span></span> <span data-ttu-id="ddb44-149">新しいコンテキストの名前は "Contoso1" です。</span><span class="sxs-lookup"><span data-stu-id="ddb44-149">The new context is named 'Contoso1'.</span></span> <span data-ttu-id="ddb44-150">コンテキストに名前を指定しない場合は、アカウント ID とサブスクリプション ID を使用した既定の名前が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-150">If you do not provide a name for the context, a default name, using the account ID and subscription ID is used.</span></span>

<span data-ttu-id="ddb44-151">既存のコンテキストの名前を変更するには、`Rename-AzureRmContext` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-151">To rename an existing context, use the `Rename-AzureRmContext` cmdlet.</span></span> <span data-ttu-id="ddb44-152">例: </span><span class="sxs-lookup"><span data-stu-id="ddb44-152">For example:</span></span>

```powershell
PS C:\> Rename-AzureRmContext '[user1@contoso.org; 123456-7890-1234-564321]` 'Contoso2'
```

<span data-ttu-id="ddb44-153">この例では、自動的に `[user1@contoso.org; 123456-7890-1234-564321]` という名前の付いたコンテキストの名前を簡単な名前 "Contoso2" に変更します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-153">This example renames the context with automatic name `[user1@contoso.org; 123456-7890-1234-564321]` to the simple name 'Contoso2'.</span></span> <span data-ttu-id="ddb44-154">コンテキストを管理するコマンドレットではタブ補完も使用されているため、コンテキストをすばやく選択できます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-154">Cmdlets that manage contexts also use tab completion, allowing you to quickly select the context.</span></span>

<span data-ttu-id="ddb44-155">最後に、コンテキストを削除するには、`Remove-AzureRmContext` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-155">Finally, to remove a context, use the `Remove-AzureRmContext` cmdlet.</span></span>  <span data-ttu-id="ddb44-156">例: </span><span class="sxs-lookup"><span data-stu-id="ddb44-156">For example:</span></span>

```powershell
PS C:\> Remove-AzureRmContext Contoso2
```

<span data-ttu-id="ddb44-157">"Contoso2" という名前のコンテキストは記憶されません。</span><span class="sxs-lookup"><span data-stu-id="ddb44-157">Forgets the context that was named 'Contoso2'.</span></span> <span data-ttu-id="ddb44-158">その後、`Set-AzureRmContext` を使用して、このコンテキストを再作成できます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-158">You can recreate this context subsequently using `Set-AzureRmContext`</span></span>

## <a name="removing-credentials"></a><span data-ttu-id="ddb44-159">資格情報の削除</span><span class="sxs-lookup"><span data-stu-id="ddb44-159">Removing credentials</span></span>

<span data-ttu-id="ddb44-160">`Remove-AzureRmAccount` (別名 `Logout-AzureRmAccount`) を使用して、ユーザーまたはサービス プリンシパルの資格情報と関連付けられたコンテキストをすべて削除できます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-160">You can remove all credentials and associated contexts for a user or service principal using `Remove-AzureRmAccount` (also known as `Logout-AzureRmAccount`).</span></span> <span data-ttu-id="ddb44-161">`Remove-AzureRmAccount` コマンドレットをパラメーターを指定せずに実行すると、現在のコンテキストのユーザーまたはサービス プリンシパルに関連付けられた資格情報とコンテキストがすべて削除されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-161">When executed without parameters, the `Remove-AzureRmAccount` cmdlet removes all credentials and contexts associated with the User or Service Principal in the current context.</span></span> <span data-ttu-id="ddb44-162">特定のプリンシパルを対象とするために、ユーザー名、サービス プリンシパル名、またはコンテキストを渡すこともできます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-162">You may pass in a Username, Service Principal Name, or context to target a particular principal.</span></span>

```powershell
Remove-AzureRmAccount user1@contoso.org
```

## <a name="using-context-scopes"></a><span data-ttu-id="ddb44-163">コンテキスト スコープの使用</span><span class="sxs-lookup"><span data-stu-id="ddb44-163">Using context scopes</span></span>

<span data-ttu-id="ddb44-164">場合によっては、他のセッションに影響を与えることなく、PowerShell セッションでコンテキストを選択、変更、または削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-164">Occasionally, you may want to select, change, or remove a context in a PowerShell session without impacting other sessions.</span></span> <span data-ttu-id="ddb44-165">コンテキストのコマンドレットの既定の動作を変更するには、`Scope` パラメーターを使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-165">To change the default behavior of context cmdlets, use the `Scope` parameter.</span></span> <span data-ttu-id="ddb44-166">`Process` スコープは、現在のセッションのみに適用されるようにすることで、既定の動作を無視します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-166">The `Process` scope overrides the default behavior by making it apply only for the current session.</span></span> <span data-ttu-id="ddb44-167">逆に、`CurrentUser` スコープは、現在のセッションだけでなく、すべてのセッションのコンテキストを変更します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-167">Conversely `CurrentUser` scope changes the context in all sessions, instead of just the current session.</span></span>

<span data-ttu-id="ddb44-168">たとえば、他のウィンドウに影響を与えることなく現在の PowerShell セッションの既定のコンテキストを変更したり、次にセッションを開いたときに使用されるコンテキストを変更したりするには、次を使用します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-168">As an example, to change the default context in the current PowerShell session without impacting other windows, or the context used the next time a session is opened, use:</span></span>

```powershell
PS C:\> Select-AzureRmContext Contoso1 -Scope Process
```

## <a name="how-the-context-autosave-setting-is-remembered"></a><span data-ttu-id="ddb44-169">コンテキストの自動保存設定を記憶する方法</span><span class="sxs-lookup"><span data-stu-id="ddb44-169">How the context autosave setting is remembered</span></span>

<span data-ttu-id="ddb44-170">コンテキストの自動保存設定は、ユーザーの Azure PowerShell ディレクトリ (`%AppData%\Roaming\Windows Azure PowerShell`) に保存されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-170">The context AutoSave setting is saved to the user Azure PowerShell directory (`%AppData%\Roaming\Windows Azure PowerShell`).</span></span> <span data-ttu-id="ddb44-171">コンピューター アカウントの中には、このディレクトリにアクセスできないものがあります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-171">Some kinds of computer accounts may not have access to this directory.</span></span> <span data-ttu-id="ddb44-172">このようなシナリオでは、環境変数を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-172">For such scenarios, you can use the environment variable</span></span>

```powershell
$env:AzureRmContextAutoSave="true" | "false"
```

<span data-ttu-id="ddb44-173">"true" に設定した場合、コンテキストは自動的に保存されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-173">If set to 'true', the context is automatically saved.</span></span> <span data-ttu-id="ddb44-174">"false" に設定した場合、コンテキストは保存されません。</span><span class="sxs-lookup"><span data-stu-id="ddb44-174">If set to 'false', the context is not saved.</span></span>

## <a name="changes-to-the-azurermprofile-module"></a><span data-ttu-id="ddb44-175">AzureRM.Profile モジュールの変更点</span><span class="sxs-lookup"><span data-stu-id="ddb44-175">Changes to the AzureRM.Profile module</span></span>

<span data-ttu-id="ddb44-176">コンテキスト管理用の新しいコマンドレット</span><span class="sxs-lookup"><span data-stu-id="ddb44-176">New cmdlets for managing context</span></span>

- <span data-ttu-id="ddb44-177">[Enable-AzureRmContextAutosave][enable] - PowerShell セッション間でのコンテキストの保存を許可します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-177">[Enable-AzureRmContextAutosave][enable] - Allow saving the context between powershell sessions.</span></span>
  <span data-ttu-id="ddb44-178">変更するとグローバル コンテキストが変更されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-178">Any changes alter the global context.</span></span>
- <span data-ttu-id="ddb44-179">[Disable-AzureRmContextAutosave][disable] - コンテキストの自動保存をオフにします。</span><span class="sxs-lookup"><span data-stu-id="ddb44-179">[Disable-AzureRmContextAutosave][disable] - Turn off autosaving the context.</span></span> <span data-ttu-id="ddb44-180">新しい PowerShell セッションごとに再度ログインが必要になります。</span><span class="sxs-lookup"><span data-stu-id="ddb44-180">Each new PowerShell session is required to log in again.</span></span>
- <span data-ttu-id="ddb44-181">[Select-AzureRmContext][select] - コンテキストを既定値として選択します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-181">[Select-AzureRmContext][select] - Select a context as the default.</span></span> <span data-ttu-id="ddb44-182">後続のすべてのコマンドレットでは、認証にこのコンテキストの資格情報が使用されます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-182">All subsequent cmdlets use the credentials in this context for authentication.</span></span>
- <span data-ttu-id="ddb44-183">[Remove-AzureRmAccount][remove-cred] - アカウントに関連付けられた資格情報とコンテキストをすべて削除します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-183">[Remove-AzureRmAccount][remove-cred] - Remove all credentials and contexts associated with an account.</span></span>
- <span data-ttu-id="ddb44-184">[Remove-AzureRmContext][remove-context] - 名前付きコンテキストを削除します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-184">[Remove-AzureRmContext][remove-context] - Remove a named context.</span></span>
- <span data-ttu-id="ddb44-185">[Rename-AzureRmContext][rename] - 既存のコンテキストの名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-185">[Rename-AzureRmContext][rename] - Rename an existing context.</span></span>

<span data-ttu-id="ddb44-186">既存のプロファイル コマンドレットの変更</span><span class="sxs-lookup"><span data-stu-id="ddb44-186">Changes to existing profile cmdlets</span></span>

- <span data-ttu-id="ddb44-187">[Add-AzureRmAccount][login] - ログインのスコープをプロセスまたは現在のユーザーにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-187">[Add-AzureRmAccount][login] - Allow scoping of the login to the process or the current user.</span></span>
  <span data-ttu-id="ddb44-188">ログイン後に既定のコンテキストに名前を付けることができます。</span><span class="sxs-lookup"><span data-stu-id="ddb44-188">Allow naming the default context after login.</span></span>
- <span data-ttu-id="ddb44-189">[Import-AzureRmContext][import] - ログインのスコープをプロセスまたは現在のユーザーにすることを許可します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-189">[Import-AzureRmContext][import] - Allow scoping of the login to the process or the current user.</span></span>
- <span data-ttu-id="ddb44-190">[Set-AzureRmContext][set-context] - 既存の名前付きコンテキストの選択と、プロセスまたは現在のユーザーへのスコープの変更を許可します。</span><span class="sxs-lookup"><span data-stu-id="ddb44-190">[Set-AzureRmContext][set-context] - Allow selection of existing named contexts, and scope changes to the process or current user.</span></span>

<!-- Hyperlinks -->
[enable]: /powershell/module/azurerm.profile/Enable-AzureRmContextAutosave
[disable]: /powershell/module/azurerm.profile/Disable-AzureRmContextAutosave
[select]: /powershell/module/azurerm.profile/Select-AzureRmContext
[remove-cred]: /powershell/module/azurerm.profile/Remove-AzureRmAccount
[remove-context]: /powershell/module/azurerm.profile/Remove-AzureRmContext
[rename]: /powershell/module/azurerm.profile/Rename-AzureRmContext

<!-- Updated cmdlets -->
[login]: /powershell/module/azurerm.profile/Add-AzureRmAccount
[import]: /powershell/module/azurerm.profile/Import-AzureRmAccount
[set-context]: /powershell/module/azurerm.profile/Import-AzureRmContext
