---
title: Azure PowerShell Service Management モジュールのインストールと構成 | Microsoft Docs
description: 初めて使う Azure PowerShell をインストールして構成する方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/06/2017
ms.openlocfilehash: 6cc6d9984e49c0cbc23c7ef3a77b98c0b7f3a8e0
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "52828333"
---
# <a name="installing-the-azure-powershell-service-management-module"></a><span data-ttu-id="739ea-103">Azure PowerShell Service Management モジュールのインストール</span><span class="sxs-lookup"><span data-stu-id="739ea-103">Installing the Azure PowerShell Service Management module</span></span>

<span data-ttu-id="739ea-104">Azure PowerShell は、[PowerShell ギャラリー](https://www.powershellgallery.com/)からインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="739ea-104">Installing Azure PowerShell from the [PowerShell Gallery](https://www.powershellgallery.com/) is the preferred method of installation.</span></span>

## <a name="step-1-install-powershellget"></a><span data-ttu-id="739ea-105">手順 1: PowerShellGet をインストールする</span><span class="sxs-lookup"><span data-stu-id="739ea-105">Step 1: Install PowerShellGet</span></span>

<span data-ttu-id="739ea-106">PowerShell ギャラリーからソフトウェアをインストールするには、PowerShellGet モジュールが必要です。</span><span class="sxs-lookup"><span data-stu-id="739ea-106">Installing items from the PowerShell Gallery requires the PowerShellGet module.</span></span> <span data-ttu-id="739ea-107">PowerShellGet のバージョンが適切であるかなど、システム要件を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="739ea-107">Make sure you have the appropriate version of PowerShellGet and other system requirements.</span></span> <span data-ttu-id="739ea-108">ご使用のシステムに PowerShellGet がインストールされているかどうかを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="739ea-108">Run the following command to see if you have PowerShellGet installed on your system.</span></span>

```powershell
Get-Module PowerShellGet -list | Select-Object Name,Version,Path
```

<span data-ttu-id="739ea-109">次のような出力結果が表示されます。</span><span class="sxs-lookup"><span data-stu-id="739ea-109">You should see something similar to the following output:</span></span>

```output
Name          Version Path
----          ------- ----
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

<span data-ttu-id="739ea-110">PowerShellGet がインストールされていない場合は、「[PowerShellGet の入手方法](#how-to-get-powershellget)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="739ea-110">If you do not have PowerShellGet installed, see the [How to get PowerShellGet](#how-to-get-powershellget).</span></span>

## <a name="step-2-install-azure-powershell"></a><span data-ttu-id="739ea-111">手順 2: Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="739ea-111">Step 2: Install Azure PowerShell</span></span>

<span data-ttu-id="739ea-112">Windows PowerShell コンソールから管理者として次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="739ea-112">Run the following command from the Windows PowerShell console running as Administrator:</span></span>

```powershell
Install-Module Azure
```

<span data-ttu-id="739ea-113">Azure モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。</span><span class="sxs-lookup"><span data-stu-id="739ea-113">The Azure module is a rollup module for the Azure Resource Manager cmdlets.</span></span> <span data-ttu-id="739ea-114">AzureRM モジュールをインストールすると、まだインストールしていない他の Azure モジュールが PowerShell ギャラリーからダウンロードされてインストールされます。</span><span class="sxs-lookup"><span data-stu-id="739ea-114">When you install the AzureRM module, any other Azure modules that have not previously been installed will be downloaded and installed from the PowerShell Gallery.</span></span>

<span data-ttu-id="739ea-115">Azure Service Management モジュールでは、Azure PowerShell Resource Manager モジュールと共通の依存コンポーネントが使用されます。</span><span class="sxs-lookup"><span data-stu-id="739ea-115">The Azure Service Management module shares dependencies with the Azure PowerShell Resource Manager modules.</span></span> <span data-ttu-id="739ea-116">Azure PowerShell Resource Manager モジュールがインストール済みである場合は、インストール コマンドに `-AllowClobber` パラメーターを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="739ea-116">If you have installed the Azure PowerShell Resource Manager modules, you will need to add the `-AllowClobber` parameter to the install command.</span></span> <span data-ttu-id="739ea-117">これにより、共通する既存の依存コンポーネントが更新されます。</span><span class="sxs-lookup"><span data-stu-id="739ea-117">This allows this existing shared dependencies to be updated.</span></span> <span data-ttu-id="739ea-118">このパラメーターを指定しないと、モジュールのインストールは失敗します。</span><span class="sxs-lookup"><span data-stu-id="739ea-118">Without this parameter, installation of the module fails.</span></span>

```powershell
Install-Module Azure -AllowClobber
```

<span data-ttu-id="739ea-119">このモジュールのインストール後、次のコマンドを実行することでモジュールをインポートすることができます。</span><span class="sxs-lookup"><span data-stu-id="739ea-119">After you install this module, you can import the module by running the following command:</span></span>

```powershell
Import-Module Azure
```

## <a name="to-use-the-cmdlets"></a><span data-ttu-id="739ea-120">コマンドレットを使用するには</span><span class="sxs-lookup"><span data-stu-id="739ea-120">To use the cmdlets</span></span>

<span data-ttu-id="739ea-121">Azure Service Management コマンドレットを使うにはまず、Azure アカウントにログオンする必要があります。</span><span class="sxs-lookup"><span data-stu-id="739ea-121">To start working with the Azure Service Management cmdlets, first log on to your Azure account.</span></span> <span data-ttu-id="739ea-122">アカウントにログオンするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="739ea-122">To log on to your account, run the following command:</span></span>

```powershell
Add-AzureAccount
```

<span data-ttu-id="739ea-123">Azure にログインすると、指定されたセッションのコンテキストが Azure PowerShell によって作成されます。</span><span class="sxs-lookup"><span data-stu-id="739ea-123">After logging into Azure, Azure PowerShell creates a context for the given session.</span></span> <span data-ttu-id="739ea-124">コンテキストには、そのセッション内のすべてのコマンドレットで使われる Azure PowerShell 環境、アカウント、テナント、サブスクリプションが保持されています。</span><span class="sxs-lookup"><span data-stu-id="739ea-124">That context contains the Azure PowerShell environment, account, tenant, and subscription that will be used for all cmdlets within that session.</span></span> <span data-ttu-id="739ea-125">これで以下のモジュールを使う準備が整いました。</span><span class="sxs-lookup"><span data-stu-id="739ea-125">Now you are ready to use the modules below.</span></span>

## <a name="azure-service-management-cmdlets"></a><span data-ttu-id="739ea-126">Azure Service Management のコマンドレット</span><span class="sxs-lookup"><span data-stu-id="739ea-126">Azure Service Management cmdlets</span></span>

<span data-ttu-id="739ea-127">Azure PowerShell モジュールは頻繁に更新されます。</span><span class="sxs-lookup"><span data-stu-id="739ea-127">Azure PowerShell modules are updated frequently.</span></span> <span data-ttu-id="739ea-128">コマンドレットのオンライン ヘルプに、ご利用のモジュールに存在しないコマンドレットやパラメーターの記述が見つかった場合は、最新バージョンのモジュールをダウンロードしてインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="739ea-128">If you notice that the online cmdlet help includes cmdlets or parameters that are not in your module, download and install the latest version of the module.</span></span> <span data-ttu-id="739ea-129">ご利用のモジュールのバージョンを調べるには、「`(Get-Module Azure).Version`」と入力します。</span><span class="sxs-lookup"><span data-stu-id="739ea-129">To find the version of your module, type: `(Get-Module Azure).Version`.</span></span>

<span data-ttu-id="739ea-130">Azure における定型的なタスクを自動化する際に利用できるサンプル スクリプトについては、[Microsoft Azure スクリプト センター](http://www.windowsazure.com/documentation/scripts/)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="739ea-130">For sample scripts that can help you automate some of the common tasks in Azure, see the [Windows Azure Script Center](http://www.windowsazure.com/documentation/scripts/).</span></span>

<span data-ttu-id="739ea-131">Windows PowerShell のインストール、学習、使用、カスタマイズ全般については、「[Windows PowerShell を使用したスクリプト](http://go.microsoft.com/fwlink/p/?linkid=320210)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="739ea-131">For general information about installing, learning, using, and customizing Windows PowerShell, see [Scripting with Windows PowerShell](http://go.microsoft.com/fwlink/p/?linkid=320210).</span></span>

### <a name="how-to-get-powershellget"></a><span data-ttu-id="739ea-132">PowerShellGet の入手方法</span><span class="sxs-lookup"><span data-stu-id="739ea-132">How to get PowerShellGet</span></span>

|<span data-ttu-id="739ea-133">OS バージョン</span><span class="sxs-lookup"><span data-stu-id="739ea-133">OS Version</span></span>|<span data-ttu-id="739ea-134">インストール手順</span><span class="sxs-lookup"><span data-stu-id="739ea-134">Install instructions</span></span>|
|---|---|
|<span data-ttu-id="739ea-135">Windows 10 または Windows Server 2016 を所有している</span><span class="sxs-lookup"><span data-stu-id="739ea-135">I have Windows 10 or Windows Server 2016</span></span>|<span data-ttu-id="739ea-136">OS 標準の Windows Management Framework (WMF) 5.0 に組み込まれています。</span><span class="sxs-lookup"><span data-stu-id="739ea-136">Built into Windows Management Framework (WMF) 5.0 included in the OS</span></span>|
|<span data-ttu-id="739ea-137">PowerShell 5 にアップグレードしたい</span><span class="sxs-lookup"><span data-stu-id="739ea-137">I want to upgrade to PowerShell 5</span></span>|<span data-ttu-id="739ea-138">[最新バージョンの WMF をインストール](https://www.microsoft.com/en-us/download/details.aspx?id=54616)します。</span><span class="sxs-lookup"><span data-stu-id="739ea-138">[Install the latest version of WMF](https://www.microsoft.com/en-us/download/details.aspx?id=54616)</span></span>|
|<span data-ttu-id="739ea-139">PowerShell 3 または PowerShell 4 が付属するバージョンの Windows を使っている</span><span class="sxs-lookup"><span data-stu-id="739ea-139">I am running on a version of Windows with PowerShell 3 or PowerShell 4</span></span>|<span data-ttu-id="739ea-140">[PackageManagement モジュールを入手](http://go.microsoft.com/fwlink/?LinkID=746217)します。</span><span class="sxs-lookup"><span data-stu-id="739ea-140">[Get the PackageManagement modules](http://go.microsoft.com/fwlink/?LinkID=746217)</span></span>|

<div id="helpmechoose"/>

### <a name="checking-the-version-of-azure-powershell"></a><span data-ttu-id="739ea-141">Azure PowerShell のバージョン確認</span><span class="sxs-lookup"><span data-stu-id="739ea-141">Checking the version of Azure PowerShell</span></span>

<span data-ttu-id="739ea-142">Azure PowerShell は、できるだけ早く最新バージョンにアップグレードすることをお勧めしますが、いくつかのバージョンがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="739ea-142">Although we encourage you to upgrade to the latest version as early as possible, several versions of Azure PowerShell are support.</span></span> <span data-ttu-id="739ea-143">インストールされている Azure PowerShell のバージョンを確認するには、コマンド ラインから `Get-Module AzureRM` を実行します。</span><span class="sxs-lookup"><span data-stu-id="739ea-143">To determine the version of Azure PowerShell you have installed, run `Get-Module AzureRM` from your command line.</span></span>

```powershell
Get-Module AzureRM -list | Select-Object Name,Version,Path
```
