---
title: Azure PowerShell による Azure サブスクリプションの管理
description: Azure PowerShell による Azure サブスクリプションの管理
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/11/2018
ms.openlocfilehash: 41cf9b06f736f22eb3c2a9e2fbe1f047534cc09d
ms.sourcegitcommit: 797c18f93aaa495ef005993b2e202d7378588dfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/19/2018
ms.locfileid: "53594887"
---
# <a name="manage-multiple-azure-subscriptions"></a><span data-ttu-id="f9de5-103">複数の Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="f9de5-103">Manage multiple Azure subscriptions</span></span>

<span data-ttu-id="f9de5-104">Azure を使い始めたばかりの場合、所有しているサブスクリプションは 1 つだけだと思われます。</span><span class="sxs-lookup"><span data-stu-id="f9de5-104">If you're brand new to Azure, you probably only have a single subscription.</span></span> <span data-ttu-id="f9de5-105">一方、しばらく前から Azure を使用している場合は、複数の Azure サブスクリプションを作成済みであることも考えられます。</span><span class="sxs-lookup"><span data-stu-id="f9de5-105">But if you have been using Azure for a while, you may have created multiple Azure subscriptions.</span></span> <span data-ttu-id="f9de5-106">その場合は、特定のサブスクリプションに対してコマンドを実行するように Azure PowerShell を構成することができます。</span><span class="sxs-lookup"><span data-stu-id="f9de5-106">You can configure Azure PowerShell to execute commands against a particular subscription.</span></span>

1. <span data-ttu-id="f9de5-107">アカウント内のすべてのサブスクリプションの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="f9de5-107">Get a list of all subscriptions in your account.</span></span>

    ```azurepowershell-interactive
    Get-AzSubscription
    ```

    ```output
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

2. <span data-ttu-id="f9de5-108">既定のサブスクリプションを設定します。</span><span class="sxs-lookup"><span data-stu-id="f9de5-108">Set the default.</span></span>

    ```azurepowershell-interactive
    Select-AzSubscription -Subscription "My Demos"
    ```

3. <span data-ttu-id="f9de5-109">`Get-AzContext` コマンドレットを実行して変更内容を確認します。</span><span class="sxs-lookup"><span data-stu-id="f9de5-109">Verify the change by running the `Get-AzContext` cmdlet.</span></span>

    ```azurepowershell-interactive
    Get-AzContext
    ```

    ```output
    Environment           : AzureCloud
    Account               : username@contoso.com
    TenantId              : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionId        : XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX
    SubscriptionName      : My Demos
    CurrentStorageAccount :
    ```

<span data-ttu-id="f9de5-110">既定のサブスクリプションを設定すると、すべての Azure PowerShell コマンドが、このサブスクリプションに対して実行されます。</span><span class="sxs-lookup"><span data-stu-id="f9de5-110">Once you set your default subscription, all Azure PowerShell commands run against this subscription.</span></span>
