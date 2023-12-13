magnify.js
===========

Protect photo is a module that prevents image theft by preventing right-click and obscuring the image source in the console log.
it helps prevent image theft by disrupting traditional user interactions to download/copy images.

This is useful for copyrighted images.

This module uses the HTML5 CanvasAPI and the Protected Image theme to protect your images.
It disables and prevents the client from downloading, copying, and duplicating image titles by transferring
the image to a canvas. Unlike images that are protected by layers, 
this prevents the source of the image from being visible through the developer tools.


Usage
-----

Alternatively, download the package and reference the `protectImage.min.js` file in your HTML file.
Ensure you have included the latest stable jQuery version before including `protectImage.min.js`.

```html
<script src="src/script.min.js"></script>
```

 Add the protected attribute to images.

```html
<img src="1.jpg" protected />
```

Initialize the library and done.

```javascript
window.onload = function() {
    ProtectImageJS.init()
}
```

 The library will show the image on an HTML5 canvas element instead and hide the real image path in the console log:

```html
<canvas width="620" height="465"></canvas>
<img src="" protected="">
```
