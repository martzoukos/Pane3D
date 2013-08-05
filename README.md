Pane3D
==========

Pane3D is a jQuery plugin that creates a zoomable three dimensional interface from a simple HTML structure. If the browser is not capable of running CSStransforms or the programmer decides to now use it, the interface falls back to a nice full width/height panel, that's easily editable as a normal 2D site.
Based on David Desandro's http://2011.beercamp.com/ site.


## Directions:
1. Include the following dependencies:
	* jQuery (tested with 1.10 but older version should not have a problem)
	* modernizr
	* jquery.pane3D.js or jquery.pane3D.min.js
2. Set your HTML up:
    * Just keep the 3 level structure with the .panes-environment -> .panes-container -> .pane (multiple).
    * **You only need to keep the classes**, you can add any ID you want, you can add any content inside them, you can wrap them in another div.
3. Call the script:
	* Call the Pane3D function on the ".panes-environment" DOM Node, like that: **$(".panes-environment").pane3D();**
	* Configuration options include:
		* onLevelChange(currentPane): callback function that runs whenever the current pane is changed and this specific DOM Node is returned as a parameter
		* perspective: it's a number that defines the perspective of the 3D space. More info: http://desandro.github.io/3dtransforms/docs/perspective.html. (default value: 400)
		* perspectiveOrigin: It defines the vanishing point of the 3D space. More info: http://desandro.github.io/3dtransforms/docs/perspective.html. (default value: "center")
		* spacing: The Z distance between the panes, in pixels (default value: 1000)

## Demo Page:
http://www.martzoukos.com/wp-content/uploads/misc/personal/Pane3D/index.html