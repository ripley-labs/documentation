# Install Basic cli stack for Windows 

```
choco install -y curl git rsync vim-x64 yarn
```

# Install Basic Windows Applications

```
choco install -y 7zip  autohotkey ccleaner coretemp cyberduck firefox libreoffice-fresh opera rambox robo3t teamviewer virtualbox vivaldi
```

# Install Development Tools

```
choco install -y android-sdk androidstudio dbeaver ccleaner cmder docker-for-windows jdk8 postman python robo3t virtualbox wireshark

choco install -y visualstudiocode --pre
```

# Install Fonts

```
choco install -y firacode
```


# Install Ubuntu linux subsystem packages 

```
sudo apt update
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add 

sudo apt update
sudo apt upgrade -y
 
sudo apt install fish htop zsh
```

# Install Docker client in Ubuntu linux subsystem packages 

https://medium.com/@sebagomez/installing-the-docker-client-on-ubuntus-windows-subsystem-for-linux-612b392a44c4

```
sudo apt update
sudo apt-get install apt-transport-https ca-certificates curl software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add 
sudo apt update
sudo apt install -y docker-ce
```

# Enable bash / fish / zsh in cmder
[Running Windows 10 Ubuntu bash in cmder](https://gingter.org/2016/11/16/running-windows-10-ubuntu-bash-in-cmder/)

# NodeJS development
* See our suggested [NodeJS global packages](app-nodejs-globals.md)

# Visual Studio Code (extensions)
* See our suggested [Visual Studio Code extensions](app-vscode.md)

# Google Chrome 
* See our suggested [Google Chrome extensions](app-googlechrome.md)
