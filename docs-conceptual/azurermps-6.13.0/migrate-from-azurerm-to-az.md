---
title: AzureRM から Az への Azure PowerShell スクリプトの移行
description: AzureRM モジュールから新しい Az モジュールにスクリプトを移行するための手順とツールについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/07/2018
ms.openlocfilehash: 720387ec1b23f10ddf2b153cf0705b2b6d1b7b82
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "52828724"
---
# <a name="migrate-from-azurerm-to-azure-powershell-az"></a>AzureRM から Azure PowerShell Az への移行

Az モジュールには AzureRM との機能パリティがありますが、より短く一貫性のあるコマンドレット名が使用されます。
AzureRM コマンドレット用に記述されたスクリプトは、新しいモジュールで自動的に機能するわけではありません。 移行を容易にするために、Az には AzureRM を使用する既存のスクリプトを実行できるようにするツールが用意されています。 新しいコマンド セットへの移行がないに越したことはありませんが、この記事は、新しいモジュールへの切り替えを開始する際に役立ちます。

## <a name="ensure-your-existing-scripts-work-with-the-latest-azurerm-release"></a>既存スクリプトが AzureRM の最新リリースで機能することを確認する

これは最も重要な手順です。 既存のスクリプトを実行し、AzureRM の "_最新_" リリース (__6.13.0__) で機能することを確認します。 スクリプトが機能しない場合は、必ず [AzureRM 移行ガイド](migration-guide.6.0.0.md)をお読みください。

## <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell Az モジュールをインストールする

最初の手順では、お使いのプラットフォームに Az モジュールをインストールします。 Az をインストールするには、AzureRM をアンインストールする必要があります。
次の手順では、既存のスクリプトを引き続き実行できるようにする方法と、古いコマンドレット名の互換性を有効にする方法について説明します。

Azure PowerShell Az モジュールをインストールするには、次の手順を実行します。

* [AzureRM モジュールをアンインストールする](uninstall-azurerm-ps.md)。 最新のバージョンだけでなく、インストールした "_すべて_" のバージョンの AzureRM を必ず削除します。
* [Az モジュールをインストールする](install-az-ps.md)

## <a name="a-namealiasesenable-azurerm-alias-mode"></a><a name="aliases"/>AzureRM 別名モードを有効にする

スクリプトが最新バージョンの AzureRM で機能し、AzureRM をアンインストールしたら、次は Az モジュールの互換モードを有効にします。 次のコマンドを使用して、互換性を有効にします。

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

別名を使用することによって、`Az` モジュールがインストールされた状態で、古いコマンドレット名を使用できるようになります。 これらの別名は、選択したスコープのユーザー プロファイルに書き込まれます。 ユーザー プロファイルが存在しない場合は、ユーザー プロファイルが作成されます。

> [!WARNING]
>
> このコマンドに別の `-Scope` を使用することができますが、これはお勧めしません。 別名は選択したスコープのユーザー プロファイルに書き込まれるので、できるだけ限られたスコープに対して有効にしてください。 別名をシステム全体で有効にすると、ローカル スコープに `AzureRM` をインストールしている他のユーザーに問題が生じることもあります。

別名モードを有効にしたら、、スクリプトを再度実行して、スクリプトが引き続き想定どおりに機能することを確認します。 

## <a name="change-module-imports-and-cmdlet-names"></a>モジュールのインポートとコマンドレット名を変更する

一般的に、モジュール名は `AzureRM` および `Azure` が `Az` になるように変更されています。また、コマンドレットについても同様です。
たとえば、`AzureRM.Compute` モジュールは名前が `Az.Compute` に変更されています。 `New-AzureRmVM` は `New-AzVM` になり、`Get-AzureStorageBlob` は `Get-AzStorageBlob` になっています。

この名前付けの変更には例外があるため、名前を変更する前に注意する必要があります。

| AzureRM モジュール | Az モジュール |
|----------------|-----------|
| AzureRM.DataFactories | Az.DataFactory |
| AzureRM.DataFactoryV2 | Az.DataFactory |
| AzureRM.RecoveryServices.Backup | Az.RecoveryServices |
| AzureRM.RecoveryServices.SiteRecovery | Az.RecoveryServices |

## <a name="summary"></a>まとめ

これらの手順に従うと、既存のスクリプトをすべて更新して、新しいモジュールを使用できるようになります。 これらの手順に関する質問や、移行を困難にしている問題がある場合は、手順を改善できるようにこの記事にコメントを追加してください。
