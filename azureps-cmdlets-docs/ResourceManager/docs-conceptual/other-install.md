---
title: "Azure PowerShell のその他のインストール方法 | Microsoft Docs"
description: "MSI パッケージまたは Web Platform Installer を使って Azure PowerShell をインストールする方法について説明します。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.product: azure
ms.service: azure-powershell
ms.devlang: powershell
ms.topic: conceptual
ms.date: 05/15/2017
ms.openlocfilehash: 9cee582f74b7f3260c6ae167a8ac358d360ad8ab
ms.sourcegitcommit: 45587b5091293288e16cfae8ac412e0d42f8f450
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2017
---
# <a name="other-installation-methods"></a><span data-ttu-id="cd4f8-103">その他のインストール方法</span><span class="sxs-lookup"><span data-stu-id="cd4f8-103">Other installation methods</span></span>

<span data-ttu-id="cd4f8-104">Azure PowerShell には、複数のインストール方法があります。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-104">Azure PowerShell has multiple installation methods.</span></span> <span data-ttu-id="cd4f8-105">その中でも、PowerShell ギャラリーに対して PowerShellGet を使う方法をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-105">Using PowerShellGet with the PowerShell Gallery is the preferred method.</span></span> <span data-ttu-id="cd4f8-106">それ以外にも、Web Platform Installer (WebPI) を使うか、[GitHub](https://github.com/Azure/azure-powershell/releases/latest) から入手した MSI ファイルを使って Azure PowerShell をインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-106">Azure PowerShell can be installed using the Web Platform Installer (WebPI) or by using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span>

## <a name="docker"></a><span data-ttu-id="cd4f8-107">Docker</span><span class="sxs-lookup"><span data-stu-id="cd4f8-107">Docker</span></span>

<span data-ttu-id="cd4f8-108">Microsoft では、Azure PowerShell が事前構成されている Docker イメージを保持しています。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-108">We maintain a Docker image preconfigured with Azure PowerShell.</span></span>

<span data-ttu-id="cd4f8-109">`docker run` でコンテナーを実行します。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-109">Run the container with `docker run`.</span></span>

```powershell
docker run azuresdk/azure-powershell
```

<span data-ttu-id="cd4f8-110">また Microsoft では、PowerShell Core コンテナーとしてコマンドレットのサブセットを保持しています。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-110">In addition, we maintain a subset of cmdlets as a PowerShell Core container.</span></span>

<span data-ttu-id="cd4f8-111">Mac/Linux の場合、`latest` イメージを使用します。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-111">For Mac/Linux, use the `latest` image.</span></span>

```bash
docker run azuresdk/azure-powershell-core:latest
```

<span data-ttu-id="cd4f8-112">Windows の場合、`nanoserver` イメージを使用します。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-112">For Windows, use the `nanoserver` image.</span></span>

```powershell
docker run azuresdk/azure-powershell-core:nanoserver
```

<span data-ttu-id="cd4f8-113">Azure PowerShell が [PowerShell ギャラリー](https://www.powershellgallery.com/)から `Install-Module` によってイメージにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-113">Azure PowerShell is installed on the image via `Install-Module` from the [PowerShell Gallery](https://www.powershellgallery.com/).</span></span>

## <a name="install-using-the-web-platform-installer"></a><span data-ttu-id="cd4f8-114">Web Platform Installer を使ってインストールする</span><span class="sxs-lookup"><span data-stu-id="cd4f8-114">Install using the Web Platform Installer</span></span>

<span data-ttu-id="cd4f8-115">WebPI から最新の Azure PowerShell をインストールする方法は、以前のバージョンと同じです。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-115">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="cd4f8-116">[Azure PowerShell WebPI パッケージ](http://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-116">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="cd4f8-117">以前に PowerShell ギャラリーから Azure モジュールをインストールしている場合は、これらのモジュールは自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-117">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="cd4f8-118">これによって、インストールされる Azure PowerShell のバージョンが 1 つに限定されるため、環境の複雑化を防ぐことができます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-118">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="cd4f8-119">ただし場合によっては、同時に複数のバージョンをインストールしなければならないケースもあります。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-119">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="cd4f8-120">PowerShell ギャラリー モジュールでは、`$env:ProgramFiles\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-120">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="cd4f8-121">一方、WebPI インストーラーでは、Azure モジュールは `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\` にインストールされます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-121">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="cd4f8-122">インストール中にエラーが発生した場合は、`$env:ProgramFiles\WindowsPowerShell\Modules` フォルダーから Azure* フォルダーを手動で削除したうえで、もう一度インストールを試みてください。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-122">If an error occurs during install, you can manually remove the Azure* folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="cd4f8-123">インストールが完了したら、Azure PowerShell コマンドレットを含むディレクトリが `$env:PSModulePath` の設定に含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-123">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="cd4f8-124">Azure PowerShell が適切にインストールされているかどうかは、次のコマンドを使って確認できます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-124">The following command can be used to verify that the Azure PowerShell is installed properly.</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="cd4f8-125">WebPI からのインストール時に発生する可能性のある問題が確認されています。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-125">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="cd4f8-126">システムの更新やその他のインストールでコンピューターの再起動が必要になった場合、Azure PowerShell のインストール パスが `$env:PSModulePath` の更新に含まれない場合があります。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-126">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="cd4f8-127">インストール後にコマンドレットを読み込んだり実行したりしようとすると、次のエラー メッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-127">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

```
PS C:\> Login-AzureRmAccount
Login-AzureRmAccount : The term 'Login-AzureRmAccount' is not recognized as the name of a cmdlet,
function, script file, or operable program. Check the spelling of the name, or if a path was
included, verify that the path is correct and try again.
At line:1 char:1
+ Login-AzureRmAccount
+ ~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : ObjectNotFound: (Login-AzureRmAccount:String) [], CommandNotFoundException
    + FullyQualifiedErrorId : CommandNotFoundException
```

<span data-ttu-id="cd4f8-128">このエラーは、コンピューターを再起動するか、完全修飾パスを使ってモジュールをインポートすることで修正できます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-128">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span> <span data-ttu-id="cd4f8-129">For example:</span><span class="sxs-lookup"><span data-stu-id="cd4f8-129">For example:</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-using-the-msi-package"></a><span data-ttu-id="cd4f8-130">MSI パッケージを使ってインストールする</span><span class="sxs-lookup"><span data-stu-id="cd4f8-130">Install using the MSI Package</span></span>

<span data-ttu-id="cd4f8-131">Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/latest) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-131">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="cd4f8-132">以前のバージョンの Azure モジュールをインストール済みである場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-132">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="cd4f8-133">MSI パッケージでは、モジュールが `$env:ProgramFiles\WindowsPowerShell\Modules` にインストールされますが、バージョンごとのフォルダーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="cd4f8-133">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>
