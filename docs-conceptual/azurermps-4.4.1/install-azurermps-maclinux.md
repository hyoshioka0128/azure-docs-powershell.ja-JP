---
title: macOS および Linux での Azure PowerShell のインストールおよび構成 | Microsoft Docs
description: macOS および Linux で初めて使う Azure PowerShell をインストールして構成する方法について説明します。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 01/12/2018
ms.openlocfilehash: 18f07d3eebcce74988a02b78f2cc85f7663ed225
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34821906"
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a><span data-ttu-id="b9fa9-103">macOS および Linux での Azure PowerShell のインストールおよび構成</span><span class="sxs-lookup"><span data-stu-id="b9fa9-103">Install and configure Azure PowerShell on macOS and Linux</span></span>

<span data-ttu-id="b9fa9-104">PowerShell Core v6 と Azure PowerShell を Windows 以外のプラットフォームにもインストールできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-104">It is now possible to install PowerShell Core v6 and Azure PowerShell on non-Windows platforms.</span></span>
<span data-ttu-id="b9fa9-105">Azure PowerShell を macOS や Linux にインストールするプロセスは Windows の場合とほぼ同じですが、最初に PowerShell Core v6 をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-105">The process of installing Azure PowerShell on macOS and Linux is not that different from Windows, however, you must first install PowerShell Core v6.</span></span>

> [!NOTE]

> <span data-ttu-id="b9fa9-106">現時点では、PowerShell Core v6 と Azure PowerShell for .NET Core はどちらもベータ版で提供されており、</span><span class="sxs-lookup"><span data-stu-id="b9fa9-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="b9fa9-107">これらの製品のサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-107">Support for these products is limited.</span></span> <span data-ttu-id="b9fa9-108">問題やバグを見つけた場合は、GitHub に問題を登録してください。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-108">If you have problems or discover bugs, please file Issues in GitHub.</span></span>
>
> * [<span data-ttu-id="b9fa9-109">PowerShell Core v6 の問題</span><span class="sxs-lookup"><span data-stu-id="b9fa9-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="b9fa9-110">Azure PowerShell の問題</span><span class="sxs-lookup"><span data-stu-id="b9fa9-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-core-v6"></a><span data-ttu-id="b9fa9-111">手順 1: PowerShell Core v6 をインストールする</span><span class="sxs-lookup"><span data-stu-id="b9fa9-111">Step 1: Install PowerShell Core v6</span></span>

<span data-ttu-id="b9fa9-112">PowerShell Core v6 をインストールするプロセスは、インストール先のオペレーティング システムによって異なります。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-112">The process of installing PowerShell Core v6 on varies depending on the target operating system.</span></span>
<span data-ttu-id="b9fa9-113">PowerShell Core v6 は Windows にインストールすることもできますが、この記事では、macOS および Linux へのインストールについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-113">While it is possible to install PowerShell Core v6 on Windows, this article focuses on macOS and Linux.</span></span> <span data-ttu-id="b9fa9-114">Azure PowerShell を Windows で使用する場合は、Windows 向けの[インストール](./install-azurerm-ps.md) ガイドをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-114">If you want to use Azure PowerShell on Windows, see the [install](./install-azurerm-ps.md) article for Windows.</span></span>

<span data-ttu-id="b9fa9-115">Linux または macOS への **PowerShell Core v6** のインストールは、Linux ディストリビューションまたは OS バージョンによって異なります。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-115">Installing **PowerShell Core v6** on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="b9fa9-116">詳細な手順については、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-116">Detailed instructions can be found in the following article:</span></span>

- [<span data-ttu-id="b9fa9-117">macOS および Linux への PowerShell Core のインストール</span><span class="sxs-lookup"><span data-stu-id="b9fa9-117">Installing PowerShell Core on macOS and Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos-and-linux)

## <a name="step-2-install-azure-powershell-for-net-core"></a><span data-ttu-id="b9fa9-118">手順 2: Azure PowerShell for .NET Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="b9fa9-118">Step 2: Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="b9fa9-119">PowerShell Core v6 には、インストール済みの PowerShellGet モジュールが付属しています。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-119">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="b9fa9-120">これにより、PowerShell ギャラリーで公開されている任意のモジュールを簡単にインストールできます。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-120">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="b9fa9-121">Azure PowerShell をインストールするには、新しい PowerShell セッションを開き、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-121">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a><span data-ttu-id="b9fa9-122">手順 3: AzureRM.Netcore モジュールを読み込む</span><span class="sxs-lookup"><span data-stu-id="b9fa9-122">Step 3: Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="b9fa9-123">モジュールは、インストール後、PowerShell セッションに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-123">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="b9fa9-124">モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-124">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="b9fa9-125">インポートが完了したら、次のコマンドを使って Azure へのサインインを試みることで、新しくインストールしたモジュールをテストすることができます。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-125">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Login-AzureRMAccount
```

<span data-ttu-id="b9fa9-126">上記のコマンドを実行すると、`https://aka.ms/devicelogin` に移動して指定されたコードを入力するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-126">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="b9fa9-127">利用可能なコマンドレット</span><span class="sxs-lookup"><span data-stu-id="b9fa9-127">Available cmdlets</span></span>

<span data-ttu-id="b9fa9-128">.NET Standard 向けの Azure PowerShell モジュールはまだ開発途中です。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-128">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="b9fa9-129">これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-129">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="b9fa9-130">AzureRM.Netcore モジュールには次の関数が実装されています。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-130">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="b9fa9-131">アカウント管理</span><span class="sxs-lookup"><span data-stu-id="b9fa9-131">Account management</span></span>
  - <span data-ttu-id="b9fa9-132">Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでログインする</span><span class="sxs-lookup"><span data-stu-id="b9fa9-132">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="b9fa9-133">Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む</span><span class="sxs-lookup"><span data-stu-id="b9fa9-133">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="b9fa9-134">環境</span><span class="sxs-lookup"><span data-stu-id="b9fa9-134">Environment</span></span>
  - <span data-ttu-id="b9fa9-135">すぐに使えるさまざまな Microsoft Azure 環境を取得する</span><span class="sxs-lookup"><span data-stu-id="b9fa9-135">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="b9fa9-136">カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する</span><span class="sxs-lookup"><span data-stu-id="b9fa9-136">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="b9fa9-137">Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット</span><span class="sxs-lookup"><span data-stu-id="b9fa9-137">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="b9fa9-138">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="b9fa9-138">Virtual Machine</span></span>
  - <span data-ttu-id="b9fa9-139">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="b9fa9-139">App Service (Websites)</span></span>
  - <span data-ttu-id="b9fa9-140">SQL Database</span><span class="sxs-lookup"><span data-stu-id="b9fa9-140">SQL Database</span></span>
  - <span data-ttu-id="b9fa9-141">Storage</span><span class="sxs-lookup"><span data-stu-id="b9fa9-141">Storage</span></span>
  - <span data-ttu-id="b9fa9-142">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="b9fa9-142">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="b9fa9-143">次の手順</span><span class="sxs-lookup"><span data-stu-id="b9fa9-143">Next Steps</span></span>

<span data-ttu-id="b9fa9-144">Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="b9fa9-144">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
