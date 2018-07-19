---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: 7c6446a66cd3ab9fe8f5d8adf13fed36ee093340
ms.sourcegitcommit: cb1fd248920d7efca67bd6c738a3b47206df7890
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2018
ms.locfileid: "39025312"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a><span data-ttu-id="7c033-103">MSI または Web Platform Installer を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="7c033-103">Install Azure PowerShell on Windows with MSI or Web Platform Installer</span></span>

<span data-ttu-id="7c033-104">この記事では、MSI または Web Platform Installer (WebPI) を使って Windows に Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c033-104">This article explains how to install Azure PowerShell on Windows using an MSI or Web Platform Installer (WebPI).</span></span>  
<span data-ttu-id="7c033-105">これらのインストール方法は、システムで必要とされる場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="7c033-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="7c033-106">Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7c033-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="7c033-107">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c033-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

<span data-ttu-id="7c033-108">Docker コンテナー内で Azure PowerShell を実行するには、[Docker 内での Azure PowerShell の実行](azurerm-ps-in-docker.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7c033-108">To run Azure PowerShell in a Docker container, see [Run Azure PowerShell in Docker](azurerm-ps-in-docker.md).</span></span>

<span data-ttu-id="7c033-109">Linux または macOS 環境でのインストールについては、「[macOS または Linux で Azure PowerShell をインストールする](install-azurermps-maclinux.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7c033-109">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="7c033-110">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="7c033-110">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="7c033-111">Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="7c033-111">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018).</span></span> <span data-ttu-id="7c033-112">以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="7c033-112">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="7c033-113">MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="7c033-113">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="7c033-114">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="7c033-114">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="7c033-115">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="7c033-115">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="7c033-116">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c033-116">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="7c033-117">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c033-117">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="7c033-118">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7c033-118">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="7c033-119">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7c033-119">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="7c033-120">Web Platform Installer を使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="7c033-120">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="7c033-121">[Azure PowerShell WebPI パッケージ](http://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。</span><span class="sxs-lookup"><span data-stu-id="7c033-121">Download the [Azure PowerShell WebPI package](http://aka.ms/webpi-azps) and start the install.</span></span> <span data-ttu-id="7c033-122">MSI または WebPI を使用して以前のバージョンの Azure モジュールがインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="7c033-122">If you have installed previous versions of Azure modules from an MSI or with WebPI, the installer automatically removes them.</span></span> <span data-ttu-id="7c033-123">モジュールは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にインストールされます。</span><span class="sxs-lookup"><span data-stu-id="7c033-123">Modules are installed into `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="7c033-124">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="7c033-124">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="7c033-125">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="7c033-125">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="7c033-126">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c033-126">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="7c033-127">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="7c033-127">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="7c033-128">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7c033-128">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="7c033-129">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="7c033-129">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>