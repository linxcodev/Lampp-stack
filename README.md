# Install LAMP Stack
## 1. Install Apache
- ` sudo apt-get install apache2`
### Check Apache
- [localhost](http://localhost/)
### Restart Apache
- ` service apache2 restart`
### Change permission
- ` chmod -R 777 /var/www/html`
## 2. Install MySQL
- ` sudo apt-get install mysql-server`
### Check MySQL
- ` mysqladmin -u root -p status`
### Restart MySQL
- `sudo service mysql restart`
## 3. Install PHP
- `sudo add-apt-repository ppa:ondrej/php
sudo apt-get update
sudo apt-get install php
apt-get install php-pear php7.0-dev php7.0-zip php7.0-curl php7.0-gd php7.0-mysql php7.0-mcrypt php7.0-xml libapache2-mod-php7.0`
### Search module installed php
- ` apt-cache search --names-only ^php `
### Check PHP
- ` php -v`
#### or
- ` sudo vim /var/www/html/info.php`
#### add
- ` <?php
     phpinfo();
?>`
#### check
- ` http://server_ip_address/info.php`
### 4. Install Php My Admin
- ` sudo apt-get install phpmyadmin`
