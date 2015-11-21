# Getting Started With [Drupal 8](https://www.drupal.org/)

## Practice (on Windows)

#### Download XAMPP and install Xampp on your computer (Windows, OSX, or Linux)

https://www.apachefriends.org/

This will provide PHP, MySQL, and Apache server. Use default installation directory "c:\xampp".

#### Download Drupal 8 from

https://www.drupal.org/node/2619030

Then extract the .zip or .gz file under "c:\xampp\htdocs", so that a new folder "C:\xampp\htdocs\drupal-8.0.0" is created with Drupal files.

#### Start Installation

In XAMPP, start Apache. From a browser, visit 

http://localhost/drupal-8.0.0

A Drupal installation page should show up. Here are the choices to make during installation:

1. Choose Language -- "English"

2. Select an installation profile -- "Standard"

3. Requirements review -- "continue anyway" upon any warning

4. Database configuration -- "SQLite" with default database file path

5. Configure site -- fill in "site name", "site email address" (doesn't have to be real), site maintenance account (make up a user name, such as "admin"), password (make up a password), Email address (doesn't have to be real), and other options

After that, just wait for the installation process to complete.

### Play around and have fun !





```
<?php
    echo "OCEF ROCKS! ^_^";
?>
```

And name it with file extension .php.

#### Run the PHP file from command line

Under command line, enter work directory (where your file resides), and run the ofllowing command

```
php YOUR-PHP-FILE-NAME
```

#### Visit the web page created by this PHP file via a Browser

###### Under command line, enter work directory.

###### Run the following command to start a built-in simple web server that comes with PHP

```
php -S localhost:9999
```

###### Open a browser and type in URL

```
http://localhost:9999/YOUR-PHP-FILE-NAME
```

You should now see "OCEF Rocks! ^_^" on the page in your browser.
