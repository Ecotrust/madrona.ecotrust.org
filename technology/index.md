---
layout: page
title: madrona spatial planning framework
tagline: 
---
<div class="row">
	<div class="span8">
		Philosophy
		Madrona was created to make lots of choices out of the box for you while providing lots of options, so you can get to the fun part of building tools right away.  You, the web programmer, are still required to make many choices about your application and Madrona gives you the building blocks you need to piece together your mental model of the problem quickly without getting distracted by the nuts and bolts.  Still, there is no way for any framework to think through the problem for you.  Madrona is the path not the destination.
		The Zen of Madrona

		    Capture the mental model of your decision-making process.
		    Let the mental model define which Features and Links are needed.
		    The Features and Links will then define the REST API.
		    The REST API and its workspace document will drive the client interface
		    Let these conventions be your guide but they should get out of the way when no longer useful.
		    Don’t worry about creating new functionality as a one-off but if you reuse it, then consider generalizing it to a core feature.


		Visit the Madrona Knowledge Base to learn more
		Significant Features
		These are the key building blocks of Madrona.  Most are some combination of Use only what you need.
		Spatial Features

		    Links - Generic views/urls to perform create, read, update, delete, conversion, copying, sharing, etc.(creating, reading, editing, updating, downloading, copying, sharing, etc)
		    Shareable
		    User-created
		    typically discrete geometries but always represented as KML or GeoJSON
		    Collection - contain other features or collections. have their own behaviors, etc

		Data layers
		KML data layers - http://ecotrust.github.com/madrona/docs/layers.html
		Content Management
		Flatblocks
		Collaboration
		Flexible Analysis
		The analysistools module provides a toolkit to standardize interaction with external modeling/analysis software.  http://ecotrust.github.com/madrona/docs/analysistools.html
		Study Regions
		We designed the study region concept as a central component of marinemap/madrona implementations. It is used by default manipulators and to zoom the initial map view. If you want to implement custom zooming mechanisms or custom manipulators, those will occur as customizations at the project code level.  http://ecotrust.github.com/madrona/docs/studyregion.html
		Manipulators
		There are many cases in which a user-defined geometry needs to be modified or cleaned by an automated process. This process can be initiated the user as a tool or context action, or as part of the initial creation of a new feature. Typically, the user is provided an opportunity to review any changes made to their geometry.  Individual manipulators can be applied in series producing the desired output.  Use cases might include:

		    Clipping a shape to your study region
		    Clipping a shape to the shoreline
		    Clipping out exclusion areass


		http://ecotrust.github.com/madrona/docs/manipulators.html
		Import/Export
		Import and export common spatial formats.  You don’t want your tool to be a black box.  Integrates the workflows you have in other GIS and modeling environments.

		http://ecotrust.github.com/madrona/docs/loadshp.html
		http://ecotrust.github.com/madrona/docs/export.html
		Asynchronous Tasking
		Custom Projections

		2D and 3D Support
		Raster Statistics
		The raster_stats app allows you to analyze raster datasets based on a polygon geometry. For example, for a given polygon, you may want to know the average elevation or the maximum temperature, etc. Essentially this performs a vector-on-raster intersection.  The app uses an optional caching mechanism so that any geometry/raster combination only needs to be run once.

		http://ecotrust.github.com/madrona/docs/raster_stats.html
		Architecture
		Core Libraries
		Django
		PostGIS
		GDAL/OGR
		Work with any of the wide range of data formats and databases supported by GDAL and OGR including shapefiles, KML, GeoJSON, CouchDB, Spatialite, Google Fusion Tables, GeoTiff, ESRI Grid, ESRI Geodatabase, Excel, CSV, etc.
		REST API
		Defined bahavior, methods and relationships with other data
		KML
		GeoJSON
		Caching
		Reporting
		Workspace Document
		Actions [Links] (creating, reading, editing, updating, downloading, copying, sharing, etc)
		Helpers

		    Raster Stats
		    Manipulators
		    Async
		    Study Region
		    Public and private data layers

		Client Widgets
		KmlTree
		KmlEditor
		Potential Software Stacks
		All options require the client working with the workspace document.

		    Madrona/Google Earth Web Plugin/JQuery
		        3D Mapping
		        KML-driven
		        KmlTree
		        KmlEditor
		    Madrona/2DMap/MapBox
		        Map Publishing
		            Create using TileMill
		            Publish online using TileStream or hosted service
		            Reference in datalayers app
		        2D Mapping Client
		            OpenLayers if you need complex drawing capabilities
		            Leaflet
		            Google Maps
		        GeoJSON-driven
		            Use the Madrona GeoJSON support in feature API
		        UTF-Grid
		            Leaflet and OpenLayers both supported
		    Madrona/OpenLayers/GeoExt/GeoServer
		        Could use OpenGeo Studio
		    Madrona/SenchaTouch/OpenLayers (mobile app)
		        http://openlayers.org/dev/examples/mobile-sencha.html

		Third-party Integration
		Modeling/Analysis

		    FVS
		    Marxan
		    Grass
		    ArcServer REST API
		    ArcPy

		Mapservers

		    GeoServer
		        WMS
		        WFS
		        WPS/Geoprocessing
		    Mapnik
		        staticmap
		        WMS

		Client-side Mapping

		    Google Earth Web Plugin
		        Extensive support
		    OpenLayers
		        Feature layer
		    Leaflet
		        Feature layer
		    GeoExt
		        GeoJson feature layer

		Visualization

		    D3
		        Choropleth - http://mbostock.github.com/d3/ex/choropleth.html
		    JQPlot

		Platforms

		    ESRI
		        ArcServer Rest API
		        WMS
		        KML
		    MapBox
		        Use TileMill for creating your data layers.  Link to them using datalayers app
		        Make them available on your map (Leaflet/OpenLayers)
		    OpenGeo Studio
		        See Geoserver
		        See GeoExt
		    CartoDB
		        Can complement each other... integration is not totally clear
		        Could be installed together on the same system. https://github.com/Vizzuality/cartodb 

		Deployment
		Anywhere Python and WSGI is supported
		Linux
		Point at instructions
		Windows
		https://docs.djangoproject.com/en/dev/ref/contrib/gis/install/#windows
		Cloud-based Hosting

	</div>
	<div class="span4">
		<ul class="nav nav-list">
		</ul>
	</div>
</div>