##Requirements:
* A definition list of items with a title, and description
   + title = title of info item (this will be the icon)
   + description = the actual info description (hidden until selected)


***

##How To Use:
* Add both the js/css to your page
* At document.ready script, altering any variables required (defaults are set by the plugin)
* Create <dl> with dt as the icon and title, and the dd as the info copy
* Modify css as required


***

##Example Usage:
    <script>
      $(document).ready(function(){
        $("dl.infographic_rotate").infoCircle({
          initSpeed = 5.5;
        });
      });
    </script>
    

***

##Options (and defaults):
* initSpeed: Speed of load animation (0.1-10)
* frameLength: How many milliseconds for each frame (1000/24 for 24fps is common)
* continuousSpeed: Speed of continuous animation (0.1-10)
* iconRadius: Radius of span - do not use a css border as can break things (plugin should calculate this itself using your css)
* iconZoomRadius: Radius of zoomed item (plugin should calculate this itself using your css)
* circleRadius: Radius of the circle path to use (in pixels)
* continuousEnabled: Set this to true if you want a continuous animation after initial load.  note: this can have perform,ance issues
* defaultItem: Sets a default item if greater than 0, so if after transition you want an item automatically selected, put it's number in here (otherwise set to 0)