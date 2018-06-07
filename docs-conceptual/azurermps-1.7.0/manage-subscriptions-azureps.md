---
title: Azure PowerShell による Azure サブスクリプションの管理 | Microsoft Docs
description: Azure PowerShell による Azure サブスクリプションの管理
keywords: Azure PowerShell, サブスクリプション
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 03/30/2017
ms.openlocfilehash: d28da700efbc2927cb3f73ae696759fb1e0c0cd6
ms.sourcegitcommit: 2eea03b7ac19ad6d7c8097743d33c7ddb9c4df77
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/06/2018
ms.locfileid: "34820053"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="22b06-104">複数の Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="22b06-104">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="22b06-105">Azure を使い始めたばかりの場合、所有しているサブスクリプションは 1 つだけだと思われます。</span><span class="sxs-lookup"><span data-stu-id="22b06-105">If you are brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="22b06-106">一方、しばらく前から Azure を使用している場合は、複数の Azure サブスクリプションを作成済みであることも考えられます。</span><span class="sxs-lookup"><span data-stu-id="22b06-106">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="22b06-107">その場合は、特定のサブスクリプションに対してコマンドを実行するように Azure PowerShell を構成することができます。</span><span class="sxs-lookup"><span data-stu-id="22b06-107">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="22b06-108">アカウント内のすべてのサブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="22b06-108">Get a list of all subscriptions in your account.</span></span>

    ```powershell
    Get-AzureRmSubscription
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Production Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My DevTest Subscription
    CurrentStorageAccount :

    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

2. <span data-ttu-id="22b06-109">既定のサブスクリプションを設定します。</span><span class="sxs-lookup"><span data-stu-id="22b06-109">Set the default.</span></span>

    ```powershell
    Select-AzureRmSubscription -SubscriptionName "My Demos"
    ```

3. <span data-ttu-id="22b06-110">`Get-AzureRmContext` コマンドレットを実行して変更内容を確認します。</span><span class="sxs-lookup"><span data-stu-id="22b06-110">Verify the change by running the `Get-AzureRmContext` cmdlet.</span></span>

    ```powershell
    Get-AzureRmContext
    ```

    ```
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

<span data-ttu-id="22b06-111">既定のサブスクリプションを設定すると、後続のすべての Azure PowerShell コマンドは、このサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="22b06-111">Once you set your default subscription, all subsequent Azure PowerShell commands run against this subscription.</span></span>
