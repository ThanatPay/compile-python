# compile-python
This is a repo for compiling and installing python from scratch

## check update
```
sudo apt-get update
```

## compile Python and Create VirtualEnv with It
#### Download python version
install any library
```
sudo apt-get install build-essential gdb lcov libbz2-dev libffi-dev libgdbm-dev liblzma-dev libncurses5-dev libreadline6-dev libsqlite3-dev libssl-dev lzma lzma-dev tk-dev uuid-dev zlib1g-dev
```
download python version form website
```
wget https://www.python.org/ftp/python/3.10.14/Python-3.10.14.tgz
```
unzip file
```
tar zxvf Python-3.10.14
```
if you need to delete file zip
```
rm Python-3.10.14.tgz
```
go to file Python-3.10.14
```
cd Python-3.10.14
```
configure the optimizations for it
```
./configure --enable-optimizations
```
make alt and stall and this will actually put everything in place
```
sudo altinstall
```
#### Set key python to create python version
make python to be default
```
vim ~/.bashrc
```
and add this command to bashrc
```
alias python="/usr/local/bin/python3.10"
```
save file bashrc
```
source ~/.bashrc
```

#### Create VirtualEnv with python version
create a virtual environment
```
python -m venv ~/.venv
```
we want this virtual environment to live in this directory. It's going to be working with that particular version of Python. 
```
vim ~/.bashrc
```
make default
```
source ~/.venv/bin/activate
```
save bashrc
```
source ~/.bashrc
```
