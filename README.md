Zoom3d is a jQuery plugin for native-like momentum panning and zooming in mobile browsers.

###Usage

```
$(function () {
    $(".zoom3d").zoom3d({
        content: ".content",
        translate3d: true
    });
});
```

###Plugin options

```
accelerationRatio
```
Higher number produces slower acceleration. Default: ```0.0005```
     
```       
content
```
A jQuery selector or an element that becomes zoomable/pannable. 
If no selector is provided, the first child of the plugin element is selected. 
Default: ```""```

```
doubleClickTime
```
Maximum time in milliseconds between two touchend events required for a double tap to occur. 
Default: ```200```

```
bounceLimit
```
The distance in pixels within which the content can exceed its parent before it bounces back. 
Default: ```100```
       
``` 
maxScale
```
Maximum scale. Default: ```2```

```
midScale
```
Medium scale. Used after a double tap. Default: ```1```

```
momentumTime
```
Maximum time between touchstart and touchend events required for momentum panning to occur.
Default: ```200```

```
onScale
``` 
The function called when the content scale changes. The function is passed the scale.
