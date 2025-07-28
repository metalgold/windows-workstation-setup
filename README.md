# How to setup a Windows Workstation with WSL (Windows Subsystem for Linux)

Install all required tools:

```
winget install Microsoft.WSL Git.Git KeePassXCTeam.KeePassXC Microsoft.VisualStudioCode WireGuard.Wireguard Mozilla.Thunderbird.de Mattermost.MattermostDesktop Zoom.Zoom suse.RancherDesktop LibreHardwareMonitor.LibreHardwareMonitor JetBrains.Toolbox OpenWhisperSystems.Signal
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

Install aws-cli:
