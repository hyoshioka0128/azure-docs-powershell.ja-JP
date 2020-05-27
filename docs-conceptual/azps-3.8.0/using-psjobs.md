---
title: PowerShell ジョブで Azure PowerShell コマンドレットを実行する
description: -AsJob と Start-Job を使用して、Azure PowerShell コマンドレットを並列で、またはバックグラウンド タスクとして実行する方法について説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.openlocfilehash: 36fcfc42fed91c5a0c8eff200c662e1e31cacfb9
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386852"
---
# <a name="run-azure-powershell-cmdlets-in-powershell-jobs"></a><span data-ttu-id="d931b-103">PowerShell ジョブで Azure PowerShell コマンドレットを実行する</span><span class="sxs-lookup"><span data-stu-id="d931b-103">Run Azure PowerShell cmdlets in PowerShell Jobs</span></span>

<span data-ttu-id="d931b-104">Azure PowerShell は、Azure クラウドへの接続と応答の待機に依存します。そのため、これらのコマンドレットのほとんどは、クラウドからの応答を取得するまで PowerShell セッションをブロックします。</span><span class="sxs-lookup"><span data-stu-id="d931b-104">Azure PowerShell depends on connecting to an Azure cloud and waiting for responses, so most of these cmdlets block your PowerShell session until they get a response from the cloud.</span></span>
<span data-ttu-id="d931b-105">PowerShell ジョブを使用すると、1 つの PowerShell セッション内から、バックグラウンドでコマンドレットを実行したり、一度に複数のタスクを Azure で実行したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="d931b-105">Powershell Jobs let you run cmdlets in the background or do multiple tasks on Azure at once, from inside a single PowerShell session.</span></span>

<span data-ttu-id="d931b-106">この記事では、Azure PowerShell コマンドレットを PowerShell ジョブとして実行し、完了を確認する方法について簡単に説明します。</span><span class="sxs-lookup"><span data-stu-id="d931b-106">This article is a brief overview of how to run Azure PowerShell cmdlets as PowerShell Jobs and check for completion.</span></span> <span data-ttu-id="d931b-107">Azure PowerShell でコマンドを実行するには Azure PowerShell コンテキストを使用する必要があります。詳細については、[Azure コンテキストとサインイン情報](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d931b-107">Running commands in Azure PowerShell requires the use of Azure PowerShell contexts, which are covered in detail in [Azure contexts and sign-in credentials](context-persistence.md).</span></span>
<span data-ttu-id="d931b-108">PowerShell ジョブの詳細については、「[PowerShell ジョブについて](/powershell/module/microsoft.powershell.core/about/about_jobs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d931b-108">To learn more about PowerShell Jobs, see [About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="azure-contexts-with-powershell-jobs"></a><span data-ttu-id="d931b-109">PowerShell ジョブでの Azure コンテキスト</span><span class="sxs-lookup"><span data-stu-id="d931b-109">Azure contexts with PowerShell jobs</span></span>

<span data-ttu-id="d931b-110">PowerShell ジョブは、PowerShell セッションがアタッチされていない個別のプロセスとして実行されるため、Azure の資格情報をそれらと共有する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d931b-110">PowerShell Jobs are run as separate processes without an attached PowerShell session, so your Azure credentials must be shared with them.</span></span> <span data-ttu-id="d931b-111">資格情報は、次のいずれかの方法を使用して、Azure コンテキスト オブジェクトとして渡されます。</span><span class="sxs-lookup"><span data-stu-id="d931b-111">Credentials are passed as Azure context objects, using one of these methods:</span></span>

* <span data-ttu-id="d931b-112">自動的なコンテキストの永続化。</span><span class="sxs-lookup"><span data-stu-id="d931b-112">Automatic context persistence.</span></span> <span data-ttu-id="d931b-113">コンテキストの永続化は既定で有効になっており、サインイン情報が複数のセッションにわたって保持されます。</span><span class="sxs-lookup"><span data-stu-id="d931b-113">Context persistence is enabled by default and preserves your sign-in information across multiple sessions.</span></span> <span data-ttu-id="d931b-114">コンテキストの永続化が有効になっていると、現在の Azure コンテキストが新しいプロセスに渡されます。</span><span class="sxs-lookup"><span data-stu-id="d931b-114">With context persistence enabled, the current Azure context is passed to the new process:</span></span>

  ```azurepowershell-interactive
  Enable-AzContextAutosave # Enables context autosave if not already on
  $creds = Get-Credential
  $job = Start-Job { param($vmadmin) New-AzVM -Name MyVm -Credential $vmadmin } -ArgumentList $creds
  ```

* <span data-ttu-id="d931b-115">`-AzContext` パラメーターを任意の Azure PowerShell コマンドレットで使用して、Azure コンテキスト オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="d931b-115">Use the `-AzContext` parameter with any Azure PowerShell cmdlets to provide an Azure context object:</span></span>

  ```azurepowershell-interactive
  $context = Get-AzContext -Name 'mycontext' # Get an Azure context object
  $creds = Get-Credential
  $job = Start-Job { param($context, $vmadmin) New-AzVM -Name MyVm -AzContext $context -Credential $vmadmin} -ArgumentList $context,$creds }
  ```

  <span data-ttu-id="d931b-116">コンテキストの永続化が無効になっている場合は、`-AzContext` 引数が必要です。</span><span class="sxs-lookup"><span data-stu-id="d931b-116">If context persistence is disabled, the `-AzContext` argument is required.</span></span>

* <span data-ttu-id="d931b-117">一部の Azure PowerShell コマンドレットによって提供される `-AsJob` スイッチを使用します。</span><span class="sxs-lookup"><span data-stu-id="d931b-117">Use the `-AsJob` switch provided by some Azure PowerShell cmdlets.</span></span> <span data-ttu-id="d931b-118">このスイッチは、現在アクティブな Azure コンテキストを使用して、コマンドレットを PowerShell ジョブとして自動的に開始します。</span><span class="sxs-lookup"><span data-stu-id="d931b-118">This switch automatically starts the cmdlet as a PowerShell Job, using the currently active Azure context:</span></span>

  ```azurepowershell-interactive
  $creds = Get-Credential
  $job = New-AzVM -Name MyVm -Credential $creds -AsJob
  ```

  <span data-ttu-id="d931b-119">コマンドレットが `-AsJob` をサポートしているかどうかを確認するには、そのリファレンス ドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="d931b-119">To see if a cmdlet supports `-AsJob`, check its reference documentation.</span></span> <span data-ttu-id="d931b-120">`-AsJob` スイッチでは、コンテキストの自動保存が有効になっている必要はありません。</span><span class="sxs-lookup"><span data-stu-id="d931b-120">The `-AsJob` switch doesn't require context autosave to be enabled.</span></span>

<span data-ttu-id="d931b-121">[Get-Job](/powershell/module/microsoft.powershell.core/get-job) コマンドレットを使用して、実行中のジョブの状態を確認できます。</span><span class="sxs-lookup"><span data-stu-id="d931b-121">You can check the status of a running job with the [Get-Job](/powershell/module/microsoft.powershell.core/get-job) cmdlet.</span></span> <span data-ttu-id="d931b-122">ジョブからの現時点までの出力を取得するには、[Receive-Job](/powershell/module/microsoft.powershell.core/receive-job) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="d931b-122">To get the output from a job so far, use the [Receive-Job](/powershell/module/microsoft.powershell.core/receive-job) cmdlet.</span></span>

<span data-ttu-id="d931b-123">Azure で操作の進行状況をリモートで確認するには、ジョブによって変更されているリソースの種類に関連付けられている `Get-` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="d931b-123">To check an operation's progress remotely on Azure, use the `Get-` cmdlets associated with the type of resource being modified by the job:</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$context = Get-AzContext -Name 'mycontext'
$vmName = "MyVm"

$job = Start-Job { param($context, $vmName, $vmadmin) New-AzVM -Name $vmName -AzContext $context -Credential $vmadmin} -ArgumentList $context,$vmName,$creds }

Get-Job $job
Get-AzVM -Name $vmName
```

## <a name="see-also"></a><span data-ttu-id="d931b-124">参照</span><span class="sxs-lookup"><span data-stu-id="d931b-124">See Also</span></span>

* [<span data-ttu-id="d931b-125">Azure PowerShell のコンテキスト</span><span class="sxs-lookup"><span data-stu-id="d931b-125">Azure PowerShell contexts</span></span>](context-persistence.md)
* [<span data-ttu-id="d931b-126">PowerShell ジョブについて</span><span class="sxs-lookup"><span data-stu-id="d931b-126">About PowerShell Jobs</span></span>](/powershell/module/microsoft.powershell.core/about/about_jobs)
* [<span data-ttu-id="d931b-127">Get-Job のリファレンス</span><span class="sxs-lookup"><span data-stu-id="d931b-127">Get-Job reference</span></span>](/powershell/module/microsoft.powershell.core/get-job)
* [<span data-ttu-id="d931b-128">Receive-Job のリファレンス</span><span class="sxs-lookup"><span data-stu-id="d931b-128">Receive-Job reference</span></span>](/powershell/module/microsoft.powershell.core/receive-job)
