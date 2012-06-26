---
layout: post
title: "Madrona version 4.0 released"
description: ""
category: news
tags: []
---
{% include JB/setup %}
<p>
After months of development, Ecotrust is pleased to announce the release of version 4.0 of the Madrona framework.  Madrona is the evolution of the <a href="http://marinemap.org">MarineMap</a> project, which reached end-of-life with version 3 in 2011.</p>

<p>Learn more about Madrona's history</p>

<p>
Updates and fixes in the 4.0 release include:
<ul>
	<li><a href="http://ecotrust.github.com/madrona/docs/bookmarks.html">Map bookmarks</a></li>
	<li><a href="http://ecotrust.github.com/madrona/docs/geojson.html">GeoJSON links to features</a> providing support for 2D map clients</li>
	<li>New analysistools app</li>
	<li>Switched to new-style Django url and absurl template tags. (Use `{% url 'url-name' %}` versus `{% url url-name %}` )</li>
	<li>Reorganization of setup code</li>
	<li>Overhaul of setup.py and associated installation procedures</li>
	<li>Added flatblocks to manage content</li>
	<li>Added create-madrona-project.py script as a madrona replacement for startproject</li>
	<li>Fixed several bugs in raster_stats - improved tempfile and cache handling</li>
	<li>Improved study region loading via management command</li>
	<li>Improved geometry validity handling in manipulators</li>
	<li>Improved logging system</li>
	<li>Install_media command flag to handle admin static files</li>
	<li>Numerous bug fixes and lots of code cleanup</li>
</ul>
</p>