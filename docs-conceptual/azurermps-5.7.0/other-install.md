---
title: Azure PowerShell のその他のインストール方法
description: MSI パッケージまたは Web Platform Installer を使って Azure PowerShell をインストールする方法について説明します。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/06/2018
ms.openlocfilehash: 0919583d9cb05a75fae3b812eed84109be8b28aa
ms.sourcegitcommit: bcf80dfd7fbe17e82e7ad029802cfe8a2f02b15c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "35323273"
---
# <a name="other-installation-methods"></a><span data-ttu-id="e962b-103">その他のインストール方法</span><span class="sxs-lookup"><span data-stu-id="e962b-103">Other installation methods</span></span>

<span data-ttu-id="e962b-104">この記事では、MSI または Web Platform Installer (WebPI) を使って Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="e962b-104">This article explains how to install Azure PowerShell using an MSI or Web Platform Installer (WebPI).</span></span> <span data-ttu-id="e962b-105">Docker コンテナー内から Azure PowerShell を実行することもできます。</span><span class="sxs-lookup"><span data-stu-id="e962b-105">You can also run Azure PowerShell from inside of a Docker container.</span></span> <span data-ttu-id="e962b-106">これらのインストール方法は、システムで必要とされる場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="e962b-106">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="e962b-107">通常、Azure PowerShell は、PowerShellGet を使用してインストールすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e962b-107">The canonical way to install Azure PowerShell is through PowerShellGet.</span></span> <span data-ttu-id="e962b-108">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e962b-108">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

<span data-ttu-id="e962b-109">Linux または macOS 環境でのインストールについては、「[macOS または Linux で Azure PowerShell をインストールする](install-azurermps-maclinux.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e962b-109">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="e962b-110">Web Platform Installer を使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="e962b-110">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="e962b-111">WebPI から最新の Azure PowerShell をインストールする方法は、以前のバージョンと同じです。</span><span class="sxs-lookup"><span data-stu-id="e962b-111">Installing the latest Azure PowerShell from WebPI is the same as it was for previous versions.</span></span>
<span data-ttu-id="e962b-112">[Azure PowerShell WebPI パッケージ](http://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。</span><span class="sxs-lookup"><span data-stu-id="e962b-112">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span>

> [!NOTE]
> <span data-ttu-id="e962b-113">以前に PowerShell ギャラリーから Azure モジュールをインストールしている場合は、これらのモジュールは自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="e962b-113">If you have previously installed Azure modules from the PowerShell Gallery, the installer automatically removes them.</span></span> <span data-ttu-id="e962b-114">これによって、インストールされる Azure PowerShell のバージョンが 1 つに限定されるため、環境の複雑化を防ぐことができます。</span><span class="sxs-lookup"><span data-stu-id="e962b-114">This simplifies your environment by ensuring that only one version of Azure PowerShell is installed.</span></span> <span data-ttu-id="e962b-115">ただし場合によっては、同時に複数のバージョンをインストールしなければならないケースもあります。</span><span class="sxs-lookup"><span data-stu-id="e962b-115">However, there are scenarios where you may need multiple versions installed at the same time.</span></span>
>
> <span data-ttu-id="e962b-116">PowerShell ギャラリー モジュールでは、`$env:ProgramFiles\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="e962b-116">PowerShell Gallery modules install modules in `$env:ProgramFiles\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="e962b-117">一方、WebPI インストーラーでは、Azure モジュールは `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\` にインストールされます。</span><span class="sxs-lookup"><span data-stu-id="e962b-117">In contrast, the WebPI installer installs the Azure modules in `$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\`.</span></span>
>
> <span data-ttu-id="e962b-118">インストール中にエラーが発生した場合は、ご自身の `$env:ProgramFiles\WindowsPowerShell\Modules` フォルダーから `Azure*` フォルダーを手動で削除したうえで、もう一度インストールを試みてください。</span><span class="sxs-lookup"><span data-stu-id="e962b-118">If an error occurs during install, you can manually remove the `Azure*` folders in your `$env:ProgramFiles\WindowsPowerShell\Modules` folder, and try the installation again.</span></span>

<span data-ttu-id="e962b-119">インストールが完了したら、Azure PowerShell コマンドレットを含むディレクトリが `$env:PSModulePath` の設定に含まれている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e962b-119">Once the installation completes, your `$env:PSModulePath` setting should include the directories containing the Azure PowerShell cmdlets.</span></span> <span data-ttu-id="e962b-120">Azure PowerShell が適切にインストールされているかどうかは、次のコマンドを使って確認できます。</span><span class="sxs-lookup"><span data-stu-id="e962b-120">The following command can be used to verify that the Azure PowerShell is installed properly:</span></span>

```powershell
# To make sure the Azure PowerShell module is available after you install
Get-Module -ListAvailable Azure* | Select-Object Name, Version, Path
```

> [!NOTE]
> <span data-ttu-id="e962b-121">WebPI からのインストール時に発生する可能性のある問題が確認されています。</span><span class="sxs-lookup"><span data-stu-id="e962b-121">There is a known issue that can occur when installing from WebPI.</span></span> <span data-ttu-id="e962b-122">システムの更新やその他のインストールでコンピューターの再起動が必要になった場合、Azure PowerShell のインストール パスが `$env:PSModulePath` の更新に含まれない場合があります。</span><span class="sxs-lookup"><span data-stu-id="e962b-122">If your computer requires a restart due to system updates or other installations, it may cause updates to `$env:PSModulePath` to fail to include the path where Azure PowerShell is installed.</span></span>

<span data-ttu-id="e962b-123">インストール後にコマンドレットを読み込んだり実行したりしようとすると、次のエラー メッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e962b-123">When attempting to load or execute cmdlets after installation, you can receive the following error message:</span></span>

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

<span data-ttu-id="e962b-124">このエラーは、コンピューターを再起動するか、完全修飾パスを使ってモジュールをインポートすることで修正できます。</span><span class="sxs-lookup"><span data-stu-id="e962b-124">This error can be corrected by restarting the machine or importing the module using the fully qualified path.</span></span>

```powershell
Import-Module "$env:ProgramFiles(x86)\Microsoft SDKs\Azure\PowerShell\AzureRM.psd1"
```

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="e962b-125">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="e962b-125">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="e962b-126">Azure PowerShell は、[GitHub](https://aka.ms/azps-release) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="e962b-126">Azure PowerShell can be installed using the MSI file available from [GitHub](https://aka.ms/azps-release).</span></span> <span data-ttu-id="e962b-127">以前のバージョンの Azure モジュールをインストール済みである場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="e962b-127">If you have installed previous versions of Azure modules, the installer automatically removes them.</span></span> <span data-ttu-id="e962b-128">MSI パッケージでは、モジュールが `$env:ProgramFiles\WindowsPowerShell\Modules` にインストールされますが、バージョンごとのフォルダーは作成されません。</span><span class="sxs-lookup"><span data-stu-id="e962b-128">The MSI package installs modules in `$env:ProgramFiles\WindowsPowerShell\Modules` but does not create version-specific folders.</span></span>

## <a name="run-in-a-docker-container"></a><span data-ttu-id="e962b-129">Docker コンテナーでの実行</span><span class="sxs-lookup"><span data-stu-id="e962b-129">Run in a Docker container</span></span>

<span data-ttu-id="e962b-130">Microsoft では、Azure PowerShell が事前構成されている一連の Docker イメージを保持しています。</span><span class="sxs-lookup"><span data-stu-id="e962b-130">We maintain a set of Docker images preconfigured with Azure PowerShell.</span></span> <span data-ttu-id="e962b-131">使用できるコンテナーは 2 種類あります。Windows 上で従来の PowerShell を実行しているコンテナーと、Windows または Linux のいずれかの上で PowerShell Core を実行しているコンテナーです。</span><span class="sxs-lookup"><span data-stu-id="e962b-131">There are two types of containers available: Those running traditional PowerShell on Windows, and a container running PowerShell Core on either Windows or Linux.</span></span>

| <span data-ttu-id="e962b-132">環境</span><span class="sxs-lookup"><span data-stu-id="e962b-132">Environment</span></span> | <span data-ttu-id="e962b-133">Docker イメージ</span><span class="sxs-lookup"><span data-stu-id="e962b-133">Docker image</span></span> |
|-------------|--------------|
| <span data-ttu-id="e962b-134">Windows 上の PowerShell</span><span class="sxs-lookup"><span data-stu-id="e962b-134">PowerShell on Windows</span></span> | [<span data-ttu-id="e962b-135">azuresdk/azure-powershell</span><span class="sxs-lookup"><span data-stu-id="e962b-135">azuresdk/azure-powershell</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell/) |
| <span data-ttu-id="e962b-136">Windows 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="e962b-136">PowerShell Core on Windows</span></span> | [<span data-ttu-id="e962b-137">azuresdk/azure-powershell-core:nanoserver</span><span class="sxs-lookup"><span data-stu-id="e962b-137">azuresdk/azure-powershell-core:nanoserver</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |
| <span data-ttu-id="e962b-138">Linux 上の PowerShell Core</span><span class="sxs-lookup"><span data-stu-id="e962b-138">PowerShell Core on Linux</span></span> | [<span data-ttu-id="e962b-139">azuresdk/azure-powershell-core:latest</span><span class="sxs-lookup"><span data-stu-id="e962b-139">azuresdk/azure-powershell-core:latest</span></span>](https://hub.docker.com/r/azuresdk/azure-powershell-core/) |

<span data-ttu-id="e962b-140">これらのコンテナーのいずれかを実行するには、`docker run -it $ImageName` を使用して、対話型ターミナルを取得します。</span><span class="sxs-lookup"><span data-stu-id="e962b-140">To run any of these containers, you use `docker run -it $ImageName` to get an interactive terminal.</span></span> <span data-ttu-id="e962b-141">たとえば、Linux コンテナー上で PowerShell Core を実行するには、次を使用します。</span><span class="sxs-lookup"><span data-stu-id="e962b-141">For example, to run the PowerShell Core on Linux container, use:</span></span>

```powershell
docker run -it azuresdk/azure-powershell-core:latest
```

> [!NOTE]
> <span data-ttu-id="e962b-142">Docker で Windows コンテナーを実行するには、お使いのホスト OS が Windows でなければなりません。また、Windows コンテナーを実行するように Docker が設定されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e962b-142">To run a Windows container in Docker, your host OS must be Windows and Docker must be set to run Windows containers.</span></span> <span data-ttu-id="e962b-143">Docker での Windows 環境と Linux 環境の切り替えについては、[Windows コンテナーと Linux コンテナーの切り替え](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers)に関する Docker のドキュメントをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="e962b-143">To learn about switching between Windows and Linux environments in Docker, see the Docker documentation [Switch between Windows and Linux containers](https://docs.docker.com/docker-for-windows/#switch-between-windows-and-linux-containers).</span></span>