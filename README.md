# ArcGIS Pro workshop for LA 6020, focusing on Tompkins County

Workshop 2025-02-10 by Keith Jenkins, GIS Librarian at Mann Library, Cornell University. \
This document is online at: <https://kgjenkins.github.io/la-6020-tompkins/>

For help after this workshop, contact me at kgj2@cornell.edu  
Or set up a Zoom appointment at <https://guides.library.cornell.edu/gis/help>

All the data and documentation for this workshop can be downloaded from: \
<https://github.com/kgjenkins/la-6020-tompkins/archive/main.zip>

After downloading the zip file, be sure to UNZIP it!  (Right-click > Extract All)


# Loading data into ArcGIS Pro

1. Shapefiles - drag the .shp file onto the map
2. Geopackage - Map menu > Add data > browse to .gpkg file and select layer
3. GeoTIFF - drag the .tif file onto the map
4. GTFS - use the "GTFS Shapes to Features" tool for route lines
    or the "GTFS Stops to Features" tool for stop points


# Measuring distances

1. Straight-line distances
2. Network distance (along a road network)



# Data Sources

Elevation: https://cugir.library.cornell.edu/catalog/cugir-009096 (1 arcsec = 30m pixels)
  see also https://cugir.library.cornell.edu/catalog/cugir-009000 (1/3 arcsec = 10m pixels)
  see also https://gis.ny.gov/nys-dem#nys-high-resolution-dem (1m pixels)
Land Use: https://tcdata-tompkinscounty.opendata.arcgis.com/datasets/tompkinscounty::tompkins-county-natural-resources-inventory-old/about?layer=24
Parcels: https://tcdata-tompkinscounty.opendata.arcgis.com/datasets/tompkinscounty::parcels-public/about
Roads: https://gis.ny.gov/streets-addresses#nys-streets-data
Tourism: OpenStreetMap data via https://export.hotosm.org/v3/
Traffic: https://nysdottrafficdata.drakewell.com/publicmultinodemap.asp
Trails: https://tcdata-tompkinscounty.opendata.arcgis.com/datasets/tompkinscounty::trails-2020/about
Transit: https://www.transit.land/feeds/f-dr997-tompkinsconsolidatedareatransit

