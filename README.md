# How to setup a Windows Workstation with WSL (Windows Subsystem for Linux)

Install chocolatey package manager:

```
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))
```

Enable auto-confirmation:

```
choco feature enable -n=allowGlobalConfirmation
```

Install all required tools:

```
choco install keepassxc git vscode openvpn jetbrainstoolbox thunderbird mattermost-desktop slack zoom libre-hardware-monitor rancher-desktop
```

Install Ubuntu dependencies:

```
sudo apt update && sudo apt upgrade -y
sudo apt install zip unzip git pass
```

Install sdkman:

```
curl -s "https://get.sdkman.io" | bash
```

Install nvm:

```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

Install Ubuntu cypress dependencies:

```
sudo apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libnss3 libxss1 libasound2 libxtst6 xauth xvfb
```
