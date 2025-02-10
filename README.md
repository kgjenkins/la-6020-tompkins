# ArcGIS Pro workshop for LA 6020, focusing on Tompkins County

Workshop 2025-02-10 by Keith Jenkins, GIS Librarian at Mann Library, Cornell University. \
This document is online at: <https://kgjenkins.github.io/la-6020-tompkins/>

For help after this workshop, contact me at kgj2@cornell.edu  
Or set up a Zoom appointment at <https://guides.library.cornell.edu/gis/help>

All the data and documentation for this workshop can be downloaded from: \
<https://github.com/kgjenkins/la-6020-tompkins/archive/main.zip>

After downloading the zip file, be sure to UNZIP it!  (Right-click > Extract All)


# Loading data into ArcGIS Pro

- Shapefiles: drag the .shp file onto the map
- Geopackage: Map menu > Add data > browse to .gpkg file and select layer
- GeoTIFF: drag the .tif file onto the map
- GTFS: use the "GTFS Shapes to Features" tool for route lines
    or the "GTFS Stops to Features" tool for stop points

Set the symbology as desired:
- Double-click the symbol in the Contents pane to open the symbology panel
- There are many options!  Use the back arrow at top of symbology panel to get back to the top level

Show labels when needed:
- Right-click the layer > Labels (to toggle on/off)
- Right-click the layer > Label Properties
    - Set the "Expression" to control what information is displayed
    - Set the "Symbol" to control how it is displayed

For the traffic data, you'll want to label with the "aadt" field (Annual Average Daily Traffic)


# Making a subset of features

- Map menu > Select
- Click to select first feature, shift-click to add additional features to the selection
- Right-click the layer to export from > Data > Export Features
    - Save as a layer in your geodatabase, or to an independent shapefile


# Measuring distances

- Straight-line distances: Map menu > Measure tool
- Network distance (along a road network): Analysis menu > Network Analysis > Route
    - Select "Stops" layer
    - Route Layer menu > Create Features (or import stops from an existing layer)
    - Estimate Credits, then Run
- Service areas: Analysis menu > Network Analysis > Service Area
    - Select "Facilities" layer
    - Service Area Layer menu > Create features (or import from existing layer)
    - Estimate Credits, then Run

If importing points from an existing layer, note that you can make a selection of points and just import those.


# Calculating road slope

- Load the roads and elevation data
- Geoprocessing tool "Add Surface Information"
- Try adding labels for "Avg_Slope", and set the symbology to graduated colors based on "Avg_Slope"


# Data Sources

- Elevation: <https://cugir.library.cornell.edu/catalog/cugir-009096> (1 arcsec = 30m pixels)
    - see also <https://cugir.library.cornell.edu/catalog/cugir-009000> (1/3 arcsec = 10m pixels)
    - see also <https://gis.ny.gov/nys-dem#nys-high-resolution-dem> (1m pixels)
- Land Use: <https://tcdata-tompkinscounty.opendata.arcgis.com/datasets/tompkinscounty::tompkins-county-natural-resources-inventory-old/about?layer=24>
- Parcels: <https://tcdata-tompkinscounty.opendata.arcgis.com/datasets/tompkinscounty::parcels-public/about>
- Roads: <https://gis.ny.gov/streets-addresses#nys-streets-data>
- Tourism: OpenStreetMap data via <https://export.hotosm.org/v3/>
- Traffic: <https://nysdottrafficdata.drakewell.com/publicmultinodemap.asp>
- Trails: <https://tcdata-tompkinscounty.opendata.arcgis.com/datasets/tompkinscounty::trails-2020/about>
- Transit: <https://www.transit.land/feeds/f-dr997-tompkinsconsolidatedareatransit>

