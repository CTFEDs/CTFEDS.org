---
layout: page
title: How are we doing?
---

Popular site noupe.com released a post [10 Hand-Picked WordPress Themes of August 2016](http://www.noupe.com/wordpress/hand-picked-wordpress-themes-august-2016-98679.html) a few weeks ago, and we decided to have a look at the performance of those Themes. Check the pulse, have a look at the state of nation, see how we (as people who make websites) are doing. Unfortunately, it's more of a case of "Nope" than "Noupe" (sorry).

## Statistics

We decided to just look at the mobile PageSpeed scores of the demo page for each Theme (that had a demo), to get a rough read of them. Here are the results:

- [Wanderlust](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fwanderlusthq.com%2F): 25/100
- [Travellator](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Ftravellator.net%2F): 30/100
- [The Launcher](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fdemo.accesspressthemes.com%2Fthe-launcher%2Fsimple-home%2F): 34/100
- [Acool](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fwww.coothemes.com%2Fdemos%2Facool%2F): 54/100
- [Morphology Lite](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fdemos.shapedpixels.com%2Fmorphology-lite%2F): 70/100
- [Fabulous Fluid](https://developers.google.com/speed/pagespeed/insights/?url=https%3A%2F%2Fcatchthemes.com%2Fdemo%2Ffabulous-fluid%2F): 41/100
- [Safreen](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fsafreen.imonthemes.com%2Fdemo1%2F): 66/100
- [Shopisle](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fthemeisle.com%2Fdemo%2F%3Ftheme%3DShopIsle%23): 61/100
- [Prestro](https://developers.google.com/speed/pagespeed/insights/?url=http%3A%2F%2Fthemesware.com%2Fdemo%2Fprestro%2F): 38/100

The highest score was 70 and the lowest was 25. Ouch.

## Review

The (mean) **average PageSpeed score was 47/100**. The median average was a little lower at 41/100.

You could argue that **some of PageSpeed's metrics aren't fair to test on a demo site**, such as **enabling compression, caching, and server response**. The Theme will be deployed on a different server, where those things may be fixed. While this is true, it would be great for a demo to show off a Theme as the best it can be, and to **set a good example of how to use the Theme** in the wild. The h5bp project has example server configs for [nginx](https://github.com/h5bp/server-configs-nginx) and [Apache](https://github.com/h5bp/server-configs-apache) that would help with the first two.

You could make a similar argument for optimising images. They are **content that will be different from the live site**, so shouldn't be included in the score. The flipside is that **Themes could require a Plugin that optimises images automagically**. There are quite a few on [the Plugin Directory](https://wordpress.org/plugins/search.php?q=image+optimisation). That way, the content author doesn't need to remember to optimise their images: it just happens.

Eliminate render-blocking JavaScript and CSS in above-the-fold content is a bit of a fiddly one. If we're talking about Critical CSS, that's a tricky one. It's still **a new technique that's a bit fiddly**, and it's perhaps unfair to expect it to be widely adopted already. However, the PageSpeed comments for these Themes refer to an older technique that most of the Themes aren't implementing: **having your `script` tag(s) at the bottom of your document**. This metric was in "Should Fix" for the majority of the Themes because there were a lot (double digits of both CSS and JS!) of files, making the problem worse.

So, State of the Front-end Nation (or, WordPress Theme Nation, at least)? In the red. :-/

![](/img/in-the-red.jpg)

---

Published on Friday 9th September 2016.

[Steve Barnett](https://naga.co.za/) ([@maxbarners](https://twitter.com/maxbarners)) and [Justin Slack](http://justinslack.com/) ([@justin_r_slack](https://twitter.com/justin_r_slack))

[CTFEDs](http://ctfeds.org/) Organising Team
