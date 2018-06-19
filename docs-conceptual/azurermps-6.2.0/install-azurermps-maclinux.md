---
title: macOS または Linux で Azure PowerShell をインストールする
description: macOS または Linux で Azure PowerShell をインストールする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 17912c155255b6fdfd3cfb9242163b67d405dc03
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323171"
---
# <a name="install-azure-powershell-on-macos-or-linux"></a><span data-ttu-id="05600-103">macOS または Linux で Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="05600-103">Install Azure PowerShell on macOS or Linux</span></span>

<span data-ttu-id="05600-104">Windows 以外のプラットフォームについては、PowerShell Core v6 上で Azure PowerShell を実行できます。</span><span class="sxs-lookup"><span data-stu-id="05600-104">For non-Windows platforms, it's possible to run Azure PowerShell on top of PowerShell Core v6.</span></span> <span data-ttu-id="05600-105">この製品は、.NET Core 用に構築されており、.Net Core ランタイムをサポートするすべてのプラットフォームで実行できます。Windows 用に .NET Framework 上に構築される標準の Azure PowerShell ではありません。</span><span class="sxs-lookup"><span data-stu-id="05600-105">Rather than the standard Azure PowerShell built on .NET Framework for Windows, this product is built for .NET Core and can run on any platform which supports the .Net Core runtime.</span></span>

> [!NOTE]
> <span data-ttu-id="05600-106">現時点では、PowerShell Core v6 と Azure PowerShell for .NET Core はどちらもベータ版で提供されており、</span><span class="sxs-lookup"><span data-stu-id="05600-106">At this time, both PowerShell Core v6 and Azure PowerShell for .NET Core are still in beta.</span></span>
> <span data-ttu-id="05600-107">これらの製品のサポートには制限があります。</span><span class="sxs-lookup"><span data-stu-id="05600-107">Support for these products is limited.</span></span> <span data-ttu-id="05600-108">問題やバグを見つけた場合は、GitHub で問題を登録してください。</span><span class="sxs-lookup"><span data-stu-id="05600-108">If you have problems or discover bugs, please file an issue on GitHub.</span></span>
>
> * [<span data-ttu-id="05600-109">PowerShell Core v6 の問題</span><span class="sxs-lookup"><span data-stu-id="05600-109">Issues for PowerShell Core v6</span></span>](https://github.com/PowerShell/PowerShell/issues)
> * [<span data-ttu-id="05600-110">Azure PowerShell の問題</span><span class="sxs-lookup"><span data-stu-id="05600-110">Issues for Azure PowerShell</span></span>](https://github.com/azure/azure-docs-powershell/issues)

## <a name="install-powershell-core-v6"></a><span data-ttu-id="05600-111">PowerShell Core v6 をインストールする</span><span class="sxs-lookup"><span data-stu-id="05600-111">Install PowerShell Core v6</span></span>

<span data-ttu-id="05600-112">Linux または macOS への PowerShell Core v6 のインストールは、Linux ディストリビューションまたは OS バージョンによって異なります。</span><span class="sxs-lookup"><span data-stu-id="05600-112">Installing PowerShell Core v6 on Linux or macOS varies depending on the Linux distribution and OS version.</span></span>
<span data-ttu-id="05600-113">詳細な手順については、次の記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="05600-113">Detailed instructions can be found in the following articles:</span></span>

- [<span data-ttu-id="05600-114">macOS で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="05600-114">Install PowerShell Core on macOS</span></span>](/powershell/scripting/setup/installing-powershell-core-on-macos)
- [<span data-ttu-id="05600-115">Linux で PowerShell Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="05600-115">Install PowerShell Core on Linux</span></span>](/powershell/scripting/setup/installing-powershell-core-on-linux)

## <a name="install-azure-powershell-for-net-core"></a><span data-ttu-id="05600-116">Azure PowerShell for .NET Core をインストールする</span><span class="sxs-lookup"><span data-stu-id="05600-116">Install Azure PowerShell for .NET Core</span></span>

<span data-ttu-id="05600-117">PowerShell Core v6 には、インストール済みの PowerShellGet モジュールが付属しています。</span><span class="sxs-lookup"><span data-stu-id="05600-117">PowerShell Core v6 comes with the PowerShellGet module already installed.</span></span> <span data-ttu-id="05600-118">これにより、PowerShell ギャラリーで公開されている任意のモジュールを簡単にインストールできます。</span><span class="sxs-lookup"><span data-stu-id="05600-118">This makes it easy to install any module that is published to the PowerShell Gallery.</span></span> <span data-ttu-id="05600-119">Azure PowerShell をインストールするには、新しい PowerShell セッションを開き、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="05600-119">To install Azure PowerShell, open a new PowerShell session and run the following command:</span></span>

```powershell
Install-Module AzureRM.NetCore
```

## <a name="load-the-azurermnetcore-module"></a><span data-ttu-id="05600-120">AzureRM.Netcore モジュールを読み込む</span><span class="sxs-lookup"><span data-stu-id="05600-120">Load the AzureRM.Netcore module</span></span>

<span data-ttu-id="05600-121">モジュールは、インストール後、PowerShell セッションに読み込む必要があります。</span><span class="sxs-lookup"><span data-stu-id="05600-121">Once the module is installed, you need to load the module into your PowerShell session.</span></span> <span data-ttu-id="05600-122">モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。</span><span class="sxs-lookup"><span data-stu-id="05600-122">Modules are loaded using the `Import-Module` cmdlet, as follows:</span></span>

```powershell
Import-Module AzureRM.Netcore
Import-Module AzureRM.Profile.Netcore
```

<span data-ttu-id="05600-123">インポートが完了したら、次のコマンドを使って Azure へのサインインを試みることで、新しくインストールしたモジュールをテストすることができます。</span><span class="sxs-lookup"><span data-stu-id="05600-123">After the import completes, you can test your newly installed and module by attempting to sign into Azure using the following command:</span></span>

```powershell
Connect-AzureRmAccount
```

<span data-ttu-id="05600-124">上記のコマンドを実行すると、`https://aka.ms/devicelogin` に移動して指定されたコードを入力するよう求められます。</span><span class="sxs-lookup"><span data-stu-id="05600-124">The above command should prompt you to go to `https://aka.ms/devicelogin` and enter the provided code.</span></span>

## <a name="available-cmdlets"></a><span data-ttu-id="05600-125">利用可能なコマンドレット</span><span class="sxs-lookup"><span data-stu-id="05600-125">Available cmdlets</span></span>

<span data-ttu-id="05600-126">.NET Standard 向けの Azure PowerShell モジュールはまだ開発途中です。</span><span class="sxs-lookup"><span data-stu-id="05600-126">The Azure PowerShell modules for .NET Standard are still in development.</span></span> <span data-ttu-id="05600-127">これらのモジュールでは、Windows 版で利用可能なコマンドレットの一部が提供されません。</span><span class="sxs-lookup"><span data-stu-id="05600-127">These modules do not provide the full set of cmdlets that are available for the Windows version of the modules.</span></span> <span data-ttu-id="05600-128">AzureRM.Netcore モジュールには次の関数が実装されています。</span><span class="sxs-lookup"><span data-stu-id="05600-128">The following functions are implemented in AzureRM.Netcore modules:</span></span>

* <span data-ttu-id="05600-129">アカウント管理</span><span class="sxs-lookup"><span data-stu-id="05600-129">Account management</span></span>
  - <span data-ttu-id="05600-130">Microsoft Azure Active Directory を通じて、Microsoft アカウント、組織のアカウント、またはサービス プリンシパルでログインする</span><span class="sxs-lookup"><span data-stu-id="05600-130">Login with Microsoft account, Organizational account, or Service Principal through Microsoft Azure Active Directory</span></span>
  - <span data-ttu-id="05600-131">Save-AzureRmContext を使って資格情報をディスクに保存し、Import-AzureRmContext を使って保存した資格情報を読み込む</span><span class="sxs-lookup"><span data-stu-id="05600-131">Save Credentials to disk with Save-AzureRmContext and load saved credentials using Import-AzureRmContext</span></span>
* <span data-ttu-id="05600-132">環境</span><span class="sxs-lookup"><span data-stu-id="05600-132">Environment</span></span>
  - <span data-ttu-id="05600-133">すぐに使えるさまざまな Microsoft Azure 環境を取得する</span><span class="sxs-lookup"><span data-stu-id="05600-133">Get the different out-of-box Microsoft Azure environments</span></span>
  - <span data-ttu-id="05600-134">カスタマイズした環境 (Azure Stack や Windows Azure Pack 環境など) を追加、設定、削除する</span><span class="sxs-lookup"><span data-stu-id="05600-134">Add/Set/Remove customized environments (like your Azure Stack or Windows Azure Pack environments)</span></span>
* <span data-ttu-id="05600-135">Resource Manager と Service Management のインターフェイスを使用する Azure サービスの管理プレーン コマンドレット</span><span class="sxs-lookup"><span data-stu-id="05600-135">Management plane cmdlets for Azure services using Resource Manager and Service Management interfaces.</span></span>
  - <span data-ttu-id="05600-136">仮想マシン</span><span class="sxs-lookup"><span data-stu-id="05600-136">Virtual Machine</span></span>
  - <span data-ttu-id="05600-137">App Service (Websites)</span><span class="sxs-lookup"><span data-stu-id="05600-137">App Service (Websites)</span></span>
  - <span data-ttu-id="05600-138">SQL Database</span><span class="sxs-lookup"><span data-stu-id="05600-138">SQL Database</span></span>
  - <span data-ttu-id="05600-139">Storage</span><span class="sxs-lookup"><span data-stu-id="05600-139">Storage</span></span>
  - <span data-ttu-id="05600-140">ネットワーク</span><span class="sxs-lookup"><span data-stu-id="05600-140">Network</span></span>

## <a name="next-steps"></a><span data-ttu-id="05600-141">次の手順</span><span class="sxs-lookup"><span data-stu-id="05600-141">Next Steps</span></span>

<span data-ttu-id="05600-142">Azure PowerShell の使用方法の詳細については、「[Azure PowerShell を使ってみる](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="05600-142">For more information about using Azure PowerShell, see the [Get started with Azure PowerShell](get-started-azureps.md) article.</span></span>
