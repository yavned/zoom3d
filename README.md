##Zoom3d

###About

Zoom3d is a jQuery plugin for native-like momentum panning and zooming in mobile browsers.

###Usage

```javascript
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
Higher number produces slower acceleration. Default: ```0.0005```.

```       
content
```
jQuery selector or an element that becomes zoomable/pannable.
If no selector is provided, the first child of the plugin element is selected.
Default: ```""```.

```
doubleClickTime
```
Maximum time in milliseconds between two touchend events required for a double
tap to occur.
Default: ```200```.

```
bounceLimit
```
Distance in pixels within which the content can exceed its parent before it
bounces back.
Default: ```100```.

```
maxScale
```
Maximum scale. Default: ```2```.

```
midScale
```
Medium scale. Used after a double tap. Default: ```1```.

```
momentumTime
```
Maximum time between touchstart and touchend events required for momentum
panning to occur.
Default: ```200```.

```
translate3d
```
Boolean. When ```true```, the plugin uses 3d transforms to help software
acceleration. Default: ```false```.

```
onScale
```
Function called when the content scale changes. The function is passed the
scale.
