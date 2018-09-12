# google-homepage

This is a clone of the Google homepage. 
The structure of the page, positioning and basic styling of elements were made by myself. I just checked the original source code to fine tune the styling so that the page looks exactly like the original.  
I separated the page in three sections:

1. The `header`, which contains an unordered list for the links at the top
2. A `div` of class "content", which contains the main elements (the logo image and a form element for the search box and buttons)
3. The `footer`, which contains an unordered list for the links at the bottom

To position the links of the header exactly as I wanted without much effort, I used **CSS Flexbox**.

To center the buttons bellow the search box, I set the `text-align` property of its parent element (`<form>`) to `center`	. By the way, this solution is much more elegant than the solution used by someone at Google, who put the buttons between `<center>` tags. The `<center>` tag is not supported in HTML5.

I used **descendant selectors**, **attribute selectors** and **structural pseudo-classes** (`:nth-child()`) to avoid filling the HTML with classes.

For the links in the footer, Google uses `font-size: small;`. This is not consistent across browsers (I tested on Chrome and Firefox). For consistency, I used `font-size: 13px;`. This is how Chrome interprets `small`. 

From The Odin Project's [curriculum](http://www.theodinproject.com/courses/web-development-101/lessons/html-css). 
