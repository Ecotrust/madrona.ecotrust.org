---
layout: post
title: "UTFGrids and Madrona"
description: "Ecotrust has created a utility for creating UTFGrids thats being leveraged by Madrona-based tools"
category: news
tags: [utfgrid, utilities]
author: Tim Welch
---
{% include JB/setup %}

<a href='http://ecotrust.github.com/marco-portal' class='thumbnail thumb-wrap'><img src='{{BASE_PATH}}/assets/img/news/marco-utfgrid.png' alt='MARCO UTFGrid example' /></a>

UTFGrids are an elegant solution to providing scalable access to thousands of map features, and they're a key interactive element of the 2D maps we're developing with Madrona.  However, the workflows for creating UTFGrid JSON files with Tilemill and Tilestache have until now been pretty intimately tied to the cartographic rendering of map layers.  

For the [MARCO Marine Planner](http://ecotrust.github.com/marco-portal/) project, we found ourselves just wanting to generate the UTFGrid JSON files directly from a shapefile. It turns out this wasn't too difficult to do using Mapnik's UTFGrid support.  Our senior developer Matt Perry whipped up a utility called [create-utgfrids](https://github.com/Ecotrust/create-utfgrids) in a couple of hours.

* [Read Matt's full blog post](http://blog.perrygeo.net/2012/08/20/creating-utfgrids-directly-from-a-polygon-datasource/)
* [Learn more about UTFGrids](http://mapbox.com/developers/utfgrid/)
