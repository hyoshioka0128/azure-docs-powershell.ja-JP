---
title: Azure PowerShell Az モジュールの概要
description: AzureRM モジュールに代わる新しい Azure PowerShell Az モジュールの概要。
ms.date: 05/20/2020
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: 1626bb4bee775ac173d078cf67934ee5a22632c4
ms.sourcegitcommit: 9f5c7d231b069ad501729bf015a829f3fe89bc6a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/28/2020
ms.locfileid: "84122133"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>新しい Azure PowerShell Az モジュールの概要

2018 年 12 月から、Azure PowerShell Az モジュールが一般公開リリースされました。このモジュールは、Azure の操作を目的とする PowerShell モジュールです。 Az で、コマンドの短縮、安定性の向上、およびクロスプラットフォームのサポートが実現します。 また、Az は AzureRM と同等の機能を持ち、簡単な移行パスも提供されます。

> [!NOTE]
> Powershell 7.x 以降が、すべてのプラットフォームで Azure PowerShell に使用できる PowerShell の推奨バージョンです。

最新の Az モジュールを使用すると、Azure PowerShell は、Windows、macOS、Linux を含むどのプラットフォームでも PowerShell 6.x 以降で動作します。 また、Windows では PowerShell 5.1 にも対応しています。

Az は新しいモジュールであるため、バージョンが 1.0.0 にリセットされます。

## <a name="why-a-new-module"></a>新しいモジュールである理由

主要な更新プログラムの適用には手間取る可能性があります。そのため、PowerShell から Azure を操作するために、新しいコマンドレットと一緒に新しいモジュールのセットを導入することが決定された理由をお知らせすることは重要です。

最大かつ最も重要な変更は、.NET Standard ライブラリに基づいた [PowerShell](/powershell/scripting/overview) の導入以来、PowerShell がクロスプラット フォーム対応製品であることです。
Microsoft は すべてのプラットフォームに Azure サポートを導入することに取り組んでいます。これは、.NET Standard の使用と PowerShell Core との互換性のためには Azure PowerShell モジュールを更新する必要があることを意味します。 既存の AzureRM モジュールを取得し、複雑な変更を導入してこのサポートを追加する代わりに、Az モジュールが作成されました。

また、新しいモジュールを作成することで、エンジニアがコマンドレットとモジュールの設計と名前付けに一貫性を確保することもできます。 すべてのモジュールの先頭は `Az.` プレフィックスになり、コマンドレットはすべて _動詞_-`Az`_名詞_ の形式を使用するようになりました。 以前は、コマンドレット名が長いだけでなく、コマンドレット名に一貫性もありませんでした。

モジュールの数も少なくなりました。同じサービスで動作する複数のモジュールが一緒にまとめられました。 管理プレーンとデータ プレーンのコマンドレットはすべて、サービス用の 1 つのモジュールに含まれるようになりました。 依存関係とインポートを手動で管理している場合は、これにより操作がはるかに簡単になります。

チームでは、新しい Azure PowerShell モジュールの構築を必要とするこれらの重要な変更を加えることによって、Azure PowerShell コマンドレットを以前よりも多くのプラットフォーム上でかつてないほど簡単に使用できるようにすることに取り組んできました。

## <a name="upgrade-to-az"></a>Az にアップグレードする

PowerShell の Azure の最新機能に対応するには、できるだけ早く Az モジュールに移行する必要があります。 Az モジュールを AzureRM の代わりとしてインストールする準備ができていない場合は、Az を試してみるために使用できるいくつかのオプションがあります。

- [Azure Cloud Shell](https://docs.microsoft.com/azure/cloud-shell/overview) で `PowerShell` 環境変数を使用します。 Azure Cloud Shell は、Az モジュールがインストールされていて、`Enable-AzureRM` と互換性のあるエイリアスが有効になっている、ブラウザー ベースのシェル環境です。
- AzureRM モジュールを Windows 用の PowerShell 5.1 と共にインストールしたままにし、PowerShell 6.x 以降の Az モジュールをインストールしてください。 Windows 用の PowerShell 5.1 と PowerShell 6.x 以降では、別個のモジュール コレクションが使用されます。 手順に従って[最新バージョンの PowerShell](/powershell/scripting/install/installing-powershell) をインストールした後、PowerShell 6.x 以降から [Az モジュールをインストール](install-az-ps.md)してください。

既存の AzureRM インストールからアップグレードするには、次の手順に従います。

1. [Azure PowerShell AzureRM モジュールをアンインストールする](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)
2. [Azure PowerShell Az モジュールをインストールする](install-az-ps.md)
3. **省略可能**:新しいコマンド セットについて理解を深めながら、[Enable-AzureRMAlias](/powershell/module/az.accounts/enable-azurermalias) を使用して AzureRM コマンドレットのエイリアスを互換モードで追加できるようにします。 詳細については、次のセクション、または [AzureRM から Az への移行の開始](migrate-from-azurerm-to-az.md)に関するページを参照してください。

## <a name="migrate-existing-scripts-to-az"></a>Az に既存のスクリプトを移行する

新しいコマンドレット名は、覚えやすいように設計されています。 コマンドレット名では `AzureRm` や `Azure` を使用する代わりに、`Az` を使用します。 たとえば、古いコマンド `New-AzureRMVm` は `New-AzVm` になりました。
移行は、単に新しいコマンドレット名に慣れることだけでなく、次のようなそれ以上のことがあります。モジュールやパラメーターの名前の変更や、その他の重要な変更があります。

AzureRM から Az への移行プロセスを支援するために、いくつかのリソースを用意しました。

- [AzureRM から Az への移行の概要](migrate-from-azurerm-to-az.md)
- [AzureRM から Az 1.0.0 への重大な変更の詳細な一覧](migrate-az-1.0.0.md)
- [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) コマンドレット

Az モジュールには互換モードがあり、既存のスクリプトを使用しながら、新しい構文に更新することができます。 [Enable-AzureRmAlias](/powershell/module/az.accounts/enable-azurermalias) コマンドレットにより、エイリアスを使用して互換モードを有効にすることで、最小限の変更を加えた既存のスクリプトを使用しながら、Az への完全な移行に向けて取り組むことができます。 既定では、`Enable-AzureRmAlias` によって、現在の PowerShell セッション用の互換性のあるエイリアスが有効になるだけです。 PowerShell セッション間で互換性のあるエイリアスを保持するには、`Scope` パラメーターを使用してください。 詳細については、[Enable-AzureRmAlias のリファレンス ドキュメント](/powershell/module/az.accounts/enable-azurermalias)を参照してください。

> [!IMPORTANT]
> コマンドレット名がエイリアス化されているとしても、Az コマンドレットの新しい (または名前が変更された) パラメーターや変更された戻り値はまだ残っている可能性があります。 エイリアスで移行を管理できるとは思わないでください。 スクリプトの更新が必要になる可能性のある変更については、[重大な変更の詳細な一覧](migrate-az-1.0.0.md)を参照してください。

## <a name="continued-support-for-azurerm"></a>AzureRM で継続されるサポート

AzureRM は、新しいコマンドレットや機能を受け入れなくなります。 ただし、AzureRM モジュールは 2020 年 12 月まで引き続き正式に維持され、バグの修正プログラムも取得されます。
