---
title: "Azure CLI 2.0 설치"
description: "Azure CLI 2.0 설치에 대한 참조 문서입니다."
keywords: "Azure CLI, Azure CLI 설치, Azure Python CLI, Azure CLI 참조"
author: sptramer
ms.author: sttramer
manager: routlaw
ms.date: 08/17/2017
ms.topic: article
ms.prod: azure
ms.technology: azure
ms.devlang: azurecli
ms.service: multiple
ms.assetid: ea5c0ee1-c530-4a1e-a83f-e1be71f6d416
ms.openlocfilehash: 935814d56d0a6be00f626da860dc643adbf14804
ms.sourcegitcommit: 9f38efbb7efd800ee5cab80d6641770d268c5a68
ms.translationtype: HT
ms.contentlocale: ko-KR
ms.lasthandoff: 09/22/2017
---
# <a name="install-azure-cli-20"></a><span data-ttu-id="70614-104">Azure CLI 2.0 설치</span><span class="sxs-lookup"><span data-stu-id="70614-104">Install Azure CLI 2.0</span></span>

<span data-ttu-id="70614-105">지금 새 버전의 Azure CLI를 설치하세요.</span><span class="sxs-lookup"><span data-stu-id="70614-105">Install the new version of the Azure CLI today!</span></span>
<span data-ttu-id="70614-106">Azure 리소스 관리를 위한 훌륭한 기본 명령줄 환경을 제공하도록 개선되고 업데이트되었습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-106">We've improved and updated it to provide a great native command-line experience for managing Azure resources.</span></span>
<span data-ttu-id="70614-107">macOS, Linux 및 Windows에서 사용할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-107">It can be used on macOS, Linux, and Windows.</span></span>
<span data-ttu-id="70614-108">최신 릴리스에 대한 자세한 내용은 [릴리스 정보](release-notes-azure-cli.md)를 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="70614-108">For information about the latest release, see the [release notes](release-notes-azure-cli.md).</span></span>

> [!NOTE]
> <span data-ttu-id="70614-109">이전 버전의 Azure CLI가 필요한 경우 [Azure CLI 1.0 설치](/azure/cli-install-nodejs) 방법을 참조하세요.</span><span class="sxs-lookup"><span data-stu-id="70614-109">If you need the previous version of the Azure CLI, here's how to [install Azure CLI 1.0](/azure/cli-install-nodejs).</span></span>

## <a name="a-namemacosinstall-on-macos"></a><span data-ttu-id="70614-110"><a name="macOS"/>macOS에 설치</span><span class="sxs-lookup"><span data-stu-id="70614-110"><a name="macOS"/>Install on macOS</span></span>

<span data-ttu-id="70614-111">macOS에서는 [Homebrew](https://brew.sh/) 또는 수동으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-111">On macOS, you are able to install either with [Homebrew](https://brew.sh/) or manually.</span></span>

### <a name="install-with-homebrew"></a><span data-ttu-id="70614-112">Homebrew로 설치</span><span class="sxs-lookup"><span data-stu-id="70614-112">Install with Homebrew</span></span>

1. <span data-ttu-id="70614-113">아직 설치하지 않은 경우 [Homebrew 설치 지침](https://docs.brew.sh/Installation.html)에 따라 Homebrew를 설치하십시오.</span><span class="sxs-lookup"><span data-stu-id="70614-113">If you don't have it already, install Homebrew by following the [Homebrew installation instructions](https://docs.brew.sh/Installation.html).</span></span>

2. <span data-ttu-id="70614-114">이전에 CLI를 수동으로 설치한 경우 [수동 제거](#UninstallManually) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="70614-114">If you have previously installed the CLI manually, follow the [manual uninstall](#UninstallManually) instructions.</span></span>

3. <span data-ttu-id="70614-115">로컬 Homebrew 리포지토리를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-115">Update your local Homebrew repositories.</span></span>

   ```bash
   brew update
   ```

4. <span data-ttu-id="70614-116">`azure-cli` 패키지를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-116">Install the `azure-cli` package.</span></span>

  ```bash
  brew install azure-cli
  ```

> [!NOTE]
> <span data-ttu-id="70614-117">이전에 Azure CLI 1.0을 Homebrew로 설치한 경우 패키지를 설치하는 대신 일반 Homebrew 업데이트 프로세스를 통해 CLI 2.0을 확보할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-117">If you previously installed the Azure CLI 1.0 with Homebrew, instead of installing the package you can get CLI 2.0 through the regular Homebrew upgrade process.</span></span>
>
> ```bash
> brew upgrade
> ```

### <a name="install-manually"></a><span data-ttu-id="70614-118">수동 설치</span><span class="sxs-lookup"><span data-stu-id="70614-118">Install manually</span></span>

1. <span data-ttu-id="70614-119">`curl`을 사용하여 Azure CLI 2.0을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-119">Install Azure CLI 2.0 with `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

2. <span data-ttu-id="70614-120">일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-120">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```
   
3. <span data-ttu-id="70614-121">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-121">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-windows"></a><span data-ttu-id="70614-122">Windows에 설치</span><span class="sxs-lookup"><span data-stu-id="70614-122">Install on Windows</span></span>

### <a name="install-with-msi-for-the-windows-command-line"></a><span data-ttu-id="70614-123">Windows 명령줄용 MSI를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="70614-123">Install with MSI for the Windows command-line</span></span> 

<span data-ttu-id="70614-124">Windows에 CLI를 설치하고 Windows 명령줄에서 사용하려면 [Azure CLI 설치 관리자(MSI)](https://aka.ms/InstallAzureCliWindows)를 다운로드하여 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-124">To install the CLI on Windows and use it in the Windows command-line, download and run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows).</span></span>

### <a name="install-with-apt-get-for-bash-on-ubuntu-on-windows"></a><span data-ttu-id="70614-125">Windows의 Ubuntu에 있는 Bash용 apt-get을 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="70614-125">Install with apt-get for Bash on Ubuntu on Windows</span></span>

1. <span data-ttu-id="70614-126">Windows에 Bash가 없을 경우 [설치](https://msdn.microsoft.com/commandline/wsl/install_guide)합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-126">If you don't have Bash on Windows, [install it](https://msdn.microsoft.com/commandline/wsl/install_guide).</span></span>

2. <span data-ttu-id="70614-127">Bash 셸을 엽니다.</span><span class="sxs-lookup"><span data-stu-id="70614-127">Open the Bash shell.</span></span>

3. <span data-ttu-id="70614-128">소스 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-128">Modify your sources list.</span></span>

   ```bash
   echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
        sudo tee /etc/apt/sources.list.d/azure-cli.list
   ```

4. <span data-ttu-id="70614-129">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-129">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

5.  <span data-ttu-id="70614-130">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-130">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-debianubuntu-with-apt-get"></a><span data-ttu-id="70614-131">apt-get을 사용하여 Debian/Ubuntu에 설치</span><span class="sxs-lookup"><span data-stu-id="70614-131">Install on Debian/Ubuntu with apt-get</span></span>

<span data-ttu-id="70614-132">Debian/Ubuntu 기반 시스템의 경우 `apt-get`를 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-132">For Debian/Ubuntu based systems, you can install Azure CLI 2.0 via `apt-get`.</span></span>

1. <span data-ttu-id="70614-133">원본 목록을 수정합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-133">Modify your sources list:</span></span>
 
   - <span data-ttu-id="70614-134">32비트 시스템</span><span class="sxs-lookup"><span data-stu-id="70614-134">32-bit system</span></span>

     ```bash
     echo "deb https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

   - <span data-ttu-id="70614-135">64비트 시스템</span><span class="sxs-lookup"><span data-stu-id="70614-135">64-bit system</span></span>

     ```bash
     echo "deb [arch=amd64] https://packages.microsoft.com/repos/azure-cli/ wheezy main" | \
          sudo tee /etc/apt/sources.list.d/azure-cli.list
     ```

2. <span data-ttu-id="70614-136">다음과 같은 sudo 명령을 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-136">Run the following sudo commands:</span></span>

   ```bash
   sudo apt-key adv --keyserver packages.microsoft.com --recv-keys 417A0893
   sudo apt-get install apt-transport-https
   sudo apt-get update && sudo apt-get install azure-cli
   ```

3.  <span data-ttu-id="70614-137">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-137">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-rhel-fedora-and-centos-with-yum"></a><span data-ttu-id="70614-138">Yum을 사용하여 RHEL, Fedora 및 CentOS에 설치</span><span class="sxs-lookup"><span data-stu-id="70614-138">Install on RHEL, Fedora, and CentOS with yum</span></span>

<span data-ttu-id="70614-139">RedHat에서 기반으로 하지 않고 `yum` 패키지 관리자를 포함하는 배포판의 경우 `yum`을 통해 Azure CLI 2.0을 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-139">For any distribution which is based off of RedHat and contains the `yum` package manager, you can install Azure CLI 2.0 via `yum`.</span></span>

1. <span data-ttu-id="70614-140">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="70614-140">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="70614-141">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="70614-141">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/yum.repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="70614-142">`yum` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-142">Update the `yum` package index and install:</span></span>

   ```bash
   yum check-update
   sudo yum install azure-cli
   ```

4. <span data-ttu-id="70614-143">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-143">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-on-opensuse-and-sle-with-zypper"></a><span data-ttu-id="70614-144">Zypper를 사용하여 openSUSE 및 SLE에 설치</span><span class="sxs-lookup"><span data-stu-id="70614-144">Install on openSUSE and SLE with zypper</span></span>

1. <span data-ttu-id="70614-145">Microsoft 리포지토리 키를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="70614-145">Import the Microsoft repository key:</span></span>

   ```bash
   sudo rpm --import https://packages.microsoft.com/keys/microsoft.asc
   ```

2. <span data-ttu-id="70614-146">로컬 `azure-cli` 리포지토리 정보를 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="70614-146">Create local `azure-cli` repository information:</span></span>

   ```bash
   sudo sh -c 'echo -e "[azure-cli]\nname=Azure CLI\nbaseurl=https://packages.microsoft.com/yumrepos/azure-cli\nenabled=1\ntype=rpm-md\ngpgcheck=1\ngpgkey=https://packages.microsoft.com/keys/microsoft.asc" > /etc/zypp/repos.d/azure-cli.repo'
   ```

3. <span data-ttu-id="70614-147">`zypper` 패키지 인덱스를 업데이트하고 다음을 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-147">Update the `zypper` package index and install:</span></span>

   ```bash
   sudo zypper refresh
   sudo zypper install azure-cli
   ```

4. <span data-ttu-id="70614-148">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-148">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="install-with-docker"></a><span data-ttu-id="70614-149">Docker를 사용하여 설치</span><span class="sxs-lookup"><span data-stu-id="70614-149">Install with Docker</span></span>

<span data-ttu-id="70614-150">Azure CLI 2.0으로 미리 구성된 Docker 이미지를 유지하고 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-150">We maintain a Docker image preconfigured with the Azure CLI 2.0.</span></span>

<span data-ttu-id="70614-151">`docker run`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-151">Install the CLI using `docker run`.</span></span>

   ```bash
   docker run azuresdk/azure-cli-python:<version>
   ```

<span data-ttu-id="70614-152">[Docker 태그](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/)를 통해 사용 가능한 버전을 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-152">See our [Docker tags](https://hub.docker.com/r/azuresdk/azure-cli-python/tags/) for available versions.</span></span>

<span data-ttu-id="70614-153">CLI는 `/usr/local/bin`에 있는 `az` 명령으로 이미지에 설치됩니다.</span><span class="sxs-lookup"><span data-stu-id="70614-153">The CLI is installed on the image as the `az` command in `/usr/local/bin`.</span></span>

> [!NOTE]
> <span data-ttu-id="70614-154">사용자 환경에서 SSH 키를 선택하려는 경우 `-v ${HOME}:/root`를 사용하여 $HOME을 `/root`로 탑재할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-154">If you want to pick up the SSH keys from your user environment, you can use `-v ${HOME}:/root` to mount $HOME as `/root`.</span></span>

> ```bash
> docker run -v ${HOME}:/root azuresdk/azure-cli-python:<version>
> ```

## <a name="a-namelinuxinstall-on-linux-without-apt-get"></a><span data-ttu-id="70614-155"><a name="Linux"/>apt-get을 사용하지 않고 Linux에 설치</span><span class="sxs-lookup"><span data-stu-id="70614-155"><a name="Linux"/>Install on Linux without apt-get</span></span>

<span data-ttu-id="70614-156">가능한 경우 패키지 관리자를 사용하여 CLI를 설치하는 것이 좋습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-156">It is recommended that you install the CLI with a package manager if you are able to.</span></span> <span data-ttu-id="70614-157">이에 제공되는 패키지가 없는 배포판의 경우 수동으로 설치할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-157">For distributions which do not have a package provided for them, you can manually install.</span></span>

1. <span data-ttu-id="70614-158">Linux 배포판에 따라 필수 구성 요소를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-158">Install the prerequisites based on your Linux distribution.</span></span>

   ```
   Platform              | Prerequisites
   ----------------------|---------------------------------------------
   Ubuntu 15.10 or 16.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Ubuntu 12.04 or 14.04 | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   Debian 8              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev build-essential
   Debian 7              | sudo apt-get update && sudo apt-get install -y python libssl-dev libffi-dev python-dev
   CentOS 7.1 or 7.2     | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   RedHat 7.2            | sudo yum check-update; sudo yum install -y gcc python libffi-devel python-devel openssl-devel
   SUSE OpenSUSE 13.2    | sudo zypper refresh && sudo zypper --non-interactive install curl gcc python python-xml libffi-devel python-devel openssl-devel
   ```

<span data-ttu-id="70614-159">위에서 배포판이 나열되지 않으면 [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/) 및 [OpenSSL](https://www.openssl.org/source/)을 설치해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-159">If your distribution is not listed above, you will need to install [Python](https://www.python.org/downloads/), [libffi](https://sourceware.org/libffi/), and [OpenSSL](https://www.openssl.org/source/).</span></span>

2. <span data-ttu-id="70614-160">`curl`을 사용하여 CLI를 설치합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-160">Install the CLI with  `curl`.</span></span>

   ```bash
   curl -L https://aka.ms/InstallAzureCli | bash
   ```

3. <span data-ttu-id="70614-161">일부 변경 내용을 적용하려면 셸을 다시 시작해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-161">You may have to restart your shell for some changes to take effect.</span></span>

   ```bash
   exec -l $SHELL
   ```

4. <span data-ttu-id="70614-162">명령 프롬프트에서 `az` 명령으로 CLI를 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-162">Run the CLI from the command prompt with the `az` command.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="70614-163">문제 해결</span><span class="sxs-lookup"><span data-stu-id="70614-163">Troubleshooting</span></span>

<span data-ttu-id="70614-164">CLI 설치 중에 문제가 발생하면 이 섹션을 확인하여 해당 사례가 적용되는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-164">If you encounter an issue during CLI install, check this section to see if your particular case is covered.</span></span> <span data-ttu-id="70614-165">해당 문제가 여기에 없으면 [Github에 문제를 제출하세요](https://github.com/Azure/azure-cli/issues).</span><span class="sxs-lookup"><span data-stu-id="70614-165">If your issue is not here, please [file a Github issue](https://github.com/Azure/azure-cli/issues).</span></span>

### <a name="curl-object-moved-error"></a><span data-ttu-id="70614-166">"개체 이동됨" curl 오류</span><span class="sxs-lookup"><span data-stu-id="70614-166">curl "Object Moved" error</span></span>

<span data-ttu-id="70614-167">`-L` 매개 변수와 관련된 `curl`에서 오류가 발생하거나 "개체 이동됨"이라는 텍스트가 포함된 오류 메시지가 표시되면 `aka.ms` 리디렉션 전체 URL을 사용해 보세요.</span><span class="sxs-lookup"><span data-stu-id="70614-167">If you get an error from `curl` related to the `-L` parameter, or an error message including the text "Object Moved", try using the full URL instead of the `aka.ms` redirect:</span></span>

```bash
curl https://azurecliprod.blob.core.windows.net/install | bash
```

### <a name="az-command-not-found"></a><span data-ttu-id="70614-168">`az` 명령을 찾을 수 없음</span><span class="sxs-lookup"><span data-stu-id="70614-168">`az` command not found</span></span>

<span data-ttu-id="70614-169">셸의 명령 해시 캐시를 지워야 할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-169">You may need to clear your shell's command hash cache.</span></span> <span data-ttu-id="70614-170">실행</span><span class="sxs-lookup"><span data-stu-id="70614-170">Run</span></span>

```bash
hash -r
```

<span data-ttu-id="70614-171">한 다음 문제가 해결되었는지 확인합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-171">and see if the problem is resolved.</span></span>

## <a name="uninstall-cli-1x-versions"></a><span data-ttu-id="70614-172">CLI 1.x 버전 제거</span><span class="sxs-lookup"><span data-stu-id="70614-172">Uninstall CLI 1.x versions</span></span>

<span data-ttu-id="70614-173">시스템에서 이전의 CLI 1.x 버전을 사용할 수 있는 경우 사용된 설치 유형에 따라 이를 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-173">If you have an earlier CLI 1.x version available on your system, you can uninstall it based upon the type of install used.</span></span>

### <a name="uninstall-with-npm"></a><span data-ttu-id="70614-174">npm을 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="70614-174">Uninstall with npm</span></span>

<span data-ttu-id="70614-175">`npm uninstall`을 사용하여 이전 버전의 CLI를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-175">Remove the older CLI with `npm uninstall`.</span></span>

  ```bash
  npm uninstall -g azure-cli
  ```

### <a name="uninstall-with-distributable"></a><span data-ttu-id="70614-176">배포 패키지를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="70614-176">Uninstall with distributable</span></span>

<span data-ttu-id="70614-177">[Azure CLI 설치 관리자(MSI)](http://aka.ms/webpi-azure-cli) 또는 [macOS 패키지](http://aka.ms/mac-azure-cli)를 통해 설치한 경우 동일한 도구를 사용하여 설치를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-177">If you installed via the [Azure CLI Installer (MSI)](http://aka.ms/webpi-azure-cli) or a [macOS package](http://aka.ms/mac-azure-cli), use the same tool to remove your install.</span></span>

### <a name="uninstall-with-docker"></a><span data-ttu-id="70614-178">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="70614-178">Uninstall with Docker</span></span>

<span data-ttu-id="70614-179">Docker 이미지를 설치하여 이전 버전의 CLI를 사용한 경우 해당 이미지 및 관련 컨테이너를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-179">If you installed a Docker image to use the earlier CLI version, remove that image and any associated containers.</span></span> <span data-ttu-id="70614-180">그런 다음 설치 지침에서 설명하는 대로 새 Docker 이미지를 설치한 후 컨테이너를 다시 만들 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-180">You can then re-create the containers after installing the new Docker image as described in the install instructions.</span></span>

  ```bash
  docker rmi -f microsoft/azure-cli
  ```

## <a name="update-the-cli"></a><span data-ttu-id="70614-181">CLI 업데이트</span><span class="sxs-lookup"><span data-stu-id="70614-181">Update the CLI</span></span>

<span data-ttu-id="70614-182">Azure CLI를 업데이트하려면 설치하는 데 사용된 동일한 방법을 사용합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-182">To update the Azure CLI, use the same method that you used to install it.</span></span>

### <a name="update-with-homebrew"></a><span data-ttu-id="70614-183">Homebrew로 업데이트</span><span class="sxs-lookup"><span data-stu-id="70614-183">Update with Homebrew</span></span>

1. <span data-ttu-id="70614-184">이전에 수동으로 설치한 경우 [Homebrew로 설치](#macOS) 지침을 따르세요.</span><span class="sxs-lookup"><span data-stu-id="70614-184">If you previously installed manually, follow the [install with Homebrew](#macOS) instructions.</span></span>

2. <span data-ttu-id="70614-185">로컬 Homebrew 리포지토리 정보를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-185">Update your local Homebrew repository information.</span></span>

   ```bash
   brew update
   ```

3. <span data-ttu-id="70614-186">설치된 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-186">Upgrade your installed packages.</span></span>

   ```bash
   brew upgrade
   ```

### <a name="update-with-msi"></a><span data-ttu-id="70614-187">MSI를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="70614-187">Update with MSI</span></span>

<span data-ttu-id="70614-188">[Azure CLI 설치 관리자(MSI)](https://aka.ms/InstallAzureCliWindows)를 다시 실행합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-188">Run the [Azure CLI Installer (MSI)](https://aka.ms/InstallAzureCliWindows) again.</span></span>

### <a name="update-with-apt-get"></a><span data-ttu-id="70614-189">apt-get을 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="70614-189">Update with apt-get</span></span>

<span data-ttu-id="70614-190">`apt-get upgrade`를 사용하여 CLI 패키지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-190">Use `apt-get upgrade` to update the CLI package.</span></span>

   ```bash
   sudo apt-get update && sudo apt-get upgrade
   ```

> [!NOTE]
> <span data-ttu-id="70614-191">이렇게 하면 시스템에 설치되었지만 종속성이 변경되지 않은 모든 패키지를 업그레이드합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-191">This will upgrade all of the installed packages on your system which have not had a dependency change.</span></span>
> <span data-ttu-id="70614-192">CLI만 업그레이드하려면 `apt-get install`을 사용하세요.</span><span class="sxs-lookup"><span data-stu-id="70614-192">To upgrade only the CLI, use `apt-get install`.</span></span>
> ```bash
> sudo apt-get update && sudo apt-get install --only-upgrade -y azure-cli
> ```

### <a name="update-with-docker"></a><span data-ttu-id="70614-193">Docker를 사용하여 업데이트</span><span class="sxs-lookup"><span data-stu-id="70614-193">Update with Docker</span></span>

1. <span data-ttu-id="70614-194">`docker pull`을 사용하여 로컬 이미지를 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-194">Update your local image with `docker pull`.</span></span>

   ```bash
   docker pull azuresdk/azure-cli-python
   ```

2. <span data-ttu-id="70614-195">현재 CLI 이미지를 사용 중인 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="70614-195">Get the containers currently using the CLI image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

> [!NOTE]
> <span data-ttu-id="70614-196">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-196">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

3. <span data-ttu-id="70614-197">컨테이너를 중지하고 다시 만듭니다.</span><span class="sxs-lookup"><span data-stu-id="70614-197">Halt and recreate the containers.</span></span>

   ```bash
   docker stop inspiring_benz
   docker rm inspiring_benz
   docker run azuresdk/azure-cli-python
   ```

### <a name="update-manually"></a><span data-ttu-id="70614-198">수동으로 업데이트</span><span class="sxs-lookup"><span data-stu-id="70614-198">Update manually</span></span>

<span data-ttu-id="70614-199">[macOS](#macOS) 또는 [Linux](#Linux)에 대한 수동 설치 지침에 따라 업데이트합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-199">Follow the manual installation instructions for [macOS](#macOS) or [Linux](#Linux) to update.</span></span>

## <a name="uninstall"></a><span data-ttu-id="70614-200">제거</span><span class="sxs-lookup"><span data-stu-id="70614-200">Uninstall</span></span>

<span data-ttu-id="70614-201">CLI를 제거하려는 경우 유감스럽게 생각합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-201">If you decide to uninstall the CLI, we're sorry to see you go.</span></span> <span data-ttu-id="70614-202">CLI를 설치하는 데 사용한 동일한 방법을 사용하여 제거해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-202">You should uninstall using the same method that you used to install the CLI.</span></span>

### <a name="uninstall-with-homebrew"></a><span data-ttu-id="70614-203">Homebrew로 제거</span><span class="sxs-lookup"><span data-stu-id="70614-203">Uninstall with Homebrew</span></span>

<span data-ttu-id="70614-204">`azure-cli` 패키지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-204">Uninstall the `azure-cli` package.</span></span>

   ```bash
   brew uninstall azure-cli
   ```

### <a name="uninstall-with-msi"></a><span data-ttu-id="70614-205">MSI를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="70614-205">Uninstall with MSI</span></span>

<span data-ttu-id="70614-206">[MSI](https://aka.ms/InstallAzureCliWindows)를 다시 실행하고 제거를 선택합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-206">Run the [MSI](https://aka.ms/InstallAzureCliWindows) again and choose uninstall.</span></span>

### <a name="uninstall-with-apt-get"></a><span data-ttu-id="70614-207">apt-get을 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="70614-207">Uninstall with apt-get</span></span>

<span data-ttu-id="70614-208">`apt-get remove`를 통해 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-208">Uninstall via `apt-get remove`:</span></span>

  ```bash
  sudo apt-get remove -y azure-cli
  ```

### <a name="uninstall-with-docker"></a><span data-ttu-id="70614-209">Docker를 사용하여 제거</span><span class="sxs-lookup"><span data-stu-id="70614-209">Uninstall with Docker</span></span>

<span data-ttu-id="70614-210">Docker 이미지를 설치한 경우 이를 실행하는 컨테이너를 모두 제거한 다음 로컬 이미지를 삭제해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-210">If you installed a docker image, you will need to remove any containers running it, and then delete the local image.</span></span>

1. <span data-ttu-id="70614-211">azure-cli 이미지를 실행하는 컨테이너를 가져옵니다.</span><span class="sxs-lookup"><span data-stu-id="70614-211">Get the containers which are running the azure-cli image.</span></span>

   ```bash
   docker container ls -a --filter 'ancestor=azuresdk/azure-cli-python'
   ```

   ```output
   CONTAINER ID        IMAGE                              COMMAND             CREATED             STATUS                        PORTS               NAMES
   34a868beb2ab        azuresdk/azure-cli-python:latest      "/bin/sh -c bash"   8 minutes ago       Exited (0) 8 minutes ago                       inspiring_benz
   ```

2. <span data-ttu-id="70614-212">CLI 이미지가 있는 컨테이너를 모두 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-212">Delete any containers with the CLI image.</span></span>

   ```bash
   docker rm 34a868beb2ab
   ```

3. <span data-ttu-id="70614-213">로컬로 설치된 CLI 이미지를 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-213">Remove the locally installed CLI image.</span></span>

   ```bash
   docker rmi azuresdk/azure-cli-python
   ```

> [!NOTE]
> <span data-ttu-id="70614-214">특정 버전의 이미지를 설치한 경우 이미지 이름 끝에 `:<version>`을 추가해야 합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-214">If you installed a specific version of the image, you will need to add `:<version>` to the end of the image name.</span></span>

###<a name="a-nameuninstallmanuallyuninstall-manually"></a><span data-ttu-id="70614-215"><a name="UninstallManually"/>수동으로 제거</span><span class="sxs-lookup"><span data-stu-id="70614-215"><a name="UninstallManually"/>Uninstall manually</span></span>

<span data-ttu-id="70614-216">https://aka.ms/InstallAzureCli의 스크립트를 사용하여 CLI를 설치한 경우 이러한 단계를 따라 제거할 수 있습니다.</span><span class="sxs-lookup"><span data-stu-id="70614-216">If you used the script at https://aka.ms/InstallAzureCli to install the CLI, you can uninstall it with these steps.</span></span>

1. <span data-ttu-id="70614-217">설치된 파일을 제거합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-217">Remove the installed files.</span></span>

   ```bash
   rm -r <install location>/lib/azure-cli
   rm <install location>/bin/az
   ```

2. <span data-ttu-id="70614-218">`<install location>/.bash_profile`에서 `<install location>/lib/azure-cli/az.completion` 줄을 삭제합니다.</span><span class="sxs-lookup"><span data-stu-id="70614-218">Delete the line `<install location>/lib/azure-cli/az.completion` from `<install location>/.bash_profile`.</span></span>

> [!Note]
> <span data-ttu-id="70614-219">기본 설치 위치는 `/Users/<username>`입니다.</span><span class="sxs-lookup"><span data-stu-id="70614-219">The default install location is `/Users/<username>`.</span></span>

## <a name="report-cli-issues-and-feedback"></a><span data-ttu-id="70614-220">CLI 문제 보고 및 피드백</span><span class="sxs-lookup"><span data-stu-id="70614-220">Report CLI issues and feedback</span></span>

<span data-ttu-id="70614-221">도구에서 버그가 발생하면 GitHub 리포지토리의 [Issues](https://github.com/Azure/azure-cli/issues) 섹션에서 문제를 제출해 주세요.</span><span class="sxs-lookup"><span data-stu-id="70614-221">If you encounter any bugs with the tool, file an issue in the [Issues](https://github.com/Azure/azure-cli/issues) section of our GitHub repository.</span></span>
<span data-ttu-id="70614-222">명령줄에서 피드백을 제공하려면 `az feedback` 명령을 사용해 주세요.</span><span class="sxs-lookup"><span data-stu-id="70614-222">To provide feedback from the command line, use the `az feedback` command.</span></span>