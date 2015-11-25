## Introduction

There's a Selenium IDE and a Selenium Webdriver. The former is a Firefox plugin, 
that works like an "action recorder" on FireFox. The later can work with different programming languages.

## Drive Selenium with NodeJS

The following steps will get you set up for programming to drive a browser under Windows:

* Install NodeJS (and npm of course)

* Create a project folder

* Go to Git Bash command line

* Enter project folder, and run
 
```
npm install --save selenium-webdriver 
npm install --save chromedriver
```

Now you are all set for the environment.

*  Write a short script under the project folder, such as 

```
// File name: test.js
 
var webdriver = require('selenium-webdriver');
var driver = new webdriver.Builder()
    .forBrowser('chrome')
    .build();
    
driver.get('http://www.ocef.org');
driver.quit();
``` 

* Run it (still under Git Bash command line) to prove that you can program to drive a Chrome browser: 

```
node test.js
```

A new Chrome browser should be opened at this point. As soon as the window is completely loaded, it will be closed. 
Because this particular website (ocef.org) involves loading external resources such as Sina weibo, the process is enjoyably slow.

### Have fund with Selenium and NodeJS