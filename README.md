Swipe Page Navigation
=================

Provides touch gesture control to navigate site pages

* The project site: https://github.com/dsheiko/spn
* The demo site: http://demo.dsheiko.com/spn

 Usually we hide all auxiliary page components on mobile to save space of the viewing area. So we have to provide in return alternative navigation tool out of the screen. Since keyboard with navigation keys isn't available, we can use touch gestures.

This script enables "swipe left/right" navigation on your site. It looks for sibling page links in the page head section (<link rel="prev" href="..">) and when found responds on swipe gesture to redirect on the requested page. When user starts the gesture (swiping) the script displays an arrow on the screen edge. But it gives more than that:

* It warns user about the captured gesture.
* It shows direction of swiping (prev/next).
* User can cancel the gesture, moving finger back to the initial position before finishing the gesture.


### Usage and API

1. Add to the pages you want available for swipe the navigation siblings links:
```
    <head>
        ...
        <link rel="prev" title="Page 2" href="page2.html" />
        <link rel="next" title="Page 1" href="page1.html" />
        ...
    </head>
```

2. Now it's enough to include the script and its css:

```
    <link rel="stylesheet" type="text/css" href="../src/assets/spn.css" />
    <script type="text/javascript" src="../src/js/spn.js"></script>
```
[![githalytics.com alpha](https://cruel-carlota.pagodabox.com/fd6941c91b72d881c4786416a69c4248 "githalytics.com")](http://githalytics.com/dsheiko/spn)