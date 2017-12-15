---
title: "macOS および Linux での Azure PowerShell のインストールおよび構成 | Microsoft Docs"
description: "macOS および Linux で初めて使う Azure PowerShell をインストールして構成する方法について説明します。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 94b39c18acaca7a4b17b5207feed025442665acc
ms.sourcegitcommit: c42c7176276ec4e1cc3360a93e6b15d32083bf9f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/14/2017
---
# <a name="install-and-configure-azure-powershell-on-macos-and-linux"></a><span data-ttu-id="a129c-103">macOS および Linux での Azure PowerShell のインストールおよび構成</span><span class="sxs-lookup"><span data-stu-id="a129c-103">Install and configure Azure PowerShell on macOS and Linux</span></span>

<span data-ttu-id="a129c-104">PowerShell 6 (ベータ版) と Azure PowerShell を Windows 以外のプラットフォームにもインストールできるようになりました。</span><span class="sxs-lookup"><span data-stu-id="a129c-104">It is now possible to install PowerShell 6 (beta) and Azure PowerShell on non-Windows platforms.</span></span>
<span data-ttu-id="a129c-105">Azure PowerShell を macOS や Linux にインストールする場合、そのプロセスは Windows の場合とほぼ同じですが、最初に PowerShell 6 (ベータ版) をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a129c-105">The process of installing Azure PowerShell on macOS and Linux is not that different from Windows, however, you must first install PowerShell 6 (beta).</span></span>

> [!NOTE]

> <span data-ttu-id="a129c-106">現時点では、PowerShell 6 (ベータ版) と Azure PowerShell for .NET Core のどちらもベータ版で提供されており、</span><span class="sxs-lookup"><span data-stu-id="a129c-106">At this time, both PowerShell 6 (beta) and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="a129c-107">これらの製品のサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="a129c-107">Support for these products is limited.</span></span> <span data-ttu-id="a129c-108">問題やバグを見つけた場合は、GitHub に問題を登録してください。</span><span class="sxs-lookup"><span data-stu-id="a129c-108">If you have problems or discover bugs, please file Issues in GitHub.</span></span>
>
> * [<span data-ttu-id="a129c-109">PowerShell 6 (ベータ版) の問題</span><span class="sxs-lookup"><span data-stu-id="a129c-109">Issues for PowerShell 6 (beta)</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="a129c-110">Azure PowerShell の問題</span><span class="sxs-lookup"><span data-stu-id="a129c-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="step-1-install-powershell-6-beta"></a><span data-ttu-id="a129c-111">手順 1: PowerShell 6 (ベータ版) をインストールする</span><span class="sxs-lookup"><span data-stu-id="a129c-111">Step 1: Install PowerShell 6 (beta)</span></span>

<span data-ttu-id="a129c-112">PowerShell 6 (ベータ版) のインストール プロセスは、インストール先のオペレーティング システムによって異なります。</span><span class="sxs-lookup"><span data-stu-id="a129c-112">The process of installing PowerShell 6 (beta) on varies depending on the target operating system.</span></span>
<span data-ttu-id="a129c-113">PowerShell 6 (ベータ版) は Windows にインストールすることもできますが、この記事では、macOS および Linux へのインストールについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a129c-113">While it is possible to install PowerShell 6 (beta) on Windows, this article focuses on macOS and Linux.</span></span> <span data-ttu-id="a129c-114">Azure PowerShell を Windows で使用する場合は、Windows 向けの[インストール](./install-azurerm-ps.md) ガイドをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a129c-114">If you want to use Azure PowerShell on Windows, see the [install](./install-azurerm-ps.md) article for Windows.</span></span>

<span data-ttu-id="a129c-115">Linux または macOS に **PowerShell 6** (ベータ版) をインストールするには、次のことが必要です。</span><span class="sxs-lookup"><span data-stu-id="a129c-115">To install **PowerShell 6** (beta) on Linux or macOS, you need to:</span></span>

1. <span data-ttu-id="a129c-116">[GitHub](https://github.com/powershell/powershell#get-powershell) から特定の OS とバージョン向けの PowerShell を取得する</span><span class="sxs-lookup"><span data-stu-id="a129c-116">Get PowerShell for the specific OS and version, from [GitHub](https://github.com/powershell/powershell#get-powershell)</span></span>
2. <span data-ttu-id="a129c-117">それぞれのインストール手順に従う</span><span class="sxs-lookup"><span data-stu-id="a129c-117">Follow the installation instructions</span></span>
   - [<span data-ttu-id="a129c-118">Linux</span><span class="sxs-lookup"><span data-stu-id="a129c-118">Linux</span></span>](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md)
   - [<span data-ttu-id="a129c-119">macOS</span><span class="sxs-lookup"><span data-stu-id="a129c-119">macOS</span></span>](https://github.com/PowerShell/PowerShell/blob/master/docs/installation/linux.md#macos-1012)

## <a name="step-2-install-azure-powershell-for-net-core"></a><span data-ttu-id="a129c-120">手順 2: Azure PowerShell for .NET Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="a129c-120">Step 2: Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="a129c-121">PowerShell 6 (ベータ版) には、インストール済みの PowerShellGet モジュールが付属しています。</span><span class="sxs-lookup"><span data-stu-id="a129c-121">PowerShell 6 (beta) comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="a129c-122">これにより、PowerShell ギャラリーで公開されている任意のモジュールを簡単にインストールできます。</span><span class="sxs-lookup"><span data-stu-id="a129c-122">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="a129c-123">Azure PowerShell をインストールするには、新しい PowerShell セッションを開き、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="a129c-123">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="step-3-load-the-azurermnetcore-module"></a><span data-ttu-id="a129c-124">手順 3: AzureRM.Netcore モジュールを読み込む</span><span class="sxs-lookup"><span data-stu-id="a129c-124">Step 3: Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="a129c-125">モジュールは、インストール後、PowerShell セッションに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="a129c-125">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="a129c-126">モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="a129c-126">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
```

<span data-ttu-id="a129c-127">インポートが完了したら、次のコマンドを使って Azure へのサインインを試みることで、新しくインストールしたモジュールをテストすることができます。</span><span class="sxs-lookup"><span data-stu-id="a129c-127">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Login-AzureRMAccount
```

<span data-ttu-id="a129c-128">上記のコマンドを実行すると、`https://aka.ms/devicelogin` に移動して指定されたコードを入力するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="a129c-128">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="a129c-129">利用可能なコマンドレット</span><span class="sxs-lookup"><span data-stu-id="a129c-129">Available cmdlets</span></span>

<span data-ttu-id="a129c-130">.NET Standard 向けの Azure PowerShell モジュールはまだ開発途中です。</span><span class="sxs-lookup"><span data-stu-id="a129c-130">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="a129c-131">これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。</span><span class="sxs-lookup"><span data-stu-id="a129c-131">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="a129c-132">AzureRM.Netcore モジュールには次の関数が実装されています。</span><span class="sxs-lookup"><span data-stu-id="a129c-132">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="a129c-133">[Account Management]</span><span class="sxs-lookup"><span data-stu-id="a129c-133">Account management</span></span>
  - <span data-ttu-id="a129c-134">Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでログインする</span><span class="sxs-lookup"><span data-stu-id="a129c-134">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="a129c-135">Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む</span><span class="sxs-lookup"><span data-stu-id="a129c-135">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="a129c-136">環境</span><span class="sxs-lookup"><span data-stu-id="a129c-136">Environment</span></span>
  - <span data-ttu-id="a129c-137">すぐに使えるさまざまな Microsoft Azure 環境を取得する</span><span class="sxs-lookup"><span data-stu-id="a129c-137">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="a129c-138">カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する</span><span class="sxs-lookup"><span data-stu-id="a129c-138">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="a129c-139">Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット</span><span class="sxs-lookup"><span data-stu-id="a129c-139">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="a129c-140">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="a129c-140">Virtual Machine</span></span>
  - <span data-ttu-id="a129c-141">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="a129c-141">App Service (Websites)</span></span>
  - <span data-ttu-id="a129c-142">SQL Database</span><span class="sxs-lookup"><span data-stu-id="a129c-142">SQL Database</span></span>
  - <span data-ttu-id="a129c-143">ストレージ</span><span class="sxs-lookup"><span data-stu-id="a129c-143">Storage</span></span>
  - <span data-ttu-id="a129c-144">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="a129c-144">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="a129c-145">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a129c-145">Next Steps</span></span>

<span data-ttu-id="a129c-146">Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="a129c-146">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
