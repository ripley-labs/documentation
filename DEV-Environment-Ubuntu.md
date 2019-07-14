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

# Visual Studio Code (extensions)

```
# Editor
code --install-extension 2gua.rainbow-brackets # Rainbow Brackets
code --install-extension EditorConfig.EditorConfig # Editor Config
code --install-extension SirTori.indenticator # Indenticator


# Theme
code --install-extension Equinusocio.vsc-material-theme # Material Theme for VSCode
code --install-extension PKief.material-icon-theme # Material Icon theme

# Formats
code --install-extension PeterJausovec.vscode-docker # Docker
code --install-extension dbaeumer.vscode-eslint # ESLint
code --install-extension eriklynd.json-tools # JSON Tools
code --install-extension mikestead.dotenv # dotenv
code --install-extension yzane.markdown-pdf # Markdown to PDF
code --install-extension yzhang.markdown-all-in-one # Markdown

# Integrations
code --install-extension donjayamanne.githistory # Git history
code --install-extension eamodio.gitlens # Gitlens
code --install-extension msjsdiag.debugger-for-chrome # Chrome Debugger 
code --install-extension hbenl.vscode-firefox-debug # Firefox Debugger
code --install-extension esbenp.prettier-vscode  # Prettier
code --install-extension humao.rest-client # Rest Client

# Programming Languages
code --install-extension lukehoban.Go # Go
code --install-extension felixfbecker.php-debug # PHP Debug
code --install-extension ms-python.python # Python

# Nodejs / React
code --install-extension wix.vscode-import-cost

```

# React Native

```
```

# NodeJS development

```
sudo npm install -g concurrently cross-env dotenv-cli eslint newman serverless   
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
