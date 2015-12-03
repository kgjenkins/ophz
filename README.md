Open Plant Hardiness Zones (OPHZ)
===

![ophz](ophz.png)

_OPHZ-C is the most-current flavor - it is recommended you start there_

OPHZ is free and open raster and vector data derived from the public domain map images available at:
    http://planthardiness.ars.usda.gov/

The data is available in different flavors, each representing a different level of processing.

* **PHZM-US48** is the original PDF (in an Albers Conical Equal Area projection), downloaded from
    http://planthardiness.ars.usda.gov/PHZMWeb/Images/All_states_halfzones_poster_rgb_300dpi.pdf

* **OPHZ-A** is a raster of data values, where each colored pixel of PHZM-US48 has been translated to a value representing lower end of each zone's temperature range.  Labels, state boundaries, and the elevation hillshade have been removed, although international borders, coastlines, and a few major rivers appear as -98.  Open water is -99.  This raster is currently limited to the 48 contiguous US states (US48).

* **OPHZ-B** is identical to OPHZ-A, except that international borders and coastlines have been filled with the nearest data values.  This is particularly useful for regions such as the lovely crinkly edges of Maine.

* **OPHZ-C** Fills riverways and splits the dataset by state, though the CONUS full dataset is available here as well. All subsets here are in WGS84
