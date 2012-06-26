---
layout: post
title: "Enhanced 2D mapping support"
description: ""
category: news
tags: []
author: Tim Welch
---
{% include JB/setup %}

Improved support for 2D mapping libraries such as OpenLayers and Leaflet has been added to the Madrona platform through the addition of GeoJSON support for the Madrona Feature API.  What's unique about this implementation is that it supports arbitrarily nested feature collections, something that is not defined in the GeoJSON spec.  It does this by allowing an empty geometry within a FeatureCollection with a special feature_set property.  That property is the id of another FeatureCollection.  This means that traversing the hierarchy requires knowledge of this convention, so we make it optional.  

This enhancement is within the GeoJSON spec and the benefit is that like KML Network Links, the server doesn't send the entire tree structure, just the child features of a given collection.  This requires additional requests overall in order to get a full view of the tree but allows better performance to be maintained for large trees.  We're curious what people think about it.  Kudos to Matt Perry for working this through, it was one of the more memorable brainstorming sessions with the team around the whiteboard.

[Learn More](http://ecotrust.github.com/madrona/docs/geojson.html)

The intention going forward is for server-side features to support both 2D and 3D mapping clients giving you the flexibility to choose the one you want.  Look for the map bookmark and layer manager apps to support 2D mapping clients over the next month.