---
layout: page
title: An Event Apart
---

## Statistics

* Google's PageSpeedInsight: [74 / 100 mobile, 90 / 100 desktop](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Faneventapart.com%2F)
* Webaim's WAVE: [5 errors](http://wave.webaim.org/report#/http://aneventapart.com/)
* WebPageTest on 3G: [SpeedIndex of 2826](https://www.webpagetest.org/result/160812_7A_VS2/)

## Review

[An Event Apart](http://aneventapart.com/) is a conference that is (in their own words) "an intensely educational two-day learning session for passionate practitioners of standards-based web design."

Given the premise of the event one would assume that the website would follow best practice and be highly performant. This is largely the case. When it comes to best practice in performance [An Event Apart](http://aneventapart.com/) ticks most of the boxes.

- Standard performance techniques like enabling keep-alive, compressing transfer and images, caching static content and using a CDN are all enabled.
- The server is optimised for fast delivery and the HTML is minified reducing its size significantly.
- The site loads relatively quickly, even on a 3G connection.

There are a few areas where performance can be improved.

- **Total page size is 1.3mb**, over 800kb of which is images. While images are optimised some of them are still between 150 and 200kb.
- There are **54 requests**: a little over a reasonable number. These could be reduced by combining JS files where possible. 27 of these are also for images.
- **CSS and JS files are not minified**. Minifying these will speed up download, parsing and execution time.

While [An Event Apart](http://aneventapart.com/) performs well and follows a number of best practices and bit of additional tweaking could make it even better.

---

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
