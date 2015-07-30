<!-- ---
layout: default
title: Checklist / CTFEDs event at Open Design Cape Town
--- -->

# CTFEDs event at Open Design Cape Town

## Checklist

### HTML

* [Validate](http://validator.w3.org/) your HTML.
* Use HTML5 input types like `search`, `email`, and `date`.
* Use HTML5 elements like `section`, `article`, `header`, `footer`, and `nav`.

#### Images

* Optimise your images and use as few as possible.
* Make sure every image has `alt` text.
* Use the best format for your image: SVGs; JPGs (for photos, images with many colours); PNGs (for images with fewer colours); GIFs (for animations).
* Use the `picture` element and `srcset` to provide the image most suitable for the user's device. You can use [Picturefill](http://scottjehl.github.io/picturefill/) to enable support for `picture` in browsers that don't support it yet.

### CSS

* Don't use inline CSS (using the `style` tag or `style` attribute on HTML elements): use external stylesheets (using the `link` tag). The exception is for [critical CSS](https://developers.google.com/speed/docs/insights/PrioritizeVisibleContent#RemoveUnusedCSS): initially sending a small amount of CSS in the head of the document so that page rendering starts as early as possible.
* Lint your CSS (check for errors and style).
* Reduce sizes of CSS files by minifying them. 
* Minimise the number of HTTP requests by combining CSS files.
* Use CSS instead of images where possible.
* Provide fallbacks for CSS features: `px` for `rem` units; `rgb` for `rgba`, suitable `background-color` for `background` images, `png` for `svg` images.
* Keep selectors simple: just use element or shallow class selectors. Don't use IDs or over-qualify selectors. Try using a style guide like [SMACSS](https://smacss.com/).
* Serve a base stylesheet to all browsers. Then use Media Queries to serve fancier browsers with fancier styles.
* Be careful with web font usage. More weights and more fonts can mean a heavier, slower, site. Also make sure you supply a suitable fallback font.

### Responsive Web Design

* Use a fluid grid: use `%` instead of `px`.
* Make your images responsive, using `max-width: 100%; height: auto;`
* Use Media Queries to adjust elements of your site over varying screens sizes.
* Approach your site [Mobile First](http://www.lukew.com/resources/mobile_first.asp). Start with a small screen size and work your way up from there.
* Use `min-width` rather than `max-width` Media Queries, and use `em` for breakpoints rather than `px`.

### JavaScript

* Don't use inline JS (using a `script` tag or directly on an HTML element): include external JS files (using the `src` attribute on a `script` element).
* Hint your JS (check for errors and style).
* Reduce sizes of JS files by minifying them.
* Minimise the number of HTTP requests by combining JS files.
* Place `script` elements at the bottom of the page, or load them asynchronously by adding the `async` attribute to the `script` tag (this means that the loading of the JavaScript files won't block loading of the page).
* Use feature detection (possibly using a library like [Modernizr](http://modernizr.com/)) rather than device detection.
* Consider carefully if a feature is worth polyfilling. Would it be better to apply a technique like [cutting the mustard](http://responsivenews.co.uk/post/18948466399/cutting-the-mustard), and serve a simpler, faster, experience instead?
* Consider carefully if it's worth adding jQuery, or whether you can use regular JavaScript instead. Check out [You might not need jQuery](http://youmightnotneedjquery.com/).
* Consider carefully if it's worth adding a jQuery plugin for a feature, rather than writing a smaller amount of code yourself. Check out [You might not need jQuery Plugins](http://youmightnotneedjqueryplugins.com/).

### Performance

* Make sure `gzip` compression is enabled on your web server.
* Use [PageSpeed Insights](https://developers.google.com/speed/pagespeed/insights/) to get some ideas for performance optimisation from Google's list of guidelines.
* Use [WebPageTest](http://www.webpagetest.org/) to measure your site's performance and get stats that let you compare your site with new version and with competitors.


### Tools

* Image optimisation: [Kraken](https://kraken.io/)
* CSS Linting: [csslint](http://csslint.net/)
* CSS Minification: [cssminifier](http://cssminifier.com/)
* Get CSS stats and look for improvements: [cssstats](http://cssstats.com/) and [stylestats](http://www.stylestats.org/).
* JS Hinting: [JSHint](http://jshint.com/)
* JS Minification: [jscompress](http://jscompress.com/).
* Linting, Hinting, and Minification are also possible using plugins for editors like [Sublime Text](http://www.sublimetext.com/), [Atom](https://atom.io/), and [CodeKit](https://incident57.com/codekit/), or by using a build tool like [Grunt](http://gruntjs.com/) or [Gulp](http://gulpjs.com/).