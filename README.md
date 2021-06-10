# google-homepage

This is a clone of the Google search results page. The goal was to have something indistinguishable from the originial even for the keenest of eyes. For that, I would check the original source code to fine tune the styling accordingly.  

The page was divided into three sections:

1. The `header`, which contains an unordered list for the links at the top
2. The `main`, which contains the main elements (the logo image and a `form` element for the search box and buttons)
3. The `footer`, which contains an unordered list for the links at the bottom

I used **CSS Flexbox** to position the links of the header exactly as I wanted without insane effort.

To center the buttons bellow the search box, I set the `text-align` property of its parent element (`form`) to `center`. By the way, this solution is much more elegant than the solution used by some intern at Google who put the buttons between `<center>` tags. The `center` element is [not supported](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/center) in HTML5.

I used **descendant selectors**, **attribute selectors** and **structural pseudo-classes** (`:nth-child()`) to avoid cluttering the HTML with classes.

For the links in the footer, the Google intern used `font-size: small;`. This is not consistent across browsers (I tested on Chrome and Firefox). For consistency, I used `font-size: 13px;`. This is how Chrome interprets `small`. 

---

From The Odin Project's [curriculum](http://www.theodinproject.com/courses/web-development-101/lessons/html-css). 
