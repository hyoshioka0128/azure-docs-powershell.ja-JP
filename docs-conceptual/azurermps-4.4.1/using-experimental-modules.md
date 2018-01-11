---
title: "試験版 Azure PowerShell モジュールを使用する"
description: "試験版 Azure PowerShell モジュールの開発思想と使用方法を説明します。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/05/2017
ms.openlocfilehash: c11e4503c07b0a0c4a71021bc511da723098188e
ms.sourcegitcommit: 42bfd513fe646494d3d9eb0cfc35b049f7e1fbb7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/19/2017
---
# <a name="using-experimental-azure-powershell-modules"></a><span data-ttu-id="b6003-103">試験版 Azure PowerShell モジュールを使用する</span><span class="sxs-lookup"><span data-stu-id="b6003-103">Using experimental Azure PowerShell modules</span></span>

<span data-ttu-id="b6003-104">Azure PowerShell チームでは現在、Azure の開発者ツール (特に CLI) を中心に Azure PowerShell のエクスペリエンスに多数の改善を加え、その評価試験を実施しています。</span><span class="sxs-lookup"><span data-stu-id="b6003-104">With the emphasis on developer tools (especially CLIs) in Azure, the Azure PowerShell team is experimenting with many improvements to the Azure PowerShell experience.</span></span>

## <a name="experimentation-methodology"></a><span data-ttu-id="b6003-105">試験の手法</span><span class="sxs-lookup"><span data-stu-id="b6003-105">Experimentation methodology</span></span>

<span data-ttu-id="b6003-106">Microsoft では、試験を円滑に進めるため、既存の Azure SDK の機能を新たに使いやすい方法で実装した新しい Azure PowerShell モジュールの作成に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="b6003-106">To facilitate experimentation, we are creating new Azure PowerShell modules that implement existing Azure SDK functionality in new, easier to use ways.</span></span> <span data-ttu-id="b6003-107">そのコマンドレットはほとんどの場合、既存のものとまったく変わりません。</span><span class="sxs-lookup"><span data-stu-id="b6003-107">In most cases, the cmdlets exactly mirror existing cmdlets.</span></span> <span data-ttu-id="b6003-108">ただし、この試験版モジュールのコマンドレットでは、Azure リソースの作成と管理がいっそう簡単に行えるよう、短縮表記を採用すると共に、既定値を改善しています。</span><span class="sxs-lookup"><span data-stu-id="b6003-108">However, the experimental cmdlets provide a shorthand notation and smarter default values that make it easier to create and manage Azure resources.</span></span>

<span data-ttu-id="b6003-109">試験版モジュールは、既存の Azure PowerShell モジュールと共存させることができます。</span><span class="sxs-lookup"><span data-stu-id="b6003-109">These modules can be installed side-by-side with existing Azure PowerShell modules.</span></span> <span data-ttu-id="b6003-110">コマンドレット名が短くなっているため、既存の (試験段階ではない) コマンドレットとの間に名前の競合が発生することはありません。</span><span class="sxs-lookup"><span data-stu-id="b6003-110">The cmdlet names have been shortened to provide shorter names and avoid name conflicts with existing, non-experimental cmdlets.</span></span>

<span data-ttu-id="b6003-111">試験版モジュールでは、名前付け規則 `AzureRM.*.Experiments` を使用しています。</span><span class="sxs-lookup"><span data-stu-id="b6003-111">The experimental modules use the following naming convention: `AzureRM.*.Experiments`.</span></span> <span data-ttu-id="b6003-112">この名前付け規則は、プレビュー版モジュールの名前の付け方によく似ています (プレビュー版では、`AzureRM.*.Preview` のようになっています)。</span><span class="sxs-lookup"><span data-stu-id="b6003-112">This naming convention is similar to the naming of Preview modules: `AzureRM.*.Preview`.</span></span> <span data-ttu-id="b6003-113">プレビュー版モジュールと試験版モジュールは異なるものです。</span><span class="sxs-lookup"><span data-stu-id="b6003-113">Preview modules differ from experimental modules.</span></span> <span data-ttu-id="b6003-114">プレビュー版モジュールには、Azure サービスの新機能のうち、プレビュー版限定で利用できるものが実装されています。</span><span class="sxs-lookup"><span data-stu-id="b6003-114">Preview modules implement new functionality of Azure services that is only available as a Preview offering.</span></span> <span data-ttu-id="b6003-115">プレビュー版モジュールは、既存の Azure PowerShell モジュールに代わるものであるため、採用しているコマンドレット名やパラメーター名が同じになっています。</span><span class="sxs-lookup"><span data-stu-id="b6003-115">Preview modules replace existing Azure PowerShell modules and use the same cmdlet and parameter names.</span></span>

## <a name="how-to-install-an-experimental-module"></a><span data-ttu-id="b6003-116">試験版モジュールをインストールする方法</span><span class="sxs-lookup"><span data-stu-id="b6003-116">How to install an experimental module</span></span>

<span data-ttu-id="b6003-117">試験版モジュールは、既存の Azure PowerShell モジュールと同じように PowerShell ギャラリーに公開されています。</span><span class="sxs-lookup"><span data-stu-id="b6003-117">Experimental modules are published to the PowerShell Gallery just like the existing Azure PowerShell modules.</span></span> <span data-ttu-id="b6003-118">試験版モジュールの一覧を表示するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="b6003-118">To see a list of experimental modules, run the following command:</span></span>

```powershell
Find-Module AzureRM.*.Experiments
```

```Output
Version Name                         Repository Description
------- ----                         ---------- -----------
1.0.25  AzureRM.Compute.Experiments  PSGallery  Azure Compute experiments for VM creation
1.0.0   AzureRM.Websites.Experiments PSGallery  Create and deploy web applications using Azure App Services.
```

<span data-ttu-id="b6003-119">試験版モジュールをインストールするには、管理者特権の PowerShell セッションから次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="b6003-119">To install the experimental module, use the following commands from an elevated PowerShell session:</span></span>

```powershell
Install-Module AzureRM.Compute.Experiments
Install-Module AzureRM.Websites.Experiments
```

### <a name="documentation-and-support"></a><span data-ttu-id="b6003-120">ドキュメントとサポート</span><span class="sxs-lookup"><span data-stu-id="b6003-120">Documentation and support</span></span>

<span data-ttu-id="b6003-121">ドキュメントはインストール パッケージに同梱されているため、`Get-Help` コマンドレットを使ってアクセスします。</span><span class="sxs-lookup"><span data-stu-id="b6003-121">Documentation is included in the install package and is accessed using the `Get-Help` cmdlet.</span></span> <span data-ttu-id="b6003-122">試験版モジュールに関して公式のドキュメントは公開されていません。</span><span class="sxs-lookup"><span data-stu-id="b6003-122">No official documentation is published for experimental modules.</span></span>

<span data-ttu-id="b6003-123">モジュールのテストにぜひご協力ください。</span><span class="sxs-lookup"><span data-stu-id="b6003-123">We encourage you to test these modules.</span></span> <span data-ttu-id="b6003-124">皆さまからのフィードバックは、ユーザビリティの改善とニーズ対応の拡充に役立てられます。</span><span class="sxs-lookup"><span data-stu-id="b6003-124">Your feedback allows us to improve usability and respond to your needs.</span></span> <span data-ttu-id="b6003-125">もっとも、試験段階であるという関係上、試験版モジュールへのサポートには一定の制約が存在します。</span><span class="sxs-lookup"><span data-stu-id="b6003-125">However, being experimental, support for these modules is limited.</span></span> <span data-ttu-id="b6003-126">質問や問題の報告は、GitHub リポジトリで[イシュー](https://github.com/Azure/azure-powershell/issues)を作成して行ってください。</span><span class="sxs-lookup"><span data-stu-id="b6003-126">Questions or problem reports can be submitted by creating an [issue](https://github.com/Azure/azure-powershell/issues) in the GitHub repository.</span></span>

## <a name="experiments-and-areas-of-improvement"></a><span data-ttu-id="b6003-127">試験的変更点および改善領域</span><span class="sxs-lookup"><span data-stu-id="b6003-127">Experiments and areas of improvement</span></span>

<span data-ttu-id="b6003-128">ここに挙げた改善点は、競合製品との主な差別化要因に基づいて選定したものです。</span><span class="sxs-lookup"><span data-stu-id="b6003-128">These improvements were selected based on key differentiators in competing products.</span></span> <span data-ttu-id="b6003-129">たとえば、Azure CLI 2.0 では "_API の表面的な部分_" ではなく、"_シナリオ_" に基づいてコマンドを実装することを基本的な方針としています。</span><span class="sxs-lookup"><span data-stu-id="b6003-129">For example, Azure CLI 2.0 has made a point of basing commands on _scenarios_ rather than _API surface area_.</span></span>
<span data-ttu-id="b6003-130">また、Azure CLI 2.0 はエンド ユーザーが "初めて使用する" という局面に簡単に対応できるように、スマートな既定値を多数採用しています。</span><span class="sxs-lookup"><span data-stu-id="b6003-130">Azure CLI 2.0 use a number of smart defaults that make "getting started" scenarios easier for end users.</span></span>

### <a name="core-improvements"></a><span data-ttu-id="b6003-131">重要な改善点</span><span class="sxs-lookup"><span data-stu-id="b6003-131">Core improvements</span></span>

<span data-ttu-id="b6003-132">ここで紹介する重要な改善点はいわば "常識" であるため、実装段階に進むにあたって必要な試験はわずかにとどまります。</span><span class="sxs-lookup"><span data-stu-id="b6003-132">The core improvements are regarded as "common sense", and little experimentation is needed to move forward in implementing these updates.</span></span>

- <span data-ttu-id="b6003-133">シナリオベースのコマンドレット - コマンドレットは "*すべて*"、Azure REST サービスではなくシナリオを中心として設計する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6003-133">Scenario-based Cmdlets - \**All*- cmdlets should be designed around scenarios, not the Azure REST service.</span></span>

- <span data-ttu-id="b6003-134">名前の短縮 - コマンドレット名 (例: `New-AzureRmVM` => `New-AzVm`) とパラメーター名 (例: `-ResourceGroupName` => `-Rg`) が対象です。</span><span class="sxs-lookup"><span data-stu-id="b6003-134">Shorter Names - Includes the names of cmdlets (for example, `New-AzureRmVM` => `New-AzVm`) and the names of parameters (for example, `-ResourceGroupName` => `-Rg`).</span></span> <span data-ttu-id="b6003-135">"以前の" コマンドレットとの互換性を確保するには、エイリアスを使用します。</span><span class="sxs-lookup"><span data-stu-id="b6003-135">Use aliases for compatibility with "old" cmdlets.</span></span> <span data-ttu-id="b6003-136">"_下位互換性を備えた_" パラメーター セットを提供します。</span><span class="sxs-lookup"><span data-stu-id="b6003-136">Provide _backwards compatible_ parameter sets.</span></span>

- <span data-ttu-id="b6003-137">スマートな既定値 - "必須の" 情報を入力するためのスマートな既定値を作成します。</span><span class="sxs-lookup"><span data-stu-id="b6003-137">Smart Defaults - Create smart defaults to fill in "required" information.</span></span> <span data-ttu-id="b6003-138">例: </span><span class="sxs-lookup"><span data-stu-id="b6003-138">For example:</span></span>
  - <span data-ttu-id="b6003-139">リソース グループ</span><span class="sxs-lookup"><span data-stu-id="b6003-139">Resource Group</span></span>
  - <span data-ttu-id="b6003-140">場所</span><span class="sxs-lookup"><span data-stu-id="b6003-140">Location</span></span>
  - <span data-ttu-id="b6003-141">依存リソース</span><span class="sxs-lookup"><span data-stu-id="b6003-141">Dependent resources</span></span>

### <a name="experimental-improvements"></a><span data-ttu-id="b6003-142">試験的改善点</span><span class="sxs-lookup"><span data-stu-id="b6003-142">Experimental improvements</span></span>

<span data-ttu-id="b6003-143">試験的改善点としてここに挙げた項目は、試験によりその有効性を確認するという点でチーム内の要請が強い重大な変更です。</span><span class="sxs-lookup"><span data-stu-id="b6003-143">The experimental improvements present a significant change that the team wants to validate via experimentation.</span></span>

- <span data-ttu-id="b6003-144">単純型 - 何かを作成するシナリオ (作成シナリオ) では、複雑な型や構成オブジェクトを使用しないようにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6003-144">Simple types - Create scenarios should move away from complex types and config objects.</span></span> <span data-ttu-id="b6003-145">構成を 1 つか 2 つのパラメーターに簡略化します。</span><span class="sxs-lookup"><span data-stu-id="b6003-145">Simplify the configuration down to one or two parameters.</span></span>

- <span data-ttu-id="b6003-146">"スマート作成" - あらゆる作成シナリオに "スマート作成" を実装できれば、必要な情報をすべて Azure PowerShell が選定してくれるようになるため、必須のパラメーターが "_なくなります_"。</span><span class="sxs-lookup"><span data-stu-id="b6003-146">"Smart Create" - All create scenarios implementing "Smart Create" would have _no_ required parameters: all necessary information would be chosen by Azure PowerShell in an opinionated fashion.</span></span>

- <span data-ttu-id="b6003-147">グレー パラメーター - 多くの場合、指定が半分任意となっているパラメーター (グレー パラメーター) がいくつか存在するものです。</span><span class="sxs-lookup"><span data-stu-id="b6003-147">Gray Parameters - In many cases, some parameters could be "gray" or semi-optional.</span></span> <span data-ttu-id="b6003-148">そのようなパラメーターを指定しなかった場合には、自動で生成するかどうかを尋ねるメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="b6003-148">If the parameter is not specified, the user is asked if they want the parameter generated for them.</span></span> <span data-ttu-id="b6003-149">また、ユーザーが同意したコンテキストに基づいてグレー パラメーターの側で値を推測できるようにするのも良いでしょう。</span><span class="sxs-lookup"><span data-stu-id="b6003-149">It also makes sense for gray parameters to infer a value based on context with the user's consent.</span></span>
  <span data-ttu-id="b6003-150">たとえば、グレー パラメーターから最近使用した値が提案されるようにすることが考えられます。</span><span class="sxs-lookup"><span data-stu-id="b6003-150">For example, it may make sense to have the gray parameter suggest the most recently used value.</span></span>

- <span data-ttu-id="b6003-151">`-Auto` スイッチ - `-Auto` スイッチは、メインライン パスの必須パラメーターの整合性を保ちつつ、ユーザーが "_あらゆるものを既定値に戻す_" ための "オプトイン" 手段となります。</span><span class="sxs-lookup"><span data-stu-id="b6003-151">`-Auto` Switch - The `-Auto` switch would provide an "opt-in" way for users to _default all the things_ while maintaining the integrity of required parameters in the mainline path.</span></span>

### <a name="feature-specific-switches"></a><span data-ttu-id="b6003-152">機能固有のスイッチ</span><span class="sxs-lookup"><span data-stu-id="b6003-152">Feature-specific switches</span></span>

<span data-ttu-id="b6003-153">たとえば、"Web アプリを作成する" シナリオであれば、既存の Git リポジトリにリモートの Azure を自動で追加するスイッチとして `-Git` または `-AddRemote` が考えられます。</span><span class="sxs-lookup"><span data-stu-id="b6003-153">For example, the "Create web app" scenario might have a `-Git` or `-AddRemote` switch that would automatically add an "azure" remote to an existing git repository.</span></span>

- <span data-ttu-id="b6003-154">既定値の設定機能 - `-ResourceGroupName` や `-Location` など、さまざまな局面で使用するパラメーターに既定値を設定できる機能が必要です。</span><span class="sxs-lookup"><span data-stu-id="b6003-154">Settable Defaults - Users should have the ability to default certain ubiquitous parameters like `-ResourceGroupName` and `-Location`.</span></span>

- <span data-ttu-id="b6003-155">サイズの既定値 - リソースの "サイズ" は、("Standard\_DS1\_v2"、"S1" などのように) 多数のリソース プロバイダーがさまざまな名称を使用しているため、ユーザーにとってはわかりにくいものです。</span><span class="sxs-lookup"><span data-stu-id="b6003-155">Size Defaults - Resource "sizes" can be confusing to users since many Resource Providers use different names (for example, "Standard\_DS1\_v2" or "S1").</span></span> <span data-ttu-id="b6003-156">もっとも、ほとんどのユーザーがこれよりも気にするのはコストです。</span><span class="sxs-lookup"><span data-stu-id="b6003-156">However, most users care more about cost.</span></span> <span data-ttu-id="b6003-157">このため、価格体系に基づいて "汎用の" サイズを定めておくと効果的です。</span><span class="sxs-lookup"><span data-stu-id="b6003-157">Therefore, it makes sense to define "universal" sizes based on a pricing schedule.</span></span> <span data-ttu-id="b6003-158">これにより、ユーザー自身が特定のサイズを選択することも、リソースと予算に基づいて Azure PowerShell に "_最適な選択肢_" を選択してもらうこともできるようになります。</span><span class="sxs-lookup"><span data-stu-id="b6003-158">Users can choose a specific size or let Azure PowerShell choose the _best option_ based on the resource the budget.</span></span>

- <span data-ttu-id="b6003-159">出力形式 - 現在、Azure PowerShell から返されるのは `PSObject` であり、コンソールに出力される情報はわずかしかありません。</span><span class="sxs-lookup"><span data-stu-id="b6003-159">Output Format - Azure PowerShell currently returns `PSObject`s and there is little console output.</span></span> <span data-ttu-id="b6003-160">Azure PowerShell では、使用している "スマートな既定値" に関する情報を表示する必要が出てくることも考えられます。</span><span class="sxs-lookup"><span data-stu-id="b6003-160">Azure PowerShell may need to display some information to the user regarding the "smart defaults" used.</span></span>
