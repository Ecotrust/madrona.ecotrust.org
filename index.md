---
layout: page
title: madrona spatial planning framework
---
{% include JB/setup %}
  <div class="row">
    <div class="span12">
      <h2 class="tagline">A framework for building spatial planning tools at any scale.</h2>
    </div>
  </div>
  <div class="row-fluid">
   <div class="span12">
    {% include carousel.html %}
    <hr/>
  </div>
  </div>
  <div class="row">
    <div class="span6">
      <p class="madrona-text">Madrona offers a flexible set of building blocks and design patterns for developing spatial planning and decision support tools. Our support services can help you implement cutting-edge tools for effective place-based decision making.</p>
    </div>
    <div class="span6">
    <div class="row feature">
      <div class="span3 bug">
        <a href="{{ BASE_PATH }}/technology/#Spatial-Features">
          <h3><img src="{{ BASE_PATH }}/assets/img/features.png">&nbsp;<span>Spatial&nbsp;Features</span></h3>
          <p>Provides a powerful spatial content management system complete with API...</p>
        </a>
      </div>
      <div class="span3 bug">
        <a href="{{ BASE_PATH }}/technology/#Data-Layers">
          <h3><img src="{{ BASE_PATH }}/assets/img/layers.png">&nbsp;<span>Data&nbsp;Layers</span></h3>
          <p>Manage a hierarchy of data layers important to your decision-making process...</p>
        </a>
      </div>
      <div class="span3 bug">
        <a href="{{ BASE_PATH }}/technology/#Collaboration">
          <h3><img src="{{ BASE_PATH }}/assets/img/collaboration.png">&nbsp;<span>Collaboration</span></h3>
          <p>The best ideas often evolve through connecting with other people....</p>
        </a>
      </div>
      <div class="span3 bug">
        <a href="{{ BASE_PATH }}/technology/#Flexible-Analysis">
          <h3><img src="{{ BASE_PATH }}/assets/img/analysis.png">&nbsp;<span>Flexible&nbsp;Analysis</span></h3>
          <p>Interact with external modeling and analysis software such as Grass, Marxan or ArcGIS Server...</p>
        </a>
      </div>
     <!--
    <div class="row feature">
      <div class="span3">
        <a href="{{ BASE_PATH }}/technology/#Collaboration">
          <div class="bug">
            <div class="row">
              <div class="header">
                <h4><img src="{{ BASE_PATH }}/assets/img/collaboration.png">&nbsp;<span class="wide">Collaboration</span></h4>
              </div>
              <div class="text">
                <p>consensus driven</p>
              </div>
            </div>
          </div>
        </a>
      </div>
      <div class="span3">
        <a href="{{ BASE_PATH }}/technology/#Flexible-Analysis">
          <div class="bug">
            <div class="row">
              <div class="header">
                <h4><img src="{{ BASE_PATH }}/assets/img/analysis.png">&nbsp;<span class="wide">Flexible Analysis</span></h4>
              </div>
              <div class="text">
                <p>visualize and report</p>
              </div>
            </div>
          </div>
        </a>
      </div>
    -->
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