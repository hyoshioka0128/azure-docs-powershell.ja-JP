---
title: Azure PowerShell のアンインストール
description: Azure PowerShell の完全アンインストールを実行する方法
ms.date: 06/20/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 92af0fdd8db451e2f0f092d66a3e296ad8d6a09e
ms.sourcegitcommit: fd11600079ee3844986552bccc4e274a231332b6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2018
ms.locfileid: "39368213"
---
# <a name="uninstall-the-azure-powershell-module"></a>Azure PowerShell モジュールのアンインストール

この記事では、古いバージョンの Azure PowerShell をアンインストールする (システムから完全に削除する) 方法について説明します。 Azure PowerShell を完全にアンインストールすることにした場合は、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用してフィードバックをお送りください。
バグが見つかった場合は、[GitHub で問題を報告](https://github.com/azure/azure-powershell/issues)していただきますよう、よろしくお願いいたします。

## <a name="uninstall-msi"></a>MSI のアンインストール

MSI パッケージを使用して Azure PowerShell をインストールした場合は、PowerShell ではなく Windows システムからアンインストールする必要があります。

| プラットフォーム | このサンプルについての指示 |
|----------|--------------|
| Windows 10 | [スタート] > [設定] > [アプリ] |
| Windows 7 </br>Windows 8 | [スタート] > [コントロール パネル] > [プログラム] > [プログラムのアンインストール] |

この画面のプログラムの一覧に [Azure PowerShell] が表示されたら、そこからアンインストールできます。

## <a name="uninstall-from-powershell"></a>PowerShell からのアンインストール

PowerShellGet を使用して Azure PowerShell をインストールした場合は、[Uninstall-Module](/powershell/module/powershellget/uninstall-module) コマンドレットを使用します。 ただし、`Uninstall-Module` でアンインストールされるモジュールは 1 つだけです。 Azure PowerShell を完全に削除するには、各モジュールを個別にアンインストールする必要があります。 複数のバージョンの Azure PowerShell がインストールされている場合、アンインストールが複雑になることがあります。

次のスクリプトは、1 つのバージョンの Azure PowerShell を完全に削除するときに使用できます。 このスクリプトでは、PowerShell ギャラリーに照会して依存サブモジュールの一覧を取得します。 次に、各サブモジュールの適切なバージョンがアンインストールされます。

```powershell
function Uninstall-AllModules {
  param(
    [Parameter(Mandatory=$true)]
    [string]$TargetModule,

    [Parameter(Mandatory=$true)]
    [string]$Version,

    [switch]$Force
  )

  $AllModules = @()

  'Creating list of dependencies...'
  $target = Find-Module $TargetModule -RequiredVersion $version
  $target.Dependencies | ForEach-Object {
    $AllModules += New-Object -TypeName psobject -Property @{name=$_.name; version=$_.requiredversion}
  }
  $AllModules += New-Object -TypeName psobject -Property @{name=$TargetModule; version=$Version}

  foreach ($module in $AllModules) {
    Write-Host ('Uninstalling {0} version {1}' -f $module.name,$module.version)
    try {
      Uninstall-Module -Name $module.name -RequiredVersion $module.version -Force:$Force -ErrorAction Stop
    } catch {
      Write-Host ("`t" + $_.Exception.Message)
    }
  }
}
```

この関数を使用するには、コードをコピーして PowerShell セッションに貼り付けます。 次の例は、関数を実行して古いバージョンの Azure PowerShell を削除する方法を示しています。

```powershell
Uninstall-AllModules -TargetModule AzureRM -Version 4.4.1 -Force
```

スクリプトを実行すると、アンインストールされる各サブモジュールの名前とバージョンが表示されます。

```output
Creating list of dependencies...
Uninstalling AzureRM.Profile version 3.4.1
Uninstalling Azure.Storage version 3.4.1
Uninstalling AzureRM.AnalysisServices version 0.4.7
Uninstalling Azure.AnalysisServices version 0.4.7
...
```

アンインストールする Azure PowerShell のバージョンごとにこのコマンドを実行します。
