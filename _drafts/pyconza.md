---
layout: page
title: PyConZA
---

PyConZA is an annual conference on the open-source programming language Python.

## Statistics

* Google's PageSpeedInsight: [70 on mobile, 83 on desktop](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fza.pycon.org%2F)
* Webaim's WAVE: [10 errors, 1 alert](http://wave.webaim.org/report#/https://za.pycon.org/)
* WebPageTest on Motorola G - Chrome on 3G: [SpeedIndex of 4446](http://www.webpagetest.org/result/160622_AG_8430f2a25dd99853a5230e7a91311a13/) on first run and 2616 on a repeat.

## Review

- Pretty lean and mean, clocking in at about 0.5MB.
- Images could do with optimisation and having alt text added.
- Things could be squeezed even smaller by removing the dependencies on Bootstrap (by writing some small, short, CSS) and jQuery (writing vanilla JS instead: looks like it's just used for menus?)

## The quick win

300KB of 500KB of the page size comes from one (background) image: `clouds_top.png` at 2300 x 450 px. Some different approaches that could be taken:

* Optimise the image. Running it through [kraken](https://kraken.io/web-interface) crunches the image down to 75KB.
* Use a different file format: the same image as a gif is only 34KB.
* The image contains a lot of blank space: split it into two separate images and apply them as multiple background images.
* Make a few smaller versions of the image, and include those at different sizes using media queries.

<!-- submit a PR at https://github.com/CTPUG/pyconza2016 for optimised images with this post? -->

---

Published on ddd dd mmm yyy.

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
