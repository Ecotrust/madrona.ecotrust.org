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
                <div class="pull-left icon">
                  <img class="tall" src="assets/img/features.png">
                </div>
                <div class="pull-left">
                  <h4>Spatial&nbsp;Features</h4>
                  <p>define, sketch, share</p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="span3">
          <a href="{{ BASE_PATH }}/technology/#data_layers">
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <img src="assets/img/layers.png">
                </div>
                <div class="pull-left">
                  <h4>Data&nbsp;Layers</h4>
                  <p>public and private</p>
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
                <div class="pull-left icon">
                  <img class="tall" src="assets/img/collaboration.png">
                </div>
                <div class="pull-left">
                  <h4>Collaboration</h4>
                  <p>consensus driven</p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="span3">
          <a href="{{ BASE_PATH }}/technology/#flexible_analysis">
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <img src="assets/img/analysis.png">
                </div>
                <div class="pull-left">
                  <h4>Flexible&nbsp;Analysis</h4>
                  <p>visualize and report</p>
                </div>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="span6">
        <p>Madrona offers a flexible set of building blocks and design patterns for software development. Our portfolio of services, training, and support can help you develop, analyze, and implement effective place-based decision making–in any social or environmental context.</p>
      </div>
    </div>
  </div>
  <div class="span6">
    <div id="showcase" class="carousel">
    <!-- Carousel items -->
      <div class="carousel-inner">
      <div class="active item">
        <img src="assets/img/fsp.png">
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
        <img src="assets/img/fsp.png">
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