Open Plant Hardiness Zones (OPHZ)
===

OPHZ is free and open raster and vector data derived from the public domain map images available at http://planthardiness.ars.usda.gov/

In the [original public domain PDF map](http://planthardiness.ars.usda.gov/PHZMWeb/Images/All_states_halfzones_poster_rgb_300dpi.pdf) (305MB!), there are some gaps due to rivers, borders, and coastlines.  Most of these gaps have been filled with the nearest values.

OPHZ currently covers the 48 contiguous US states (US48), and is available in the following formats:
* **shp/ophz.shp** - national polygon shapefile
* **geojson/\*.geojson** - polygon geojson files (one for each state)
* **topojson/\*.topojson** - national topojson file
* **tif/ophz-us48.tif** - geotiff raster.  Each colored pixel of the original map image has been translated to a value representing lower end of the corresponding zone's temperature range.  Most gaps have been filled with the nearest data value.
* **tif/ophz-alpha-us48.tif** - for those who want the original, unfilled raster with no interpolation of nodata values.  International borders, coastlines, and a few major rivers appear as -98.  Open water is -99.

All vector formats are in WGS84 (EPSG:4326), and the raster formats are in the original Albers projection (EPSG:5070).

![ophz](ophz.png)

