---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 10/29/2018
ms.openlocfilehash: 8b085720aeabe26c1293ece193e050b31f99a693
ms.sourcegitcommit: ae81b08a45d8729fc8d40156422e3eb2e94de8c7
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/27/2018
ms.locfileid: "53786681"
---
# <a name="sign-in-with-azure-powershell"></a>Azure PowerShell を使用してサインインする

Azure PowerShell では、複数の認証方法がサポートされています。 最も簡単に始められるのは、コマンド ラインから対話形式でサインインする方法です。

## <a name="sign-in-interactively"></a>対話操作でサインインする

対話形式でサインインするには、[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用します。

```azurepowershell-interactive
Connect-AzAccount
```

このコマンドレットを実行すると、トークン文字列が表示されます。 ログインするには、この文字列をコピーし、ブラウザーの https://microsoft.com/devicelogin に貼り付けます。 Azure に接続するために PowerShell セッションが認証されます。 この認証は、現在の PowerShell セッションが終了するまで有効です。

> [!IMPORTANT]
>
> サインインしたままであれば、資格情報は複数の PowerShell セッション間で共有されます。
> 詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。

## <a name="sign-in-with-a-service-principal"></a>サービス プリンシパルを使ってサインインする

サービス プリンシパルは、非対話型の Azure アカウントです。 他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。 サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。

Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。

サービス プリンシパルを使用してサインインするには、`Connect-AzAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。 サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。 サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。 このコマンドレットでは、サービス プリンシパルのユーザー ID とパスワードの入力を求められます。

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -ApplicationId  "http://my-app" -Credential $pscredential -TenantId $tenantid
```

## <a name="sign-in-using-an-azure-managed-service-identity"></a>Azure マネージド サービス ID を使用してサインインする

Azure リソースのマネージドID は、Azure Active Directory の機能です。 サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。 マネージド ID は、Azure クラウドで実行されている仮想マシンでのみ使用できます。

Azure リソースのマネージド ID の詳細については、「[How to use managed identities for Azure resources on an Azure VM to acquire an access token (Azure VM 上で Azure リソースのマネージド ID を使用してアクセス トークンを取得する方法)](/azure/active-directory/managed-identities-azure-resources/how-to-use-vm-token)」を参照してください。

## <a name="sign-in-as-a-cloud-solution-provider-csp"></a>クラウド ソリューション プロバイダー (CSP) としてサインインする

[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/en-us/offers/ms-azr-0145p/) のサインインには、`-TenantId` を使用する必要があります。 通常は、このパラメーターにはテナント ID またはドメイン名を指定できます。 しかし、CSP のサインインの場合、**テナント ID** を指定する必要があります。

```azurepowershell-interactive
Connect-AzAccount -TenantId 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>別のクラウドにサインインする

Azure クラウド サービスでは、リージョンのデータ処理規制に準拠した環境を提供します。
リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。
たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

次のコマンドでは、使用可能な環境の一覧を取得します。

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```

## <a name="learn-more-about-managing-azure-role-based-access"></a>Azure ロールベース アクセスの管理についての詳細情報

Azure での認証とサブスクリプション管理の詳細については、[アカウント、サブスクリプション、管理者ロールの管理](/azure/active-directory/role-based-access-control-configure)に関するページを参照してください。

ロール管理を目的とした Azure PowerShell のコマンドレット:

* [Get-AzRoleAssignment](/powershell/module/az.Resources/Get-azRoleAssignment)
* [Get-AzRoleDefinition](/powershell/module/az.Resources/Get-azRoleDefinition)
* [New-AzRoleAssignment](/powershell/module/az.Resources/New-azRoleAssignment)
* [New-AzRoleDefinition](/powershell/module/az.Resources/New-azRoleDefinition)
* [Remove-AzRoleAssignment](/powershell/module/az.Resources/Remove-azRoleAssignment)
* [Remove-AzRoleDefinition](/powershell/module/az.Resources/Remove-azRoleDefinition)
* [Set-AzRoleDefinition](/powershell/module/az.Resources/Set-azRoleDefinition)
