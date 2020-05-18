---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/20/2018
ms.openlocfilehash: aaba0ce38129b96e3d691f1a9d9cfdc929188ffd
ms.sourcegitcommit: d661f38bec34e65bf73913db59028e11fd78b131
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/05/2020
ms.locfileid: "75722409"
---
# <a name="install-azure-powershell-on-windows-with-msi-or-web-platform-installer"></a><span data-ttu-id="d164f-103">MSI または Web Platform Installer を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="d164f-103">Install Azure PowerShell on Windows with MSI or Web Platform Installer</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="d164f-104">この記事では、MSI または Web Platform Installer (WebPI) を使って Windows に Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="d164f-104">This article explains how to install Azure PowerShell on Windows using an MSI or Web Platform Installer (WebPI).</span></span>  
<span data-ttu-id="d164f-105">これらのインストール方法は、システムで必要とされる場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="d164f-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="d164f-106">Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d164f-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="d164f-107">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d164f-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="d164f-108">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="d164f-108">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="d164f-109">Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="d164f-109">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v5.7.0-April2018).</span></span> <span data-ttu-id="d164f-110">以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="d164f-110">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="d164f-111">MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="d164f-111">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="d164f-112">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="d164f-112">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="d164f-113">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="d164f-113">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="d164f-114">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d164f-114">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="d164f-115">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="d164f-115">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="d164f-116">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d164f-116">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="d164f-117">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d164f-117">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="install-or-update-on-windows-using-the-web-platform-installer"></a><span data-ttu-id="d164f-118">Web Platform Installer を使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="d164f-118">Install or update on Windows using the Web Platform Installer</span></span>

<span data-ttu-id="d164f-119">[Azure PowerShell WebPI パッケージ](https://aka.ms/webpi-azps)をダウンロードしてインストールを開始してください。</span><span class="sxs-lookup"><span data-stu-id="d164f-119">Download the [Azure PowerShell WebPI package](https://aka.ms/webpi-azps) and start the install.</span></span> <span data-ttu-id="d164f-120">MSI または WebPI を使用して以前のバージョンの Azure モジュールがインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="d164f-120">If you have installed previous versions of Azure modules from an MSI or with WebPI, the installer automatically removes them.</span></span> <span data-ttu-id="d164f-121">モジュールは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にインストールされます。</span><span class="sxs-lookup"><span data-stu-id="d164f-121">Modules are installed into `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="d164f-122">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="d164f-122">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="d164f-123">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="d164f-123">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="d164f-124">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d164f-124">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="d164f-125">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="d164f-125">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="d164f-126">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d164f-126">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="d164f-127">Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="d164f-127">To learn how to persist your Azure sign in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>