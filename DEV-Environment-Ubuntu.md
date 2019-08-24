# Install Basic cli stack for Ubuntu
```
sudo apt install -y curl fish git htop net-tools nmap pv vim
```

# Install Basic Ubuntu Applications
```

sudo apt install -y guake vim-gtk3

# Visual Studio Code
# curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > microsoft.gpg
# sudo mv microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg
# sudo sh -c 'echo "deb [arch=amd64] https://packages.microsoft.com/repos/vscode stable main" > /etc/apt/sources.list.d/vscode.list'

#sudo apt update

#sudo apt install -y code

# Google Chrome
wget -q -O - https://dl.google.com/linux/linux_signing_key.pub | sudo apt-key add -
sudo add-apt-repository "deb http://dl.google.com/linux/deb/ stable main"
sudo apt-get update
sudo apt-get install -y google-chrome-stable


# Docker

sudo apt-get install -y apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu $(lsb_release -cs) stable"

sudo apt update
sudo apt install -y docker-ce

# NodeJS

### https://nodejs.org/es/download/package-manager/#distribuciones-de-linux-basadas-en-debian-y-ubuntu

sudo curl -sL https://deb.nodesource.com/setup_12.x | bash -
sudo apt install -y nodejs npm

# YARN

sudo apt remove -y cmdtest

curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt update
sudo apt install -y yarn

```

# Install snap apps

```
sudo snap install insomnia postman rambox robo3t-snap
sudo snap install code --classic
sudo snap install sublime-text --classic
sudo snap install skype --classic
```

# Install typography for coding

https://github.com/tonsky/FiraCode/

```
sudo apt install -y fonts-firacode 
```

# Terminal
```
curl -L http://get.oh-my.fish | fish
chsh -s $(which fish)
fish
omf install zish
```

# Hyper
Install Hyper as terminal emulator

Download from https://hyper.is/#installation

Then install following themes + plugins:

```
hyper i hyper-solarized-dark2
hyper i hypercwd
hyper i hyper-dark-scrollbar
hyper i hyper-search
hyper i hyper-highlight-active-pane
hyper i hyperborder
hyper i hyperlinks
hyper i hyper-savetext
hyper i hyper-pane
```

# NodeJS development
* See our suggested [NodeJS global packages](app-nodejs-globals.md)

# Visual Studio Code (extensions)
* See our suggested [Visual Studio Code extensions](app-vscode.md)

# Google Chrome 
* See our suggested [Google Chrome extensions](app-googlechrome.md)

# React Native

```
```

# PHP Development

```
apt install -y php7.1-cli
```

## COMPOSER

```
wget https://raw.githubusercontent.com/composer/getcomposer.org/1b137f8bf6db3e79a38a5bc45324414a6b1f9df2/web/installer -O - -q | php -- 
```

## Drupal

```
# DRUSH

wget -O drush.phar https://github.com/drush-ops/drush-launcher/releases/download/0.6.0/drush.phar
chmod +x drush.phar
sudo mv drush.phar /usr/local/bin/drush

```

## Wordpress

```
# WORDPRESS CLI
curl -O https://raw.githubusercontent.com/wp-cli/builds/gh-pages/phar/wp-cli.phar
chmod +x wp-cli.phar
sudo mv wp-cli.phar /usr/local/bin/wp
```

# ANDROID Development 

https://mfonville.github.io/android-studio/

```
sudo apt-add-repository ppa:maarten-fonville/android-studio 
sudo apt-get update
sudo apt-get install android-studio
```
