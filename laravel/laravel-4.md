# Getting Started With Laravel

This is NOT an actual project, but rather a set of document to describe how to get started with Laravel.

Note that Laravel is now on version 5.1. This document only reflects Laravel version 4.2.

## ["Homestead approach" by Laravel](http://laravel.com/docs/4.2/homestead)

If desired, Laravel described an approach using Oracle VirtualBox and Vagrant, etc. This could potentially bring many benefits. If not, then the old fashion way would include two parts: environment setup and Laravel project creation.

## General Setup of Environment

Obviously, we'll need PHP. 

Later version of PHP ( > 5.4.0 ) has a built-in web server for development purpose. So, installing a web server is actually optional. 

Note that database is optional as well. But of course, any meaningful application would usually require a database.

Composer is widely used for package management with PHP. It is required by Laravel.

Here's how I set up:

1. Installing [XAMPP](https://www.apachefriends.org/) takes care of PHP, Apache and MySQL. When using Windows, it's better to add PHP path to system path.

2. Composer can be downloaded or installed following instructions on [Composer website](https://getcomposer.org/doc/00-intro.md). When using Windows, I found it convenient to download Composer to PHP directory, then create a bat file as instructed. Something like this:

c:\xampp\php>echo @php "%~dp0composer.phar" %*>composer.bat

## Create a Blank Laravel Project

It everything went well, we should be able to creat a blank Laravel project now.

Running the following command line would create a new project folder, and install Laravel there:

composer create-project laravel/laravel ACTUAL-PROJECT-FOLDER-NAME 4.2 --prefer-dist

## Running the blank project

Enter the newly created project folder, run the following command line

php artisan serv

Then visiting http://localhost:8000/ from a browser should show a simple page with Laravel logo. 

## Useful resources

First, Laravel website did a great job on documentation. Here's the direct link to 4.2 documenation [http://laravel.com/docs/4.2](http://laravel.com/docs/4.2).

[Laracast](https://laracasts.com/) is a great site for not only Laravel, but also PHP in general. There's a paid plan option, but one could learn a lot just from the videos that are freely available.

 
