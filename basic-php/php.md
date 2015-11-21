# Getting Started With PHP

## Reading

http://php.net/manual/en/tutorial.php

## Practice

#### Download XAMPP and install Xampp on your computer (Windows, OSX, or Linux)

https://www.apachefriends.org/

This will provide PHP, MySQL, and Apache server.

#### Run PHP from any directory under command line

On Windows, it'll be convenient to add PHP installation directory to your system path. By default, you should have installed PHP under c:\xampp\php. 

For more information about adding directory to Windows system path, please look up online.

After this, open a command prompt window, and you should be able to run php command from any directory. 

#### Work directory

With PHP path included in system path, create a work directory anywhere you like. 

#### Create a PHP file

Create a new PHP file under the work directory, like so

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
