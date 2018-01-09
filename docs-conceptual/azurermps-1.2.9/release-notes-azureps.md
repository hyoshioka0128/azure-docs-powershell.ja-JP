---
title: "Azure PowerShell の変更履歴 | Microsoft Docs"
description: "Azure PowerShell の最新リリースで行われた変更の履歴です。"
services: azure
author: sdwheeler
ms.author: sewhee
manager: carmonm
ms.service: azure-powershell
ms.product: azure
ms.devlang: powershell
ms.topic: conceptual
ms.workload: 
ms.date: 05/18/2017
ms.openlocfilehash: 5fe7591855577e083aad5923aed37b18d0b2a40c
ms.sourcegitcommit: b256bf48e15ee98865de0fae50e7b81878b03a54
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/03/2017
---
# <a name="release-notes"></a>リリース ノート

これは Azure PowerShell の今回のリリースで行われた変更の一覧です。

## <a name="version-129"></a>バージョン 1.2.9

このリリースの変更

* AzureRm.AzureStackAdmin モジュール
    + 管理者の Azure Resource Manager とテナントの Azure Resource Manager の分割に対応するために Add-AzureRmResourceProviderRegistration コマンドレットを変更しました。 新しいパラメーター (-ResourceManagerType) を追加しました。
    + 各コマンドレットから -AdminUri、-ApiVersion、-SubscriptionId、-Token の各パラメーターを削除しました。 これらのパラメーターが廃止予定であると、かねてからお伝えしてきましたが、今回でそれらが削除されたことになります。
* AzureStackStorage モジュール
    + コンテナーの移行のシナリオに対応するために新しいコマンドレットを追加しました。
    + 内部コンポーネントと基になる機能を参照するコマンドレットを削除しました。
* AzureRM.BootStrapper
    + バージョン プロファイルを使って Azure PowerShell コマンドレットのバージョンを管理する新しいモジュールを作成しました。