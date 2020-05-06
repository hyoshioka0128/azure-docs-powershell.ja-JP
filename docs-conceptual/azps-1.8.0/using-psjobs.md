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
ms.locfileid: "72791486"
---
# <a name="run-azure-powershell-cmdlets-in-powershell-jobs"></a>PowerShell ジョブで Azure PowerShell コマンドレットを実行する

Azure PowerShell は、Azure クラウドへの接続と応答の待機に依存します。そのため、これらのコマンドレットのほとんどは、クラウドからの応答を取得するまで PowerShell セッションをブロックします。
PowerShell ジョブを使用すると、1 つの PowerShell セッション内から、バックグラウンドでコマンドレットを実行したり、一度に複数のタスクを Azure で実行したりすることができます。

この記事では、Azure PowerShell コマンドレットを PowerShell ジョブとして実行し、完了を確認する方法について簡単に説明します。 Azure PowerShell でコマンドを実行するには Azure PowerShell コンテキストを使用する必要があります。詳細については、[Azure コンテキストとサインイン情報](context-persistence.md)に関する記事をご覧ください。
PowerShell ジョブの詳細については、「[PowerShell ジョブについて](/powershell/module/microsoft.powershell.core/about/about_jobs)」を参照してください。

## <a name="azure-contexts-with-powershell-jobs"></a>PowerShell ジョブでの Azure コンテキスト

PowerShell ジョブは、PowerShell セッションがアタッチされていない個別のプロセスとして実行されるため、Azure の資格情報をそれらと共有する必要があります。 資格情報は、次のいずれかの方法を使用して、Azure コンテキスト オブジェクトとして渡されます。

* 自動的なコンテキストの永続化。 コンテキストの永続化は既定で有効になっており、サインイン情報が複数のセッションにわたって保持されます。 コンテキストの永続化が有効になっていると、現在の Azure コンテキストが新しいプロセスに渡されます。

  ```azurepowershell-interactive
  Enable-AzContextAutosave # Enables context autosave if not already on
  $creds = Get-Credential
  $job = Start-Job { param($vmadmin) New-AzVM -Name MyVm -Credential $vmadmin } -ArgumentList $creds
  ```

* `-AzContext` パラメーターを任意の Azure PowerShell コマンドレットで使用して、Azure コンテキスト オブジェクトを提供します。

  ```azurepowershell-interactive
  $context = Get-AzContext -Name 'mycontext' # Get an Azure context object
  $creds = Get-Credential
  $job = Start-Job { param($context, $vmadmin) New-AzVM -Name MyVm -AzContext $context -Credential $vmadmin} -ArgumentList $context,$creds }
  ```

  コンテキストの永続化が無効になっている場合は、`-AzContext` 引数が必要です。

* 一部の Azure PowerShell コマンドレットによって提供される `-AsJob` スイッチを使用します。 このスイッチは、現在アクティブな Azure コンテキストを使用して、コマンドレットを PowerShell ジョブとして自動的に開始します。

  ```azurepowershell-interactive
  $creds = Get-Credential
  $job = New-AzVM -Name MyVm -Credential $creds -AsJob
  ```

  コマンドレットが `-AsJob` をサポートしているかどうかを確認するには、そのリファレンス ドキュメントを参照してください。 `-AsJob` スイッチでは、コンテキストの自動保存が有効になっている必要はありません。

[Get-Job](/powershell/module/microsoft.powershell.core/get-job) コマンドレットを使用して、実行中のジョブの状態を確認できます。 ジョブからの現時点までの出力を取得するには、[Receive-Job](/powershell/module/microsoft.powershell.core/receive-job) コマンドレットを使用します。

Azure で操作の進行状況をリモートで確認するには、ジョブによって変更されているリソースの種類に関連付けられている `Get-` コマンドレットを使用します。

```azurepowershell-interactive
$creds = Get-Credential
$context = Get-AzContext -Name 'mycontext'
$vmName = "MyVm"

$job = Start-Job { param($context, $vmName, $vmadmin) New-AzVM -Name $vmName -AzContext $context -Credential $vmadmin} -ArgumentList $context,$vmName,$creds }

Get-Job $job
Get-AzVM -Name $vmName
```

## <a name="see-also"></a>参照

* [Azure PowerShell のコンテキスト](context-persistence.md)
* [PowerShell ジョブについて](/powershell/module/microsoft.powershell.core/about/about_jobs)
* [Get-Job のリファレンス](/powershell/module/microsoft.powershell.core/get-job)
* [Receive-Job のリファレンス](/powershell/module/microsoft.powershell.core/receive-job)
