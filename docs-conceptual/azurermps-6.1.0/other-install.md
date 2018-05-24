---
title: Azure PowerShell のその他のインストール方法 | Microsoft Docs
description: MSI パッケージまたは Web Platform Installer を使って Azure PowerShell をインストールする方法について説明します。
services: azure
author: sptramer
ms.author: sttramer
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/06/2017
ms.openlocfilehash: 8b7d9631581046800c772d7bc6f654bb6a9eb483
ms.sourcegitcommit: 5971c92cb023bdd1d71fa2ad0a3b378abfbd092a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2018
---
# <a name="other-installation-methods"></a><span data-ttu-id="5e449-103">その他のインストール方法</span><span class="sxs-lookup"><span data-stu-id="5e449-103">Other installation methods</span></span>

<span data-ttu-id="5e449-104">Azure PowerShell には、複数のインストール方法があります。</span><span class="sxs-lookup"><span data-stu-id="5e449-104">Azure PowerShell has multiple installation methods.</span></span> <span data-ttu-id="5e449-105">その中でも、PowerShell ギャラリーに対して PowerShellGet を使う方法をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="5e449-105">Using PowerShellGet with the PowerShell Gallery is the preferred method.</span></span> <span data-ttu-id="5e449-106">それ以外にも、Web Platform Installer (WebPI) を使うか、GitHub から入手した MSI ファイルを使って Windows に Azure PowerShell をインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="5e449-106">Azure PowerShell can be installed on Windows using the Web Platform Installer (WebPI) or by using the MSI file available from GitHub.</span></span> <span data-ttu-id="5e449-107">Azure PowerShell は Docker コンテナーにインストールすることもできます。</span><span class="sxs-lookup"><span data-stu-id="5e449-107">Azure PowerShell can also be installed in a Docker container.</span></span>

## <a name="install-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="5e449-108">Web Platform Installer を使って Windows にインストールする</span><span class="sxs-lookup"><span data-stu-id="5e449-108">Install on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="5e449-109">WebPI から最新の Azure PowerShell をインストールする方法は、以前のバージョンと同じです。</span><span class="sxs-lookup"><span data-stu-id="5e449-109">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="5e449-110">[Azure PowerShell WebPI パッケージ](http://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。</span><span class="sxs-lookup"><span data-stu-id="5e449-110">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="5e449-111">以前に PowerShell ギャラリーから Azure モジュールをインストールしている場合は、これらのモジュールは自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="5e449-111">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="5e449-112">これによって、インストールされる Azure PowerShell のバージョンが 1 つに限定されるため、環境の複雑化を防ぐことができます。</span><span class="sxs-lookup"><span data-stu-id="5e449-112">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="5e449-113">ただし場合によっては、同時に複数のバージョンをインストールしなければならないケースもあります。</span><span class="sxs-lookup"><span data-stu-id="5e449-113">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="5e449-114">PowerShell ギャラリー モジュールでは、`$env:ProgramFiles\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="5e449-114">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="5e449-115">一方、WebPI インストーラーでは、Azure モジュールは `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\` にインストールされます。</span><span class="sxs-lookup"><span data-stu-id="5e449-115">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="5e449-116">インストール中にエラーが発生した場合は、`$env:ProgramFiles\WindowsPowerShell\Modules` フォルダーから Azure\* フォルダーを手動で削除したうえで、もう一度インストールを試みてください。</span><span class="sxs-lookup"><span data-stu-id="5e449-116">If an error occurs during install, you can manually remove the Azure\* folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="5e449-117">インストールが完了したら、Azure PowerShell コマンドレットを含むディレクトリが `$env:PSModulePath` の設定に含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e449-117">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="5e449-118">Azure PowerShell が適切にインストールされているかどうかは、次のコマンドを使って確認できます。</span><span class="sxs-lookup"><span data-stu-id="5e449-118">The following command can be used to verify that the Azure PowerShell is installed properly.</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="5e449-119">WebPI からのインストール時に発生する可能性のある問題が確認されています。</span><span class="sxs-lookup"><span data-stu-id="5e449-119">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="5e449-120">システムの更新やその他のインストールでコンピューターの再起動が必要になった場合、Azure PowerShell のインストール パスが `$env:PSModulePath` の更新に含まれない場合があります。</span><span class="sxs-lookup"><span data-stu-id="5e449-120">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="5e449-121">インストール後にコマンドレットを読み込んだり実行したりしようとすると、次のエラー メッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5e449-121">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

```
PS C:\> Connect-AzureRmAccount
Connect-AzureRmAccount : The term 'Connect-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Connect-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Connect-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

<span data-ttu-id="5e449-122">このエラーは、コンピューターを再起動するか、完全修飾パスを使ってモジュールをインポートすることで修正できます。</span><span class="sxs-lookup"><span data-stu-id="5e449-122">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span> <span data-ttu-id="5e449-123">例: </span><span class="sxs-lookup"><span data-stu-id="5e449-123">For example:</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-on-windows-using-the-msi-package"></a><span data-ttu-id="5e449-124">MSI パッケージを使って Windows にインストールする</span><span class="sxs-lookup"><span data-stu-id="5e449-124">Install on Windows using the MSI Package</span></span>

<span data-ttu-id="5e449-125">Azure PowerShell は、[GitHub](https://aka.ms/azps-release) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="5e449-125">Azure PowerShell can be installed using the MSI file available from [GitHub](https://aka.ms/azps-release).</span></span> <span data-ttu-id="5e449-126">以前のバージョンの Azure モジュールをインストール済みである場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="5e449-126">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="5e449-127">MSI パッケージでは、モジュールが `$env:ProgramFiles\WindowsPowerShell\Modules` にインストールされますが、バージョンごとのフォルダーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="5e449-127">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>

## <a name="install-in-a-docker-container"></a><span data-ttu-id="5e449-128">Docker コンテナーにインストールする</span><span class="sxs-lookup"><span data-stu-id="5e449-128">Install in a Docker container</span></span>

<span data-ttu-id="5e449-129">Microsoft では、Azure PowerShell が事前構成されている Docker イメージを保持しています。</span><span class="sxs-lookup"><span data-stu-id="5e449-129">We maintain a Docker image preconfigured with Azure PowerShell.</span></span>

<span data-ttu-id="5e449-130">`docker run` でコンテナーを実行します。</span><span class="sxs-lookup"><span data-stu-id="5e449-130">Run the container with `docker run`.</span></span>

```powershell
docker run azuresdk/azure-powershell
```

<span data-ttu-id="5e449-131">また Microsoft では、PowerShell Core コンテナーとしてコマンドレットのサブセットを保持しています。</span><span class="sxs-lookup"><span data-stu-id="5e449-131">In addition, we maintain a subset of cmdlets as a PowerShell Core container.</span></span>

<span data-ttu-id="5e449-132">Mac/Linux の場合、`latest` イメージを使用します。</span><span class="sxs-lookup"><span data-stu-id="5e449-132">For Mac/Linux, use the `latest` image.</span></span>

```bash
docker run azuresdk/azure-powershell-core:latest
```

<span data-ttu-id="5e449-133">Windows の場合、`nanoserver` イメージを使用します。</span><span class="sxs-lookup"><span data-stu-id="5e449-133">For Windows, use the `nanoserver` image.</span></span>

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

<span data-ttu-id="5e449-134">Azure PowerShell が [PowerShell ギャラリー](https://www.powershellgallery.com/)から `Install-Module` によってイメージにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="5e449-134">Azure PowerShell is installed on the image via `Install-Module` from the [PowerShell Gallery](https://www.powershellgallery.com/).</span></span>
