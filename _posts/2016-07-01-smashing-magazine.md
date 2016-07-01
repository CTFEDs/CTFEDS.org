---
layout: page
title:
---

[Smashing Magazine](https://www.smashingmagazine.com/) is a well-known, long running, industry magazine that's evolved from listicles to in-depth articles over the years. A few years ago they did a big responsive redesign. We have a look at how it's doing in terms of Front-end performance.

## Statistics

* Google's PageSpeedInsight: [99/100 on mobile and desktop](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.smashingmagazine.com%2F)
  * Webaim's WAVE: [2 errors and 63 alert](http://wave.webaim.org/report#/https://www.smashingmagazine.com/)
* WebPageTest on Motorola G, Chrome, 3G: [SpeedIndex of 4539, 4724 on repeat view](http://www.webpagetest.org/result/160701_G5_093bd85b12358f314b322058aff9b1df/)

## Review

Summary

- pretty great results on PSI, WAVE, and WPT!
- lots of image requests, quite a lot of JS requests.

Generally speaking, the Smashing Magazine site is doing well on performance: they're even using ServiceWorkers to cache a bunch of resources, which is great! It would be good to try and reduce the number of HTTP requests: currently about 55 images and 9 JS files. The images could be sprited and the JS files could be combined.


---

Published on 1st July 2016.

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
