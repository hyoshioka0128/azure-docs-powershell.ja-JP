---
title: Azure PowerShell を使用してサインインする
description: Azure PowerShell で、ユーザーとして、あるいはサービス プリンシパルまたは Azure リソースのマネージド ID を使用してサインインする方法。
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: conceptual
ms.date: 09/04/2019
ms.openlocfilehash: 0de487cc34593ceac05aa2077358d692470dc23e
ms.sourcegitcommit: fb95591c45bb5f12b98e0690938d18f2ec611897
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/15/2020
ms.locfileid: "79402750"
---
# <a name="sign-in-with-azure-powershell"></a>Azure PowerShell を使用してサインインする

Azure PowerShell では、複数の認証方法がサポートされています。 [Azure Cloud Shell](/azure/cloud-shell/overview) を使用すると自動的にログインできるため、最も簡単に作業を開始できます。 ローカル インストールを利用すると、ブラウザーから対話形式でサインインできます。 自動化のスクリプトを記述するとき、必要なアクセス許可で[サービス プリンシパル](create-azure-service-principal-azureps.md)を使用する方法が推奨されます。 ユース ケースに対して可能な限りサインイン アクセス許可を制限することで、Azure リソースのセキュリティを維持できます。

サインイン後、コマンドが既定のサブスクリプションに対して実行されます。 セッションのアクティブ サブスクリプションを変更するには、[Set-AzContext](/powershell/module/az.accounts/set-azcontext) コマンドレットを使用します。 Azure PowerShell でログインするときに使用される既定のサブスクリプションを変更するには、[Set-AzDefault](/powershell/module/az.accounts/set-azdefault) を使用します。

> [!IMPORTANT]
>
> サインインしたままであれば、資格情報は複数の PowerShell セッション間で共有されます。
> 詳細については、[永続的な資格情報](context-persistence.md)に関する記事を参照してください。

## <a name="sign-in-interactively"></a>対話操作でサインインする

対話形式でサインインするには、[Connect-AzAccount](/powershell/module/az.accounts/connect-azaccount) コマンドレットを使用します。

```azurepowershell-interactive
Connect-AzAccount
```

このコマンドレットを実行すると、トークン文字列が表示されます。 サインインするには、この文字列をコピーし、ブラウザーの https://microsoft.com/devicelogin に貼り付けます。 Azure に接続するために PowerShell セッションが認証されます。

> [!IMPORTANT]
>
> ユーザー名とパスワードの資格情報による承認は、Active Directory 認証の実装の変更とセキュリティ上の懸念から、Azure PowerShell では削除されました。
> 資格情報による承認を使用して自動化を行う場合は、代わりに[サービス プリンシパルを作成](create-azure-service-principal-azureps.md)してください。

## <a name="sign-in-with-a-service-principal-a-namesp-signin"></a>サービス プリンシパルを使用してサインインする <a name="sp-signin"/>

サービス プリンシパルは、非対話型の Azure アカウントです。 他のユーザー アカウントと同様、そのアクセス許可は Azure Active Directory で管理されます。 サービス プリンシパルに、必要なアクセス許可のみを付与することで、自動化スクリプトのセキュリティが維持されます。

Azure PowerShell で使用するサービス プリンシパルを作成する方法については、「[Azure PowerShell で Azure サービス プリンシパルを作成する](create-azure-service-principal-azureps.md)」を参照してください。

サービス プリンシパルを使用してサインインするには、`Connect-AzAccount` コマンドレットで `-ServicePrincipal` 引数を使用します。 サービス プリンシパルのアプリケーション ID、サインイン資格情報、およびサービス プリンシパルに関連付けられたテナント ID も必要です。 サービス プリンシパルを使用してサインインする方法は、パスワードベースの認証用と証明書ベースの認証用のどちらに構成されているかによって異なります。

### <a name="password-based-authentication"></a>パスワードベースの認証

サービス プリンシパルの資格情報を適切なオブジェクトとして取得するには、[Get-Credential](/powershell/module/microsoft.powershell.security/get-credential) コマンドレットを使用します。 このコマンドレットによって、ユーザー名とパスワードの入力を求めるプロンプトが表示されます。 ユーザー名にはサービス プリンシパル ID を使用します。

```azurepowershell-interactive
$pscredential = Get-Credential
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

自動化のシナリオでは、ユーザー名とセキュリティで保護された文字列から資格情報を作成する必要があります。

```azurepowershell-interactive
$passwd = ConvertTo-SecureString <use a secure password here> -AsPlainText -Force
$pscredential = New-Object System.Management.Automation.PSCredential('service principal name/id', $passwd)
Connect-AzAccount -ServicePrincipal -Credential $pscredential -Tenant $tenantId
```

サービス プリンシパルへの接続を自動化する場合は、必ず適切なパスワード保存プラクティスを使用してください。

### <a name="certificate-based-authentication"></a>証明書ベースの認証

証明書ベースの認証では、Azure PowerShell で、証明書の拇印に基づいてローカル証明書ストアから情報を取得できる必要があります。

```azurepowershell-interactive
Connect-AzAccount -ApplicationId $appId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

登録されたアプリケーションではなくサービス プリンシパルを使用する場合は、`-ServicePrincipal` 引数を追加し、`-ApplicationId` パラメーターの値としてサービス プリンシパルのアプリケーション ID を指定します。

```azurepowershell-interactive
Connect-AzAccount -ServicePrincipal -ApplicationId $servicePrincipalId -Tenant $tenantId -CertificateThumbprint <thumbprint>
```

PowerShell 5.1 では、[PKI](/powershell/module/pkiclient) モジュールを使用して、証明書ストアを管理および検査できます。 PowerShell Core 6.x 以降の場合は、プロセスがさらに複雑になります。 次のスクリプトでは、PowerShell からアクセスできる証明書ストアに、既存の証明書をインポートする方法を示します。

#### <a name="import-a-certificate-in-powershell-51"></a>PowerShell 5.1 で証明書をインポートする

```azurepowershell-interactive
# Import a PFX
$credentials = Get-Credential -Message "Provide PFX private key password"
Import-PfxCertificate -FilePath <path to certificate> -Password $credentials.Password -CertStoreLocation cert:\CurrentUser\My
```

#### <a name="import-a-certificate-in-powershell-core-6x-and-later"></a>PowerShell Core 6.x 以降で証明書をインポートする

```azurepowershell-interactive
# Import a PFX
$storeName = [System.Security.Cryptography.X509Certificates.StoreName]::My 
$storeLocation = [System.Security.Cryptography.X509Certificates.StoreLocation]::CurrentUser 
$store = [System.Security.Cryptography.X509Certificates.X509Store]::new($storeName, $storeLocation) 
$certPath = <path to certificate>
$credentials = Get-Credential -Message "Provide PFX private key password"
$flag = [System.Security.Cryptography.X509Certificates.X509KeyStorageFlags]::Exportable 
$certificate = [System.Security.Cryptography.X509Certificates.X509Certificate2]::new($certPath, $credentials.Password, $flag) 
$store.Open([System.Security.Cryptography.X509Certificates.OpenFlags]::ReadWrite) 
$store.Add($Certificate) 
$store.Close()
```

## <a name="sign-in-using-a-managed-identity"></a>マネージド ID を使用したサインイン

マネージド ID は Azure Active Directory の機能です。 マネージド ID は、Azure で実行されるリソースに割り当てられたサービス プリンシパルです。 サインインにマネージド ID サービス プリンシパルを使用し、その他のリソースにアクセスするためにアプリ専用のアクセス トークンを取得できます。 マネージド ID は、Azure クラウドで実行されているリソースでのみ使用できます。

このコマンドは、ホスト環境のマネージド ID を使用して接続します。 たとえば、割り当てられたマネージド サービス ID を使用して VirtualMachine で実行した場合、コードはその割り当てられた ID を使用してサインインできます。

```azurepowershell-interactive
 Connect-AzAccount -Identity 
```

## <a name="sign-in-with-a-non-default-tenant-or-as-a-cloud-solution-provider-csp"></a>既定ではないテナントで、あるいはクラウド ソリューション プロバイダー (CSP) としてサインインする

アカウントが複数のテナントに関連付けられている場合、接続時に `-Tenant` パラメーターを使用することがサインインで要求されます。 このパラメーターはあらゆるサインイン メソッドで動作します。 ログイン時、テナントの Azure オブジェクト ID (テナント ID) またはテナントの完全修飾ドメイン名がこのパラメーター値になります。

[クラウド ソリューション プロバイダー (CSP)](https://azure.microsoft.com/offers/ms-azr-0145p/) の場合、`-Tenant` 値はテナント ID にすることが**必要**となります。

```azurepowershell-interactive
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

## <a name="sign-in-to-another-cloud"></a>別のクラウドにサインインする

Azure クラウド サービスでは、リージョンのデータ処理の法律に準拠した環境を提供します。
リージョン クラウド内のアカウントの場合は、サインインするときに `-Environment` 引数で環境を設定します。
このパラメーターはあらゆるサインイン メソッドで動作します。 たとえば、ご自身のアカウントが中国のクラウドにある場合は、次のように指定します。

```azurepowershell-interactive
Connect-AzAccount -Environment AzureChinaCloud
```

次のコマンドでは、使用可能な環境の一覧を取得します。

```azurepowershell-interactive
Get-AzEnvironment | Select-Object Name
```
