---
layout: page
title: The Sunday Times
---

The Sunday Times is South Africa's largest selling Sunday print newspaper and is part of the Times Media Group, one of the largest media houses in South Africa. The website for the Sunday Times sits apart from their flagship Times Live site in a subdirectory of the main url.

## Statistics

* Google's PageSpeedInsight: [58 on mobile and 66 on desktop](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fwww.timeslive.co.za%2Fsundaytimes%2F&tab=mobile)
* Webaim's WAVE: [67 errors and 72 alerts](http://wave.webaim.org/report#/http%3A%2F%2Fwww.timeslive.co.za%2Fsundaytimes%2F)
* WebPageTest on 3G, running Chrome: [SpeedIndex of 13625 on first view](http://www.webpagetest.org/result/160617_QG_HX5/)

## Review

Here are a few things that stand out as areas for improvement:

- lots of static assets, especially images, could be cached;
- lots of images could be optimised;
- CSS and JavaScript files can be combined / concatenated and minified.
- Javascript files can be moved to the bottom of the page
- Move inline CSS and Javascript to external files.


**Setting expiry date or maximum age headers** for image files would mean files get cached by the browser: instead of fetching those files from the web every time, the browser would use the local ones. That means **the page would load faster and use less of the user's data**.

**Optimising the images** would reduce the file sizes. **That means the page would load faster and use less of the user's data**.

**Combining / concatenating both the JavaScript and CSS files** and if only one Javascript and one CSS file is loaded, this would lead to fewer HTTP requests, meaning a **faster page load**. **Minifying Javascript and CSS files** would lead to smaller file sizes and faster page load.

A number of Javascript files (such as jQuery) are being loaded in the `<head>` section of the page. These should be moved to the **bottom** of the page as they can potentially block downloading of other static content.

There are a number of inline script and CSS blocks that can be moved to **external files**. This will make them more **maintainable**
 and will ensure that they can be **cached** by the browser.

---

Published on Friday 17th June 2016.

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
