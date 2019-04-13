Leaflet.FileLayer (with MapLayer Support)
=================

Forked from https://github.com/makinacorpus/Leaflet.FileLayer

Loads local files (GeoJSON, JSON, GPX, KML, MapLayer) into the map using the [HTML5 FileReader API](http://caniuse.com/filereader), **without server call** !


Does everything the original does - so see  https://github.com/makinacorpus/Leaflet.FileLayer for details, 
but adds support for loading `.maplayer` definition files. So for example users can load a file that adds a dynamic layer to the map. 

For example

    {
    	"name": "OpenRailwayMap - Standard",
    	"type": "overlay",
    	"url": "https://{s}.tiles.openrailwaymap.org/standard/{z}/{x}/{y}.png", 
    	"attribution": "Rendering: <a href=https://www.openrailwaymap.org/>OpenRailwayMap</a>"
    }

could be saved as `OpenRailwayMap.maplayer` and when uploaded, would render https://www.OpenRailwayMap.org/ tiles as a new layer on map (using L.TileLayer)

(Full definition of .maplayer files to follow!)


... currently supports basic `L.TileLayer` layers, support for more like, WMS, ImageOverlay and 'AJAX' vector layers expected soon!







Authors
-------

[![Makina Corpus](http://depot.makina-corpus.org/public/logo.gif)](http://makinacorpus.com)

Contributions

* Barry Hunter
* Mathieu Leplatre
* Joey Baker http://byjoeybaker.com
* CJ Cenizal
* Jens-duttke
* Jmuccigr
* Matthew Mueller
* George Silva
* Simon Bats
* Opoto
* Lachlan Phillips
* kkdd


