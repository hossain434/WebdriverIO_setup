# WebdriverIO_setup

1.	What is the purpose to use  this tool?
https://blog.kevinlamping.com/4-reasons-why-you-should-think-about-using-webdriverio/
1.	It's Front-end Friendly
2.	It has the Power of Selenium
3.	It Strives for Simplicity
4.	It's Easily Extendable
5.	Support for the WebDriver specification as well as to Appium
6.	Run tests on desktop and mobile, Command line interface
7.	Cross browser support
8.	You can run your tests using WDIO Testrunner or Standalone Mode
9.	Works with many assertion libraries and testing frameworks (Jasmine, Mocha, Cucumber)
10.	Enables running tests on desktop as well as on mobile

2.	Why this is better than other tool?
Same s #1
3.	Why you're using this tool?
Same as #1
4. Usability:
a. Normal scripting using page object and with different browsers. and platform e.g Windows, MAC, Mobile
Page Object: Yes
Cross Browser: Yes
Mac: Yes
Mobile: Yes, Appium 

b. Parallel execution. Yes

c. Datadriven with Assertion using csv or xlsx  Yes
Assertion: Yes
d. Jenkins build or execution in Docker Yes

e. Result Report Yes , Allure Report

f. Advantages and drawback

CON Must run with WDIO to debug

Tasks written in this beautiful Selenium API can only be debugged using the provided WDIO task runner. You can't set breakpoints within tasks, but you can have WDIO pause the run between Selenium commands.

CON Selenium server must be started independently

selenium-webdriverjs starts the Selenium server automatically, and actually manages to achieve a faster startup time (4 seconds vs. 5.5) than WebdriverIO.

CON Have no docs for latest version (4.0.5)
Assertions are problematic at the beginning

WebdriverIO Setup:

https://webdriver.io/docs/gettingstarted.html

Install Visual Studio 2015. Do custom install and add Windows SDK 8.1 and Visual C++. 

Below command used on Windows CMD as Admin privilege:

Install build tool: npm install --global --production windows-build-tools

Install node gyp:  https://github.com/nodejs/node-gyp 

$ mkdir webdriverio-test && cd webdriverio-test

$ npm init -y

$ npm i --save-dev @wdio/cli

$ npx wdio config -y

$ mkdir .\test\spec

$ touch ./test/specs/basic.js (create a file called basic.js)

$ npx wdio wdio.conf.js  (to run the script)
