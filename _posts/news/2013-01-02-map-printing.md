---
layout: post
title: "Printing web maps made easier"
description: ""
category: news
tags: []
author: Tim Welch
---
{% include JB/setup %}
One of the most requested features for any web mapping application is printing.  <a target="_blank" href="http://ecotrust.github.com/madrona/docs/bookmarks.html">Map bookmarks</a> get you most of the way there for sharing your map view, but people want the digital equivalent of a hard copy.  

The simple answer has always been to take a screenshot in your operating system of choice.  But wait you want it as a PDF, with a title on it, and a legend, and 300dpi?  And so more sophisticated server-side print capabilities were developed a la <a target="_blank" href="http://video.esri.com/watch/1058/arcgis-for-server-101-printingtools-service-tutorial">ArcGIS Server printing</a> and <a target="_blank" href='http://docs.geoserver.org/latest/en/user/community/printing/index.html'>GeoServer printing</a>.  But these are pretty heavy-handed solutions, often needing access to your original datasets and/or a map engine to be able to render them all together in a single print image.  What if you don't have access to the original datasets?  What if a number of the data layers in your application are map tile services from third-party providers?

Our developer Edwin knew there had to be a simpler way.  He saw that people were using <a target="_blank" href="http://phantomjs.org/">PhantomJS</a> with its headless Webkit engine to load web pages and make screen captures.  What if he thought, we could develop a lightweight print service that given the state of the users map, could load up the same exact map view the user sees in their browser and export it in a variety of formats and sizes (PNG, JPEG, PDF, etc.)?

So Edwin created just that, a standalone print service for the Mid-Atlantic Data Portal and it's pretty sweet.  

<img src='{{BASE_PATH}}/assets/img/news/print.png' alt='Print/Export feature screenshot' />

This module, <a target="_blank" href="https://github.com/Ecotrust/marco-portal/tree/master/printing">available on GitHub</a>, was created using NodeJS and integrates with the <a target="_blank" href="http://madrona.ecotrust.org">Madrona</a> and Django-based Mid-Atlantic Marine Planner.  To try it out yourself, go to <a target="_blank" href="http://goo.gl/a98nG">this map bookmark</a> visualizing waterbird density around Great Bay and click the print button in the top right corner of the map.  Here's an example output.

<img src='{{BASE_PATH}}/assets/img/news/print-example.png' alt='Print/Export feature screenshot' />

Look for this printing module to become its own project in coming months, and a core feature of Madrona.  

To learn more about the development of the Mid-Atlantic Ocean Data Portal and its integration of a number of data layers published by ESRI, NOAA, and The Nature Conservancy, visit its <a target="_blank" href="http://ecotrust.github.com/marco-portal/">Project Log</a>
