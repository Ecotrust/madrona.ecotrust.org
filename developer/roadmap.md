---
layout: page
title: madrona spatial planning framework
active: experience
---
# Version 4.1

* More robust **user-agent parsing**. 
* Integrate **raster stats** more closely with polygon features; a get_raster_stats(rastername) method
* Improved **shapefile import** including field mapping, validation, and multi-feature uploads
* Improvements to **test coverage** and continuous integration.

# Version 4.2

* Simple **point drag-drop widget** for inputing point geometries (from the bioregions app)
* **Layer manager** to organize KML base data layers. 
* An **admin dashboard** for analyzing site usage.
* Asynchronous **notification system** to allow messaging the user in real-time without polling.

# Version 5.0 

* Complete **2D interface** 
                          
    * Autoconfigures based on workspace
    * Full CRUD capabilities and REST API integration 
    * GeoJSON driven
    * OpenLayers map interface with Tree-view feature list. 
    * Ability to author base map tiles and interactivity layers (UTFGrids) using Tilemill

# Other functionality under consideration 

* ArcGIS Server Rest API intgration
* Marxan integration for conservation priorities (currently implemented in the aquatic priorities tool)
* Geosearch: a search interface which searches local features database as well as external geocoding services
* Internationalization and localization