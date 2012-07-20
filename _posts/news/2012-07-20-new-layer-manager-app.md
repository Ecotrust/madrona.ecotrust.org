---
layout: post
title: "New Layer Manager App"
description: ""
category: news
tags: [layer manager, new feature]
author: Ryan Hodges
---
{% include JB/setup %}
Layer Management fans rejoice! We have added an app to handle basic layer management. If you develop an application that requires displaying multiple data layers on the map, it will be easier to create, edit, save, and access the data of the layers. This will be very useful for creating layer controls for displaying, organizing and toggling visibility of layers.

Currently we're supporting layers organized by themes: a data layer displaying an ocean's sediment grain size could be associated with an "Ocean" theme, or a "Soils" theme, depending on your needs. The relationship is many to many, so it could belong to both, and each theme can be associated with other data layers.

Currently, the Theme model includes a name field and can return a list of layer ids associated with it. 

The Layer model includes fields for 
* Name
* Layer type (WMS, Vector, XYZ, etc...)
* URL location - allowing the maps to be stored locally or pulled from a different server
* Themes
* Sublayers - allowing user to select from multiple datalayers to fill one need
* Legend
* UTF URL - for UTF grids

Use `.toDict()` to generate a dictionary data structure of either model.

As you can see, there's a lot of room for this to grow! We will be sure to update this as our needs develop, but we are also excited to see what you do with it!

View the code now: [Layer Manager](https://github.com/Ecotrust/madrona/tree/master/madrona/layer_manager)