---
title: PowerShell ジョブで Azure PowerShell コマンドレットを実行する
description: -AsJob と Start-Job を使用して、Azure PowerShell コマンドレットを並列で、またはバックグラウンド タスクとして実行する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/21/2019
ms.openlocfilehash: d74d3681794398534fe2c75a0c8fc314767ffa85
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "81740492"
---
# <a name="run-azure-powershell-cmdlets-in-powershell-jobs"></a><span data-ttu-id="767ad-103">PowerShell ジョブで Azure PowerShell コマンドレットを実行する</span><span class="sxs-lookup"><span data-stu-id="767ad-103">Run Azure PowerShell cmdlets in PowerShell Jobs</span></span>

<span data-ttu-id="767ad-104">Azure PowerShell は、Azure クラウドへの接続と応答の待機に依存します。そのため、これらのコマンドレットのほとんどは、クラウドからの応答を取得するまで PowerShell セッションをブロックします。</span><span class="sxs-lookup"><span data-stu-id="767ad-104">Azure PowerShell depends on connecting to an Azure cloud and waiting for responses, so most of these cmdlets block your PowerShell session until they get a response from the cloud.</span></span>
<span data-ttu-id="767ad-105">PowerShell ジョブを使用すると、1 つの PowerShell セッション内から、バックグラウンドでコマンドレットを実行したり、一度に複数のタスクを Azure で実行したりすることができます。</span><span class="sxs-lookup"><span data-stu-id="767ad-105">Powershell Jobs let you run cmdlets in the background or do multiple tasks on Azure at once, from inside a single PowerShell session.</span></span>

<span data-ttu-id="767ad-106">この記事では、Azure PowerShell コマンドレットを PowerShell ジョブとして実行し、完了を確認する方法について簡単に説明します。</span><span class="sxs-lookup"><span data-stu-id="767ad-106">This article is a brief overview of how to run Azure PowerShell cmdlets as PowerShell Jobs and check for completion.</span></span> <span data-ttu-id="767ad-107">Azure PowerShell でコマンドを実行するには Azure PowerShell コンテキストを使用する必要があります。詳細については、[Azure コンテキストとサインイン情報](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="767ad-107">Running commands in Azure PowerShell requires the use of Azure PowerShell contexts, which are covered in detail in [Azure contexts and sign-in credentials](context-persistence.md).</span></span>
<span data-ttu-id="767ad-108">PowerShell ジョブの詳細については、「[PowerShell ジョブについて](/powershell/module/microsoft.powershell.core/about/about_jobs)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="767ad-108">To learn more about PowerShell Jobs, see [About PowerShell Jobs](/powershell/module/microsoft.powershell.core/about/about_jobs).</span></span>

## <a name="azure-contexts-with-powershell-jobs"></a><span data-ttu-id="767ad-109">PowerShell ジョブでの Azure コンテキスト</span><span class="sxs-lookup"><span data-stu-id="767ad-109">Azure contexts with PowerShell jobs</span></span>

<span data-ttu-id="767ad-110">PowerShell ジョブは、PowerShell セッションがアタッチされていない個別のプロセスとして実行されるため、Azure の資格情報をそれらと共有する必要があります。</span><span class="sxs-lookup"><span data-stu-id="767ad-110">PowerShell Jobs are run as separate processes without an attached PowerShell session, so your Azure credentials must be shared with them.</span></span> <span data-ttu-id="767ad-111">資格情報は、次のいずれかの方法を使用して、Azure コンテキスト オブジェクトとして渡されます。</span><span class="sxs-lookup"><span data-stu-id="767ad-111">Credentials are passed as Azure context objects, using one of these methods:</span></span>

* <span data-ttu-id="767ad-112">自動的なコンテキストの永続化。</span><span class="sxs-lookup"><span data-stu-id="767ad-112">Automatic context persistence.</span></span> <span data-ttu-id="767ad-113">コンテキストの永続化は既定で有効になっており、サインイン情報が複数のセッションにわたって保持されます。</span><span class="sxs-lookup"><span data-stu-id="767ad-113">Context persistence is enabled by default and preserves your sign-in information across multiple sessions.</span></span> <span data-ttu-id="767ad-114">コンテキストの永続化が有効になっていると、現在の Azure コンテキストが新しいプロセスに渡されます。</span><span class="sxs-lookup"><span data-stu-id="767ad-114">With context persistence enabled, the current Azure context is passed to the new process:</span></span>

  ```azurepowershell-interactive
  Enable-AzContextAutosave # Enables context autosave if not already on
  $creds = Get-Credential
  $job = Start-Job { param($vmadmin) New-AzVM -Name MyVm -Credential $vmadmin } -ArgumentList $creds
  ```

* <span data-ttu-id="767ad-115">`-AzContext` パラメーターを任意の Azure PowerShell コマンドレットで使用して、Azure コンテキスト オブジェクトを提供します。</span><span class="sxs-lookup"><span data-stu-id="767ad-115">Use the `-AzContext` parameter with any Azure PowerShell cmdlets to provide an Azure context object:</span></span>

  ```azurepowershell-interactive
  $context = Get-AzContext -Name 'mycontext' # Get an Azure context object
  $creds = Get-Credential
  $job = Start-Job { param($context, $vmadmin) New-AzVM -Name MyVm -AzContext $context -Credential $vmadmin} -ArgumentList $context,$creds }
  ```

  <span data-ttu-id="767ad-116">コンテキストの永続化が無効になっている場合は、`-AzContext` 引数が必要です。</span><span class="sxs-lookup"><span data-stu-id="767ad-116">If context persistence is disabled, the `-AzContext` argument is required.</span></span>

* <span data-ttu-id="767ad-117">一部の Azure PowerShell コマンドレットによって提供される `-AsJob` スイッチを使用します。</span><span class="sxs-lookup"><span data-stu-id="767ad-117">Use the `-AsJob` switch provided by some Azure PowerShell cmdlets.</span></span> <span data-ttu-id="767ad-118">このスイッチは、現在アクティブな Azure コンテキストを使用して、コマンドレットを PowerShell ジョブとして自動的に開始します。</span><span class="sxs-lookup"><span data-stu-id="767ad-118">This switch automatically starts the cmdlet as a PowerShell Job, using the currently active Azure context:</span></span>

  ```azurepowershell-interactive
  $creds = Get-Credential
  $job = New-AzVM -Name MyVm -Credential $creds -AsJob
  ```

  <span data-ttu-id="767ad-119">コマンドレットが `-AsJob` をサポートしているかどうかを確認するには、そのリファレンス ドキュメントを参照してください。</span><span class="sxs-lookup"><span data-stu-id="767ad-119">To see if a cmdlet supports `-AsJob`, check its reference documentation.</span></span> <span data-ttu-id="767ad-120">`-AsJob` スイッチでは、コンテキストの自動保存が有効になっている必要はありません。</span><span class="sxs-lookup"><span data-stu-id="767ad-120">The `-AsJob` switch doesn't require context autosave to be enabled.</span></span>

<span data-ttu-id="767ad-121">[Get-Job](/powershell/module/microsoft.powershell.core/get-job) コマンドレットを使用して、実行中のジョブの状態を確認できます。</span><span class="sxs-lookup"><span data-stu-id="767ad-121">You can check the status of a running job with the [Get-Job](/powershell/module/microsoft.powershell.core/get-job) cmdlet.</span></span> <span data-ttu-id="767ad-122">ジョブからの現時点までの出力を取得するには、[Receive-Job](/powershell/module/microsoft.powershell.core/receive-job) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="767ad-122">To get the output from a job so far, use the [Receive-Job](/powershell/module/microsoft.powershell.core/receive-job) cmdlet.</span></span>

<span data-ttu-id="767ad-123">Azure で操作の進行状況をリモートで確認するには、ジョブによって変更されているリソースの種類に関連付けられている `Get-` コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="767ad-123">To check an operation's progress remotely on Azure, use the `Get-` cmdlets associated with the type of resource being modified by the job:</span></span>

```azurepowershell-interactive
$creds = Get-Credential
$context = Get-AzContext -Name 'mycontext'
$vmName = "MyVm"

$job = Start-Job { param($context, $vmName, $vmadmin) New-AzVM -Name $vmName -AzContext $context -Credential $vmadmin} -ArgumentList $context,$vmName,$creds }

Get-Job $job
Get-AzVM -Name $vmName
```

## <a name="see-also"></a><span data-ttu-id="767ad-124">参照</span><span class="sxs-lookup"><span data-stu-id="767ad-124">See Also</span></span>

* [<span data-ttu-id="767ad-125">Azure PowerShell のコンテキスト</span><span class="sxs-lookup"><span data-stu-id="767ad-125">Azure PowerShell contexts</span></span>](context-persistence.md)
* [<span data-ttu-id="767ad-126">PowerShell ジョブについて</span><span class="sxs-lookup"><span data-stu-id="767ad-126">About PowerShell Jobs</span></span>](/powershell/module/microsoft.powershell.core/about/about_jobs)
* [<span data-ttu-id="767ad-127">Get-Job のリファレンス</span><span class="sxs-lookup"><span data-stu-id="767ad-127">Get-Job reference</span></span>](/powershell/module/microsoft.powershell.core/get-job)
* [<span data-ttu-id="767ad-128">Receive-Job のリファレンス</span><span class="sxs-lookup"><span data-stu-id="767ad-128">Receive-Job reference</span></span>](/powershell/module/microsoft.powershell.core/receive-job)
