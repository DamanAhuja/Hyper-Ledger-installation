# Hyper-Ledger-installation
## Pre-Requisites 
- CURL latest version
- Docker - [Installation](https://github.com/DamanAhuja/Docker.git)
- Docker Compose
- GoLang - [Installation](https://github.com/KRIISHSHARMA/go-installation.git)
- Node JS
- NPM
### Check Versions 
![image](https://github.com/DamanAhuja/Hyper-Ledger-installation/assets/142963733/b8ecc4f6-b626-4f71-b461-fbe3b7c4bdbf)
## Installation
First create a directory named fabric
```
mkdir fabric
```
then enter the directory by 
```
cd fabric
```
Then Enter the command
```
sudo su
```
to become a super user and get the required permissions

To get the installation script - 
```
curl -sSLO https://raw.githubusercontent.com/hyperledger/fabric/main/scripts/install-fabric.sh && chmod +x install-fabric.sh
```
Pulling the docker images - 
```
./install-fabric.sh docker samples binary
```
or
```
./install-fabric.sh d s b
```
## Running a Test network
Change the current directory
```cd fabric-samples/test-network```
