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

```

