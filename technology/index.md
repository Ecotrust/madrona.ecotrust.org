---
layout: page
title: madrona spatial planning framework
active: technology  
---
{% include JB/setup %}
<div class="row">
	<div class="span9">
		<h2>Philosophy</h2>
		<p>Madrona makes many choices for you while still providing lots of options, so you can get to the fun part of building tools right away.  You, the web developer, are still required to make many choices about your application and Madrona gives you building blocks to piece together the mental model of your solution quickly without getting distracted by all of the nuts and bolts.</p>
		<a name="zen"> </a>
		<h3>The Zen of Madrona</h3>
		<ul>
		    <li>The best process for making decisions will vary depending on scale, geography and culture.</li>
		    <li>Work directly with the intended users to capture the mental model of your decision-making process</li>
		    <li>Let the mental model define which spatial features and user actions are needed</li>
		    <li>The spatial features and user actions will define the API</li>
		    <li>The API and its workspace document will drive the client interface</li>
		    <li>Let these conventions be your guide but they should get out of the way when no longer useful</li>
		</ul>

		<h2>Core Building Blocks</h2>
		<p>Madrona is built on libraries such as Django, PostGIS, JQuery, OpenLayers and Google Earth which provide all of the essential building blocks for developing modern spatial web applications.</p>

		<div class="row blocks">
			<div class="span3">
				<div class="well">
					<a name="django"> </a>
					<h3>Django</h3>
					<a href="http://www.djangoproject.com">http://www.djangoproject.com</a>
					<p>
						<ul>
							<li>Model-Template-View architecture</li>
							<li>Automatic admin interface</li>
							<li>Elegant URL design</li>
							<li>Template system</li>
							<li>Caching</li>
							<li>Internationalization</li>
							<li>User accounts and groups</li>
							<li>Content management</li>
							<li>Extensive <a href="http://djangopackages.com/">third-party packages</a></li>
						</ul>
					</p>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="geodjango"> </a>
					<h3>GeoDjango</h3>
					<a href="http://geodjango.org/">http://geodjango.org/</a>
					<p>
						<ul>
							<li>PostGIS support</li>
							<li>Geographic models</li>
							<li>Object-oriented spatial queries</li>
							<li>GEOS Python API</li>
							<li>GDAL Python API</li>
						</ul>
					</p>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="postgis"> </a>
					<h3>PostGIS</h3>
						<a href="http://postgis.refractions.net/ ">http://postgis.refractions.net/ </a>
					<p>
						<ul>
							<li>Vector and raster support</li>
							<li>First-class geographic data types</li>
							<li>Full spatial query support</li>
							<li>GiST indexing</li>
						</ul>
					</p>
				</div>
			</div>
		</div>
		<div class="row blocks">
			<div class="span3">
				<div class="well">
					<a name="jquery"> </a>
					<h3>JQuery</h3>
					<a href="http://jquery.com">http://jquery.com</a>
					<p>
						<ul>
							<li>Lightweight</li>
							<li>Cross-browser DOM manipulation and event handling</li>
							<li>Extendable through plugin architecture</li>
							<li>Extensive third-party plugins</li>
						</ul>
					</p>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="openlayers"> </a>
					<h3>OpenLayers</h3>
					<a href="http://openlayers.org">http://openlayers.org</a>
					<p>
						<ul>
							<li>2D tile-based maps</li>
							<li>Vector support with drawing tools</li>				
							<li>Extensive support for mapping services including <a href="http://mapbox.com/mbtiles-spec/utfgrid/">UTF-Grid</a></li>
							<li>Google maps integration</li>
						</ul>
					</p>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="google_earth"> </a>
					<h3>Google Earth Plugin</h3>
					<a href="Z">Learn More</a>
					<p>
						<ul>
							<li>Immersive 3D environment</li>
							<li>KML support including superoverlays</li>
							<li>Global base imagery</li>
							<li>Simplified use through <a href="http://code.google.com/p/earth-api-utility-library/">extensions</a></li>
						</ul>
					</p>								
				</div>
			</div>
		</div>

		<h2>Madrona Building Blocks</h2>
		<p>We've taken the core building blocks and combined them to create new building blocks tailored specifically for decision support and spatial planning.  You can mix and match them to meet your specific needs.</p>

		<a name="2d_and_3d_support"> </a>
		<div class="row">
			<div class="span3">
				<div class="well">
					<h3>2D and 3D Support</h3>
					<p>2D and 3D mapping clients have their strengths and weaknesses, choose the one that works best for your project.  Madrona supports both using the KML and GeoJSON data standards.</p>
					<ul>
						<li><a href="http://ecotrust.github.com/madrona/docs/geojson.html">GeoJSON support</a></li>
						<li><a href="http://ecotrust.github.com/madrona/docs/kmlapp.html">KML support</a></li>
					</ul>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="spatial_features"> </a>
					<h3>Spatial Features</h3>
					<p>Provides a powerful spatial content management system complete with API.  Define new features (point, line, polygon) that are unique to your needs (wind energy sites, bike paths, event locations), then let users sketch, copy and share them.</p>
					<a href="http://ecotrust.github.com/madrona/docs/features.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="collaboration"> </a>
					<h3>Collaboration</h3>
					<p>The best ideas often evolve through many iterations and through connecting with other people.  Madrona is developed with quick iteration and sharing in mind. Our robust permissions model is secure but allows you to share your work when you want.</p>
					<a href="http://ecotrust.github.com/madrona/docs/managing_users.html">Learn More</a>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="feature_manipulators"> </a>
					<h3>Feature Manipulators</h3>
					<p>Features sketched by users often need to be modified or cleaned, Madrona provides a workflow for doing that.  Examples include clipping a polygon to a study region or excluding specific areas.</p>
					<a href="http://ecotrust.github.com/madrona/docs/manipulators.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="import_export"> </a>
					<h3>Import/Export</h3>
					<p>Planning tools shouldn’t be black boxes.  Import and export features are provided so that users can get out what they put in and integrate their external planning and GIS workflows.</p>
					<ul>
						<li><a href="http://ecotrust.github.com/madrona/docs/loadshp.html">Import</a></li>
						<li><a href="http://ecotrust.github.com/madrona/docs/export.html">Export</a></li>
					</ul>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="map_bookmarks"> </a>
					<h3>Map Bookmarks</h3>
					<p>Let’s users take a snapshot of their map view including the data layers and features they had turned on then share and manage the views as bookmarks (Google Earth support only currently)</p>
					<a href="http://ecotrust.github.com/madrona/docs/bookmarks.html">Learn More</a>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="study_regions"> </a>
					<h3>Study Regions</h3>
					<p>Focus the user’s attention on a specific geographic region and then create or limit user actions specific to that region.</p>
					<a href="http://ecotrust.github.com/madrona/docs/studyregion.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="data_layers"> </a>
					<h3>Data Layers</h3>
					<p>Manage a hierarchy of data layers important to your decision-making process and provide fine-grained access for viewing.  Also let users upload their own data layers. (KML support only currently).</p>
					<a href="http://ecotrust.github.com/madrona/docs/layers.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="reports"> </a>
					<h3>Reports</h3>
					<p>Provide feedback to users by performing real-time spatial analyses on their features.  Quickly organize information as tabular data and interactive charts using Django’s template system and your favorite visualization library.</p>
					<a href="http://ecotrust.github.com/madrona/docs/sidebar.html">Learn More</a>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="flexible_analysis"> </a>
					<h3>Flexible Analysis</h3>
					<p>Interact with external modeling and analysis software such as Grass, Marxan or ArcServer in a standardized way.  Define your model inputs and capture the output as Features that the user can interact with and share.</p>
					<a href="http://ecotrust.github.com/madrona/docs/analysistools.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="asynchronous_tasking"> </a>
					<h3>Asynchronous Tasking</h3>
					<p>Analysis can take a lot of time and system resources.  Users should be able to do other things while they are waiting.  Run processes in the background and get notified when they finish.</p>
					<a href="http://ecotrust.github.com/madrona/docs/async.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="static_maps"> </a>
					<h3>Static Maps</h3>
					<p>Create static map images for putting into reports and printing that include user defined shapes and other features.</p>
					<a href="http://ecotrust.github.com/madrona/docs/staticmap.html">Learn More</a>		
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span4">
				<div class="well">
					<a name="custom_projections"> </a>
					<h3>Custom Projections</h3>
					<p>Use one of the thousands of projections available with Proj.4 or define your own.</p>
					<a href="http://ecotrust.github.com/madrona/docs/custom_projection.html">Learn More</a>
				</div>
			</div>
			<div class="span5">
				<div class="well">
					<a name="raster_statistics"> </a>
					<h3>Raster Statistics</h3>
					<p>Quickly calculate statistics for a polygon Feature such as the average elevation or maximum temperature using raster data layers.  Provides an optional caching mechanism.</p>
					<a href="http://ecotrust.github.com/madrona/docs/raster_stats.html">Learn More</a>	
				</div>
			</div>
		</div>
		<p>One-size-fits-all rarely works.  The assumption is you will want to integrate different technology with Madrona whether it’s a mapping library like Leaflet, data management and data serving tools like Geoserver or ArcServer or a more robust client-side framework like GeoExt.</p>

		<a name="architecture"> </a>
		<h2>Architecture</h2>

		<p>[High-level software stack diagram. database, django, madrona, your tool, other services, data layers]</p>

		<p>Madrona sits near the top of the software stack as one of the frameworks for building web applications</p>

		<p>[Madrona internal architecture diagram.  client/server, rest api]</p>

		<p>Place where we introduce the architecture</p>

		<a name="feature_model"> </a>
		<h3>Feature Classes</h3>

		<p>Features are the first thing you define and once you register them the REST API and its associated workspace document will automatically publish them.  Out of the box features can be output in GeoJSON and KML.  They can also be imported from shapefiles and KML documents.

		For more information consult the <a href="http://ecotrust.github.com/madrona/docs/features.html">Madrona Feature documentation</a>
		</p>

	{% highlight python %}
class Mpa(PolygonFeature):
    ext = models.CharField(max_length="12")

    class Options:
        verbose_name = 'Marine Protected Area'
        form = 'myproject.forms.MpaForm'
        links = (
            alternate('Shapefile',
                'mlpa.views.shapefile',
                select='single',
                type='application/shapefile'),

            alternate('KMZ (Google Earth)',
                'mlpa.views.kml_export',
                select='single multiple',
                type='application/vnd.google-earth.kmz',
                generic=True),

            related('MPA Spreadsheet',
                'mlpa.views.spreadsheet',
                select='single',
                type='application/excel'),

            edit('Delete w/Grids',
                'mlpa.views.delete_w_grids',
                confirm="Are you sure you want to delete with grids?",
                select="single multiple",
                args=[MpaArray],
                kwargs={'keyword_argument': True}),

            edit_form('Tags',
                'mlpa.views.tag',
                select='single multiple',
                generic=True,
                models=(MpaArray, MlpaMpa)),
        )
		{% endhighlight %}
		<a name="rest_api"> </a>
		<h3>REST API</h3>

		<p>The madrona application programming interface (API) follows the representational state transfer or <a href="http://en.wikipedia.org/wiki/Representational_state_transfer">REST architecture</a> architecture.  This REST API is the communication channel allowing the client to interact with the server.  Using it you can:</p>
		<ul>
			<li>Create, read, update and delete Features</li>
			<li>Copy and share Features between user groups</li>
			<li>Manage Features within collections</li>
			<li>Convert to export formats</li>
			<li>Access reports and related documents</li>
		</ul>

		<a name="workspace_document"> </a>
		<h3>Workspace Document</h3>

		<p>The workspace document is part of the REST API.  It is a JSON document that the client fetches from the server at startup that describes the server-side API.  Specifically:
		<ul>
			<li>What Features are defined for the current user</li>
			<li>What Feature actions are available for the current user</li>
			<li>How Features can relate to one another</li>
		</ul>

		Specifically, the workspace document describes the URLs for:
		<ul>
			<li>Creating, Updating, and Deleting Feature instances</li>
			<li>Editing actions that can be performed such as Copying and Sharing</li>
			<li>Managing relationships between Features</li>
			<li>Alternative export formats, such as KMZ or shapefile downloads</li>
			<li>Related files that can be downloaded, such as spreadsheet or pdf reports</li>
			<li>Reading feature attributes or reports</li>
		</ul>
		</p>
		<p>
		For more information consult the <a href="http://ecotrust.github.com/madrona/docs/workspace_specification.html">Madrona workspace specification</a>
		</p>

		<h4>Example Workspace Document Snippet</h4>

		<pre class="prettyprint">
{
    "title": "Renewable Energy Site",
    "id": "features_renewableenergysite",
    "link-relations": {
        "self": {
          "uri-template": "/features/renewableenergysite/{id}/"
        },
        "create": {
          "uri-template": "/features/renewableenergysite/form/"
        },
        "related": [
          {
            "title": "Viewshed Map"
            "uri-template": "/features/renewableenergysite/links/viewshed-map/{id+}/",
            "select": "single",
            "rel": "related"
          }
        ],
        "update": {
          "uri-template": "/features/renewableenergysite/{id}/form/"
        }
    }
}
</pre>
		<p> This snippet defines a </p>

		<p>This document can be interpreted as follows:
		<ul>
			<li>There are three Features defined - marine protected areas, renewable energy sites and folders</li>
			<li>Both the marine protected areas and renewable energy site Features have a 'self' link for getting more information about a specific Feature, a 'create' link for creating a new instance of that Feature and an 'update' link for updating the geometry or attributes for a specific instance of that Feature.</li> 
			<li>Marine protected area instances have a 'related' habitat spreadsheet</li>
			<li>Renewable energy site instances have a 'related' viewshed map</li>
			<li>Folders are a special Feature type called a Collection.  'valid-children' is defining what Features can be associated with a folder.</li>
		</ul>
		This document has all of the information needed by the client to fetch/create/edit/delete feature instances, display them to the user, figure out what actions the user can take on them and finally how features can relate to each other (eg. what features can go into what collections).  For every feature, action and related element there is a URL for accessing it from the server.  Life is much easier for the client with a workspace document.</p>

		<a name="3d_web_client"> </a>
		<h3>3D Web Client</h3>

	</div>
	<div class="span3">
		<div class="row">
			<div class="span3">
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