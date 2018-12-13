---
title: 試験版 Azure PowerShell モジュールを使用する
description: 試験版 Azure PowerShell モジュールの開発思想と使用方法を説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/05/2017
ms.openlocfilehash: ff58693c8ec21b7e50e37bd85975a9ae3980a5e7
ms.sourcegitcommit: 087c588169786c005a3c177624fb3ac6c8870125
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/13/2018
ms.locfileid: "53217203"
---
# <a name="using-experimental-azure-powershell-modules"></a>試験版 Azure PowerShell モジュールを使用する

Azure PowerShell チームでは現在、Azure の開発者ツール (特に CLI) を中心に Azure PowerShell のエクスペリエンスに多数の改善を加え、その評価試験を実施しています。

## <a name="experimentation-methodology"></a>試験の手法

Microsoft では、試験を円滑に進めるため、既存の Azure SDK の機能を新たに使いやすい方法で実装した新しい Azure PowerShell モジュールの作成に取り組んでいます。 そのコマンドレットはほとんどの場合、既存のものとまったく変わりません。 ただし、この試験版モジュールのコマンドレットでは、Azure リソースの作成と管理がいっそう簡単に行えるよう、短縮表記を採用すると共に、既定値を改善しています。

試験版モジュールは、既存の Azure PowerShell モジュールと共存させることができます。 コマンドレット名が短くなっているため、既存の (試験段階ではない) コマンドレットとの間に名前の競合が発生することはありません。

試験版モジュールでは、名前付け規則 `AzureRM.*.Experiments` を使用しています。 この名前付け規則は、プレビュー版モジュールの名前の付け方によく似ています (プレビュー版では、`AzureRM.*.Preview` のようになっています)。 プレビュー版モジュールと試験版モジュールは異なるものです。 プレビュー版モジュールには、Azure サービスの新機能のうち、プレビュー版限定で利用できるものが実装されています。 プレビュー版モジュールは、既存の Azure PowerShell モジュールに代わるものであるため、採用しているコマンドレット名やパラメーター名が同じになっています。

## <a name="how-to-install-an-experimental-module"></a>試験版モジュールをインストールする方法

試験版モジュールは、既存の Azure PowerShell モジュールと同じように PowerShell ギャラリーに公開されています。 試験版モジュールの一覧を表示するには、次のコマンドを実行します。

```azurepowershell-interactive
Find-Module AzureRM.*.Experiments
```

```output
Version Name                         Repository Description
------- ----                         ---------- -----------
1.0.25  AzureRM.Compute.Experiments  PSGallery  Azure Compute experiments for VM creation
1.0.0   AzureRM.Websites.Experiments PSGallery  Create and deploy web applications using Azure App Services.
```

試験版モジュールをインストールするには、管理者特権の PowerShell セッションから次のコマンドを実行します。

```azurepowershell-interactive
Install-Module AzureRM.Compute.Experiments
Install-Module AzureRM.Websites.Experiments
```

### <a name="documentation-and-support"></a>ドキュメントとサポート

ドキュメントはインストール パッケージに同梱されているため、`Get-Help` コマンドレットを使ってアクセスします。 試験版モジュールに関して公式のドキュメントは公開されていません。

モジュールのテストにぜひご協力ください。 皆さまからのフィードバックは、ユーザビリティの改善とニーズ対応の拡充に役立てられます。 もっとも、試験段階であるという関係上、試験版モジュールへのサポートには一定の制約が存在します。 質問や問題の報告は、GitHub リポジトリで[イシュー](https://github.com/Azure/azure-powershell/issues)を作成して行ってください。

## <a name="experiments-and-areas-of-improvement"></a>試験的変更点および改善領域

ここに挙げた改善点は、競合製品との主な差別化要因に基づいて選定したものです。 たとえば、Azure CLI 2.0 では "_API の表面的な部分_" ではなく、"_シナリオ_" に基づいてコマンドを実装することを基本的な方針としています。
また、Azure CLI 2.0 はエンド ユーザーが "初めて使用する" という局面に簡単に対応できるように、スマートな既定値を多数採用しています。

### <a name="core-improvements"></a>重要な改善点

ここで紹介する重要な改善点はいわば "常識" であるため、実装段階に進むにあたって必要な試験はわずかにとどまります。

- シナリオベースのコマンドレット - コマンドレットは "<em>すべて</em>"、Azure REST サービスではなくシナリオを中心として設計する必要があります。

- 名前の短縮 - コマンドレット名 (例: `New-AzureRmVM` => `New-AzVm`) とパラメーター名 (例: `-ResourceGroupName` => `-Rg`) が対象です。 "以前の" コマンドレットとの互換性を確保するには、エイリアスを使用します。 "_下位互換性を備えた_" パラメーター セットを提供します。

- スマートな既定値 - "必須の" 情報を入力するためのスマートな既定値を作成します。 例: 
  - リソース グループ
  - 場所
  - 依存リソース

### <a name="experimental-improvements"></a>試験的改善点

試験的改善点としてここに挙げた項目は、試験によりその有効性を確認するという点でチーム内の要請が強い重大な変更です。

- 単純型 - 何かを作成するシナリオ (作成シナリオ) では、複雑な型や構成オブジェクトを使用しないようにする必要があります。 構成を 1 つか 2 つのパラメーターに簡略化します。

- "スマート作成" - あらゆる作成シナリオに "スマート作成" を実装できれば、必要な情報をすべて Azure PowerShell が選定してくれるようになるため、必須のパラメーターが "_なくなります_"。

- グレー パラメーター - 多くの場合、指定が半分任意となっているパラメーター (グレー パラメーター) がいくつか存在するものです。 そのようなパラメーターを指定しなかった場合には、自動で生成するかどうかを尋ねるメッセージが表示されます。 また、ユーザーが同意したコンテキストに基づいてグレー パラメーターの側で値を推測できるようにするのも良いでしょう。
  たとえば、グレー パラメーターから最近使用した値が提案されるようにすることが考えられます。

- `-Auto` スイッチ - `-Auto` スイッチは、メインライン パスの必須パラメーターの整合性を保ちつつ、ユーザーが "_あらゆるものを既定値に戻す_" ための "オプトイン" 手段となります。

### <a name="feature-specific-switches"></a>機能固有のスイッチ

たとえば、"Web アプリを作成する" シナリオであれば、既存の Git リポジトリにリモートの Azure を自動で追加するスイッチとして `-Git` または `-AddRemote` が考えられます。

- 既定値の設定機能 - `-ResourceGroupName` や `-Location` など、さまざまな局面で使用するパラメーターに既定値を設定できる機能が必要です。

- サイズの既定値 - リソースの "サイズ" は、("Standard\_DS1\_v2"、"S1" などのように) 多数のリソース プロバイダーがさまざまな名称を使用しているため、ユーザーにとってはわかりにくいものです。 もっとも、ほとんどのユーザーがこれよりも気にするのはコストです。 このため、価格体系に基づいて "汎用の" サイズを定めておくと効果的です。 これにより、ユーザー自身が特定のサイズを選択することも、リソースと予算に基づいて Azure PowerShell に "_最適な選択肢_" を選択してもらうこともできるようになります。

- 出力形式 - 現在、Azure PowerShell から返されるのは `PSObject` であり、コンソールに出力される情報はわずかしかありません。 Azure PowerShell では、使用している "スマートな既定値" に関する情報を表示する必要が出てくることも考えられます。
