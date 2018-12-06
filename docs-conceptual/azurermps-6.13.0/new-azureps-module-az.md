---
title: Azure PowerShell Az モジュールの概要
description: AzureRM モジュールに代わる新しい Azure PowerShell Az モジュールの概要。
ms.date: 11/07/2018
author: sptramer
ms.author: sttramer
ms.manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.openlocfilehash: b0f31341d4344bdac5b4d657a1f66acfd9984dda
ms.sourcegitcommit: 93f93b90ef88c2659be95f3acaba514fe9639169
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/05/2018
ms.locfileid: "52828112"
---
# <a name="introducing-the-new-azure-powershell-az-module"></a>新しい Azure PowerShell Az モジュールの概要

2018 年 11 月以降、Azure PowerShell `Az` モジュールが完全なパブリック プレビューとして提供されます。
Az では、コマンドの短縮と安定性の向上が実現し、Windows、macOS、および Linux がサポートされます。 また、機能パリティと、AzureRM からの簡単な移行パスも提供されます。

Az では .NET Standard ライブラリが使用されます。つまり、PowerShell 5.x と PowerShell 6.x で実行できます。
PowerShell 6.x は Linux、macOS、および Windows で実行できるため、Az はすべてのプラットフォームで利用可能です。
.NET Standard を使用すると Azure PowerShell のコード ベースを統合でき、ユーザーへの影響を最小限に抑えることができます。

Az は新しいモジュールであるため、バージョンがリセットされます。 最初の安定版リリースが 1.0 になりますが、モジュールが AzureRm との機能パリティを持つのは 2018 年 11 月からです。

## <a name="upgrade-to-az"></a>Az にアップグレードする

新しい `Az` モジュールにアップグレードすることをお勧めします。 そのためには、次の手順を実行します。

* [Azure PowerShell AzureRM モジュールをアンインストールする](/powershell/azure/uninstall-azurerm-ps)
* [Azure PowerShell Az モジュールをインストールする](/powershell/azure/install-az-ps)
* `Enable-AzureRMAlias` を使用して AzureRM の互換モードを有効にし、新しいコマンド セットに慣れる

## <a name="migrate-existing-scripts-to-az"></a>Az に既存のスクリプトを移行する

主要な更新プログラムの適用には手間取る可能性があります。 ただし、`Az` モジュールには、新しい構文への更新に取り組みながら、既存のスクリプトを使用できるようにする互換モードがあります。 `AzureRM` 互換モードを有効にするには、`Enable-AzureRmAlias` コマンドレットを使用します。 このコマンドレットで、新しい `Az` コマンドレット名の別名として `AzureRM` コマンドレット名を定義できます。

新しいコマンドレット名は、覚えやすいように設計されています。 コマンドレット名では `AzureRm` や `Azure` を使用する代わりに、`Az` を使用します。 たとえば、古いコマンド `New-AzureRmVm` は `New-AzVm` になりました。

移行プロセスの詳細については、[AzureRM から Az への移行](migrate-from-azurerm-to-az.md)に関するページを参照してください。

## <a name="the-future-of-support-for-azurerm"></a>今後の AzureRM のサポート

`Az` バージョン 1.0 が 2018 年の 12 月にリリースされると、既存の `AzureRM` モジュールは新しいコマンドレットまたは機能を受け入れなくなります。 ただし、`AzureRM` は引き続き正式に維持され、バグの修正プログラムを取得できます。 Azure の最新のサービスと機能に対応するには、`Az` モジュールに切り替える必要があります。