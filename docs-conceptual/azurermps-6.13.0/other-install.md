---
title: Azure PowerShell のその他のインストール方法
description: PowerShellGet を使用せずに MSI を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 11/16/2018
ms.openlocfilehash: e1d8877c185b4537c476128e279eda563f2575d1
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83385866"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="77095-103">MSI を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="77095-103">Install Azure PowerShell on Windows with MSI</span></span>

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

<span data-ttu-id="77095-104">この記事では、MSI インストーラーを使って Windows に Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="77095-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span>  
<span data-ttu-id="77095-105">これらのインストール方法は、システムで必要とされる場合にのみ使用してください。</span><span class="sxs-lookup"><span data-stu-id="77095-105">Use these installation methods only if they're necessary for your system.</span></span> <span data-ttu-id="77095-106">Windows に Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="77095-106">The recommended way to install Azure PowerShell on Windows is with PowerShellGet.</span></span> <span data-ttu-id="77095-107">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-azurerm-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="77095-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-azurerm-ps.md).</span></span>

> [!NOTE]
> <span data-ttu-id="77095-108">Azure PowerShell 6.x 以降のバージョンでは、Web Platform Installer によるインストール方法は使用できなくなりました。</span><span class="sxs-lookup"><span data-stu-id="77095-108">The Web Platform Installer method of installation is no longer available for versions of Azure PowerShell 6.x and higher.</span></span> <span data-ttu-id="77095-109">Web Platform Installer を使用する必要がある場合は、代わりに MSI の使用を検討するか、以前のバージョンの Azure PowerShell をインストールしてください。</span><span class="sxs-lookup"><span data-stu-id="77095-109">If you require use of the Web Platform Installer please consider using the MSI instead, or you can install an earlier version of Azure PowerShell.</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="77095-110">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="77095-110">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="77095-111">Windows PowerShell 5.x 対応の Azure PowerShell は、[GitHub](https://github.com/Azure/azure-powershell/releases/tag/v6.13.1-November2018) から入手可能な MSI ファイルを使ってインストールできます。</span><span class="sxs-lookup"><span data-stu-id="77095-111">Azure PowerShell for Windows PowerShell 5.x can be installed using the MSI file available from [GitHub](https://github.com/Azure/azure-powershell/releases/tag/v6.13.1-November2018).</span></span> <span data-ttu-id="77095-112">以前のバージョンの Azure モジュールが MSI としてインストールされている場合、それらのモジュールはインストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="77095-112">If you have installed previous versions of Azure modules as an MSI, the installer automatically removes them.</span></span> <span data-ttu-id="77095-113">MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="77095-113">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span> <span data-ttu-id="77095-114">`AzureRM` モジュールと `Azure` モジュールの両方がインストールされます。</span><span class="sxs-lookup"><span data-stu-id="77095-114">Both the `AzureRM` and `Azure` modules are installed.</span></span>

> [!NOTE]
> <span data-ttu-id="77095-115">Azure クラシック デプロイ モデルを使用している場合は、`Azure` モジュールのみを使用してください。</span><span class="sxs-lookup"><span data-stu-id="77095-115">Only use the `Azure` module if you are working with the Azure classic deployment model.</span></span>

<span data-ttu-id="77095-116">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="77095-116">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

> [!NOTE]
>
> <span data-ttu-id="77095-117">モジュールの自動読み込みを無効にしている場合は、`Import-Module AzureRM` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="77095-117">If you've disabled module autoloading, you need to manually import the module with `Import-Module AzureRM`.</span></span> <span data-ttu-id="77095-118">モジュールが構造化されているため、これには数秒かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="77095-118">Because of the way the module is structured, this can take a few seconds.</span></span>

<span data-ttu-id="77095-119">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="77095-119">You'll need to repeat this step for every new PowerShell session you start.</span></span> <span data-ttu-id="77095-120">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="77095-120">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>
