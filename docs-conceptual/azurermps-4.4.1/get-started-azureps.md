---
title: Azure PowerShell を使ってみる | Microsoft Docs
description: ''
author: sptramer
ms.author: sttramer
manager: carmonm
ms.devlang: powershell
ms.topic: get-started-article
ms.date: 11/15/2017
ms.openlocfilehash: 7eb5e3fad31b5a92be1cfb36aefdaa7b920bae5f
ms.sourcegitcommit: ac4b53bb42a25aae013a9d8cd9ae98ada9397274
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/08/2018
ms.locfileid: "51273975"
---
# <a name="getting-started-with-azure-powershell"></a><span data-ttu-id="1b4f1-102">Azure PowerShell を使ってみる</span><span class="sxs-lookup"><span data-stu-id="1b4f1-102">Getting started with Azure PowerShell</span></span>

<span data-ttu-id="1b4f1-103">Azure PowerShell は、コマンド ラインから Azure リソースを管理したり、Azure Resource Manager を操作対象とする自動化スクリプトを作成したりできるように設計されています。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-103">Azure PowerShell is designed for managing and administering Azure resources from the command line, and for building automation scripts that work against the Azure Resource Manager.</span></span> <span data-ttu-id="1b4f1-104">これは、[Azure Cloud Shell](/azure/cloud-shell/overview) を使用してブラウザーで使用することも、ローカル コンピューターにインストールして PowerShell セッションで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-104">You can use it in your browser with [Azure Cloud Shell](/azure/cloud-shell/overview), or you can install it on your local machine and use it in any PowerShell session.</span></span> <span data-ttu-id="1b4f1-105">この記事では、その基本的な使い方と核となる概念について説明します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-105">This article helps get you started using it, and teaches you the core concepts behind it.</span></span>

## <a name="connect"></a><span data-ttu-id="1b4f1-106">接続</span><span class="sxs-lookup"><span data-stu-id="1b4f1-106">Connect</span></span>

<span data-ttu-id="1b4f1-107">最も簡単に始められるのは、[Cloud Shell を起動](/azure/cloud-shell/quickstart)する方法です。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-107">The simplest way to get started is to [launch Cloud Shell](/azure/cloud-shell/quickstart).</span></span>

1. <span data-ttu-id="1b4f1-108">Cloud Shell は、Azure Portal の上部のナビゲーションから起動します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-108">Launch Cloud Shell from the top navigation of the Azure portal.</span></span>

   ![Shell アイコン](~/media/get-started-azureps/shell-icon.png)

2. <span data-ttu-id="1b4f1-110">使用するサブスクリプションを選択し、ストレージ アカウントを作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-110">Choose the subscription you want to use and create a storage account.</span></span>

   ![ストレージ アカウントの作成](~/media/get-started-azureps/storage-prompt.png)

<span data-ttu-id="1b4f1-112">ストレージが作成されたら、Cloud Shell によってブラウザーで PowerShell セッションが開きます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-112">Once your storage has been created, the Cloud Shell will open a PowerShell session in the browser.</span></span>

![Cloud Shell for PowerShell](~/media/get-started-azureps/cloud-powershell.png)

<span data-ttu-id="1b4f1-114">Azure PowerShell をインストールし、ローカルの PowerShell セッションで使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-114">You can also install Azure PowerShell and use it locally in a PowerShell session.</span></span>

## <a name="install-azure-powershell"></a><span data-ttu-id="1b4f1-115">Azure PowerShell をインストールする</span><span class="sxs-lookup"><span data-stu-id="1b4f1-115">Install Azure PowerShell</span></span>

<span data-ttu-id="1b4f1-116">初めに最新バージョンの Azure PowerShell がインストールされていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-116">The first step is to make sure you have the latest version of the Azure PowerShell installed.</span></span> <span data-ttu-id="1b4f1-117">最新リリースについては、[リリース ノート](./release-notes-azureps.md)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-117">For information about the latest release, see the [release notes](./release-notes-azureps.md).</span></span>

1. <span data-ttu-id="1b4f1-118">[Azure PowerShell をインストールします](install-azurerm-ps.md)。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-118">[Install Azure PowerShell](install-azurerm-ps.md).</span></span>

2. <span data-ttu-id="1b4f1-119">インストールが成功したことを確認するために、コマンド ラインから `Get-Module AzureRM -ListAvailable` を実行します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-119">To verify the installation was successful, run `Get-Module AzureRM -ListAvailable` from your command line.</span></span>

## <a name="sign-in-to-azure"></a><span data-ttu-id="1b4f1-120">Azure へのサインイン</span><span class="sxs-lookup"><span data-stu-id="1b4f1-120">Sign in to Azure</span></span>

<span data-ttu-id="1b4f1-121">対話操作でサインオンするには:</span><span class="sxs-lookup"><span data-stu-id="1b4f1-121">Sign on interactively:</span></span>

1. <span data-ttu-id="1b4f1-122">「 `Login-AzureRmAccount`」と入力します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-122">Type `Login-AzureRmAccount`.</span></span> <span data-ttu-id="1b4f1-123">Azure の資格情報の入力を求めるダイアログ ボックスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-123">You will get dialog box asking for your Azure credentials.</span></span> <span data-ttu-id="1b4f1-124">"-EnvironmentName" オプションを使用すると、Azure China または Azure Germany を認証できます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-124">Option '-EnvironmentName' can let you authenticate for Azure China or Azure Germany.</span></span>

   <span data-ttu-id="1b4f1-125">例: Login-AzureRmAccount -EnvironmentName AzureChinaCloud</span><span class="sxs-lookup"><span data-stu-id="1b4f1-125">e.g. Login-AzureRmAccount -EnvironmentName AzureChinaCloud</span></span>

2. <span data-ttu-id="1b4f1-126">アカウントに関連付けられている電子メール アドレスとパスワードを入力します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-126">Type the email address and password associated with your account.</span></span> <span data-ttu-id="1b4f1-127">Azure により資格情報が認証および保存され、ウィンドウが閉じます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-127">Azure authenticates and saves the credential information, and then closes the window.</span></span>

<span data-ttu-id="1b4f1-128">Azure アカウントへのサインイン後、Azure PowerShell のコマンドレットを使って自分のサブスクリプションのリソースにアクセスし、管理することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-128">Once you have signed in to an Azure account, you can use the Azure PowerShell cmdlets to access and manager the resources in your subscription.</span></span>

## <a name="create-a-resource-group"></a><span data-ttu-id="1b4f1-129">リソース グループの作成</span><span class="sxs-lookup"><span data-stu-id="1b4f1-129">Create a resource group</span></span>

<span data-ttu-id="1b4f1-130">必要な設定がすべて整ったら、Azure PowerShell を使って Azure にリソースを作成してみましょう。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-130">Now that we've got everything set up, let's use Azure PowerShell to create resources within Azure.</span></span>

<span data-ttu-id="1b4f1-131">まずリソース グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-131">First, create a Resource Group.</span></span> <span data-ttu-id="1b4f1-132">Azure ではリソース グループを使うことで、複数のリソースを論理上のグループとして 1 つにまとめて管理することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-132">Resource Groups in Azure provide a way to manage multiple resources that you want to logically group together.</span></span> <span data-ttu-id="1b4f1-133">たとえばアプリケーションまたはプロジェクトのリソース グループを作成し、仮想マシンやデータベース、CDN サービスをそこに追加することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-133">For example, you might create a Resource Group for an application or project and add a virtual machine, a database and a CDN service within it.</span></span>

<span data-ttu-id="1b4f1-134">"MyResourceGroup" という名前のリソース グループを Azure の westeurope リージョンに作成しましょう。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-134">Let's create a resource group named "MyResourceGroup" in the westeurope region of Azure.</span></span> <span data-ttu-id="1b4f1-135">そのためには次のコマンドを入力します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-135">To do so type the following command:</span></span>

```powershell-interactive
New-AzureRmResourceGroup -Name 'myResourceGroup' -Location 'westeurope'
```

```Output
ResourceGroupName : myResourceGroup
Location          : westeurope
ProvisioningState : Succeeded
Tags              :
ResourceId        : /subscriptions/XXXXXXXX-XXXX-XXXX-XXXX-XXXXXXXXXXXX/resourceGroups/myResourceGroup
```

## <a name="create-a-windows-virtual-machine"></a><span data-ttu-id="1b4f1-136">Windows 仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="1b4f1-136">Create a Windows Virtual Machine</span></span>

<span data-ttu-id="1b4f1-137">リソース グループが完成したら、そこに Windows VM を作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-137">Now that we have our resource group, let's create a Windows VM within it.</span></span> <span data-ttu-id="1b4f1-138">新しい VM を作成するには、その他の必要なリソースを最初に作成し、構成に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-138">To create a new VM we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="1b4f1-139">その構成を使って VM を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-139">Then we can use that configuration to create the VM.</span></span>

### <a name="create-the-required-network-resources"></a><span data-ttu-id="1b4f1-140">必要なネットワーク リソースの作成</span><span class="sxs-lookup"><span data-stu-id="1b4f1-140">Create the required network resources</span></span>

<span data-ttu-id="1b4f1-141">まず、仮想ネットワークの作成プロセスで使用するサブネット構成を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-141">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="1b4f1-142">その VM に接続できるように、さらにパブリック IP アドレスも作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-142">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="1b4f1-143">そのパブリック アドレスへのアクセスについては、ネットワーク セキュリティ グループを作成してセキュリティを確保します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-143">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="1b4f1-144">最後に、前述のリソースをすべて使って仮想 NIC を作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-144">Finally we create the virtual NIC using all of the previous resources.</span></span>

```powershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myWindowsVM"

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet1 -AddressPrefix 192.168.1.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET1 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 3389
$nsgRuleRDP = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleRDP  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 3389 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup1 -SecurityRules $nsgRuleRDP

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic1 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="1b4f1-145">仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="1b4f1-145">Create the virtual machine</span></span>

<span data-ttu-id="1b4f1-146">最初に、OS の一連の資格情報が必要です。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-146">First we need a set of credentials for the OS.</span></span>

```powershell-interactive
# Create user object
$cred = Get-Credential -Message "Enter a username and password for the virtual machine."
```

<span data-ttu-id="1b4f1-147">これで必要なリソースが揃ったので、VM を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-147">Now that we have the required resources we can create the VM.</span></span> <span data-ttu-id="1b4f1-148">このステップでは、VM 構成オブジェクトを作成し、その構成を使って VM を作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-148">For this step, we create a VM configuration object, then we use the configuration to create the VM.</span></span>

```powershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Windows -ComputerName $vmName -Credential $cred |
  Set-AzureRmVMSourceImage -PublisherName MicrosoftWindowsServer -Offer WindowsServer -Skus 2016-Datacenter -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="1b4f1-149">VM の作成が完了し、使用する準備ができると、`New-AzureRmVM` コマンドから結果が出力されます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-149">The `New-AzureRmVM` command outputs results once the VM has been fully created and is ready to be used.</span></span>

```Output
RequestId IsSuccessStatusCode StatusCode ReasonPhrase
--------- ------------------- ---------- ------------
                         True         OK OK
```

<span data-ttu-id="1b4f1-150">新しく作成した Windows Server VM のパブリック IP アドレスとリモート デスクトップを使って VM にサインインします。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-150">Now sign in to your newly created Windows Server VM using Remote Desktop and the public IP address of the VM.</span></span> <span data-ttu-id="1b4f1-151">次のコマンドを実行すると、前述のスクリプトで作成したパブリック IP アドレスが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-151">The following command displays the public IP address created in the previous script.</span></span>

```powershell-interactive
$publicIp | Select-Object Name,IpAddress
```

```Output
Name                  IpAddress
----                  ---------
mypublicdns1400512543 xx.xx.xx.xx
```

<span data-ttu-id="1b4f1-152">Windows ベースのシステムでは、コマンド ラインで mstsc コマンドを使って同じ操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-152">If you are on a Windows-based system, you can do this from the command line using the mstsc command:</span></span>

```powershell-interactive
mstsc /v:xx.xxx.xx.xxx
```

<span data-ttu-id="1b4f1-153">VM を作成したときと同じユーザー名/パスワードの組み合わせを指定してサインインしてください。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-153">Supply the same username/password combination you used when creating the VM to sign in.</span></span>

## <a name="create-a-linux-virtual-machine"></a><span data-ttu-id="1b4f1-154">Linux 仮想マシンを作成する</span><span class="sxs-lookup"><span data-stu-id="1b4f1-154">Create a Linux Virtual Machine</span></span>

<span data-ttu-id="1b4f1-155">新しい Linux VM を作成するには、その他の必要なリソースを最初に作成し、構成に割り当てる必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-155">To create a new Linux VM we must first create the other required resources and assign them to a configuration.</span></span> <span data-ttu-id="1b4f1-156">その構成を使って VM を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-156">Then we can use that configuration to create the VM.</span></span> <span data-ttu-id="1b4f1-157">ここでは、前述のリソース グループが既に作成済みであることを前提としています。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-157">This assumes that you have already created the resource group as previously shown.</span></span> <span data-ttu-id="1b4f1-158">また、`id_rsa.pub` という名前の SSH 公開キーがユーザー プロファイルの .ssh ディレクトリに必要です。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-158">Also, you will need to have an SSH public key named `id_rsa.pub` in the .ssh directory of your user profile.</span></span>

### <a name="create-the-required-network-resources"></a><span data-ttu-id="1b4f1-159">必要なネットワーク リソースの作成</span><span class="sxs-lookup"><span data-stu-id="1b4f1-159">Create the required network resources</span></span>

<span data-ttu-id="1b4f1-160">まず、仮想ネットワークの作成プロセスで使用するサブネット構成を作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-160">First we need to create a subnet configuration to be used with the virtual network creation process.</span></span> <span data-ttu-id="1b4f1-161">その VM に接続できるように、さらにパブリック IP アドレスも作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-161">We also create a public IP address so that we can connect to this VM.</span></span> <span data-ttu-id="1b4f1-162">そのパブリック アドレスへのアクセスについては、ネットワーク セキュリティ グループを作成してセキュリティを確保します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-162">We create a network security group to secure access to the public address.</span></span> <span data-ttu-id="1b4f1-163">最後に、前述のリソースをすべて使って仮想 NIC を作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-163">Finally we create the virtual NIC using all of the previous resources.</span></span>

```powershell-interactive
# Variables for common values
$resourceGroup = "myResourceGroup"
$location = "westeurope"
$vmName = "myLinuxVM"

# Definer user name and blank password
$securePassword = ConvertTo-SecureString ' ' -AsPlainText -Force
$cred = New-Object System.Management.Automation.PSCredential ("azureuser", $securePassword)

# Create a subnet configuration
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 192.168.2.0/24

# Create a virtual network
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName $resourceGroup -Location $location `
  -Name MYvNET2 -AddressPrefix 192.168.0.0/16 -Subnet $subnetConfig

# Create a public IP address and specify a DNS name
$publicIp = New-AzureRmPublicIpAddress -ResourceGroupName $resourceGroup -Location $location `
  -Name "mypublicdns$(Get-Random)" -AllocationMethod Static -IdleTimeoutInMinutes 4
$publicIp | Select-Object Name,IpAddress

# Create an inbound network security group rule for port 22
$nsgRuleSSH = New-AzureRmNetworkSecurityRuleConfig -Name myNetworkSecurityGroupRuleSSH  -Protocol Tcp `
  -Direction Inbound -Priority 1000 -SourceAddressPrefix * -SourcePortRange * -DestinationAddressPrefix * `
  -DestinationPortRange 22 -Access Allow

# Create a network security group
$nsg = New-AzureRmNetworkSecurityGroup -ResourceGroupName $resourceGroup -Location $location `
  -Name myNetworkSecurityGroup2 -SecurityRules $nsgRuleSSH

# Create a virtual network card and associate with public IP address and NSG
$nic = New-AzureRmNetworkInterface -Name myNic2 -ResourceGroupName $resourceGroup -Location $location `
  -SubnetId $vnet.Subnets[0].Id -PublicIpAddressId $publicIp.Id -NetworkSecurityGroupId $nsg.Id
```

### <a name="create-the-virtual-machine"></a><span data-ttu-id="1b4f1-164">仮想マシンの作成</span><span class="sxs-lookup"><span data-stu-id="1b4f1-164">Create the virtual machine</span></span>

<span data-ttu-id="1b4f1-165">これで必要なリソースが揃ったので、VM を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-165">Now that we have the required resources we can create the VM.</span></span> <span data-ttu-id="1b4f1-166">このステップでは、VM 構成オブジェクトを作成し、その構成を使って VM を作成します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-166">For this step, we create a VM configuration object, then we use the configuration to create the VM.</span></span>

```powershell-interactive
# Create a virtual machine configuration
$vmConfig = New-AzureRmVMConfig -VMName $vmName -VMSize Standard_D1 |
  Set-AzureRmVMOperatingSystem -Linux -ComputerName $vmName -Credential $cred -DisablePasswordAuthentication |
  Set-AzureRmVMSourceImage -PublisherName Canonical -Offer UbuntuServer -Skus 14.04.2-LTS -Version latest |
  Add-AzureRmVMNetworkInterface -Id $nic.Id

# Configure SSH Keys
$sshPublicKey = Get-Content "$env:USERPROFILE\.ssh\id_rsa.pub"
Add-AzureRmVMSshPublicKey -VM $vmConfig -KeyData $sshPublicKey -Path "/home/azureuser/.ssh/authorized_keys"

# Create a virtual machine
New-AzureRmVM -ResourceGroupName $resourceGroup -Location $location -VM $vmConfig
```

<span data-ttu-id="1b4f1-167">VM が作成されたら、その VM のパブリック IP アドレスを SSH で使用し、新しい Linux VM にログオンすることができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-167">Now that the VM has been created, you can log on to your new Linux VM using SSH with the public IP address of the VM you created:</span></span>

```bash
ssh xx.xxx.xxx.xxx
```

```Output
Welcome to Ubuntu 14.04.4 LTS (GNU/Linux 3.19.0-65-generic x86_64)

 * Documentation:  https://help.ubuntu.com/

  System information as of Sun Feb 19 00:32:28 UTC 2017

  System load: 0.31              Memory usage: 3%   Processes:       89
  Usage of /:  39.6% of 1.94GB   Swap usage:   0%   Users logged in: 0

  Graph this data and manage this system at:
    https://landscape.canonical.com/

  Get cloud support with Ubuntu Advantage Cloud Guest:
    http://www.ubuntu.com/business/services/cloud

0 packages can be updated.
0 updates are security updates.



The programs included with the Ubuntu system are free software;
the exact distribution terms for each program are described in the
individual files in /usr/share/doc/*/copyright.

Ubuntu comes with ABSOLUTELY NO WARRANTY, to the extent permitted by
applicable law.

my-login@MyLinuxVM:../../..$
```

## <a name="creating-other-resources-in-azure"></a><span data-ttu-id="1b4f1-168">その他の Azure リソースを作成する</span><span class="sxs-lookup"><span data-stu-id="1b4f1-168">Creating other resources in Azure</span></span>

<span data-ttu-id="1b4f1-169">ここまでは、リソース グループ、Linux VM、Windows Server VM の作成方法を見てきました。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-169">We've now walked through how to create a Resource Group, a Linux VM, and a Windows Server VM.</span></span> <span data-ttu-id="1b4f1-170">そのほかにも、さまざまな種類の Azure リソースを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-170">You can create many other types of Azure resources as well.</span></span>

<span data-ttu-id="1b4f1-171">たとえば、新しく作成した VM に関連付けるための Azure ネットワーク ロード バランサーを作成するには、次のコマンドを使います。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-171">For example, to create an Azure Network Load Balancer that we could then associate with our newly created VMs, we can use the following create command:</span></span>

```powershell-interactive
New-AzureRmLoadBalancer -Name MyLoadBalancer -ResourceGroupName myResourceGroup -Location westeurope
```

<span data-ttu-id="1b4f1-172">また、次のコマンドを使って、インフラストラクチャ用に新しいプライベート仮想ネットワーク (Azure では通常 "VNet" と呼ばれます) を作成することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-172">We could also create a new private Virtual Network (commonly referred to as a "VNet" within Azure) for our infrastructure using the following command:</span></span>

```powershell-interactive
$subnetConfig = New-AzureRmVirtualNetworkSubnetConfig -Name mySubnet2 -AddressPrefix 10.0.0.0/16
$vnet = New-AzureRmVirtualNetwork -ResourceGroupName myResourceGroup -Location westeurope `
  -Name MYvNET3 -AddressPrefix 10.0.0.0/16 -Subnet $subnetConfig
```

<span data-ttu-id="1b4f1-173">Azure と Azure PowerShell の優れている点は、それらを使ってクラウドベースのインフラストラクチャを実現できるだけでなく、管理対象となるプラットフォーム サービスを作成できることです。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-173">What makes Azure and the Azure PowerShell powerful is that we can use it not just to get cloud-based infrastructure but also to create managed platform services.</span></span> <span data-ttu-id="1b4f1-174">その管理されたプラットフォーム サービスにインフラストラクチャを組み合わせることで、さらに強力なソリューションを構築することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-174">The managed platform services can also be combined with infrastructure to build even more powerful solutions.</span></span>

<span data-ttu-id="1b4f1-175">たとえば Azure PowerShell を使って Azure AppService を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-175">For example, you can use the Azure PowerShell to create an Azure AppService.</span></span> <span data-ttu-id="1b4f1-176">Azure AppService は、管理されたプラットフォーム サービスであり、インフラストラクチャには一切気を遣わずに Web アプリをホストできるのが特徴です。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-176">Azure AppService is a managed platform service that provides a great way to host web apps without having to worry about infrastructure.</span></span> <span data-ttu-id="1b4f1-177">Azure AppService の作成後、次のコマンドを使って AppService 内に 2 つの新しい Azure Web アプリを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-177">After creating the Azure AppService, you can create two new Azure Web Apps within the AppService using the following commands:</span></span>

```powershell-interactive
# Create an Azure AppService that we can host any number of web apps within
New-AzureRmAppServicePlan -Name MyAppServicePlan -Tier Basic -NumberofWorkers 2 -WorkerSize Small -ResourceGroupName myResourceGroup -Location westeurope

# Create Two Web Apps within the AppService (note: name param must be a unique DNS entry)
New-AzureRmWebApp -Name MyWebApp43432 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
New-AzureRmWebApp -Name MyWebApp43433 -AppServicePlan MyAppServicePlan -ResourceGroupName myResourceGroup -Location westeurope
```

## <a name="listing-deployed-resources"></a><span data-ttu-id="1b4f1-178">デプロイされているリソースの一覧表示</span><span class="sxs-lookup"><span data-stu-id="1b4f1-178">Listing deployed resources</span></span>

<span data-ttu-id="1b4f1-179">Azure 内で実行されているリソースは、`Get-AzureRmResource` コマンドレットを使って一覧表示することができます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-179">You can use the `Get-AzureRmResource` cmdlet to list the resources running in Azure.</span></span> <span data-ttu-id="1b4f1-180">先ほど新しいリソース グループに作成したリソースを表示する例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-180">The following example shows the resources we just created in the new resource group.</span></span>

```powershell-interactive
Get-AzureRmResource |
  Where-Object ResourceGroupName -eq myResourceGroup |
    Select-Object Name,Location,ResourceType
```

```Output
Name                                                  Location   ResourceType
----                                                  --------   ------------
myLinuxVM_OsDisk_1_36ca038791f642ba91270879088c249a   westeurope Microsoft.Compute/disks
myWindowsVM_OsDisk_1_f627e6e2bb454c72897d72e9632adf9a westeurope Microsoft.Compute/disks
myLinuxVM                                             westeurope Microsoft.Compute/virtualMachines
myWindowsVM                                           westeurope Microsoft.Compute/virtualMachines
myWindowsVM/BGInfo                                    westeurope Microsoft.Compute/virtualMachines/extensions
myNic1                                                westeurope Microsoft.Network/networkInterfaces
myNic2                                                westeurope Microsoft.Network/networkInterfaces
myNetworkSecurityGroup1                               westeurope Microsoft.Network/networkSecurityGroups
myNetworkSecurityGroup2                               westeurope Microsoft.Network/networkSecurityGroups
mypublicdns245369171                                  westeurope Microsoft.Network/publicIPAddresses
mypublicdns779537141                                  westeurope Microsoft.Network/publicIPAddresses
MYvNET1                                               westeurope Microsoft.Network/virtualNetworks
MYvNET2                                               westeurope Microsoft.Network/virtualNetworks
micromyresomywi032907510                              westeurope Microsoft.Storage/storageAccounts
```

## <a name="deleting-resources"></a><span data-ttu-id="1b4f1-181">リソースの削除</span><span class="sxs-lookup"><span data-stu-id="1b4f1-181">Deleting resources</span></span>

<span data-ttu-id="1b4f1-182">Azure アカウントをクリーンアップするために、この例で作成したリソースを削除しましょう。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-182">To clean up your Azure account, you want to remove the resources we created in this example.</span></span> <span data-ttu-id="1b4f1-183">不要になったリソースは、`Remove-AzureRm*` コマンドレットを使って削除できます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-183">You can use the `Remove-AzureRm*` cmdlets to delete the resources you no longer need.</span></span> <span data-ttu-id="1b4f1-184">作成した Windows VM を削除するには、次のコマンドを使います。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-184">To remove the Windows VM we created, using the following command:</span></span>

```powershell-interactive
Remove-AzureRmVM -Name myWindowsVM -ResourceGroupName myResourceGroup
```

<span data-ttu-id="1b4f1-185">リソースを削除してよいか確認するメッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-185">You will be prompted to confirm that you want to remove the resource.</span></span>

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="1b4f1-186">多数のリソースを一度に削除することもできます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-186">You can also use the delete many resources at one time.</span></span> <span data-ttu-id="1b4f1-187">たとえば次のコマンドを実行すると、この概要チュートリアルのすべてのサンプルで使ってきたリソース グループ ("MyResourceGroup") が完全に削除されます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-187">For example, the following command deletes all the resource group "MyResourceGroup" that we've used for all the samples in this Get Started tutorial.</span></span> <span data-ttu-id="1b4f1-188">リソース グループだけでなく、そこに含まれるリソースもすべて削除されます。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-188">This removes the resource group and all of the resources in it.</span></span>

```powershell-interactive
Remove-AzureRmResourceGroup -Name myResourceGroup
```

```Output
Confirm
Are you sure you want to remove resource group 'myResourceGroup'
[Y] Yes  [N] No  [S] Suspend  [?] Help (default is "Y"): Y
```

<span data-ttu-id="1b4f1-189">このコマンドは、完了までに数分かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-189">This can take several minutes to complete.</span></span>

## <a name="get-samples"></a><span data-ttu-id="1b4f1-190">サンプルを入手する</span><span class="sxs-lookup"><span data-stu-id="1b4f1-190">Get samples</span></span>

<span data-ttu-id="1b4f1-191">Azure PowerShell の使用方法について詳しくは、[Linux VM](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[Windows VM](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json)、[SQL Database](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json) 用の一般的なスクリプトが用意されているので、そちらをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-191">To learn more about ways to use the Azure PowerShell, check out our most common scripts for [Linux VMs](/azure/virtual-machines/virtual-machines-linux-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Windows VMs](/azure/virtual-machines/virtual-machines-windows-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), [Web Apps](/azure/app-service-web/app-service-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json), and [SQL Databases](/azure/sql-database/sql-database-powershell-samples?toc=%2fpowershell%2fazure%%2ftoc.json).</span></span>

## <a name="next-steps"></a><span data-ttu-id="1b4f1-192">次の手順</span><span class="sxs-lookup"><span data-stu-id="1b4f1-192">Next steps</span></span>

* [<span data-ttu-id="1b4f1-193">Azure PowerShell を使用してサインインする</span><span class="sxs-lookup"><span data-stu-id="1b4f1-193">Sign in with Azure PowerShell</span></span>](authenticate-azureps.md)
* [<span data-ttu-id="1b4f1-194">Azure PowerShell による Azure サブスクリプションの管理</span><span class="sxs-lookup"><span data-stu-id="1b4f1-194">Manage Azure subscriptions with Azure PowerShell</span></span>](manage-subscriptions-azureps.md)
* [<span data-ttu-id="1b4f1-195">Azure PowerShell を使って Azure にサービス プリンシパルを作成する</span><span class="sxs-lookup"><span data-stu-id="1b4f1-195">Create service principals in Azure using Azure PowerShell</span></span>](create-azure-service-principal-azureps.md)
* <span data-ttu-id="1b4f1-196">以前のリリースからの移行については、リリース ノート ([ https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes)) を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b4f1-196">Read the Release notes about migrating from an older release: [https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes](https://github.com/Azure/azure-powershell/tree/dev/documentation/release-notes).</span></span>
* <span data-ttu-id="1b4f1-197">コミュニティに質問する:</span><span class="sxs-lookup"><span data-stu-id="1b4f1-197">Get help from the community:</span></span>
  * [<span data-ttu-id="1b4f1-198">MSDN の Azure フォーラム</span><span class="sxs-lookup"><span data-stu-id="1b4f1-198">Azure forum on MSDN</span></span>](http://go.microsoft.com/fwlink/p/?LinkId=320212)
  * [<span data-ttu-id="1b4f1-199">stackoverflow</span><span class="sxs-lookup"><span data-stu-id="1b4f1-199">stackoverflow</span></span>](http://go.microsoft.com/fwlink/?LinkId=320213)
