---
layout: post
title: "Madrona 4.1 released"
description: "Madrona 4.1 released"
category: news
tags: [madrona release madrona4.1]
author: Matt Perry
---
{% include JB/setup %}

Since the initial release of Madrona 4.0, we've been working on many projects with 2D mapping interfaces (OpenLayers or Leaflet).
Much of the work to the Madrona core is related to the <a href='/news/enhanced-2d-data-layer-management/'>Enhanced 2D Layer Management</a>
which allows knockout-based Javascript client apps to seamlessly incorporate advanced mapping interface elements. 

Updates in the 4.1 release include:

* New `layer_manager` app for managing 2D tiled map sources
* By default, `enforce_supported_browser` set to False (may cause minor change in browser detection behavior in some 3D apps)
* Clean up json import situation
* Preliminary Multipolygon support (server-side)
* Several minor bug fixes and tweaks

The <a href='https://pypi.python.org/pypi?:action=display&name=madrona&version=4.1'>4.1 version is live on PyPi</a> so updgrading is
as easy as `pip install --upgrade madrona`

Enjoy.
