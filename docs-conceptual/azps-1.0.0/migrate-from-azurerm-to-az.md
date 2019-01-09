---
title: AzureRM から Az への Azure PowerShell スクリプトの移行
description: AzureRM モジュールから新しい Az モジュールにスクリプトを移行するための手順とツールについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 12/13/2018
ms.openlocfilehash: 28122ca953d62b405f19effbbc680f2dc6202cca
ms.sourcegitcommit: 6685809f054203bd733c84f68acc69e53e5cca8c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/02/2019
ms.locfileid: "53982945"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>AzureRM から Azure PowerShell Az への移行

Az モジュールには AzureRM との機能パリティがありますが、より短く一貫性のあるコマンドレット名が使用されます。
AzureRM コマンドレット用に記述されたスクリプトは、新しいモジュールで自動的に機能するわけではありません。 移行を容易にするために、Az には AzureRM を使用する既存のスクリプトを実行できるようにするツールが用意されています。 新しいコマンド セットへの移行がないに越したことはありませんが、この記事は、新しいモジュールへの切り替えを開始する際に役立ちます。

AzureRM と Az の間の破壊的変更の完全な一覧については、「[Migration guide for Az 1.0.0 (Az 1.0.0 の移行ガイド)](migrate-az-1.0.0.md)」を参照してください。

## <a name="check-for-installed-versions-of-azurerm"></a>インストールされている AzureRM のバージョンを確認する

Az モジュールは AzureRM モジュールと同時にインストールできますが、これはお勧めしません。 移行手順を実行する前に、システムにインストールされている AzureRM のバージョンを確認します。 これにより、スクリプトが最新のリリースで既に実行中であることを確認し、AzureRM をアンインストールせずにコマンドの別名を有効にできるかどうかを把握することができます。

インストールされている AzureRM のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>既存スクリプトが AzureRM の最新リリースで機能することを確認する

これは最も重要な手順です。 既存のスクリプトを実行し、AzureRM の "_最新_" リリース (__6.13.1__) で機能することを確認します。 スクリプトが機能しない場合は、必ず [AzureRM 移行ガイド](/powershell/azure/azurerm/migration-guide.6.0.0)をお読みください。

## <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell Az モジュールをインストールする

最初の手順では、お使いのプラットフォームに Az モジュールをインストールします。 Az をインストールするときは、AzureRM をアンインストールすることをお勧めします。 次の手順では、既存のスクリプトを引き続き実行できるようにする方法と、古いコマンドレット名の互換性を有効にする方法について説明します。

Azure PowerShell Az モジュールをインストールするには、次の手順を実行します。

* __推奨__:[AzureRM モジュールをアンインストールする](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)。
  最新のバージョンだけでなく、インストールした "_すべて_" のバージョンの AzureRM を必ず削除します。
* [Az モジュールをインストールする](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-compatibility-aliases"></a><a name="aliases"/>AzureRM と互換性のある別名を有効にする 

> [!IMPORTANT]
>
> AzureRM の "_すべて_" のバージョンをアンインストールした場合のみ、互換モードを有効にしてください。 AzureRM コマンドレットがまだ使用できる状態で互換モードを有効にすると、予期しない動作が発生する可能性があります。 AzureRM をインストールしたままにする場合はこの手順をスキップしてください。ただし、AzureRM コマンドレットは、Az コマンドレットを呼び出さずに、古いモジュールを使用することに注意してください。

AzureRM をアンインストールして、スクリプトが最新バージョンの AzureRM で機能するようになったら、次の手順で Az モジュールの互換モードを有効にします。 次のコマンドを使用して、互換性を有効にします。

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

別名を使用することによって、Az モジュールがインストールされた状態で、古いコマンドレット名を使用できるようになります。 これらの別名は、選択したスコープのユーザー プロファイルに書き込まれます。 ユーザー プロファイルが存在しない場合は、ユーザー プロファイルが作成されます。

> [!WARNING]
>
> このコマンドに別の `-Scope` を使用することができますが、これはお勧めしません。 別名は選択したスコープのユーザー プロファイルに書き込まれるので、できるだけ限られたスコープに対して有効にしてください。 別名をシステム全体で有効にすると、ローカル スコープに AzureRM をインストールしている他のユーザーに問題が生じることもあります。

別名モードを有効にしたら、、スクリプトを再度実行して、スクリプトが引き続き想定どおりに機能することを確認します。 

## <a name="change-module-imports-and-cmdlet-names"></a>モジュールのインポートとコマンドレット名を変更する

一般的に、モジュール名は `AzureRM` および `Azure` が `Az` になるように変更されています。また、コマンドレットについても同様です。
たとえば、`AzureRM.Compute` モジュールは名前が `Az.Compute` に変更されています。 `New-AzureRMVM` は `New-AzVM` になり、`Get-AzureStorageBlob` は `Get-AzStorageBlob` になっています。

この名前付けの変更には例外があるため、注意する必要があります。 `AzureRM` または `Azure` から `Az` への変更以外に、一部のモジュールは、コマンドレットのサフィックスに影響を与えることなく、名前が変更されたか、既存のモジュールにマージされています。 それ以外の場合は、コマンドレットの完全なサフィックスは、新しいモジュール名を反映するように変更されました。

| AzureRM モジュール | Az モジュール | コマンドレットのサフィックスの変更 |
|----------------|-----------|------------------------|
| AzureRM.Profile | Az.Accounts | [はい] |
| AzureRM.Insights | Az.Monitor | [はい] |
| AzureRM.DataFactories | Az.DataFactory | [はい] |
| AzureRM.DataFactoryV2 | Az.DataFactory | [はい] |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices | いいえ  |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices | いいえ  |
| AzureRM.Tags | Az.Resources | いいえ  |
| AzureRM.MachineLearningCompute | Az.MachineLearning | いいえ  |
| AzureRM.UsageAggregates | Az.Billing | いいえ  |
| AzureRM.Consumption | Az.Billing | いいえ  |

## <a name="summary"></a>まとめ

これらの手順に従うと、既存のスクリプトをすべて更新して、新しいモジュールを使用できるようになります。 これらの手順に関する質問や、移行を困難にしている問題がある場合は、手順を改善できるようにこの記事にコメントを追加してください。
