# init-unix

## Update Ubuntu.
```
sudo apt-get upgrade
sudo apt-get update
```

## Create a `workspace` folder into `$HOME`.
```
mkdir ~/workspace
sudo ln -s ~/workspace/ /workspace
```

## Install Vim.
```
sudo apt-get install vim
```

## Install Phpstorm.
* [Download the tarball](https://www.jetbrains.com/phpstorm/download/#section=linux).tar.gz.
* Extract the tarball to a directory
```
sudo tar -xzf PhpStorm-*.tar.gz -C /opt
```
To create a desktop entry: menu Tools | Create Desktop Entry

## Install GIT
```
sudo apt-get install git
```
* Configure
```
vim ~/.gitconfig
```
Add the following instructions: [see](config/gitconfig).

* Add branch to bash
```
vim ~/.bashrc
```
Add the following instructions: [see](config/bashrc).

## Install Mariadb
```
sudo apt install mariadb-server
sudo mysql

```
* Add user
```
CREATE USER 'iamroot'@'localhost' IDENTIFIED BY 'iamroot';
GRANT ALL PRIVILEGES ON * . * TO 'iamroot'@'localhost';
FLUSH PRIVILEGES;
```

## Install DBeaver
```
wget -O - https://dbeaver.io/debs/dbeaver.gpg.key | sudo apt-key add -
echo "deb https://dbeaver.io/debs/dbeaver-ce /" | sudo tee /etc/apt/sources.list.d/dbeaver.list
sudo apt updatesudo apt update
sudo apt -y  install dbeaver-ce
```

## Install Postman
```
sudo apt install flameshot
```

* Settings>Keyboard Shortcuts>Custom shortcuts
```
flameshot
flameshot.gui
Print
```

## Install Postman
```
sudo snap install postman
```

## Install Curl
```
sudo apt-get install curl libcurl4
```

## Install Php
```
sudo apt install php7.4-cli php7.4-curl php7.4-xml php7.4-mysql php7.4-xsl php7.4-mbstring
```
* Check Extensions
```
php -m
```

## Install Composer
```
curl -sS https://getcomposer.org/installer | php
sudo mv composer.phar /usr/local/bin/composer
sudo chown -R llaurent /usr/local/bin/composer
```

## Install Symfony
```
wget https://get.symfony.com/cli/installer -O - | bash
sudo mv /home/llaurent/.symfony/bin/symfony /usr/local/bin/symfony
sudo chown -R llaurent /usr/local/bin/symfony
```


