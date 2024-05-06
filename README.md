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
- In this directory, you can find an annotated script, network.sh, that stands up a Fabric network using the Docker images on your local machine

- From inside the test-network directory, run the following command to remove any containers or artifacts from any previous runs:
```
./network.sh down
```
You can then bring up the network by issuing the following command. You will experience problems if you try to run the script from another directory:
```
./network.sh up
```
![image](https://github.com/DamanAhuja/Hyper-Ledger-installation/assets/142963733/46e8d061-2820-40a7-9f01-dbe61403a164)
## Creating a channel
You can use the network.sh script to create a channel between Org1 and Org2 and join their peers to the channel. Run the following command to create a channel with the default name of mychannel:
```
./network.sh createChannel
```
## Deploying a Smart Contract to a channel
If everything is done correctly - 
![image](https://github.com/DamanAhuja/Hyper-Ledger-installation/assets/142963733/4644140d-3d01-46ba-b210-efc2aeb13865)
