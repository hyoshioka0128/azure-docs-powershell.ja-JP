---
title: MSI を使用して Azure PowerShell をインストールする
description: PowerShellGet を使用せずに MSI を使用して Azure PowerShell をインストールする方法
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/10/2020
ms.openlocfilehash: 1bd5bd1ae529a63c848b7aa835272d79b4011d32
ms.sourcegitcommit: 10ec909100a70acec94d42f6084e7bf0342c6854
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2020
ms.locfileid: "83630743"
---
# <a name="install-azure-powershell-on-windows-with-msi"></a><span data-ttu-id="ec3a1-103">MSI を使用した Windows への Azure PowerShell のインストール</span><span class="sxs-lookup"><span data-stu-id="ec3a1-103">Install Azure PowerShell on Windows with MSI</span></span>

<span data-ttu-id="ec3a1-104">この記事では、MSI インストーラーを使って Windows に Azure PowerShell をインストールする方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-104">This article explains how to install Azure PowerShell on Windows using an MSI installer.</span></span> <span data-ttu-id="ec3a1-105">MSI インストーラーは、PowerShell ギャラリーがファイアウォールによってブロックされる可能性がある環境や、オフライン インストーラーが必要な環境向けに用意されています。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-105">The MSI installer is provided for environments where the PowerShell Gallery may be blocked by a firewall, or an offline installer is needed.</span></span> <span data-ttu-id="ec3a1-106">Azure PowerShell をインストールするときは、PowerShellGet を使用することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-106">The recommended way to install Azure PowerShell is with PowerShellGet.</span></span> <span data-ttu-id="ec3a1-107">PowerShellGet を使用して Azure PowerShell をインストールする手順については、「[PowerShellGet を使用して Azure PowerShell をインストールする](install-az-ps.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-107">For instructions on using PowerShellGet to install Azure PowerShell, see [Install Azure PowerShell with PowerShellGet](install-az-ps.md).</span></span>

## <a name="requirements"></a><span data-ttu-id="ec3a1-108">必要条件</span><span class="sxs-lookup"><span data-stu-id="ec3a1-108">Requirements</span></span>

<span data-ttu-id="ec3a1-109">Windows 上の MSI インストーラーは、PowerShell 5.1 のみを対象とした Azure PowerShell のインストール用に設計されています。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-109">The MSI installer on Windows is designed to install Azure PowerShell for PowerShell 5.1 only.</span></span> <span data-ttu-id="ec3a1-110">Windows 以外のプラットフォームまたはそれ以降のバージョンの PowerShell でのインストールの場合は、[PowerShellGet を使用してインストール](install-az-ps.md)してください。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-110">For installation on non-Windows platforms or later versions of PowerShell, [Install with PowerShellGet](install-az-ps.md).</span></span> <span data-ttu-id="ec3a1-111">PowerShell のバージョンを確認するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-111">To check your PowerShell version, run the command:</span></span>

```powershell-interactive
$PSVersionTable.PSVersion
```

<span data-ttu-id="ec3a1-112">PowerShell 5.1 で Azure PowerShell を使用するには、次の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-112">To use Azure PowerShell in PowerShell 5.1, you need to:</span></span>

1. <span data-ttu-id="ec3a1-113">必要に応じて [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) に更新します。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-113">Update to [Windows PowerShell 5.1](/powershell/scripting/install/installing-windows-powershell#upgrading-existing-windows-powershell) if needed.</span></span> <span data-ttu-id="ec3a1-114">Windows 10 の場合は、あらかじめ PowerShell 5.1 がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-114">If you're on Windows 10, you already have PowerShell 5.1 installed.</span></span>
2. <span data-ttu-id="ec3a1-115">[.NET Framework 4.7.2 以降](/dotnet/framework/install)をインストールします。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-115">Install [.NET Framework 4.7.2 or later](/dotnet/framework/install).</span></span>

## <a name="install-or-update-on-windows-using-the-msi-package"></a><span data-ttu-id="ec3a1-116">MSI パッケージを使って Windows でインストールまたは更新する</span><span class="sxs-lookup"><span data-stu-id="ec3a1-116">Install or update on Windows using the MSI Package</span></span>

<span data-ttu-id="ec3a1-117">Azure PowerShell 用の MSI パッケージは [GitHub](https://github.com/Azure/azure-powershell/releases/latest) から入手できます。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-117">The MSI package for Azure PowerShell is available from [GitHub](https://github.com/Azure/azure-powershell/releases/latest).</span></span> <span data-ttu-id="ec3a1-118">MSI を使用して以前のバージョンの Azure PowerShell がインストールされている場合は、インストーラーによって自動的に削除されます。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-118">If you have installed earlier versions of Azure PowerShell using the MSI, the installer automatically removes them.</span></span> <span data-ttu-id="ec3a1-119">MSI パッケージでは、`${env:ProgramFiles}\WindowsPowerShell\Modules` にモジュールがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-119">The MSI package installs modules in `${env:ProgramFiles}\WindowsPowerShell\Modules`.</span></span>

<span data-ttu-id="ec3a1-120">Azure PowerShell を使用して作業を開始するには、Azure の資格情報を使用してサインインします。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-120">To start working with Azure PowerShell, sign in with your Azure credentials.</span></span>

```powershell-interactive
# Connect to Azure with an interactive dialog for sign-in
Connect-AzAccount
```

> [!NOTE]
> <span data-ttu-id="ec3a1-121">モジュールの自動読み込みを無効にしている場合は、`Import-Module Az` を使用してモジュールを手動でインポートする必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-121">If you've disabled module autoloading, you need to manually import the module with `Import-Module Az`.</span></span> <span data-ttu-id="ec3a1-122">モジュールが構造化されているため、これには最大 1 分かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-122">Because of the way the module is structured, this can take up to a minute.</span></span>

<span data-ttu-id="ec3a1-123">新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-123">You'll need to repeat this step for every new PowerShell session you start.</span></span> <span data-ttu-id="ec3a1-124">Azure サインインを PowerShell セッション間で維持する方法については、「[PowerShell セッション間でユーザーの資格情報を保持する](context-persistence.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-124">To learn how to persist your Azure sign-in across PowerShell sessions, see [Persist user credentials across PowerShell sessions](context-persistence.md).</span></span>

## <a name="provide-feedback"></a><span data-ttu-id="ec3a1-125">フィードバックの提供</span><span class="sxs-lookup"><span data-stu-id="ec3a1-125">Provide feedback</span></span>

<span data-ttu-id="ec3a1-126">Azure PowerShell にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-126">If you find a bug in Azure PowerShell, [file an issue on GitHub](https://github.com/Azure/azure-powershell/issues).</span></span> <span data-ttu-id="ec3a1-127">コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/az.accounts/send-feedback) コマンドレットを使用します。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-127">To provide feedback from the command line, use the [Send-Feedback](/powershell/module/az.accounts/send-feedback) cmdlet.</span></span>

## <a name="next-steps"></a><span data-ttu-id="ec3a1-128">次の手順</span><span class="sxs-lookup"><span data-stu-id="ec3a1-128">Next Steps</span></span>

<span data-ttu-id="ec3a1-129">Azure PowerShell のモジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-129">To learn more about the Azure PowerShell modules and their features, see [Get Started with Azure PowerShell](get-started-azureps.md).</span></span> <span data-ttu-id="ec3a1-130">Azure PowerShell に精通していて、AzureRM から移行する必要がある場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec3a1-130">If you're familiar with Azure PowerShell and need to migrate from AzureRM, see [Migrate from AzureRM to Az](migrate-from-azurerm-to-az.md).</span></span>
