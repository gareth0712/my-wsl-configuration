# Install NVM on WSL

Reference: click [here](https://github.com/nvm-sh/nvm#install--update-script)  for the very detailed guide over usage of nvm from nvm-sh

## Instllation steps
1. `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash`
2. `export NVM_DIR="$([ -z "${XDG_CONFIG_HOME-}" ] && printf %s "${HOME}/.nvm" || printf %s "${XDG_CONFIG_HOME}/nvm")"[ -s "$NVM_DIR/nvm.sh" ] && \. "$NVM_DIR/nvm.sh" # This loads nvm`
3. Run the following to pick up the nvm command:
```
bash: `source ~/.bashrc`
zsh: source ~/.zshrc
ksh: . ~/.profile
```
4. Start using nvm

## Verify Installation

To verify that nvm has been installed, do:

`command -v nvm`

## Install Node using nvm

To install a new Node version using NVM, do:

`nvm install v15`

## Switch Node version

To switch between different node version, do:

`nvm use v15`
