# Install LAMP Stack
## 1. Install Apache
```install
$ sudo apt-get install apache2
```
* ### Check Apache
```check
http://server_ip_address
```
* #### Or
```check
http://localhost
```
* ### Restart Apache
```restart
$ service apache2 restart
```
* ### Change permission
```change
$ chmod -R 777 /var/www/html
```
## 2. Install MySQL
```install
$ sudo apt-get install mysql-server
```
* ### Check MySQL
```check
$ mysqladmin -u root -p status
```
* ### Restart MySQL
```restart
$ sudo service mysql restart
```
## 3. Install PHP
```install
$ sudo add-apt-repository ppa:ondrej/php
$ sudo apt-get update
$ sudo apt-get install php
$ apt-get install php-pear php7.0-dev php7.0-zip php7.0-curl php7.0-gd php7.0-mysql php7.0-mcrypt php7.0-xml libapache2-mod-php7.0
```
* ### Search module installed php
```search
$ apt-cache search --names-only ^php
```
* ### Check PHP
```check
$ php -v
```
#### or
```edit
$ sudo vim /var/www/html/info.php
```
#### and add
```add
<?php
     phpinfo();
?>
```
* ### check
```check
http://server_ip_address/info.php
```
### 4. Install PhpMyAdmin
```install
$ sudo apt-get install phpmyadmin
```
* ### Check PhpMyAdmin
```check
http://server_ip_address/phpmyadmin
```
* #### Or
```check
http://localhost/phpmyadmin
```
