# Print Plus Widget for ArcGIS WebApp Builder (AWAB)

The Print Plus Widget enhances and extends the AWAB Print Widget. [demo](http://gis.hamiltoncounty.in.gov/mapviewer1/index.html)

## Installation:
* Clone or download the repo.
* Move the PrintPlus folder to the widgets folder of a downloaded AWAB application on your web server.
* Configure and/or create the layout templates you need on your ArcGIS for Server.
* Edit the config.json file settings to reflect your server and your preferences.  These configuration tags have been to the tage in the AWAB Print Widget:
	1. defaultDpi - the default print resolution in DPI.
	2. noTitleBlockPrefix - the prefix for layout templates that have the same paper size and orientation as another template, but
     do not have a title block (e.g. "No TB ").  Layout templates with this prefix will not show in the dropdown list, but will activate
     the "Show Layout" checkbox when the corresponding layout template is selected (e.g. "Letter ANSI A Landscape" and "No TB Letter ANSI A Landscape").
	3. layoutParams - the alias, paper units, and paper dimensions for each layout template.  The alias will be used to populate the layout dropdown.  The 
     paper units is the string value of the Esri Units constant (e.g. "esriInches" or "esriCentimeters") and is used to project the map layout onto the map.
     The four pair of dimensions are in the paper units and represent (in order):
		* the overall layout size, 
		* the size of the map area in the layout, 
		* the offset of the map area from the lower left corner,
		* the left/right and top/bottom margins of the layout when no title block is shown.
	4. relativeScale - the string template to use for displaying the relative scale (e.g. "(1&quot; = [value]')" yields "(1" = 500')" for an absolute 
     scale of 1:6,000).
	5. relativeScaleFactor - the multiplier to use with the absolute scale to produce the relative scale (e.g. 0.08333333 for the example above).  
	6. scalePrecision - the number of decimal places for the relative scale (e.g. 1" = 1.5 miles reflects a value of 1 and 1" = 1.50 miles reflects a value of 2).
	7. mapScales - an array of the absolute scales that determines the tick locations (and labels) on the map scale slider.  Any scale can be 
     entered into the map scale input box.  
	8. outWkid - the WKID of the Spatial Reference to use for the printed map.
	9. showLayout - a boolean value that determines whether the layout template will be displayed over the map as a red graphic.
* Enjoy!

## Customize:
* Edit the PrintPlus\config.json file to customize the widget.

## TO DO:
* This widget has not been setup for easy configuration in AWAB yet.  The config.json file has to be edited manually.

## Change log:
* 6/3/2014
	1. Initial Commit.
