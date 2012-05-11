---
layout: page
title: madrona spatial planning framework   
---
<div class="row">
	<div class="span8">
		<h2>Philosophy</h2>
		<p>Madrona was created to make lots of choices out of the box for you while providing lots of options, so you can get to the fun part of building tools right away.  You, the web programmer, are still required to make many choices about your application and Madrona gives you the building blocks you need to piece together your mental model of the problem quickly without getting distracted by the nuts and bolts.  Still, there is no way for any framework to think through the problem for you.  Madrona is the path not the destination.</p>
		<h3>The Zen of Madrona</h3>
		<ul>
		    <li>Capture the mental model of your decision-making process.</li>
		    <li>Let the mental model define which Features and Links are needed.</li>
		    <li>The Features and Links will then define the REST API.</li>
		    <li>The REST API and its workspace document will drive the client interface.</li>
		    <li>Let these conventions be your guide but they should get out of the way when no longer useful.</li>
		    <li>Don’t worry about creating new functionality as a one-off but if you reuse it, then consider generalizing it to a core feature.</li>
		</ul>

		<h2>Significant Features</h2>
		<p>These are the key building blocks of Madrona.  Most are some combination of Use only what you need.</p>
		<h3>Spatial Features</h3>
		<ul>
		    <li>Links - Generic views/urls to perform create, read, update, delete, conversion, copying, sharing, etc.(creating, reading, editing, updating, downloading, copying, sharing, etc)</li>
		    <li>Shareable</li>
		    <li>User-created</li>
		    <li>typically discrete geometries but always represented as KML or GeoJSON</li>
		    <li>Collection - contain other features or collections. have their own behaviors, etc</li>
		</ul>
		<h3>Data layers</h3>
		KML data layers - http://ecotrust.github.com/madrona/docs/layers.html
		<h3>Content Management</h3>
		Flatblocks
		<h3>Collaboration</h3>
		<h3>Flexible Analysis</h3>
		The analysistools module provides a toolkit to standardize interaction with external modeling/analysis software.  http://ecotrust.github.com/madrona/docs/analysistools.html
		<h3>Study Regions</h3>
		We designed the study region concept as a central component of marinemap/madrona implementations. It is used by default manipulators and to zoom the initial map view. If you want to implement custom zooming mechanisms or custom manipulators, those will occur as customizations at the project code level.  http://ecotrust.github.com/madrona/docs/studyregion.html
		<h3>Manipulators</h3>
		<p>There are many cases in which a user-defined geometry needs to be modified or cleaned by an automated process. This process can be initiated the user as a tool or context action, or as part of the initial creation of a new feature. Typically, the user is provided an opportunity to review any changes made to their geometry.  Individual manipulators can be applied in series producing the desired output.  Use cases might include:</p>
		<ul>
		    <li>Clipping a shape to your study region</li>
		    <li>Clipping a shape to the shoreline</li>
		    <li>Clipping out exclusion areas</li>
		</ul>

		<p>http://ecotrust.github.com/madrona/docs/manipulators.html</p>
		<h3>Import/Export</h3>
		<p>Import and export common spatial formats.  You don’t want your tool to be a black box.  Integrates the workflows you have in other GIS and modeling environments.</p>

		http://ecotrust.github.com/madrona/docs/loadshp.html
		http://ecotrust.github.com/madrona/docs/export.html
		<h3>Asynchronous Tasking</h3>
		<h3>Custom Projections</h3>

		<h3>2D and 3D Support</h3>
		<h3>Raster Statistics</h3>
		<p>The raster_stats app allows you to analyze raster datasets based on a polygon geometry. For example, for a given polygon, you may want to know the average elevation or the maximum temperature, etc. Essentially this performs a vector-on-raster intersection.  The app uses an optional caching mechanism so that any geometry/raster combination only needs to be run once.</p>

		http://ecotrust.github.com/madrona/docs/raster_stats.html
		<h2>Architecture</h2>
		<h3>Core Libraries</h3>
		<h4>Django</h4>
		<h4>PostGIS</h4>
		<h4>GDAL/OGR</h4>
		<p>Work with any of the wide range of data formats and databases supported by GDAL and OGR including shapefiles, KML, GeoJSON, CouchDB, Spatialite, Google Fusion Tables, GeoTiff, ESRI Grid, ESRI Geodatabase, Excel, CSV, etc.</p>
		<h3>REST API</h3>
		<p>Defined bahavior, methods and relationships with other data</p>
		<h4>KML</h4>
		<h4>GeoJSON</h4>
		<h3>Caching</h3>
		<h3>Reporting</h3>
		<h3>Workspace Document</h3>
		<p>Actions [Links] (creating, reading, editing, updating, downloading, copying, sharing, etc)</p>
		<h3>Helpers</h3>
		<ul>
		    <li>Raster Stats</li>
		    <li>Manipulators</li>
		    <li>Async</li>
		    <li>Study Region</li>
		    <li>Public and private data layers</li>
		</ul>
		<h3>Client Widgets</h3>
		<h4>KmlTree</h4>
		<h4>KmlEditor</h4>
		<h3>Potential Software Stacks</h3>
		<p>All options require the client working with the workspace document.</p>
		<h4>Madrona/Google Earth Web Plugin/JQuery</h4>
        <ul>
	        <li>3D Mapping</li>
	        <li>KML-driven</li>
	        <li>KmlTree</li>
	        <li>KmlEditor</li>
	    </ul>
		
		<h4>Madrona/2DMap/MapBox</h4>
	    <p>Map Publishing</p>
	            <ul>
	            	<li>Create using TileMill</li>
	            	<li>Publish online using TileStream or hosted service</li>
	            	<li>Reference in datalayers app</li>
	           	</ul>
	    <p>2D Mapping Client</p>
            <ul>
            	<li>OpenLayers if you need complex drawing capabilities</li>
                <li>Leaflet</li>
                <li>Google Maps</li>
           	</ul>
        <p>GeoJSON-driven</p>
        <p>Use the Madrona GeoJSON support in feature API</p>
        <h4>UTF-Grid</h4>
            <p>Leaflet and OpenLayers both supported</p>
	    <h4>Madrona/OpenLayers/GeoExt/GeoServer</h4>
	        <p>Could use OpenGeo Studio</p>
	    <h4>Madrona/SenchaTouch/OpenLayers (mobile app)</h4>
	        <p>http://openlayers.org/dev/examples/mobile-sencha.html</p>

		<h2>Third-party Integration</h2>
		<h3>Modeling/Analysis</h3>
		<ul>
		    <li>FVS</li>
		    <li>Marxan</li>
		    <li>Grass</li>
		    <li>ArcServer REST API</li>
		    <li>ArcPy</li>
		</ul>
		<h3>Mapservers</h3>
		    <h4>GeoServer</h4>
		        <ul>
		        	<li>WMS</li>
    		        <li>WFS</li>
    		        <li>WPS/Geoprocessing</li>
    		   	</ul>
		    <h4>Mapnik</h4>
		        <ul>
		        	<li>staticmap</li>
		        <li>WMS</li></ul>
		<h3>Client-side Mapping</h3>
	    <h4>Google Earth Web Plugin</h4>
	        <p>Extensive support</p>
	    <h4>OpenLayers</h4>
	        <p>Feature layer</p>
	    <h4>Leaflet</h4>
	        <p>Feature layer</p>
	    <h4>GeoExt</h4>
	        <p>GeoJson feature layer</p>

		<h3>Visualization</h3>
		    <h4>D3</h4>
		        <p>Choropleth - http://mbostock.github.com/d3/ex/choropleth.html</p>
		    <h4>JQPlot</h4>
		<h2>Platforms</h2>

		    <h3>ESRI</h3>
		        <ul>
		        	<li>ArcServer Rest API</li>
		        	<li>WMS</li>
		        	<li>KML</li>
		        </ul>
		    <h3>MapBox</h3>
		        <ul>
		        	<li>Use TileMill for creating your data layers.</li>
		        	<li>Link to them using datalayers app</li>
		        	<li>Make them available on your map (Leaflet/OpenLayers)</li>
		        </ul>
		    <h3>OpenGeo Studio</h3>
		        See Geoserver
		        See GeoExt
		    <h3>CartoDB</h3>
		        Can complement each other... integration is not totally clear
		        Could be installed together on the same system. https://github.com/Vizzuality/cartodb 

		<h2>Deployment</h2>
		<p>Anywhere Python and WSGI is supported</p>
		<h3>Linux</h3>
		<p>Point at instructions</p>
		<h3>Windows</h3>
		<p>https://docs.djangoproject.com/en/dev/ref/contrib/gis/install/#windows</p>
		<h3>Cloud-based Hosting</h3>
	</div>
	<div class="span4">
		<div class="row">
			<ul class="thumbnails pull-right">
				<li class="span4"><a class="thumbnail"><img alt="" src="http://placehold.it/360x268"></a></li>
			</ul>
		</div>
		<div class="row">
			<h3>Content</h3>
			<div id="accordion2" class="accordion">
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseOne" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  Philosophy
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseOne" style="height: 0px;">
	                <div class="accordion-inner">
	                  Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
	                </div>
	              </div>
	            </div>
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseTwo" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  Significant Features
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseTwo" style="height: 0px;">
	                <div class="accordion-inner">
	                  Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
	                </div>
	              </div>
	            </div>
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseThree" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  Architecture
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseThree">
	                <div class="accordion-inner">
	                  Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
	                </div>
	              </div>
	            </div>
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseThree" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  Deployment
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseThree">
	                <div class="accordion-inner">
	                  Anim pariatur cliche reprehenderit, enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch. Food truck quinoa nesciunt laborum eiusmod. Brunch 3 wolf moon tempor, sunt aliqua put a bird on it squid single-origin coffee nulla assumenda shoreditch et. Nihil anim keffiyeh helvetica, craft beer labore wes anderson cred nesciunt sapiente ea proident. Ad vegan excepteur butcher vice lomo. Leggings occaecat craft beer farm-to-table, raw denim aesthetic synth nesciunt you probably haven't heard of them accusamus labore sustainable VHS.
	                </div>
	              </div>
	            </div>
	      </div>
		</div>
	</div>
</div>