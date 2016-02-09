zoom3d is a jQuery plugin for native-like momentum panning and zooming in mobile browsers.

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
Default: ```0.0005```. Higher number produces slower acceleration. 
     
```       
content
```
Default: ```""```. A jQuery selector or an element that becomes zoomable/pannable. 
If no selector is provided, the first child of the plugin element is selected.

```
doubleClickTime
```
Default: ```200```. Maximum time between two touchend events required for a double tap to occur.

```
dragLimit
```
Default: ```100```. The limit within which the content can be dragged out of the borders of its parent.
       
``` 
maxScale
```
Default: ```2```. Maximum scale.

```
midScale
```
Default: ```1```. Medium scale. Used after a double tap.

```
momentumTime
```
Default: ```200```. Maximum time between touchstart and touchend events required for momentum panning to occur.

```
onResize
``` 
The function called when the content scale changes. The function is passed the scale.