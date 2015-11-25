## Use Composer for Package Management

PHP finally had a package (or dependency) manager a few years ago -- Composer. This is the equivalency of maven in Java world.

### Install Composer

Composer can be downloaded or installed following instructions on [Composer website](https://getcomposer.org/doc/00-intro.md). 
When using Windows, I found it convenient to download Composer to PHP directory, 
then create a bat file as instructed. Something like this:

c:\xampp\php>echo @php "%~dp0composer.phar" %*>composer.bat

### Initiate a Project

Under command line, first create a new folder, then enter the folder and run 

composer init 

or 

composer.bat init

If it's already known that a package is to be used, then it can be added towards the end of the interactive process.

In the end, you get a composer.json file that describe the project information, as well as its dependencies. 

Then running the following command would actually download the dependencies -- whatever PHP packages you listed previously:

composer update 

or 

composer.bat. update


