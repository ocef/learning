## Introduction

There's a Selenium IDE and a Selenium Webdriver. The former is a Firefox plugin, 
that works like an "action recorder" on FireFox. The later can work with different programming languages.

## Drive Selenium with NodeJS

**Drive Chrome Browser**

The following steps will get you set up for programming to drive a Chrome browser under Windows:

* Install NodeJS (and npm of course)

* Download chromedriver (win32) from http://chromedriver.storage.googleapis.com/index.html?path=2.20/, then extract the zip file, place chromedriver.exe under any Windows system path.

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

**Drive Firefox Browser**

It's actually easier to drive a Firefox browser instead of Chrome browser. 
On Windows, if you already have Firefox installed under "c:\Program Files\Mozilla Firefox", which could be the case most of the time,
there's no additional environment setup needed. Simply replace 

```
.forBrowser('chrome')
```

with 

```
.forBrowser('firefox')
```

and you are good to go.

**Drive PhantomJS Headless Browser**

First, [download PhantomJS](https://bitbucket.org/ariya/phantomjs/downloads/phantomjs-2.0.0-windows.zip) and extract executable under a Windows system path
 
Then replace 

```
.forBrowser('chrome')
```

with 

```
.forBrowser('phantomjs')
```

and you are good to go.

### Have fund with Selenium and NodeJS
