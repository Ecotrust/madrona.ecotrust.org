---
layout: post
title: "Madrona version 4.0 released"
description: ""
category: news
tags: []
---
{% include JB/setup %}

After months of development, Ecotrust is pleased to announce the first public release of Madrona, version 4.0.  Madrona is the evolution of [MarineMap](http://marinemap.org), a tool for web-based marine spatial planning developed by the MarineMap Consortium which included the University of California Santa Barbara, Ecotrust, and The Nature Conservancy.  MarineMap reached end-of-life with version 3 in 2011.  [Learn more about Madrona's history]({{BASE_PATH}}/experience/history.html)

Read about the release on the [ecotrust blog.](http://blog.ecotrust.org/software-for-21st-century-decisions-2/)

Updates and fixes in the 4.0 release include:

* [Map bookmarks](http://ecotrust.github.com/madrona/docs/bookmarks.html)
* [GeoJSON support](http://ecotrust.github.com/madrona/docs/geojson.html") for the Madrona Feature API
* New analysistools app
* Switched to new-style Django url and absurl template tags
* Reorganization of setup code
* Overhaul of setup.py and associated installation procedures
* Added flatblocks to manage content
* Added create-madrona-project.py script as a madrona replacement for startproject
* Fixed several bugs in raster_stats - improved tempfile and cache handling
* Improved study region loading via management command
* Improved geometry validity handling in manipulators
* Improved logging system
* Install_media command flag to handle admin static files
* Numerous bug fixes and lots of code cleanup