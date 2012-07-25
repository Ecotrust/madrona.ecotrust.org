---
layout: post
title: "NPLCC Prioritization Tool preview"
description: "Ecotrust and the NPLCC have partnered to develop a conservation decision support system for the north pacific coastal temperate rainforest"
category: news
tags: [nplcc, priorities, newapp]
author: Matthew Perry
---
{% include JB/setup %}

[Ecotrust](http://ecotrust.org) and the [NPLCC](http://www.fws.gov/pacific/Climatechange/nplcc/) have partnered 
to develop a conservation decision support system for Alaska, British Columbia, Washington, Oregon and Californian coastal temperate rainforest.  This system will enable stakeholder to engage in strategic planning and program delivery of conservation and restoration priorities for the North Pacific Region.

<div class="row">
        <img src="{{BASE_PATH}}/assets/img/experience/nplcc/results.png" alt="NPLCC">
</div>


The prioritization tool is based on Madrona 4.0 and leverages the analytic framework established with our [aquatic priorities tool](http://madrona.ecotrust.org/experience/aquatic-priorities/). 
In addition to extending the tool to work with new data sources and a much wider geography, we are enhancing the core Madrona prioritization tool in several key ways:

* The analytical framework has been modified to accept user-defined selection of geography. This allows you to specify an area and **prioritize watersheds within a region of interest** as opposed to prioritizing across the entire study area (which may not be relevant to all users).   
* User input of prioritization targets will be greatly simplified by using a **single slider bar** to represent relative importance of the species. 
* With the recent addition of [GeoJSON](http://madrona.ecotrust.org/news/enhanced-2d-mapping-support/) support in Madrona, we are transitioning the tool to use a javascript-based **2D map interface**. Amongst the many improvements, this means we can run the application on nearly any platform (including tablets and mobile devices), use different base layers for improved cartography and utilize our recent work on OpenLayer's [UTFGrid support](http://dev.openlayers.org/docs/files/OpenLayers/Layer/UTFGrid-js.html).
* The user interface has been reworked to provide a simplified and **directed workflow**. This was accomplished using the [bootstrap](http://twitter.github.com/bootstrap/) and [knockout](http://knockoutjs.com/) frameworks on the client side. In addition to improved user experience, the new interface shows greatly improved speed and performance. 


We are currently in the *alpha* release of the software and are working on collecting region wide data for mammalian, aquatic and bird species as well as climate change and watershed condition indices. The public release of the tool is expected in fall of 2012... stay tuned. To track the technical details of the project, follow us on the [NPLCC github page](https://github.com/Ecotrust/nplcc).
