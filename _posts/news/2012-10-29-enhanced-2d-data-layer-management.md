---
layout: post
title: "Enhanced 2D data layer management"
description: "The latest revision of the layer manager functionality extends Madrona's support for 2D mapping environments" 
category: news
tags: [layer_manager madrona4.1 2D]
author: Matthew Perry
---
{% include JB/setup %}

The latest revision of the layer manager functionality extends Madrona's support for 2D mapping environments. 

We've developed a rich server-side model for managing data layers and themes and added client-side user interface elements for organizing/visualizing data layers that can incorporated into any 2D OpenLayers-based madrona mapping application.

<div class='thumbnail thumb-wrap'>
    <img src='{{BASE_PATH}}/assets/img/news/layer_manager1.png' alt='Data layer manager - Image 1' />
</div>
<br/>

Features of the user interface include:
* **Data** Layer list with an accordion view organized by theme.
* Full text **search** of layers and themes.
* Support for basic **metadata** and source attribution.
* **Active** layers list for managing opacity, visibility and layer ordering of the current map.
* **Legend** support. 

<div class='thumbnail thumb-wrap'>
    <img src='{{BASE_PATH}}/assets/img/news/layer_manager2.png' alt='Data layer manager - Image 2' />
</div>
<br/>

Test it out with our live [madrona 2d demo](http://madrona2d.labs.ecotrust.org/layer_manager/demo/)

The functionality relies on OpenLayers, Knockout, Bootstrap and jQuery-ui. To set up a 2D madrona application to use the layer manager widgets:

1. Populate the Layers and Themes with some data (we include a [comprehensive fixture](https://github.com/Ecotrust/madrona/blob/master/madrona/layer_manager/fixtures/base_layers.json) in madrona)
2. Set up some basic javascript variables and load the required js/css files
3. Include the interface elements via django *include* template tags

For full instructions on configuring the layer manager, see [the docs](http://ecotrust.github.com/madrona/docs/layer_manager.html)

The 2D layer manager functionality has been merged into the madrona `master` branch and will be the highlight of the upcoming Madrona 4.1 release. 

