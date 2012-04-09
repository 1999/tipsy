# tipsy (jquery-free)

Facebook-style tooltip plugin, jQuery-free

(c) 2008-2010 Jason Frame (jason@onehackoranother.com) - original plugin source code

(c) 2012 Dmitry Sorin (info@staypositive.ru) - jquery-free fork for modern web apps

Released under The MIT License.

## Description:

**tipsy** is a *simple jQuery plugin* for generating Facebook-style tooltips.
It's used by Twitter, Github, Slideshare and Bitbucket, amongst others.

**tipsy (jquery-free)** is its *jquery-free fork*, made specially for modern browsers (tested on Fx6 and later, Chrome15 and later).
You can use it in your chrome web store apps, mozilla marketplace apps etc. And there's no need in jQuery.

## Source:

Original jquery-tipsy package is hosted here:

  http://github.com/jaz303/tipsy/tree/master

jQuery-free tipsy fork is hosted here:

  http://github.com/1999/tipsy/tree/master

## Usage:

1. Copy the contents of src/{javascripts,stylesheets} to the corresponding asset directories in your project. 

2. Insert the neccesary elements in your document's `<head>` section, e.g.:

```html
<script type='text/javascript' src='/javascripts/tipsy.js'></script>
<link rel="stylesheet" href="/stylesheets/tipsy.css" type="text/css" />
```

3. Initialise Tipsy after DOMContentLoaded event, e.g.:

```javascript
window.addEventListener("DOMContentLoaded", function() {
  // dynamic binding (recommended for web apps)
  document.body.tipsy();

  // static binding
  // [].forEach.call(document.querySelectorAll("[title]"), function(elem) {
  //  elem.tipsy();
  // });
}, false);
```

You can also set "data-gravity" attribute to "n", "ne", "e", "se", "s", "sw", "w", "nw" values for better tooltip look.
If you don't set it tooltip's gravity will be calculated automatically. Take a look at src/example.html

## A note on forking:

By forking this project you hereby grant permission for any commits to your fork to be
merged back into this repository and, with attribution, be released under the terms of
the MIT License.
