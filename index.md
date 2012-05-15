---
layout: page
title: madrona spatial planning framework
tagline: A framework for building spatial planning tools at any scale.
---
{% include JB/setup %}
<div class="row">
  <div class="span6">
    <div class="bugs">
      <div class="row">
        <div class="span3">
          <a href="{{ BASE_PATH }}/technology/#spatial_features">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><img src="{{ BASE_PATH }}/assets/img/features.png">
                    <span>Spatial&nbsp;Features</span>
                  </h3>
                </div>
                <div class="text">
                  <p><strong>define, sketch, share</strong></p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="span3">
            <a href="{{ BASE_PATH }}/technology/#data_layers">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><img src="{{ BASE_PATH }}/assets/img/layers.png">
                    <span>Data Layers</span>
                  </h3>
                </div>
                <div class="text">
                  <p><strong>public and private</strong></p>
                </div>
              </div>
            </div>
          </a>
        </div>
      </div>
      <div class="row">
        <div class="span3">
          <a href="{{ BASE_PATH }}/technology/#collaboration">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><img src="{{ BASE_PATH }}/assets/img/collaboration.png"><span class="wide">Collaboration</span></h3>
                </div>
                <div class="text">
                  <p><strong>consensus driven</strong></p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="span3">
          <a href="{{ BASE_PATH }}/technology/#flexible_analysis">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><img src="{{ BASE_PATH }}/assets/img/analysis.png"><span class="wide">Flexible Analysis</span></h3>
                </div>
                <div class="text">
                  <p><strong>visualize and report</strong></p>
                </div>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="span6">
        <p class="madrona-text">Madrona offers a flexible set of building blocks and design patterns for software development. Our support services can help you develop and implement cutting-edge tools for effective place-based decision making.</p>
      </div>
    </div>
  </div>
  <div class="span6">
    <div id="showcase" class="carousel">
    <!-- Carousel items -->
      <div class="carousel-inner">
      <div class="active item">
        <img src="{{ BASE_PATH }}/assets/img/fsp.png">
        <div class="carousel-caption">
          <h4>Forest Scenario Planner</h4>
          <p>The Murdock Charitable Trust wanted to help private forest landowners visualize alternative management scenarios.</p>
        </div>
      </div>
      <div class="item">
        <img src="{{BASE_PATH}}/assets/img/experience/windmill-ocean.jpg">
        <div class="carousel-caption">
          <h4>Marine Decision Support</h4>
          <p>The Mid-Atlantic Regional Council on the Ocean sought to engage community involvement in zoning nearshore waters for multiple uses.</p>
        </div>
      </div>
      <div class="item">
        <img src="{{BASE_PATH}}/assets/img/experience/wwri.png">
        <div class="carousel-caption">
          <h4>Aquatic Priority Setting</h4>
          <p>U.S. Fish and Wildlife Service needed a platform for conservation and restoration planning on sub-watershed scales across the Columbia River Basin.</p>
        </div>
      </div>
      <div class="item">
        <img src="{{ BASE_PATH }}/assets/img/fsp.png">
        <div class="carousel-caption">
          <h4>Bioregional Discovery</h4>
          <p>Ecotrust wanted to allow people all over the planet to visualize their bioregions and gain an appreciation of social and environmental assets and vulnerabilities.</p>
        </div>
      </div>
    </div>
    <!-- Carousel nav -->
    <a class="carousel-control left" href="#showcase" data-slide="prev">&lsaquo;</a>
    <a class="carousel-control right" href="#showcase" data-slide="next">&rsaquo;</a>
    </div>
   </div>
</div>


<script>
  $(window).load(function() {
    $('.carousel').carousel({
      interval: 8000
    })
    
  });
</script>