# CTFEDs event at Open Design Cape Town

## Checklist

With these principles in mind, here's a checklist of things for you to apply to your own sites.

### HTML

* Use the `picture` element and `srcset` to provide the image most suitable for the user's device. You can use [Picturefill](http://scottjehl.github.io/picturefill/) to enable support for `picture` in browsers that don't support it yet.
* Every image should have `alt` text.
* Optimise your images.
* Use SVGs instead of JPGs, PNGs, and GIFs where possible.
* Use as few images as you can: they use up the most data.
* Use HTML5 input types like `search`, `email`, and `date`.
* Use HTML5 elements like `section`, `article`, `header`, `footer`, and `nav`.
* Use WAI-ARIA landmarks roles like `banner`, `contentinfo`, navigation, and `complementary`.
* Make sure your site is accessible. Use tools like [Tenon](http://tenon.io/) and [pa11y](http://pa11y.org/) to check.
* Be careful about your web font usage. Don't use too many, and make sure you supply a suitable fallback.
* Validate your HTML.

### CSS

* Don't use inline CSS.
* Use CSS instead of images where possible.
* Provide fallbacks for CSS features: `px` for `rem` units; `rgb` for `rgba`, suitable `background-color` for `background` images, `png` for `svg` images.
* Keep selectors simple: just use element or class selectors (one level deep where possible). Don't use IDs or over-qualify selectors. Try using a style guide like SMACSS.
* Look at refactoring your CSS. If you have long selectors, use IDs, or over-qualify them, try refactoring using a style guide like [SMACSS](https://smacss.com/).
* Validate your CSS.
* Lint your CSS (check for errors and style).
* Serve a base.css to all browsers. Then use Media Queries to serve fancier browsers another stylesheet with fancier styles.

### Responsive Web Design

* Use a fluid grid: use `%`s instead of `px`.
* Make your images responsive, using `max-width: 100%; height: auto;`
  * Use the `picture` element and / or `srcset`.
  * Optimise your images (using a tool like [Kraken](https://kraken.io/))
* Use Media Queries to adjust elements of your site over varying screens sizes.
  * Use `min-width` rather than `max-width`.
  * Use `em` for breakpoints rather than `px`.
* Approach your site [Mobile First](http://www.lukew.com/resources/mobile_first.asp). Start with a small screen size and work your way up from there.
* Try and avoid using burgers.

### JavaScript

* Don't use inline JS.
* Place `script` elements at the bottom of the page, or load them asynchronously.
* Use feature detection (possible using a library like [Modernizr](http://modernizr.com/)) rather than device detection.
* Consider carefully if a feature is worth polyfilling. Would it be better to apply a technique like [cutting the mustard](http://responsivenews.co.uk/post/18948466399/cutting-the-mustard), and serve a simpler, faster, experience instead?
* Consider carefully if it's worth adding a jQuery plugin for a feature, rather than writing a smaller amount of code yourself.
* Hint your JS (check for errors and style).

### Performance

* Reduce sizes of CSS files by minifying them.
* Reduce sizes of JS files by minifying them.
* Minimise the number of HTTP requests by combining CSS files.
* Minimise the number of HTTP requests by combining JS files.
* Prefer serving fewer, larger, files to serving many, smaller, ones.
* Test across various network speeds, especially slow ones.
* Use WebPageTest to measure your site's performance.
* Use PageSpeed to get some ideas for performance optimisation.
* Load critical CSS in the head of your document, and load the rest asynchronously using JS (but provide a `noscript` fallback).