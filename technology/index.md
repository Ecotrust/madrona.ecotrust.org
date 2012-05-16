---
layout: page
title: madrona spatial planning framework
active: technology  
---
{% include JB/setup %}
<div class="row">
	<div class="span9">
		<h2>Philosophy</h2>
		<div>
			<p>Madrona makes many choices for you while still providing lots of options, so you can get to the fun part of building tools right away.  You, the web developer, are still required to make many choices about your application and Madrona gives you building blocks to piece together the mental model of your solution quickly without getting distracted by all of the nuts and bolts.</p>
			<a name="The-Zen-of-Madrona"> </a>
			<h3>The Zen of Madrona</h3>
			<ul>
			    <li>The best process for making decisions will vary depending on scale, geography and culture.</li>
			    <li>Work directly with the intended users to capture the mental model of your decision-making process</li>
			    <li>Let the mental model define which spatial features and user actions are needed</li>
			    <li>The spatial features and user actions will define the API</li>
			    <li>The API and its workspace document will drive the client interface</li>
			    <li>Let these conventions be your guide but they should get out of the way when no longer useful</li>
			</ul>
		</div>
		<h2>Core Building Blocks</h2>
		<p>Madrona is built on libraries such as Django, PostGIS, JQuery, OpenLayers and Google Earth which provide all of the essential building blocks for developing modern spatial web applications.</p>

		<div class="row blocks">
			<div class="span3">
				<div class="well">
					<a name="Django"> </a>
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
					<a name="GeoDjango"> </a>
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
					<a name="PostGIS"> </a>
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
					<a name="JQuery"> </a>
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
					<a name="OpenLayers"> </a>
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
					<a name="Google-Earth-Plugin"> </a>
					<h3>Google Earth Plugin</h3>
					<a href="http://earth.google.com/plugin">http://earth.google.com/plugin</a>
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

		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="2D-and-3D-Support"> </a>
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
					<a name="Spatial-Features"> </a>
					<h3>Spatial Features</h3>
					<p>Provides a powerful spatial content management system complete with API.  Define new features (point, line, polygon) that are unique to your needs (wind energy sites, bike paths, event locations), then let users sketch, copy and share them.</p>
					<a href="http://ecotrust.github.com/madrona/docs/features.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Collaboration"> </a>
					<h3>Collaboration</h3>
					<p>The best ideas often evolve through many iterations and through connecting with other people.  Madrona is developed with quick iteration and sharing in mind. Our robust permissions model is secure but allows you to share your work when you want.</p>
					<a href="http://ecotrust.github.com/madrona/docs/managing_users.html">Learn More</a>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="Feature-Manipulators"> </a>
					<h3>Feature Manipulators</h3>
					<p>Features sketched by users often need to be modified or cleaned, Madrona provides a workflow for doing that.  Examples include clipping a polygon to a study region or excluding specific areas.</p>
					<a href="http://ecotrust.github.com/madrona/docs/manipulators.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Import-Export"> </a>
					<h3>Import-Export</h3>
					<p>Planning tools shouldn’t be black boxes.  Import and export features are provided so that users can get out what they put in and integrate their external planning and GIS workflows.</p>
					<ul>
						<li><a href="http://ecotrust.github.com/madrona/docs/loadshp.html">Import</a></li>
						<li><a href="http://ecotrust.github.com/madrona/docs/export.html">Export</a></li>
					</ul>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Map-Bookmarks"> </a>
					<h3>Map Bookmarks</h3>
					<p>Let’s users take a snapshot of their map view including the data layers and features they had turned on then share and manage the views as bookmarks (Google Earth support only currently)</p>
					<a href="http://ecotrust.github.com/madrona/docs/bookmarks.html">Learn More</a>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="Study-Regions"> </a>
					<h3>Study Regions</h3>
					<p>Focus the user’s attention on a specific geographic region and then create or limit user actions specific to that region.</p>
					<a href="http://ecotrust.github.com/madrona/docs/studyregion.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Data-Layers"> </a>
					<h3>Data Layers</h3>
					<p>Manage a hierarchy of data layers important to your decision-making process and provide fine-grained access for viewing.  Also let users upload their own data layers. (KML support only currently).</p>
					<a href="http://ecotrust.github.com/madrona/docs/layers.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Reports"> </a>
					<h3>Reports</h3>
					<p>Provide feedback to users by performing real-time spatial analyses on their features.  Quickly organize information as tabular data and interactive charts using Django’s template system and your favorite visualization library.</p>
					<a href="http://ecotrust.github.com/madrona/docs/sidebar.html">Learn More</a>
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span3">
				<div class="well">
					<a name="Flexible-Analysis"> </a>
					<h3>Flexible Analysis</h3>
					<p>Interact with external modeling and analysis software such as Grass, Marxan or ArcServer in a standardized way.  Define your model inputs and capture the output as Features that the user can interact with and share.</p>
					<a href="http://ecotrust.github.com/madrona/docs/analysistools.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Asynchronous-Tasking"> </a>
					<h3>Asynchronous Tasking</h3>
					<p>Analysis can take a lot of time and system resources.  Users should be able to do other things while they are waiting.  Run processes in the background and get notified when they finish.</p>
					<a href="http://ecotrust.github.com/madrona/docs/async.html">Learn More</a>
				</div>
			</div>
			<div class="span3">
				<div class="well">
					<a name="Static-Maps"> </a>
					<h3>Static Maps</h3>
					<p>Create static map images for putting into reports and printing that include user defined shapes and other features.</p>
					<a href="http://ecotrust.github.com/madrona/docs/staticmap.html">Learn More</a>		
				</div>
			</div>
		</div>
		<div class="row">
			<div class="span4">
				<div class="well">
					<a name="Custom-Projections"> </a>
					<h3>Custom Projections</h3>
					<p>Use one of the thousands of projections available with Proj.4 or define your own.</p>
					<a href="http://ecotrust.github.com/madrona/docs/custom_projection.html">Learn More</a>
				</div>
			</div>
			<div class="span5">
				<div class="well">
					<a name="Raster-Statistics"> </a>
					<h3>Raster Statistics</h3>
					<p>Quickly calculate statistics for a polygon Feature such as the average elevation or maximum temperature using raster data layers.  Provides an optional caching mechanism.</p>
					<a href="http://ecotrust.github.com/madrona/docs/raster_stats.html">Learn More</a>	
				</div>
			</div>
		</div>
		<p>One-size-fits-all rarely works and often times you have to roll your sleeves up.  The assumption is you will want to integrate different technology with Madrona whether it’s a mapping library like Leaflet, data management and data serving tools like Geoserver or ArcServer or a more robust client-side framework like GeoExt.</p>

		<a name="architecture"> </a>
		<h2>Architecture</h2>
		<div class="row">
			<div class="span9">
				<a name="Features"> </a>
				<h3>Features</h3>

				<p>Madrona creates a system that can best be thought of as a feature spatial content management system.  This starts with the Madrona PointFeature, LineFeature and PolygonFeature models.  You can quickly extend these models to define your own spatial features specific to the purpose of your tool.  Working with wind energy sites?  Define a PolygonFeature and give it attributes for the type and number of turbines.  Once you register your feature it’s mapped to a PostGIS table and automatically published through the REST API.</p>

				<p>For more information consult the <a href="http://ecotrust.github.com/madrona/docs/features.html">Madrona Feature documentation</a>
				</p>

			{% highlight python %}
		@register
		class WindEnergySite(PolygonFeature):
		    ext = models.CharField(max_length="12")
		    turbine_type = models.CharField(max_length="30")
		    num_turbines = models.IntegerField()

		    class Options:
		        verbose_name = 'Wind Energy Site'
		        form = 'myproject.forms.WindForm'
		        links = (
		            alternate('Shapefile',
		                'mlpa.views.shapefile',
		                select='single',
		                type='application/shapefile'),

		            alternate('KMZ (Google Earth)',
		                'wind.views.kml_export',
		                select='single multiple',
		                type='application/vnd.google-earth.kmz',
		                generic=True),

		            related('Viewshed Map',
		                'wind.views.viewshed_map',
		                select='single',
		                type='image/png'),

		            edit('Delete',
		                'wind.views.delete',
		                select="single multiple",
		                args=[WindArray],
		                kwargs={'keyword_argument': True})
		        )
				{% endhighlight %}

				<a name="REST-API"> </a>
				<h3>REST API</h3>

				<p>The madrona <a href="http://en.wikipedia.org/wiki/Representational_state_transfer">REST API</a> is the communication channel for the client and server and supports both GeoJSON and KML.  Using it you can:</p>
				<ul>
					<li>Create, read, update and delete Features</li>
					<li>Copy and share Features between user groups</li>
					<li>Manage Features within collections</li>
					<li>Convert to export formats</li>
					<li>Access reports and related documents</li>
				</ul>

				<h4>Workspace Document</h4>

				<p>The workspace document is an important part of the REST API.  It is a JSON document that the client fetches from the server at startup that describes the server-side API.  Specifically::
				<ul>
					<li>What Features are defined for the current user</li>
					<li>What Feature actions are available for the current user</li>
					<li>How Features relate to one another</li>
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
				<p>Because the API is well-defined through the workspace document, you can quickly and efficiently develop alternative client interfaces. 
				</p>
				<p>For more information consult the <a href="http://ecotrust.github.com/madrona/docs/workspace_specification.html">Madrona workspace specification</a>
				</p>

				<p>The JSON snippet below defines the wind energy site feature in the workspace document.  You can see that URL's have been published for performing create and edit actions as well as accessing associated viewshed maps and KMZ/Shapefile exports.</p>

				{% highlight javascript %}
		{
		    "title": "Wind Energy Site",
		    "id": "features_windenergysite",
		    "link-relations": {
		        "self": {
		          "uri-template": "/features/windenergysite/{id}/"
		        },
		        "create": {
		          "uri-template": "/features/windenergysite/form/"
		        },
		        "alternate": [
		          {
		            "title": "Shapefile"
		            "uri-template": "/features/windenergysite/links/shapefile/{id+}/",
		            "select": "multiple",
		            "rel": "related"
		          }
		        ],
		        "related": [
		          {
		            "title": "KMZ (Google Earth)"
		            "uri-template": "/features/windenergysite/links/kmz/{id+}/",
		            "select": "multiple",
		            "rel": "related"
		          }
		        ],
		        "related": [
		          {
		            "title": "Viewshed Map"
		            "uri-template": "/features/windenergysite/links/viewshed-map/{id+}/",
		            "select": "single",
		            "rel": "related"
		          }
		        ],
		        "update": {
		          "uri-template": "/features/windenergysite/{id}/form/"
		        }
		    }
		}
			{% endhighlight %}
			<a name="3D-Web-Client"> </a>
			<h3>3D Web Client</h3>

			<p>By default, madrona provides a robust HTML/Javascript client interface based on the 3D Google Earth plugin. It is not the only option for building a client interface but it does provide a complete solution out of the box.</p>

			<p>The 3D web client allows features to be delivered using the expressive KML format. Using the workspace document the client will automatically configure a set of javascript widgets including the Google Earth Plugin, forming an end-to-end spatial content management system. Besides the Google Earth plugin itself, madrona provides the following components:</p>

			<h4>KmlTree</h4>

			<p><a href="http://code.google.com/p/kmltree/">kmltree</a> is a javascript tree widget that can be used in conjunction with the Google Earth API. It replicates the functionality of the Google Earth desktop client, namely the ability to render complex KML documents very quickly and present the hierarchal contents of a KML document as an expandable, interactive tree view.</p>

			<h4>KmlEditor</h4>

			<p>KmlEditor provides the editing interface and menu to hook your features tree into the REST API. It will use the workspace document and configure the editing interface according to the API definition. The interface is context sensitive and provides the appropriate options for the selected features.</p>

			<h4>KML Drawing Tools</h4>

			<p>Madrona provides a robust set of drawing and editing tools for the Google Earth Plugin.  These play a part in the larger workflow of creating, editing and sharing features.</p>
			</div>
		</div>
	</div>
	<div class="span3">
		<div class="row">
			<div class="span3">
				<div id="tech-accordion" class="accordion" data-bind="foreach: headings" style="display:none">
		            <div class="accordion-group">
			            <div class="accordion-heading">
			                <a data-bind="attr: { href: '#' + tag }" data-parent="#tech-accordion" data-toggle="collapse" class="accordion-toggle">
			                 	<span data-bind="text: title"></span>
			                </a>
			            </div>
			            <div class="accordion-body collapse" data-bind="attr: { id: tag }">
			                <div class="accordion-inner">
			                	<ul data-bind="foreach: subheads" class="unstyled">
			                		<li><a data-bind="text: stitle, attr: { href: '#' + stag }">title</a></li>
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
	var timer, $accordion = $('#tech-accordion'),
		initial; 
		scrollHandler = function () {  
			var scrollTop = $(window).scrollTop(),
				offset = $accordion.offset().top;
			
			if (scrollTop > offset + 100) {
				$accordion.offset({ top: scrollTop + 100 });
			}  else {
			  	$accordion.offset({ top: scrollTop > initial? scrollTop + 100: initial });
			}
		}
	$(window).scroll(function () {
		if (timer) {
			clearTimeout(timer);
		}
		timer = setTimeout(scrollHandler, 20);
	});

	ko.applyBindings({
		headings: $('h2').map(function () {
			var $head = $(this), 
				$section = $head.nextUntil('h2'),
				subheads = $section.find('h3').map(function () {
					return {
						stitle: $(this).text(),
						stag: $(this).text().replace(/ /g, '-')
					};
				});

			return {
				'title': $head.text(),
				'tag': $head.text().replace(/ /g, '-'),
				'subheads': subheads
			}; 
		})
	});
	$accordion.show();
	initial = $accordion.offset().top;
	scrollHandler();

};
</script>