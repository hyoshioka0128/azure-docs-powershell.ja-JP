---
title: Azure PowerShell の概要
description: Azure PowerShell Az モジュールの概要と、インストールして使い始める方法に関する情報。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.manager: carmonm
ms.date: 01/10/2019
ms.openlocfilehash: 45ab083dd133c8c7b8dbe902484c92564bc216b9
ms.sourcegitcommit: ae4540a90508db73335a54408dfd6cdf3712a1e9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/17/2019
ms.locfileid: "59364164"
---
# <a name="overview-of-azure-powershell"></a>Azure PowerShell の概要

Azure PowerShell には、Azure リソースの管理に [Azure Resource Manager](/azure/azure-resource-manager/resource-group-overview) モデルを使う一連のコマンドレットが用意されています。 Azure PowerShell では .NET Standard が使用されているので、Windows、macOS、Linux で使用できます。
Azure PowerShell は、Azure Cloud Shell 上で利用することもできます。

## <a name="about-the-new-az-module"></a>新しい Az モジュールについて

このドキュメントでは、Azure PowerShell の新しい Az モジュールについて説明します。 この新しいモジュールは、.NET Standard で一から作成されています。 .NET Standard の使用により、Azure PowerShell は Windows 上の PowerShell 5 または任意のプラットフォーム上の PowerShell 6 で実行できます。 PowerShell を使用して Azure を操作するときに、Az モジュールが使用されるようになりました。
AzureRM はバグの修正プログラムを引き続き取得できますが、新機能は追加されなくなります。

コマンド名の変更や、AzureRM のメンテナンス プランなど、新しいモジュールの詳細については、[Azure PowerShell Az モジュールの概要](new-azureps-module-az.md)に関する記事をご覧ください。 新しいモジュールをすぐに使い始める場合は、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。

[AzureRM のドキュメント](/powershell/azure/azurerm)も利用できます。

> [!IMPORTANT]
>
> 新しいモジュールのコマンドレット名を反映するために、Azure のドキュメントを更新中ですが、記事で AzureRM コマンドが引き続き使用されている場合があります。 Az モジュールをインストールしたら、`Enable-AzureRmAlias` を使用して、AzureRM コマンドレットのエイリアスを有効にすることをお勧めします。 詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関する記事をご覧ください。

## <a name="run-or-install"></a>実行またはインストール

Azure PowerShell は、Windows 上の PowerShell 5.1 以上に、または任意のプラットフォーム上の PowerShell 6 にインストールでき、Azure Cloud Shell で実行できます。

* Azure Cloud Shell を使用したブラウザーでの実行方法については、「[Azure Cloud Shell の PowerShell のクイックスタート](/azure/cloud-shell/quickstart-powershell)」をご覧ください。
* お使いのシステムに Azure PowerShell をインストールするには、「[Azure PowerShell のインストール](install-az-ps.md)」をご覧ください。

Azure PowerShell の最新リリースについては、[リリース ノート](release-notes-azureps.md)をご覧ください。

## <a name="get-started"></a>作業の開始

Azure PowerShell の基礎を学ぶには、[Azure PowerShell の使用に関するページ](get-started-azureps.md)をご覧ください。 PowerShell について初めて学ぶ場合は、概要に関するページからご覧ください。

* [PowerShell のインストール](/powershell/scripting/install/installing-powershell)
* [PowerShell を使用したスクリプト](/powershell/scripting/powershell-scripting)
* [PowerShell の基礎: (パート 1) PowerShell の概要](https://channel9.msdn.com/Blogs/Taste-of-Premier/PowerShellBasicsPart1)
* Microsoft Virtual Academy の [PowerShell の概要](https://mva.microsoft.com/liveevents/powershell-jumpstart)

次のサンプルは、Azure の一般的な使用法の理解に役立ちます。

* [Linux Virtual Machines](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=/powershell/azure/toc.json)
* [Windows Virtual Machines](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=/powershell/azure/toc.json)
* [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=/powershell/azure/toc.json)
* [SQL Database](/azure/sql-database/sql-database-powershell-samples?toc=/powershell/azure/toc.json)

## <a name="build-your-skills-with-microsoft-learn"></a>Microsoft Learn でスキルを身に付ける

- [PowerShell でスクリプトを使用した Azure タスクの自動化](/learn/modules/automate-azure-tasks-with-powershell/)
- [対話型学習の詳細...](/learn/browse/?term=powershell)

## <a name="other-azure-powershell-modules"></a>その他の Azure PowerShell モジュール

* [Azure Active Directory](/powershell/azure/active-directory/)
* [Azure Service Fabric](/powershell/azure/service-fabric/)
* [Azure ElasticDB](/powershell/azure/elasticdbjobs/)
