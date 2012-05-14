---
layout: page
title: madrona spatial planning framework
active: technology  
---
<div class="row">
	<div class="span8">

		<h2>Philosophy</h2>
		<p>Madrona makes many choices for you while still providing lots of options, so you can get to the fun part of building tools right away.  You, the web developer, are still required to make many choices about your application and Madrona gives you building blocks to piece together the mental model of your solution quickly without getting distracted by the nuts and bolts.</p>
		
		<a name="zen"> </a>
		<h3>The Zen of Madrona</h3>

		<ul>
		    <li>The right decision-making process will vary by geography and culture.</li>
		    <li>Work directly with the intended users to capture the mental model of your decision-making process.</li>
		    <li>Let the mental model define which Features and Links are needed.</li>
		    <li>The Features and Links will then define the REST API.</li>
		    <li>The REST API and its workspace document will drive the client interface.</li>
		    <li>Let these conventions be your guide but they should get out of the way when no longer useful.</li>
		</ul>

		<h2>Significant Features</h2>
		<p>Madrona features can be mixed and matched to meet your unique needs.  Be sure to look at some of the many Madrona-based tools to see what’s possible.</p>

		<div class="pull-right">
			<img src="{{BASE_PATH}}/assets/img/technology/madrona_outline.png"/>
		</div>
		<a name="spatial_features"> </a>
		<h3>Spatial Features</h3>
		<p>Provides a spatial content management system complete with an API and full CRUD operations.  Define new types of features (point, line, polygon) that are unique to your needs (e.g. wind energy sites, bike paths, event locations).  Then let users sketch, copy and share them.  <a href="http://ecotrust.github.com/madrona/docs/features.html">Learn More</a></p>

		<a name="feature_manipulators"> </a>
		<h3>Feature Manipulators</h3>
		<p>Features sketched by users often need to be modified or cleaned and manipulators provide a workflow for doing that.  Example manipulators include clipping a feature to your study region or clipping out exclusion areas. <a href="http://ecotrust.github.com/madrona/docs/manipulators.html">Learn More</a></p> 

		<a name="import_export"> </a>
		<h3>Import/Export</h3>
		<p>You don’t want your tool to be a black box and you want it to integrate with external workflows.  Allow your users to import and export their Features in common spatial formats including KML, GeoJSON and Shapefiles. <a href="http://ecotrust.github.com/madrona/docs/loadshp.html">Learn More</a></p> 

		<a name="map_bookmarks"> </a>
		<h3>Map Bookmarks</h3>
		<p>Allow the user to take a snapshot of their map view including the data layers and features they had turned on.  Manage bookmarks as any other Feature and share them as links with other people. (Google Earth only currently) <a href="http://ecotrust.github.com/madrona/docs/bookmarks.html ">Learn More</a></p>

		<a name="study_regions"> </a>
		<h3>Study Regions</h3>
		<p>Focus the user’s attention on a specific geographic region and then create or limit user actions specific to that region. <a href="http://ecotrust.github.com/madrona/docs/bookmarks.html">Learn More</a></p>

		<a name="data_layers"> </a>
		<h3>Data Layers</h3>
		<p>Manage a hierarchy of data layers important to your decision-making process and provide fine-grained access for viewing.  Also let users upload their own data layers. (KML support only currently).<a href="http://ecotrust.github.com/madrona/docs/layers.html">Learn More</a></p>

		<a name="content_management"> </a>
		<h3>Content Management</h3><p>Allow site administrators to manage and edit blocks of content within pages.<a href="http://ecotrust.github.com/madrona/docs/flatblocks.html">Learn More</a></p>

		<a name="reports"> </a>
		<h3>Reports</h3>
		<p>???? Is this a feature?<a href="#">Learn More</a></p>

		<a name="flexible_analysis"> </a>
		<h3>Flexible Analysis</h3>
		<p>Interact with external modeling and analysis software in a standardized way.  Allows you to define inputs and capture outputs as Features.<a href="http://ecotrust.github.com/madrona/docs/analysistools.html">Learn More</a></p>

		<a name="asynchronous_tasking"> </a>
		<h3>Asynchronous Tasking</h3>
		<p>Analysis can take a lot of time and system resources.  Users should be able to do other things while they are waiting.  Run processes in the background and get notified when they finish. <a href="http://ecotrust.github.com/madrona/docs/async.html">Learn More</a></p>

		<a name="static_maps"> </a>
		<h3>Static Maps</h3>
		<p>Create static map images that include user defined shapes and other features.
		<a href="http://ecotrust.github.com/madrona/docs/staticmap.html">Learn More</a></p>

		<a name="custom_projections"> </a>
		<h3>Custom Projections</h3>
		<p>Use one of the thousands of projections available with Proj.4 or define your own.
		<a href="http://ecotrust.github.com/madrona/docs/custom_projection.html">Learn More</a></p>

		<a name="raster_stats"> </a>
		<h3>Raster Statistics</h3>
		<p>Quickly calculate statistics for a polygon Feature such as the average elevation or maximum temperature using raster data layers.  Provides an optional caching mechanism.<a href="http://ecotrust.github.com/madrona/docs/raster_stats.html">Learn More</a></p>

		<h2>Architecture</h2>
		<ul>
	        <li><a href="https://www.djangoproject.com/">Django</a></li>
	        <li><a href="http://geodjango.org/">GeoDjango</a></li>
	        <li><a href="http://postgis.refractions.net/">PostGIS</a></li>
	        <li><a href="http://mapnik.org/">Mapnik</a></li>
	        <li><a href="http://jquery.com/">JQuery</a></li>
	        <li><a href="https://developers.google.com/earth/">Google Earth Plugin</a></li>
	        <li><a href="http://code.google.com/p/earth-api-utility-library/">Google Earth API Util</a></li>
	        <li><a href="http://code.google.com/p/kmltree/">KmlTree</a></li>	        
	    </ul>		
		<a name="core_libraries"> </a>
		<h3>Core Libraries</h3>
		<h4>Django</h4>
		<h4>PostGIS</h4>
		<h4>GDAL/OGR</h4>
		<p>Work with any of the wide range of data formats and databases supported by GDAL and OGR including shapefiles, KML, GeoJSON, CouchDB, Spatialite, Google Fusion Tables, GeoTiff, ESRI Grid, ESRI Geodatabase, Excel, CSV, etc.</p>
		<a name="rest_api"> </a>
		<h3>REST API</h3>
		<p>Defined bahavior, methods and relationships with other data</p>
		<h4>KML</h4>
		<h4>GeoJSON</h4>
		<a name="caching"> </a>
		<h3>Caching</h3>
		<a name="reporting"> </a>
		<h3>Reporting</h3>
		<a name="workspace_document"> </a>
		<h3>Workspace Document</h3>
		<p>Actions [Links] (creating, reading, editing, updating, downloading, copying, sharing, etc)</p>
		<a name="helpers"> </a>
		<h3>Helpers</h3>
		<ul>
		    <li>Raster Stats</li>
		    <li>Manipulators</li>
		    <li>Async</li>
		    <li>Study Region</li>
		    <li>Public and private data layers</li>
		</ul>
		<a name="client_widgets"> </a>
		<h3>Client Widgets</h3>
		<h4>KmlTree</h4>
		<h4>KmlEditor</h4>
		<a name="stacks"> </a>
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
	    <a name="third-party"> </a>
		<h3>Third-party Integration</h3>
		<a name="modeling_analysis"> </a>
		<h3>Modeling/Analysis</h3>
		<ul>
		    <li>FVS</li>
		    <li>Marxan</li>
		    <li>Grass</li>
		    <li>ArcServer REST API</li>
		    <li>ArcPy</li>
		</ul>
		<a name="mapservers"> </a>
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
		<a name="client_side_mapping"> </a>
		<h3>Client-side Mapping</h3>
	    <h4>Google Earth Web Plugin</h4>
	        <p>Extensive support</p>
	    <h4>OpenLayers</h4>
	        <p>Feature layer</p>
	    <h4>Leaflet</h4>
	        <p>Feature layer</p>
	    <h4>GeoExt</h4>
	        <p>GeoJson feature layer</p>
	    <a name="visualization"> </a>
		<h3>Visualization</h3>
		    <h4>D3</h4>
		        <p>Choropleth - http://mbostock.github.com/d3/ex/choropleth.html</p>
		    <h4>JQPlot</h4>
		<a name="platforms"> </a>
		<h3>Platforms</h3>

		    <h4>ESRI</h4>
		        <ul>
		        	<li>ArcServer Rest API</li>
		        	<li>WMS</li>
		        	<li>KML</li>
		        </ul>
		    <h4>MapBox</h4>
		        <ul>
		        	<li>Use TileMill for creating your data layers.</li>
		        	<li>Link to them using datalayers app</li>
		        	<li>Make them available on your map (Leaflet/OpenLayers)</li>
		        </ul>
		    <h4>OpenGeo Studio</h4>
		        See Geoserver
		        See GeoExt
		    <h4>CartoDB</h4>
		        Can complement each other... integration is not totally clear
		        Could be installed together on the same system. https://github.com/Vizzuality/cartodb 

		<h2>Deployment</h2>
		<p>Anywhere Python and WSGI is supported</p>
		<a name="linux"> </a>
		<h3>Linux</h3>
		<p>Point at instructions</p>
		<a name="windows"> </a>
		<h3>Windows</h3>
		<p>https://docs.djangoproject.com/en/dev/ref/contrib/gis/install/#windows</p>
		<a name="cloud"> </a>
		<h3>Cloud-based Hosting</h3>
	</div>
	<div class="span4">
		<div class="row">
			<div id="accordion2" class="accordion">
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseOne" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  <h3>Philosophy</h3>
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseOne" style="height: 0px;">
	                <div class="accordion-inner">
	                  <ul class="unstyled">
	                  	<li><a href="#zen">The Zen of Madrona</a></li>
	                  </ul>
	                </div>
	              </div>
	            </div>
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseTwo" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  <h3>Significant Features</h3>
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseTwo" style="height: 0px;">
	                <div class="accordion-inner">
	                  <ul class="unstyled">
		                  <li><a href="#spatial_features">Spatial Features</a></li>
		                  <li><a href="#data_layers">Data layers</a></li>
		                  <li><a href="#content_management">Content Management</a></li>
		                  <li><a href="#collaboration">Collaboration</a></li>
		                  <li><a href="#flexible_analysis">Flexible Analysis</a></li>
		                  <li><a href="#study_regions">Study Regions</a></li>
		                  <li><a href="#manipulators">Manipulators</a></li>
		                  <li><a href="#import_export">Import/Export</a></li>
		                  <li><a href="#asynchronous_tasking">Asynchronous Tasking</a></li>
		                  <li><a href="#custom_projections">Custom Projections</a></li>
		                  <li><a href="#2d_3d_support">2D and 3D Support</a></li>
		                  <li><a href="#raster_statistics">Raster Statistics</a></li>
		              </ul>
	                </div>
	              </div>
	            </div>
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseThree" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  <h3>Architecture</h3>
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseThree">
	                <div class="accordion-inner">
		            <ul class="unstyled">
		                 <li><a href="#core_libraries">Core Libraries</a></li>
		                 <li><a href="#rest_api">REST API</a></li>
		                 <li><a href="#caching">Caching</a></li>
		                 <li><a href="#reporting">Reporting</a></li>
		                 <li><a href="#workspace_document">Workspace Document</a></li>
		                 <li><a href="#helpers">Helpers</a></li>
		                 <li><a href="#client_widgets">Client Widgets</a></li>
		                 <li><a href="#stacks">Potential Software Stacks</a></li>
		                 <li><a href="#third-party">Third-party Integration</a></li>
		                 <li><a href="#modeling_analysis">Modeling/Analysis</a></li>
		                 <li><a href="#mapservers">Mapservers</a></li>
		                 <li><a href="#client_side_mapping">Client-side Mapping</a></li>
		                 <li><a href="#visualization">Visualization</a></li>
		                 <li><a href="#platforms">Platforms</a></li>
		             </ul>
	                </div>
	              </div>
	            </div>
	            <div class="accordion-group">
	              <div class="accordion-heading">
	                <a href="#collapseFour" data-parent="#accordion2" data-toggle="collapse" class="accordion-toggle">
	                  <h3>Deployment</h3>
	                </a>
	              </div>
	              <div class="accordion-body collapse" id="collapseFour">
	                <div class="accordion-inner">
	                  <ul class="unstyled">
	                  	<li><a href="#linux">Linux</a></li>
	                  	<li><a href="#windows">Windows</a></li>
	                  	<li><a href="#cloud">Cloud-based Hosting</a></li>
	                  </ul>
	                </div>
	              </div>
	            </div>
	      </div>
		</div>
	</div>
</div>
<script>
window.onload = function () {
	var timer, $accordion = $('#accordion2');
		initial = $accordion.offset().top,
		scrollHandler = function () {  
			var scrollTop = $(window).scrollTop(),
				offset = $accordion.offset().top;
			
			if (scrollTop > offset + 100) {
				$accordion.offset({ top: scrollTop + 100 });
			}  else {
			  	$accordion.offset({ top: scrollTop > initial? scrollTop + 100: initial });
			}
		}
	scrollHandler();
	$(window).scroll(function () {
		if (timer) {
			clearTimeout(timer);
		}
		timer = setTimeout(scrollHandler, 20);
	});
};
</script>