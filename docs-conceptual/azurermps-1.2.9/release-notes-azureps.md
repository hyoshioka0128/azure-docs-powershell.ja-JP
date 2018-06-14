---
title: Azure PowerShell の変更履歴 | Microsoft Docs
description: Azure PowerShell の最新リリースで行われた変更の履歴です。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.workload: ''
ms.date: 05/18/2017
ms.openlocfilehash: 91d97260568a36e1135196899503fb0c8e1c6731
ms.sourcegitcommit: c98e3a21037ebd82936828bcb544eed902b24212
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/08/2018
ms.locfileid: "34853017"
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-129"></a>バージョン 1.2.9

このリリースの変更

* AzureRm.AzureStackAdmin モジュール
    + 管理者の Azure Resource Manager とテナントの Azure Resource Manager の分割に対応するために Add-AzureRmResourceProviderRegistration コマンドレットを変更しました。 新しいパラメーター (-ResourceManagerType) を追加しました。
    + 各コマンドレットから -AdminUri、-ApiVersion、-SubscriptionId、-Token の各パラメーターを削除しました。 これらのパラメーターが非推奨となる予定であると、かねてからお伝えしてきましたが、今回でそれらが削除されたことになります。
* AzureStackStorage モジュール
    + コンテナーの移行のシナリオに対応するために新しいコマンドレットを追加しました。
    + 内部コンポーネントと基になる機能を参照するコマンドレットを削除しました。
* AzureRM.BootStrapper
    + バージョン プロファイルを使って Azure PowerShell コマンドレットのバージョンを管理する新しいモジュールを作成しました。