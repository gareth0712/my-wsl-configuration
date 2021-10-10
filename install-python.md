# Install Python

- Installing Python to WSL might be tricky as there are some minor settings after installation and sometimes you need to switch between Python 2 and Python 3 for different operations
 
## Install Python3

1. To install
```
$ sudo apt update && sudo apt upgrade -y
$ sudo apt install python3 python3-pip ipython3
```
2. To verify
```
$ python3 -V
Python 3.8.10
```

## Install Python2

1. To install
```
$ sudo apt install python2
```
2. To verify installation
```
$ python2 -V
Python 2.7.17
```

## Setting PYTHON as executable environmental variables

1. Identify which python version, 2 or 3, is wanted, say it would like to use python2
2. Find the source of python2 by running
```
$ whereis python2
python2: /usr/bin/python2
```
4. Set the environment variable for  
  a. this shell with `export PYTHON="/usr/bin/python2"` or;  
  b. permanently by adding a line `export PYTHON="/usr/bin/python2"` in `~/.bashrc` and run `source ~/.bashrc` afterwards
5. Test the environment variable by running `echo $PYTHON`
6. If it returns `/usr/bin/python2` then done
