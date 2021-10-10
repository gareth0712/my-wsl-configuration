# Install VSCode

Installing VSCode in WSL is extremely easy. Yet, some settings are necessary in order to simplify our development work.

## Install VSCode

In any directory, run `code .` will trigger installation of VSCode in the WSL and it will then open VS Code in your Windows, with connection to the files inside WSL

## Accessing server running in WSL via your Windows

- Accessing a server running in WSL might be tricky, make sure you have [wslconfig](wslconfig.md) tuned well to allow portforwarding. 
- e.g. Server is running in 127.0.0.1:3000
- Setting portforwarding in wslconfig allows ports bound to wildcard or localhost in the WSL 2 VM connectable from the host using "localhost:port"
- Without setting portforwarding, you will not be able to access the WSL server via "localhost:3000"
