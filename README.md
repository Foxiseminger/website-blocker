# Website Blocker
What this does is if you go to a blocked website, It will open this page and not let you access the page.
# Requirements
1. [Violentmonkey Extension](https://violentmonkey.github.io)
2. A [GitHub](https://github.com/) account
3. Knowledge of how to use [GitHub](https://github.com/)
#
>[!IMPORTANT]
>
>Please fork this repository before you do anything else, then go to settings, pages, and change the dropdown from "None" to "main" then click save. And then, Wait a minute for the page to deploy (you can see the progress in the "actions" tab)

To start, when you have the violentmonkey extension installed, Go to: extensions tab, violentmonkey, + icon, and paste this in:
```javascript
// replace https://example.com/ with whatever you want
// ==UserScript==
// @name         Redirect to Local HTML
// @namespace    http://violentmonkey.net/
// @version      1.0
// @description  blocks webpages how is that not simple enough?
// @match        *https://example.com/*
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // Redirect to the local HTML file
    window.location.href = "https://foxiseminger.github.io/website-blocker/";
    // replace "foxiseminger" with your github username
})();
```
#
After you have pasted in the code, press "CTRL + S". After that, you should be able to go to the page and see the website is blocked. If it is not, go to the issues tab in my github repository.
## License

[![GPLv3 License](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
