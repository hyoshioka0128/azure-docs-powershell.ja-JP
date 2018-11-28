---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに MSI を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: b442da364a01cd6022c14cbb32a9b633676ca8c7
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2018
ms.locfileid: "52259645"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="9186d-103">MSI を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="9186d-103">Install Azure PowerShell on Windows with MSI</span></span>

<span data-ttu-id="9186d-104">この記事では、MSI インストーラーを使って Windows に Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="9186d-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span>  
<span data-ttu-id="9186d-105">これらのインストール方法は、システムで必要とされる場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="9186d-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="9186d-106">Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9186d-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="9186d-107">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9186d-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

> [!NOTE]
> <span data-ttu-id="9186d-108">Azure PowerShell 6.x 以降のバージョンでは、Web Platform Installer によるインストール方法は使用できなくなりました。</span><span class="sxs-lookup"><span data-stu-id="9186d-108">The Web Platform Installer method of installation is no longer available for versions of Azure PowerShell 6.x and higher.</span></span> <span data-ttu-id="9186d-109">Web Platform Installer を使用する必要がある場合は、代わりに MSI の使用を検討するか、以前のバージョンの Azure PowerShell をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="9186d-109">If you require use of the Web Platform Installer please consider using the MSI instead, or you can install an earlier version of Azure PowerShell.</span></span>

<span data-ttu-id="9186d-110">Linux または macOS 環境でのインストールについては、「[macOS または Linux で Azure PowerShell をインストールする](install-azurermps-maclinux.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9186d-110">To install on Linux or macOS environments, see [Install Azure PowerShell on macOS or Linux](install-azurermps-maclinux.md).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="9186d-111">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="9186d-111">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="9186d-112">Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/latest) から MSI ファイルを使ってインストールすることができます。</span><span class="sxs-lookup"><span data-stu-id="9186d-112">Azure PowerShell can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="9186d-113">以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="9186d-113">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="9186d-114">MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="9186d-114">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="9186d-115">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="9186d-115">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="9186d-116">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="9186d-116">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="9186d-117">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="9186d-117">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
>
> <span data-ttu-id="9186d-118">モジュールの自動読み込みを無効にしている場合は、`Import-Module AzureRM` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9186d-118">If you've disabled module autoloading, you need to manually import the module with `Import-Module AzureRM`.</span></span> <span data-ttu-id="9186d-119">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="9186d-119">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="9186d-120">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="9186d-120">You'll need to repeat this step for every new PowerShell session you start.</span></span> <span data-ttu-id="9186d-121">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9186d-121">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>
