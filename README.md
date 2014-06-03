# Print Plus Widget for ArcGIS WebApp Builder (AWAB)

This DOJO Mixin will add a Widget Opacity Slider to the title bar of an in-panel AWAB Widget. [demo](http://gis.hamiltoncounty.in.gov/mapviewer1/index.html)

## Installation:
* Clone or download the repo
* Move the _WidgetOpacityMixin folder to the widget folder of a downloaded AWAB application on your web server
* Add the mixin to an in-panel widget.  For example, the Measurement Widget would look like this:

```javascript
  define([
    'dojo/_base/declare',
    .
    .
    .
    'widgets/_WidgetOpacityMixin/widget'
  ],
  function(
    declare,
    .
    .
    .
    _WidgetOpacityMixin
  ) {
    var clazz = declare([BaseWidget, _WidgetsInTemplateMixin, _WidgetOpacityMixin], {
      etc.
    })
  )
```

* Enjoy!

## Customize:
* Use the _WidgetOpacityMixin\config.json file to customize the minimum and maximum opacity and the resize delay

## Change log:
* 6/2/2014
	1. Initial post.
