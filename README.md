Open Plant Hardiness Zones (OPHZ)
===

OPHZ is free and open raster and vector data derived from the public domain map images available at http://planthardiness.ars.usda.gov/

In the [original public domain PDF map](http://planthardiness.ars.usda.gov/PHZMWeb/Images/All_states_halfzones_poster_rgb_300dpi.pdf), there are some gaps due to rivers, borders, and coastlines.  Many of these gaps have been filled with the nearest values.

OPHZ is available in the following formats:

* **shp/ophz.shp** - polygon shapefile, in WGS84 coordinates
* **geojson/\*.geojson** - polygon geojson, in WGS84 coordinates, separate files for each state
* **tif/ophz-us48.tif** - GeoTIFF raster covering the 48 contiguous US states, in Albers projection (EPSG:5070).  Each colored pixel of the original map image has been translated to a value representing lower end of each zone's temperature range.
* **tif/ophz-alpha-us48.tif** -- original "alpha" version of the OPHZ raster, before any filling of pixels where zone data was missing due to rivers, borders, or coastlines.  International borders, coastlines, and a few major rivers appear as -98.  Open water is -99.

![ophz](ophz.png)

## Rendered map
Using d3js, [viewable here](http://wboykinm.github.io/ophz/map/).
