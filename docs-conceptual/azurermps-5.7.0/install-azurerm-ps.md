---
title: PowerShellGet を使用した Windows への Azure PowerShell のインストール
description: PowerShellGet を使用して Azure PowerShell をインストールする方法
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 06/15/2018
ms.openlocfilehash: a868a62bd7bb2f39775a3b7878e2c8484c50438d
ms.sourcegitcommit: 80a3da199954d0ab78765715fb49793e89a30f12
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/22/2018
ms.locfileid: "52258555"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a>PowerShellGet を使用した Windows への Azure PowerShell のインストール

この記事では、PowerShellGet を使用して、Windows 環境に Azure PowerShell モジュールをインストールする手順について説明します。 Azure PowerShell をインストールするときは、PowerShellGet およびモジュール管理を使用することをお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、[その他のインストール方法](other-install.md)に関する記事をご覧ください。

Azure PowerShell を他のプラットフォームにインストールする手順については、[macOS および Linux への Azure PowerShell のインストールと構成](install-azurermps-maclinux.md)に関する記事をご覧ください。

このバージョンの Azure PowerShell では、Azure クラシック デプロイ モデルはサポートされていません。 クラシック デプロイのサポートについては、「[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)」の手順に従ってください。

## <a name="requirements"></a>必要条件

Azure PowerShell をインストールするには、PowerShellGet バージョン 1.1.2.0 以上が必要です。 お使いのシステムで使用できるかどうかを確認するには、次のコマンドを実行します。

```powershell-interactive
Get-Module -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

次のような出力結果が表示されます。

```output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

PowerShellGet のインストールを更新する必要がある場合は、次のコマンドを実行します。

```powershell-interactive
Install-Module PowerShellGet -Force
```

PowerShellGet がインストールされていない場合は、お使いのシステムで次の表の手順に従ってください。

|シナリオ|インストール手順|
|---|---|
|Windows 10<br/>Windows Server 2016|OS 標準の Windows Management Framework (WMF) 5.0 に組み込まれています。|
|PowerShell 5 にアップグレードする| <ol><li>[最新バージョンの WMF をインストール](https://www.microsoft.com/en-us/download/details.aspx?id=54616)します。</li><li>次のコマンドを実行します。<br/>```Install-Module PowerShellGet -Force```</li></ol>|
|PowerShell 3 または PowerShell 4 がインストールされている Windows|<ol><il>[PackageManagement モジュールを入手します。](http://go.microsoft.com/fwlink/?LinkID=746217)</il><li>次のコマンドを実行します。<br/>```Install-Module PowerShellGet -Force```</li></ol>|

> [!NOTE]
> PowerShellGet を使用するには、実行ポリシーでスクリプトの実行が許可されている必要があります。 PowerShell の実行ポリシーについて詳しくは、「[About Execution Policies (実行ポリシーについて)](/powershell/module/microsoft.powershell.core/about/about_execution_policies)」をご覧ください。
>
> [!IMPORTANT]
> このドキュメントで説明するモジュール AzureRM では、.NET Framework を使用します。 そのため、.NET Core を使用する PowerShell 6.0 とは互換性がなくなります。 PowerShell 6.0 を使用している場合は、[macOS および Linux のインストール手順](install-azurermps-maclinux.md)に従います。

## <a name="install-the-azure-powershell-module"></a>Azure PowerShell モジュールのインストール

PowerShell ギャラリーからモジュールをインストールするには、昇格された特権が必要です。 Azure PowerShell をインストールするには、管理者特権のセッションで次のコマンドを実行します。

```powershell-interactive
Install-Module -Name AzureRM
```

> [!NOTE]
> ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。

既定では、PowerShell ギャラリーは、PowerShellGet の信頼できるリポジトリとしては構成されません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"):
```

インストールを続行するには、`Yes` または `Yes to All` を選択します。

`AzureRM` モジュールは、Azure PowerShell コマンドレットのロールアップ モジュールです。 これをインストールすると、利用可能な Azure Resource Manager モジュールがすべてダウンロードされ、コマンドレットを使用できるようになります。

## <a name="sign-in"></a>[サインイン]

Azure PowerShell の操作を開始するには、[Import-Module](/powershell/module/Microsoft.PowerShell.Core/Import-Module) コマンドレットを使用して、現在の PowerShell セッションに `AzureRM` を読み込み、Azure の資格情報でサインインする必要があります。

```powershell-interactive
# Import the module into the PowerShell session
Import-Module AzureRM
# Connect to Azure with an interactive dialog for sign-in
Connect-AzureRmAccount
```

新しい PowerShell セッションを開始するたびに、この手順を繰り返す必要があります。 `AzureRM` モジュールを自動的にインポートするには、PowerShell プロファイルを設定する必要があります。PowerShell プロファイルについては、「[About Profiles (プロファイルについて)](/powershell/module/microsoft.powershell.core/about/about_profiles)」をご覧ください。
Azure サインインをセッション間で維持する方法については、[PowerShell セッション間でのユーザーの資格情報の保持](context-persistence.md)に関する記事をご覧ください。

## <a name="update-the-azure-powershell-module"></a>Azure PowerShell モジュールの更新

Azure PowerShell のインストールを更新するには、[Update-Module](/powershell/module/powershellget/update-module) を実行します。 このコマンドでは、以前のバージョンはアンインストール__されません__。

```powershell-interactive
Update-Module -Name AzureRM
```

古いバージョンの Azure PowerShell をシステムから削除する場合は、「[Uninstall the Azure PowerShell module (Azure PowerShell モジュールのアンインストール)](uninstall-azurerm-ps.md)」をご覧ください。

## <a name="use-multiple-versions-of-azure-powershell"></a>複数のバージョンの Azure PowerShell の使用

複数のバージョンの Azure PowerShell をインストールできます。 オンプレミスの Azure Stack リソースを使用する場合、PowerShell 5.0 に更新できない古いバージョンの Windows を実行している場合、または Azure クラシック デプロイ モデルを使用している場合は、複数のバージョンが必要になります。 古いバージョンをインストールするには、インストール時に `-RequiredVersion` 引数を指定します。

```powershell-interactive
# Install version 1.2.9 of Azure PowerShell
Install-Module -Name AzureRM -RequiredVersion 1.2.9
```

Azure PowerShell モジュールの読み込み時には、最新バージョンが既定で読み込まれます。 別のバージョンを読み込むには、`-RequiredVersion` 引数を指定します。

```powershell-interactive
# Load version 1.2.9 of Azure PowerShell
Import-Module -Name AzureRM -RequiredVersion 1.2.9
```

## <a name="provide-feedback"></a>フィードバックの提供

Azure Powershell の使用時にバグが見つかった場合は、[GitHub で問題を報告](https://github.com/Azure/azure-powershell/issues)してください。
コマンド ラインからフィードバックを送るには、[Send-Feedback](/powershell/module/azurerm.profile/send-feedback) コマンドレットを使用します。

## <a name="next-steps"></a>次の手順

Azure PowerShell を使い始める場合、モジュールとその機能の詳細については、「[Get started with Azure PowerShell (Azure PowerShell の概要)](get-started-azureps.md)」をご覧ください。