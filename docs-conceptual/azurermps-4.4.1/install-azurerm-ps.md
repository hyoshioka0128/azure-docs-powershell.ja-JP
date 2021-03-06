---
title: Azure PowerShell のインストールおよび構成 | Microsoft Docs
description: 初めて使う Azure PowerShell をインストールして構成する方法について説明します。
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/27/2018
ms.openlocfilehash: 6f894546364e6a5ae06e1915a166edb258ccc698
ms.sourcegitcommit: 7839b82f47ef8dd522eff900081c22de0d089cfc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/14/2020
ms.locfileid: "83386750"
---
# <a name="install-azure-powershell-on-windows-with-powershellget"></a>PowerShellGet を使用した Windows への Azure PowerShell のインストール

[!INCLUDE [migrate-to-az](../includes/migrate-to-az.md)]

この記事では、PowerShellGet を使用して、Windows 用 PowerShell 5.x の Azure PowerShell モジュールをインストールする手順について説明します。 Azure PowerShell をインストールするときは、PowerShellGet およびモジュール管理を使用することをお勧めしますが、Web Platform Installer または MSI パッケージを使ってインストールすることもできます。方法については、[その他のインストール方法](other-install.md)に関する記事をご覧ください。

このバージョンの Azure PowerShell では、Azure クラシック デプロイ モデルはサポートされていません。 クラシック デプロイのサポートについては、「[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)」の手順に従ってください。

> [!IMPORTANT]
> AzureRM モジュールは、macOS または Linux ではサポートされません。 これらのプラットフォームで Azure PowerShell コマンドレットを使用するには、[Az モジュールをインストール](/powershell/azure/install-az-ps)します。

## <a name="step-1-install-powershellget"></a>手順 1:PowerShellGet をインストールする

PowerShell ギャラリーからソフトウェアをインストールするには、PowerShellGet モジュールが必要です。 PowerShellGet のバージョンが適切であるかなど、システム要件を満たしていることを確認してください。 ご使用のシステムに PowerShellGet がインストールされているかどうかを確認するには、次のコマンドを実行します。


```powershell-interactive
Get-InstalledModule -Name PowerShellGet -ListAvailable | Select-Object -Property Name,Version,Path
```

次のような出力結果が表示されます。

```Output
Name          Version Path
----          ------- ----
Name          Version Path
----          ------- ----
PowerShellGet 1.6.0   C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.6.0\PowerShellGet.psd1
PowerShellGet 1.0.0.1 C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PowerShellGet.psd1
```

PowerShellGet バージョン 1.1.2.0 以降が必要です。 PowerShellGet を更新するには、次のコマンドを使用します。

```powershell-interactive
Install-Module PowerShellGet -Force
```

PowerShellGet がインストールされていない場合は、この記事の「[PowerShellGet の入手方法](#how-to-get-powershellget)」のセクションをご覧ください。

> [!NOTE]
> PowerShellGet を使用するには、実行ポリシーでスクリプトの実行が許可されている必要があります。 PowerShell の実行ポリシーについて詳しくは、「[About Execution Policies (実行ポリシーについて)](/powershell/module/microsoft.powershell.core/about/about_execution_policies)」をご覧ください。
>
> [!IMPORTANT]
> このドキュメントで説明するモジュール AzureRM では、.NET Framework を使用します。 そのため、.NET Core を使用する PowerShell 6.0 とは互換性がなくなります。 PowerShell 6.0 を使用している場合は、[macOS および Linux のインストール手順](install-azurermps-maclinux.md)に従います。

## <a name="step-2-install-azure-powershell"></a>手順 2:Azure PowerShell をインストールする

Azure PowerShell を PowerShell ギャラリーからインストールするためには、昇格された特権が必要です。 管理者特権の PowerShell セッションから次のコマンドを実行します。

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

既定では、PowerShell ギャラリーは PowerShellGet の信頼できるリポジトリとして構成されていません。 PSGallery の初回使用時には、次のプロンプトが表示されます。

```Output
Untrusted repository

You are installing the modules from an untrusted repository. If you trust this repository, change
its InstallationPolicy value by running the Set-PSRepository cmdlet.

Are you sure you want to install the modules from 'PSGallery'?
[Y] Yes  [A] Yes to All  [N] No  [L] No to All  [S] Suspend  [?] Help (default is "N"): Y
```

インストールを続行するには、"Yes" または "Yes to All" と回答します。

> [!NOTE]
> ご利用の NuGet のバージョンが 2.8.5.201 未満である場合、最新バージョンの NuGet をダウンロードしてインストールするように求められます。

AzureRM モジュールは、Azure Resource Manager コマンドレットのロールアップ モジュールです。 AzureRM モジュールをインストールすると、まだインストールしていない Azure PowerShell モジュールが PowerShell ギャラリーからダウンロードされます。

以前のバージョンの Azure PowerShell がインストールされている場合、エラーが発生する可能性があります。 この問題を解決するには、この記事の「[新しいバージョンの Azure PowerShell に更新する](#update-azps)」を参照してください。

## <a name="step-3-load-the-azurerm-module"></a>手順 3:AzureRM モジュールを読み込む

モジュールは、インストール後、PowerShell セッションに読み込む必要があります。 これは通常の (管理者特権ではない) PowerShell セッションで実行する必要があります。 モジュールを読み込むには、次のように `Import-Module` コマンドレットを使います。

```powershell-interactive
Import-Module -Name AzureRM
```

## <a name="next-steps"></a>次の手順

Azure PowerShell の使用について詳しくは、次の記事をご覧ください。

* [Azure PowerShell の概要](get-started-azureps.md)

## <a name="reporting-issues-and-feedback"></a>問題とフィードバックの報告

ツールにバグを発見した場合は、GitHub リポジトリの [[Issues (問題)]](https://github.com/Azure/azure-powershell/issues) セクションで問題を報告してください。 コマンド ラインからフィードバックを送るには、`Send-Feedback` コマンドレットを使用します。

## <a name="frequently-asked-questions"></a>よく寄せられる質問

### <a name="how-to-get-powershellget"></a>PowerShellGet の入手方法

|OS バージョン|インストール手順|
|---|---|
|Windows 10 または Windows Server 2016 を所有している|OS 標準の Windows Management Framework (WMF) 5.0 に組み込まれています。|
|PowerShell 5 にアップグレードしたい|[最新バージョンの WMF をインストール](https://www.microsoft.com/download/details.aspx?id=54616)します。|
|PowerShell 3 または PowerShell 4 が付属するバージョンの Windows を使っている|[PackageManagement モジュールを入手](https://go.microsoft.com/fwlink/?LinkID=746217)します。|

### <a name="div-idhelpmechoosechecking-the-version-of-azure-powershell"></a><div id="helpmechoose"/>Azure PowerShell のバージョン確認

Azure PowerShell は、できるだけ早く最新バージョンにアップグレードすることをお勧めしますが、いくつかのバージョンがサポートされています。 インストールされている Azure PowerShell のバージョンを確認するには、コマンド ラインから `Get-InstalledModule AzureRM` を実行します。

```powershell-interactive
Get-InstalledModule AzureRM -AllVersions | Select-Object -Property Name,Version,Path
```

### <a name="support-for-classic-deployment-methods"></a>クラシック デプロイ方法のサポート

クラシック デプロイ モデルを現在の環境で使っている場合は、Service Management 版の Azure PowerShell をインストールできます。 詳しくは、[Azure PowerShell Service Management モジュールのインストール](/powershell/azure/servicemanagement/install-azure-ps)に関するページをご覧ください。 Azure と AzureRM のモジュールは、依存するコンポーネントが共通しています。 Azure と AzureRM の両方のモジュールを使用する場合は、各パッケージの同じバージョンをインストールする必要があります。

### <a name="div-idupdate-azpsupdating-to-a-new-version-of-azure-powershell"></a><div id="update-azps"/>新しいバージョンの Azure PowerShell に更新する

Service Management モジュールを含む、以前のバージョンの Azure PowerShell がインストールされている場合は、次のエラーが発生する可能性があります。

```Output
PackageManagement\Install-Package : A command with name 'Get-AzureStorageContainerAcl' is already
available on this system. This module 'Azure.Storage' may override the existing commands. If you
still want to install this module 'Azure.Storage', use -AllowClobber parameter.

At C:\Program Files\WindowsPowerShell\Modules\PowerShellGet\1.0.0.1\PSModule.psm1:1772 char:21
+ ...          $null = PackageManagement\Install-Package @PSBoundParameters
+                      ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
    + CategoryInfo          : InvalidOperation: (Microsoft.Power....InstallPackage:InstallPackage) [Install-Package], Exception
    + FullyQualifiedErrorId : CommandAlreadyAvailable,Validate-ModuleCommandAlreadyAvailable,Microsoft.PowerShell.PackageManagement.Cmdlets.InstallPackage
```

エラー メッセージが示すように、AllowClobber パラメーターを使用してモジュールをインストールする必要があります。 次のコマンドを使用します。

```powershell-interactive
# Install the Azure Resource Manager modules from the PowerShell Gallery
Install-Module -Name AzureRM -AllowClobber
```

詳細については、[Install-Module](https://msdn.microsoft.com/powershell/reference/5.1/PowerShellGet/install-module) に関するヘルプ トピックをご覧ください。

### <a name="installing-module-versions-side-by-side"></a>サイド バイ サイド構成でのモジュール バージョンのインストール

複数バージョンのインストールに対応しているのは、PowerShellGet を使ったインストール方法だけです。 たとえば、以前のバージョンの Azure PowerShell で記述されたスクリプトがあり、更新する時間も人材も確保できないことがあります。 次のコマンドで、複数バージョンの Azure PowerShell をインストールすることができます。

```powershell-interactive
Install-Module -Name AzureRM -RequiredVersion 3.7.0
Install-Module -Name AzureRM -RequiredVersion 2.3.0
```

PowerShell セッションに読み込むことができるモジュールのバージョンは 1 つだけです。 特定のバージョンの AzureRM コマンドレットをインポートするには、新たに PowerShell ウィンドウを開いて `Import-Module` を実行する必要があります。

```powershell-interactive
Import-Module -Name AzureRM -RequiredVersion 2.3.0
```

> [!NOTE]
> 共存インストールでの使用が想定された最初のモジュール バージョンは、バージョン 2.1.0 とバージョン 1.2.6 です。 以前のバージョンの Azure PowerShell を読み込むと、互換性のないバージョンの **AzureRM.Profile** モジュールが読み込まれます。 このため、コマンドレットでは、コマンドレットを実行するたびにサインインを要求されます。

### <a name="other-installation-methods"></a>その他のインストール方法

Web プラットフォーム インストーラーまたは MSI パッケージを使ったインストールについては、「[Other installation methods (その他のインストール方法)](other-install.md)」をご覧ください。
