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
choco install keepassxc git vscode wireguard thunderbird mattermost-desktop zoom libre-hardware-monitor rancher-desktop
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

Install aws-cli:

```
sudo snap install aws-cli --classic
```

Install granted:

```
sudo apt update && sudo apt install gpg
wget -O- https://apt.releases.commonfate.io/gpg | sudo gpg --dearmor -o /usr/share/keyrings/common-fate-linux.gpg
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/common-fate-linux.gpg] https://apt.releases.commonfate.io stable main" | sudo tee /etc/apt/sources.list.d/common-fate.list
sudo apt update
sudo apt install granted
```

Install nvm:

```
wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.7/install.sh | bash
```

Install Ubuntu cypress dependencies:

```
sudo apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libnss3 libxss1 libasound2 libxtst6 xauth xvfb
```
