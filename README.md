# Clone this repository
```
  git clone 
```
# Required Packages 
```
PHP 8 Version 
Mysql 8 Version
Install PHP required Modules
Apache File
```

# Create a databases 
```
  DB name :- hostel
  CREATE DATABASE hostel;

  Import the hostel.sql file into the hostel database
  mysql -u root -p hostel < hostel.sql

```

# Change the database Credentials in the configuration file 

# Create a config file for the apache to host our website 

```
<VirtualHost *:80>
    ServerAdmin webmaster@your_domain.com
    ServerName test.shivm07.shop
    ServerAlias test.shivm07.shop

    DocumentRoot /var/www/html/hostel-management-project-PHP/hostel
    <Directory /var/www/html/hostel-management-project-PHP/hostel>
        Options Indexes FollowSymLinks
        AllowOverride All
        Require all granted
        DirectoryIndex index.php index.html
    </Directory>

    ErrorLog ${APACHE_LOG_DIR}/your_project_error.log
    CustomLog ${APACHE_LOG_DIR}/your_project_access.log combined

    <FilesMatch \.php$>
        SetHandler application/x-httpd-php
    </FilesMatch>
</VirtualHost>

```

# 

1. Download and Unzip the file on your local system.
2. copy hostel folder Put this folder inside xampp/htdocs/ .
3. Database Configuration

Open PHPMyAdmin
Create a Database hostel.
Import database hostel.sql
Open Your browser put inside browser “http://localhost/hostel/”
Login Details
To Login as admin put inside browser “http://localhost/hostel”
Login Details for admin : admin/Test@1234
Login Details for user : test@gmail.com/Test@123
