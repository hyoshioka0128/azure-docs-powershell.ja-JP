---
title: "<span data-ttu-id=\"5bde5-101\">Azure PowerShell Service Management モジュールのインストールと構成 | Microsoft Docs</span><span class=\"sxs-lookup\"><span data-stu-id=\"5bde5-101\">Install and configure the Azure PowerShell Service Management module | Microsoft Docs</span></span>"
description: "<span data-ttu-id=\"5bde5-102\">初めて使う Azure PowerShell をインストールして構成する方法について説明します。</span><span class=\"sxs-lookup\"><span data-stu-id=\"5bde5-102\">How to install and configure Azure PowerShell for first time use.</span></span>"
services: azure
author: sdwheeler
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/06/2017
ms.openlocfilehash: c51c727c1cb022eca59f819c7f24d8e058c677da
ms.sourcegitcommit: 226527be7cb647acfe2ea9ab151185053ab3c6db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/29/2017
---
# <span data-ttu-id="5bde5-103">Azure PowerShell Service Management モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="5bde5-103">Installing the Azure PowerShell Service Management module</span></span>
<a id="installing-the-azure-powershell-service-management-module" class="xliff"></a>

<span data-ttu-id="5bde5-104">Azure PowerShell は、[PowerShell ギャラリー](https://www.powershellgallery.com/)からインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5bde5-104">Installing Azure PowerShell from the [PowerShell Gallery](https://www.powershellgallery.com/) is the preferred method of installation.</span></span>

## <span data-ttu-id="5bde5-105">手順 1: PowerShellGet をインストールする</span><span class="sxs-lookup"><span data-stu-id="5bde5-105">Step 1: Install PowerShellGet</span></span>
<a id="step-1-install-powershellget" class="xliff"></a>

<span data-ttu-id="5bde5-106">PowerShell ギャラリーからソフトウェアをインストールするには、PowerShellGet モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="5bde5-106">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="5bde5-107">PowerShellGet のバージョンが適切であるかなど、システム要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="5bde5-107">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="5bde5-108">ご使用のシステムに PowerShellGet がインストールされているかどうかを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="5bde5-108">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

<span data-ttu-id="5bde5-109">次のような出力結果が表示されます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-109">You should see something similar to the following output:</span></span>

```
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="5bde5-110">PowerShellGet がインストールされていない場合は、「[PowerShellGet の入手方法](install-azurerm-ps.md#how-to-get-powershellget)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5bde5-110">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](install-azurerm-ps.md#how-to-get-powershellget).</span></span>

## <span data-ttu-id="5bde5-111">手順 2: Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="5bde5-111">Step 2: Install Azure PowerShell</span></span>
<a id="step-2-install-azure-powershell" class="xliff"></a>

<span data-ttu-id="5bde5-112">Windows PowerShell コンソールから管理者として次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="5bde5-112">Run the following command from the Windows PowerShell console running as Administrator:</span></span>

```powershell
Install-Module Azure
```

<span data-ttu-id="5bde5-113">Azure モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="5bde5-113">The Azure module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="5bde5-114">AzureRM モジュールをインストールすると、まだインストールしていない他の Azure モジュールが PowerShell ギャラリーからダウンロードされてインストールされます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-114">When you install the AzureRM module, any other Azure modules that have not previously been installed will be downloaded and installed from the PowerShell Gallery.</span></span>

<span data-ttu-id="5bde5-115">Azure Service Management モジュールでは、Azure PowerShell Resource Manager モジュールと共通の依存コンポーネントが使用されます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-115">The Azure Service Management module shares dependencies with the Azure PowerShell Resource Manager modules.</span></span> <span data-ttu-id="5bde5-116">Azure PowerShell Resource Manager モジュールがインストール済みである場合は、インストール コマンドに `-AllowClobber` パラメーターを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bde5-116">If you have installed the Azure PowerShell Resource Manager modules, you will need to add the `-AllowClobber` parameter to the install command.</span></span> <span data-ttu-id="5bde5-117">これにより、共通する既存の依存コンポーネントが更新されます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-117">This allows this existing shared dependencies to be updated.</span></span> <span data-ttu-id="5bde5-118">このパラメーターを指定しないと、モジュールのインストールは失敗します。</span><span class="sxs-lookup"><span data-stu-id="5bde5-118">Without this parameter, installation of the module fails.</span></span>

```powershell
Install-Module Azure -AllowClobber
```

<span data-ttu-id="5bde5-119">このモジュールのインストール後、次のコマンドを実行することでモジュールをインポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-119">After you install this module, you can import the module by running the following command:</span></span>

```powershell
Import-Module Azure
```

## <span data-ttu-id="5bde5-120">コマンドレットを使用するには</span><span class="sxs-lookup"><span data-stu-id="5bde5-120">To use the cmdlets</span></span>
<a id="to-use-the-cmdlets" class="xliff"></a>

<span data-ttu-id="5bde5-121">Azure Service Management コマンドレットを使うにはまず、Azure アカウントにログオンする必要があります。</span><span class="sxs-lookup"><span data-stu-id="5bde5-121">To start working with the Azure Service Management cmdlets, first log on to your Azure account.</span></span> <span data-ttu-id="5bde5-122">アカウントにログオンするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="5bde5-122">To log on to your account, run the following command:</span></span>

```powershell
Add-AzureAccount
```

<span data-ttu-id="5bde5-123">Azure にログインすると、指定されたセッションのコンテキストが Azure PowerShell によって作成されます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-123">After logging into Azure, Azure PowerShell creates a context for the given session.</span></span> <span data-ttu-id="5bde5-124">コンテキストには、そのセッション内のすべてのコマンドレットで使われる Azure PowerShell 環境、アカウント、テナント、サブスクリプションが保持されています。</span><span class="sxs-lookup"><span data-stu-id="5bde5-124">That context contains the Azure PowerShell environment, account, tenant, and subscription that will be used for all cmdlets within that session.</span></span> <span data-ttu-id="5bde5-125">これで以下のモジュールを使う準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="5bde5-125">Now you are ready to use the modules below.</span></span>

## <span data-ttu-id="5bde5-126">Azure Service Management のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="5bde5-126">Azure Service Management cmdlets</span></span>
<a id="azure-service-management-cmdlets" class="xliff"></a>

<span data-ttu-id="5bde5-127">Azure PowerShell モジュールは頻繁に更新されます。</span><span class="sxs-lookup"><span data-stu-id="5bde5-127">Azure PowerShell modules are updated frequently.</span></span> <span data-ttu-id="5bde5-128">コマンドレットのオンライン ヘルプに、ご利用のモジュールに存在しないコマンドレットやパラメーターの記述が見つかった場合は、最新バージョンのモジュールをダウンロードしてインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="5bde5-128">If you notice that the online cmdlet help includes cmdlets or parameters that are not in your module, download and install the latest version of the module.</span></span> <span data-ttu-id="5bde5-129">ご利用のモジュールのバージョンを調べるには、「`(Get-Module Azure).Version`」と入力します。</span><span class="sxs-lookup"><span data-stu-id="5bde5-129">To find the version of your module, type: `(Get-Module Azure).Version`.</span></span>

<span data-ttu-id="5bde5-130">Azure における定型的なタスクを自動化する際に利用できるサンプル スクリプトについては、[Microsoft Azure スクリプト センター](http://www.windowsazure.com/documentation/scripts/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5bde5-130">For sample scripts that can help you automate some of the common tasks in Azure, see the [Windows Azure Script Center](http://www.windowsazure.com/documentation/scripts/).</span></span>

<span data-ttu-id="5bde5-131">Windows PowerShell のインストール、学習、使用、カスタマイズ全般については、「[Windows PowerShell を使用したスクリプト](http://go.microsoft.com/fwlink/p/?linkid=320210)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bde5-131">For general information about installing, learning, using, and customizing Windows PowerShell, see [Scripting with Windows PowerShell](http://go.microsoft.com/fwlink/p/?linkid=320210).</span></span>
