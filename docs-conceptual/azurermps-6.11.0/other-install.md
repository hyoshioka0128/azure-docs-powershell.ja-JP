---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに MSI を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 52bcbe3f91600c96546c7d8ff5648977a7917ff9
ms.sourcegitcommit: 1f699b72bf544d92459da9d888cc0091f9415b65
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/06/2018
ms.locfileid: "50972572"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="961ee-103">MSI を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="961ee-103">Install Azure PowerShell on Windows with MSI</span></span>

<span data-ttu-id="961ee-104">この記事では、MSI インストーラーを使って Windows に Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="961ee-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span>  
<span data-ttu-id="961ee-105">これらのインストール方法は、システムで必要とされる場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="961ee-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="961ee-106">Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="961ee-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="961ee-107">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="961ee-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

> [!NOTE]
> <span data-ttu-id="961ee-108">Azure PowerShell 6.x 以降のバージョンでは、Web Platform Installer によるインストール方法は使用できなくなりました。</span><span class="sxs-lookup"><span data-stu-id="961ee-108">The Web Platform Installer method of installation is no longer available for versions of Azure PowerShell 6.x and higher.</span></span> <span data-ttu-id="961ee-109">Web Platform Installer を使用する必要がある場合は、代わりに MSI の使用を検討するか、以前のバージョンの Azure PowerShell をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="961ee-109">If you require use of the Web Platform Installer please consider using the MSI instead, or you can install an earlier version of Azure PowerShell.</span></span>

<span data-ttu-id="961ee-110">Linux または macOS 環境でのインストールについては、「[macOS または Linux で Azure PowerShell をインストールする](install-azurermps-maclinux.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="961ee-110">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="961ee-111">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="961ee-111">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="961ee-112">Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/latest) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="961ee-112">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="961ee-113">以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="961ee-113">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="961ee-114">MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="961ee-114">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="961ee-115">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="961ee-115">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="961ee-116">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="961ee-116">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="961ee-117">Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="961ee-117">To start working with Azure PowerShell, you need to load `AzureRM` into your current PowerShell session with the [Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) cmdlet, and then sign in with your Azure credentials.</span></span>

```powershell
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

<span data-ttu-id="961ee-118">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="961ee-118">You'll need to repeat these steps for every new PowerShell session you start.</span></span> <span data-ttu-id="961ee-119">`AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="961ee-119">Automatically importing the `AzureRM` module requires setting up a PowerShell profile, which you can learn about in [About Profiles](/powershell/module/microsoft.powershell.core/about/about_profiles).</span></span>
<span data-ttu-id="961ee-120">Azure サインインをセッション間で維持する方法については、「[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="961ee-120">To learn how to persist your Azure sign-in across sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>
