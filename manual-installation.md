# Manual Installation

## Install WSL (e.g. ubuntu) on drive other than C drive
- Click [here](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package) for reference of getting your Windows ready to install WSL
- Click [here](https://docs.microsoft.com/en-us/windows/wsl/install-on-server) for reference of manual installation of WSL system
- This guide is to prevent loss of WSL configuration upon resetting your Windows
- steps for the installation (Assuming you have followed the first reference link for configuring the system ready for running wsl):
  - Download respective Linux distribution for WSL from the [Microsoft guide](https://docs.microsoft.com/en-us/windows/wsl/install-manual#step-4---download-the-linux-kernel-update-package)
  - Move the file (e.g. Ubuntu_2004.2020.424.0_x64.appx) to the location you preferred (e.g. D:/wsl/ubuntu/)
  - Open PowerShell for installation
  - Run `Rename-Item .\Ubuntu_2004.2020.424.0_x64.appx .\Ubuntu.zip`
  - Run `Expand-Archive .\Ubuntu.zip .\Ubuntu` to extract the file
  - `cd Ubuntu` and then `./ubuntu2004.exe` to start the init processes
  - The distribution shall ask for your username and password
- After the set up, you are ready to run Linux on Windows!
