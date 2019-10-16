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
ms.sourcegitcommit: 0b94b9566124331d0b15eb7f5a811305c254172e
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/15/2019
ms.locfileid: "72370271"
---
# <a name="migrate-azure-powershell-from-azurerm-to-az"></a><span data-ttu-id="f5e68-103">AzureRM から Az への Azure PowerShell の移行</span><span class="sxs-lookup"><span data-stu-id="f5e68-103">Migrate Azure PowerShell from AzureRM to Az</span></span>

<span data-ttu-id="f5e68-104">Az モジュールには AzureRM との機能パリティがありますが、より短く一貫性のあるコマンドレット名が使用されます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-104">The Az module has feature parity with AzureRM, but uses shorter and more consistent cmdlet names.</span></span>
<span data-ttu-id="f5e68-105">AzureRM コマンドレット用に記述されたスクリプトは、新しいモジュールで自動的に機能するわけではありません。</span><span class="sxs-lookup"><span data-stu-id="f5e68-105">Scripts written for the AzureRM cmdlets won't automatically work with the new module.</span></span> <span data-ttu-id="f5e68-106">移行を容易にするために、Az には AzureRM を使用する既存のスクリプトを実行できるようにするツールが用意されています。</span><span class="sxs-lookup"><span data-stu-id="f5e68-106">To make the transition easier, Az offers tools to allow you to run your existing scripts using AzureRM.</span></span> <span data-ttu-id="f5e68-107">新しいコマンド セットへの移行がないに越したことはありませんが、この記事は、新しいモジュールへの切り替えを開始する際に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-107">No migration to a new command set is ever convenient, but this article will help you get started on transitioning to the new module.</span></span>

<span data-ttu-id="f5e68-108">AzureRM と Az の間の重大な変更の詳細な一覧については、[AzureRM から Az への詳細な変更](migrate-az-1.0.0.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-108">To see the full list of breaking changes between AzureRM and Az, see the [full changes from AzureRM to Az](migrate-az-1.0.0.md).</span></span>

## <a name="ensure-existing-scripts-work-with-the-latest-azurerm-release"></a><span data-ttu-id="f5e68-109">既存のスクリプトが AzureRM の最新リリースで機能することを確認する</span><span class="sxs-lookup"><span data-stu-id="f5e68-109">Ensure existing scripts work with the latest AzureRM release</span></span>

<span data-ttu-id="f5e68-110">移行手順を実行する前に、システムにインストールされている AzureRM のバージョンを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5e68-110">Before taking any migration steps, check which versions of AzureRM are installed on your system.</span></span> <span data-ttu-id="f5e68-111">これにより、スクリプトが最新のリリースで既に実行中であることを確認し、アンインストールする必要のある AzureRM のバージョンを把握することができます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-111">Doing so allows you to make sure scripts are already running on the latest release, and let you know which versions of AzureRM must be uninstalled.</span></span>

<span data-ttu-id="f5e68-112">インストールされている AzureRM のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="f5e68-112">To check which version(s) of AzureRM you have installed, run the command:</span></span>

```powershell-interactive
Get-InstalledModule -Name AzureRM -AllVersions
```

<span data-ttu-id="f5e68-113">AzureRM の__最新__の一般公開リリースは __6.13.1__ です。</span><span class="sxs-lookup"><span data-stu-id="f5e68-113">The __latest__ available release of AzureRM is __6.13.1__.</span></span> <span data-ttu-id="f5e68-114">このバージョンがインストールされていない場合、既存のスクリプトでは、ここと[重大な変更の一覧](migrate-az-1.0.0.md)で説明しているもの以外の Az モジュールを操作するための追加の変更が必要になる場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-114">If you don't have this version installed, your existing scripts may need additional modification to work with the Az module beyond what's described here and in the [breaking changes list](migrate-az-1.0.0.md).</span></span>

<span data-ttu-id="f5e68-115">スクリプトが AzureRM 6.13.1 で機能しない場合は、[AzureRM 5.x から 6.x への移行ガイド](/powershell/azure/azurerm/migration-guide.6.0.0)に従ってそれらを更新します。</span><span class="sxs-lookup"><span data-stu-id="f5e68-115">If your scripts don't work with AzureRM 6.13.1, update them according to the [AzureRM 5.x to 6.x migration guide](/powershell/azure/azurerm/migration-guide.6.0.0).</span></span>
<span data-ttu-id="f5e68-116">以前のバージョンの AzureRM モジュールを使用している場合は、各メジャー バージョン用に利用できる移行ガイドがあります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-116">If you use an earlier version of the AzureRM module, there are migration guides available for each major version.</span></span>

## <a name="uninstall-azurerm"></a><span data-ttu-id="f5e68-117">AzureRM のアンインストール</span><span class="sxs-lookup"><span data-stu-id="f5e68-117">Uninstall AzureRM</span></span>

<span data-ttu-id="f5e68-118">Az モジュールは、Windows 用の PowerShell 5.1 の既存の AzureRM インストールとの互換性が保証されていません。</span><span class="sxs-lookup"><span data-stu-id="f5e68-118">The Az module is not guaranteed to be compatible with any existing AzureRM installs in PowerShell 5.1 for Windows.</span></span> <span data-ttu-id="f5e68-119">Az モジュールをインストールする前に、[AzureRM をアンインストール](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module)してください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-119">Before you install the Az module, [uninstall AzureRM](/powershell/azure/uninstall-az-ps#uninstall-the-azurerm-module).</span></span>

> [!IMPORTANT]
>
> <span data-ttu-id="f5e68-120">AzureRM モジュールをシステムから削除する準備ができていない場合は、代わりに [PowerShell Core](/powershell/scripting/install/installing-powershell-core-on-windows) 6.x 以降用の Az モジュールをインストールできます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-120">If you're not ready to remove the AzureRM module from your system, you can install the Az module for [PowerShell Core](/powershell/scripting/install/installing-powershell-core-on-windows) 6.x or later instead.</span></span> <span data-ttu-id="f5e68-121">PowerShell Core と Windows 用の PowerShell 5.1 は別のモジュール ライブラリを使用するため、競合することはありません。</span><span class="sxs-lookup"><span data-stu-id="f5e68-121">PowerShell Core and PowerShell 5.1 for Windows use different module libraries, so there will be no conflicts.</span></span> <span data-ttu-id="f5e68-122">PowerShell Core で引き続き[エイリアスを有効にする](#enable-azurerm-compatibility-aliases)ことができます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-122">You can still [enable aliases](#enable-azurerm-compatibility-aliases) in PowerShell Core.</span></span>

## <a name="install-the-azure-powershell-az-module"></a><span data-ttu-id="f5e68-123">Azure PowerShell Az モジュールをインストールする</span><span class="sxs-lookup"><span data-stu-id="f5e68-123">Install the Azure PowerShell Az module</span></span>

<span data-ttu-id="f5e68-124">最初の手順では、お使いのプラットフォームに Az モジュールをインストールします。</span><span class="sxs-lookup"><span data-stu-id="f5e68-124">The first step is to install the Az module on your platform.</span></span> <span data-ttu-id="f5e68-125">Az をインストールするときは、AzureRM をアンインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f5e68-125">When you install Az, it's recommended that you uninstall AzureRM.</span></span> <span data-ttu-id="f5e68-126">次の手順では、既存のスクリプトを引き続き実行できるようにする方法と、古いコマンドレット名の互換性を有効にする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="f5e68-126">In the following steps, you'll learn how to keep running your existing scripts and enable compatibility for old cmdlet names.</span></span>

<span data-ttu-id="f5e68-127">Azure PowerShell モジュールをインストールするには、「[Az モジュールのインストール](install-az-ps.md)」の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-127">To install the Azure PowerShell Az module, follow the instructions in [Install the Az module](install-az-ps.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f5e68-128">この時点で、Az モジュールに用意されている [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) コマンドレットを実行したい場合は、すべてのバージョンの AzureRM がアンインストールされていて、競合が発生することがないことだけ確認してください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-128">At this point, you might want to run the [Uninstall-AzureRM](/powershell/module/az.accounts/uninstall-azurerm) cmdlet provided in the Az module, just to make sure that all versions of AzureRM have been uninstalled and won't cause conflicts.</span></span>

## <a name="enable-azurerm-compatibility-aliases"></a><span data-ttu-id="f5e68-129">AzureRM と互換性のあるエイリアスを有効にする</span><span class="sxs-lookup"><span data-stu-id="f5e68-129">Enable AzureRM compatibility aliases</span></span>

<span data-ttu-id="f5e68-130">AzureRM をアンインストールして、スクリプトが最新バージョンの AzureRM で機能するようになったら、次の手順で Az モジュールの互換モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f5e68-130">With AzureRM uninstalled and your scripts working with the latest AzureRM version, the next step is to enable the compatibility mode for the Az module.</span></span> <span data-ttu-id="f5e68-131">次のコマンドを使用して、互換性を有効にします。</span><span class="sxs-lookup"><span data-stu-id="f5e68-131">Compatibility is enabled with the command:</span></span>

```powershell-interactive
Enable-AzureRmAlias -Scope CurrentUser
```

<span data-ttu-id="f5e68-132">別名を使用することによって、Az モジュールがインストールされた状態で、古いコマンドレット名を使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-132">Aliases enable the ability to use old cmdlet names with the Az module installed.</span></span> <span data-ttu-id="f5e68-133">これらのエイリアスは、選択したスコープのプロファイルに書き込まれます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-133">These aliases are written to the profile for the selected scope.</span></span> <span data-ttu-id="f5e68-134">プロファイルが存在しない場合は、作成されます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-134">If no profile exists, one is created.</span></span>
<span data-ttu-id="f5e68-135">`CurrentUser` よりも範囲が広い `-Scope` を使用する場合は、対応するプロファイル ファイルを作成または更新するための適切な権限が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5e68-135">When using a `-Scope` broader than `CurrentUser`, the appropriate permissions are required to create or update the corresponding profile file.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f5e68-136">エイリアス化されるのはコマンドレット名__のみ__で、モジュール名はエイリアス化されません。</span><span class="sxs-lookup"><span data-stu-id="f5e68-136">__Only__ cmdlet names are aliased - module names aren't!</span></span> <span data-ttu-id="f5e68-137">`#Requires`、`Import-Module`、`.psd1` の依存関係の一覧、またはコマンドレットの完全修飾名を使用している場合は、モジュール名に関連する[重大な変更の一覧](migrate-az-1.0.0.md)に記載されている手順に従って、必ずこの時点で移行してください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-137">If you're using `#Requires`, `Import-Module`, dependency lists in a `.psd1`, or fully-qualified cmdlet names, make sure that you migrate them at this point by following the process outlined in the [breaking changes list](migrate-az-1.0.0.md) regarding module names.</span></span>

> [!WARNING]
>
> <span data-ttu-id="f5e68-138">このコマンドに別の `-Scope` を使用することができますが、これはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="f5e68-138">You can use a different `-Scope` for this command, but it's not recommended.</span></span> <span data-ttu-id="f5e68-139">別名は選択したスコープのユーザー プロファイルに書き込まれるので、できるだけ限られたスコープに対して有効にしてください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-139">Aliases are written to the user profile for the selected scope, so keep enabling them to as limited a scope as possible.</span></span> <span data-ttu-id="f5e68-140">エイリアスをシステム全体で有効にすると、ローカル スコープに AzureRM をインストールしている他のユーザーに問題が生じることもあります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-140">Enabling aliases system-wide can cause issues for other users who have AzureRM installed in their local scope.</span></span>

<span data-ttu-id="f5e68-141">別名モードを有効にしたら、、スクリプトを再度実行して、スクリプトが引き続き想定どおりに機能することを確認します。</span><span class="sxs-lookup"><span data-stu-id="f5e68-141">Once the alias mode is enabled, run your scripts again to confirm that they still function as expected.</span></span>
<span data-ttu-id="f5e68-142">一部のパラメーター名は、Az モジュールで必要な変更、追加、または作成が行われています。</span><span class="sxs-lookup"><span data-stu-id="f5e68-142">Some parameter names have been changed, added, or made required by the Az module.</span></span> <span data-ttu-id="f5e68-143">コマンドレットの出力の種類も同様に変更されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-143">Output types of cmdlets may have changed as well.</span></span> <span data-ttu-id="f5e68-144">これらの変更については、[重大な変更の一覧](migrate-az-1.0.0.md)で詳しく説明します。</span><span class="sxs-lookup"><span data-stu-id="f5e68-144">These changes are detailed in the [breaking changes list](migrate-az-1.0.0.md).</span></span>

## <a name="update-cmdlets-modules-and-parameters"></a><span data-ttu-id="f5e68-145">コマンドレット、モジュール、およびパラメーターを更新する</span><span class="sxs-lookup"><span data-stu-id="f5e68-145">Update cmdlets, modules, and parameters</span></span>

<span data-ttu-id="f5e68-146">更新されてエイリアスの下で実行されているスクリプトは、新しいコマンドレットを使用したり新しい機能などのその他の変更を活用したりするように更新するには、時間がかかる可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-146">With scripts updated and running under aliases, you can take your time to update them to use the new cmdlets and take advantage of other changes like new features.</span></span> <span data-ttu-id="f5e68-147">ほとんどのスクリプトでは、[Az の新しいコマンドレット名前付けスキームに従って](migrate-az-1.0.0.md#cmdlet-noun-prefix-changes)コマンドレット名を更新するだけで済みます。</span><span class="sxs-lookup"><span data-stu-id="f5e68-147">For most scripts, you will only need to update cmdlet names, [following the new cmdlet naming scheme in Az](migrate-az-1.0.0.md#cmdlet-noun-prefix-changes).</span></span> <span data-ttu-id="f5e68-148">スクリプトの実行内容とそのスクリプトで利用される Azure PowerShell の機能によっては、スクリプトを機能させるためにその他のいくつかの変更を加える必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-148">There may also be some other changes that you need to make in order to have your scripts work, depending on what they do and which Azure PowerShell features they take advantage of.</span></span>

<span data-ttu-id="f5e68-149">たとえば、[Blob Storage コマンドレット](migrate-az-1.0.0.md#azstorage-previously-azurestorage-and-azurermstorage)は新しい非同期モデルを使用するために完全に再作成されているため、それらを使用するスクリプトを更新するには、関連する変更がコマンドレット名のみだったスクリプトよりも多くの作業が必要となります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-149">For example, the [Blob Storage cmdlets](migrate-az-1.0.0.md#azstorage-previously-azurestorage-and-azurermstorage) have been completely reworked to use a new asynchronous model, so scripts using them will take more work to update than those where the only relevant changes were cmdlet names.</span></span>

<span data-ttu-id="f5e68-150">この時点までにスクリプトに対してわずかで単純な変更しか加えていない場合でも、つまり、エイリアスが有効になっているときに追加の変更なしでスクリプトが機能する場合でも、[Az 1.0.0 の重大な変更の詳細な一覧](migrate-az-1.0.0.md)を参照して、コマンドレット名を変更してエイリアスを無効にした後に消える可能性があるエイリアスの '透過的' な動作に依存していないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="f5e68-150">Even if you've only had to make small, simple changes to your scripts up to this point - or they even work without additional modification when aliases are enabled -  read the [full list of breaking changes in Az 1.0.0](migrate-az-1.0.0.md) to make sure that you're not relying on 'transparent' behavior of aliases which could disappear after you change cmdlet names and disable aliases.</span></span>

## <a name="disable-aliases"></a><span data-ttu-id="f5e68-151">エイリアスを無効にする</span><span class="sxs-lookup"><span data-stu-id="f5e68-151">Disable aliases</span></span>

<span data-ttu-id="f5e68-152">移行が完了し、エイリアスの動作に依存しなくなったら、エイリアスを無効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="f5e68-152">Once you've completed your migration and are no longer relying on aliasing behavior, it's recommended that you disable aliases.</span></span> <span data-ttu-id="f5e68-153">これは [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias) コマンドレットを使用して行います。</span><span class="sxs-lookup"><span data-stu-id="f5e68-153">This is done with the [Disable-AzureRmAlias](/powershell/module/az.accounts/disable-azurermalias) cmdlet.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f5e68-154">このコマンドレットを実行するときは、__必ず__、`Enable-AzureRmAlias` を呼び出した `-Scope` ごとに呼び出してください。そうしないと、システム上のスクリプトが引き続きエイリアスの動作に依存する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f5e68-154">When running this cmdlet, __make sure__ that you invoke it for each `-Scope` that `Enable-AzureRmAlias` was invoked for, otherwise there may still be scripts on your system relying on the aliasing behavior.</span></span>
