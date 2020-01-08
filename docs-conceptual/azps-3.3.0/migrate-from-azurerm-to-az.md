---
title: AzureRM から Az への Azure PowerShell スクリプトの移行
description: AzureRM モジュールから新しい Az モジュールにスクリプトを移行するための手順とツールについて説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/10/2019
ms.openlocfilehash: 02b39653ebb4aa0f74d2340a7be7b35e08d5e44d
ms.sourcegitcommit: 2d0c3ffaa5246f680784fa7e15b0d2536c27ff80
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/07/2020
ms.locfileid: "75720525"
---
# <a name="migrate-azure-powershell-from-azurerm-to-az"></a>AzureRM から Az への Azure PowerShell の移行

Az モジュールには AzureRM との機能パリティがありますが、より短く一貫性のあるコマンドレット名が使用されます。
AzureRM コマンドレット用に記述されたスクリプトは、新しいモジュールで自動的に機能するわけではありません。 移行を容易にするために、Az には AzureRM を使用する既存のスクリプトを実行できるようにするツールが用意されています。 新しいコマンド セットへの移行がないに越したことはありませんが、この記事は、新しいモジュールへの切り替えを開始する際に役立ちます。

AzureRM と Az の間の重大な変更の詳細な一覧については、[AzureRM から Az への詳細な変更](migrate-az-1.0.0.md)を参照してください。

## <a name="ensure-existing-scripts-work-with-the-latest-azurerm-release"></a>既存のスクリプトが AzureRM の最新リリースで機能することを確認する

移行手順を実行する前に、システムにインストールされている AzureRM のバージョンを確認します。 これにより、スクリプトが最新のリリースで既に実行中であることを確認し、アンインストールする必要のある AzureRM のバージョンを把握することができます。

インストールされている AzureRM のバージョンを確認するには、次のコマンドを実行します。

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

AzureRM の__最新__の一般公開リリースは __6.13.1__ です。 このバージョンがインストールされていない場合、既存のスクリプトでは、ここと[重大な変更の一覧](migrate-az-1.0.0.md)で説明しているもの以外の Az モジュールを操作するための追加の変更が必要になる場合があります。

スクリプトが AzureRM 6.13.1 で機能しない場合は、[AzureRM 5.x から 6.x への移行ガイド](/powershell/azure/azurerm/migration-guide.6.0.0)に従ってそれらを更新します。
以前のバージョンの AzureRM モジュールを使用している場合は、各メジャー バージョン用に利用できる移行ガイドがあります。

## <a name="uninstall-azurerm"></a>AzureRM のアンインストール

Az モジュールは、Windows 用の PowerShell 5.1 の既存の AzureRM インストールとの互換性が保証されていません。 Az モジュールをインストールする前に、[AzureRM をアンインストール](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)してください。

> [!IMPORTANT]
>
> AzureRM モジュールをシステムから削除する準備ができていない場合は、代わりに [PowerShell Core](/powershell/scripting/install/installing-powershell-core-on-windows) 6.x 以降用の Az モジュールをインストールできます。 PowerShell Core と Windows 用の PowerShell 5.1 は別のモジュール ライブラリを使用するため、競合することはありません。 PowerShell Core で引き続き[エイリアスを有効にする](#enable-azurerm-compatibility-aliases)ことができます。

## <a name="install-the-azure-powershell-az-module"></a>Azure PowerShell Az モジュールをインストールする

最初の手順では、お使いのプラットフォームに Az モジュールをインストールします。 Az をインストールするときは、AzureRM をアンインストールすることをお勧めします。 次の手順では、既存のスクリプトを引き続き実行できるようにする方法と、古いコマンドレット名の互換性を有効にする方法について説明します。

Azure PowerShell モジュールをインストールするには、「[Az モジュールのインストール](install-az-ps.md)」の手順に従ってください。

> [!NOTE]
> この時点で、Az モジュールに用意されている [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) コマンドレットを実行したい場合は、すべてのバージョンの AzureRM がアンインストールされていて、競合が発生することがないことだけ確認してください。

## <a name="enable-azurerm-compatibility-aliases"></a>AzureRM と互換性のあるエイリアスを有効にする

AzureRM をアンインストールして、スクリプトが最新バージョンの AzureRM で機能するようになったら、次の手順で Az モジュールの互換モードを有効にします。 次のコマンドを使用して、互換性を有効にします。

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

別名を使用することによって、Az モジュールがインストールされた状態で、古いコマンドレット名を使用できるようになります。 これらのエイリアスは、選択したスコープのプロファイルに書き込まれます。 プロファイルが存在しない場合は、作成されます。
`CurrentUser` よりも範囲が広い `-Scope` を使用する場合は、対応するプロファイル ファイルを作成または更新するための適切な権限が必要です。

> [!IMPORTANT]
> エイリアス化されるのはコマンドレット名__のみ__で、モジュール名はエイリアス化されません。 `#Requires`、`Import-Module`、`.psd1` の依存関係の一覧、またはコマンドレットの完全修飾名を使用している場合は、モジュール名に関連する[重大な変更の一覧](migrate-az-1.0.0.md)に記載されている手順に従って、必ずこの時点で移行してください。

> [!WARNING]
>
> このコマンドに別の `-Scope` を使用することができますが、これはお勧めしません。 別名は選択したスコープのユーザー プロファイルに書き込まれるので、できるだけ限られたスコープに対して有効にしてください。 エイリアスをシステム全体で有効にすると、ローカル スコープに AzureRM をインストールしている他のユーザーに問題が生じることもあります。

別名モードを有効にしたら、、スクリプトを再度実行して、スクリプトが引き続き想定どおりに機能することを確認します。
一部のパラメーター名は、Az モジュールで必要な変更、追加、または作成が行われています。 コマンドレットの出力の種類も同様に変更されている場合があります。 これらの変更については、[重大な変更の一覧](migrate-az-1.0.0.md)で詳しく説明します。

## <a name="update-cmdlets-modules-and-parameters"></a>コマンドレット、モジュール、およびパラメーターを更新する

更新されてエイリアスの下で実行されているスクリプトは、新しいコマンドレットを使用したり新しい機能などのその他の変更を活用したりするように更新するには、時間がかかる可能性があります。 ほとんどのスクリプトでは、[Az の新しいコマンドレット名前付けスキームに従って](migrate-az-1.0.0.md#cmdlet-noun-prefix-changes)コマンドレット名を更新するだけで済みます。 スクリプトの実行内容とそのスクリプトで利用される Azure PowerShell の機能によっては、スクリプトを機能させるためにその他のいくつかの変更を加える必要がある場合があります。

たとえば、[Blob Storage コマンドレット](migrate-az-1.0.0.md#azstorage-previously-azurestorage-and-azurermstorage)は新しい非同期モデルを使用するために完全に再作成されているため、それらを使用するスクリプトを更新するには、関連する変更がコマンドレット名のみだったスクリプトよりも多くの作業が必要となります。

この時点までにスクリプトに対してわずかで単純な変更しか加えていない場合でも、つまり、エイリアスが有効になっているときに追加の変更なしでスクリプトが機能する場合でも、[Az 1.0.0 の重大な変更の詳細な一覧](migrate-az-1.0.0.md)を参照して、コマンドレット名を変更してエイリアスを無効にした後に消える可能性があるエイリアスの '透過的' な動作に依存していないことを確認してください。

## <a name="disable-aliases"></a>エイリアスを無効にする

移行が完了し、エイリアスの動作に依存しなくなったら、エイリアスを無効にすることをお勧めします。 これは [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias) コマンドレットを使用して行います。

> [!IMPORTANT]
> このコマンドレットを実行するときは、__必ず__、`Enable-AzureRmAlias` を呼び出した `-Scope` ごとに呼び出してください。そうしないと、システム上のスクリプトが引き続きエイリアスの動作に依存する可能性があります。
