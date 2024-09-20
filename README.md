# Website Blocker
what this does is if you go to a blocked website, It will open this page and not let you access the page.
# Requirements
1. Violentmonkey
2. github (ofc)
#
To start, when you have the violentmonkey extension installed, Go to: extensions tab, violentmonkey, + icon, and past this in:
'// ==UserScript==
// @name         Redirect to Local HTML
// @namespace    http://violentmonkey.net/
// @version      1.0
// @description  Redirect to a local HTML file when visiting a specific site
// @match        *://*.any-url-you-want/*
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // Redirect to the local HTML file
    window.location.href = "https://foxiseminger.github.io/website-blocker/";
})();
'
