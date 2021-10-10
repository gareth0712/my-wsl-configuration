# Config file (.wslconfig) for WSL

- This file is to configure the WSL settings. The changes will take effect upon user restart the wsl
- The config file consists of different sections named with the format `[section-label]` and respective key-value pair for the configuration under that section

## Restart wsl to make changes take effect

- There are too many ways of doing this and most of them are very difficult to memorize. I picked the easiest one so that we can do it without referring here again and again.
- Restart the wsl by running the following in PowerShell  
1. Run the following to show available distro
```
$ wsl -l -v
  NAME                   STATE           VERSION
* docker-desktop-data    Running         2
  docker-desktop         Running         2
  Ubuntu-20.04           Running         2
```
2. Run `wsl -t <distroName>` to kill the distro you wanna restart or `wsl --shutdown` to kill all running distro
3. Restart the distro by running the command u start it
```
$ ubuntu
```
4. The changes you made on wslconfig should take place

## Section label: [wsl2]

- Click [here](https://docs.microsoft.com/en-us/windows/wsl/wsl-config) for Reference
- We should save the file in Windows user directory, e.g. for "Benson2021", the file should be saved in "C:\users\benson2021\.wslconfig"
- Example of a wslconfig file
```
[wsl2]
memory=6GB
swap=0
localhostForwarding=true
```

- memory: How much memory to assign to the WSL 2 VM
- localhostForwarding: Boolean specifying if ports bound to wildcard or localhost in the WSL 2 VM should be connectable from the host via localhost:port.
- swap: How much swap space to add to the WSL 2 VM, 0 for no swap file.


## Section label: [user]

- These options are available in Build 18980 and later.
- example
```
[user]
default=benson2021
```
- default: specifies which user to run as when first starting a WSL session. default is the initial username created on first run
