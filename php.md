# this PHP commands Install in server local  OS ubuntu 18 to 20.04

# friest
sudo apt update
sudo apt upgrade



sudo apt install software-properties-common
sudo add-apt-repository ppa:ondrej/php
sudo apt update

sudo apt install php libapache2-mod-php php-mysql
---
sudo apt install php[version_numeber]-[package_name]
php7.4-fpm

#sudo apt install php7.4-{mysql,zip,json,common,bcmath}

sudo apt install php7.4-common php7.4-cli php7.4-bcmath php7.4-bz2 php7.4-curl php7.4-gd php7.4-intl php7.4-json php7.4-mbstring php7.4-readline php7.4-xml php7.4-zip php7.4-fpm

#To list all loaded PHP modules run the command:
php -m
#Verify the installation with:
php -v
-----
sudo a2dismod php7.4

sudo a2enmod php7.3

sudo service apache2 restart

------
sudo update-alternatives --set php /usr/bin/php7.3
sudo update-alternatives --set phar /usr/bin/phar7.3
sudo update-alternatives --set phar.phar /usr/bin/phar.phar7.3
sudo update-alternatives --set phpize /usr/bin/phpize7.3
sudo update-alternatives --set php-config /usr/bin/php-config7.3
