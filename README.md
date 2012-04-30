ExtJS Mirror
============

RTL support for Sencha Ext JS Framework

[http://behrang.github.com/extjs-mirror/](http://behrang.github.com/extjs-mirror/)

### What is extjs-mirror
It is mostly a hack that adds RTL feature to [ExtJS framework](http://www.sencha.com/products/extjs/).

Some languages like Persian, Hebrew and Arabic are [RTL (Right-To-Left)](http://en.wikipedia.org/wiki/Right-to-left). ExtJS does not support RTL. To support RTL, every component should layout itself from right to left.

This project, provides this feature by overriding some basic functionality in ExtJS. Here, positioning of elements are overridden so that instead of positioning elements from "Top Left", positioning is converted to "Top Right" (hence the name MIRROR).

There are more problems to solve. Some browsers like Firefox and IE, place scrollbars on left in RTL pages and some like Chrome, place scrollbars on right in either LTR or RTL. So scrollbar position have to be considered.

To use this, you have to develop your application for LTR. Then add a script (ext-mirror.js) and a css (ext-mirror.css) to your page and voila, everything will be converted to RTL. This way you can create a single internationalized app and use L10N to have both RTL and LTR apps.

### Examples
* Grid ([mirrored](2.html)) ([normal](2.html?ext-mirror-off))
* Tabs ([mirrored](3.html)) ([normal](3.html?ext-mirror-off))
* Feed Viewer ([mirrored](4.html)) ([normal](4.html?ext-mirror-off))