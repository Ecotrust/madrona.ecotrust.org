---
layout: page
title: madrona spatial planning framework
---
{% include JB/setup %}
<div class="hero-unit">
  <div class="row-fluid">
  <div class="span12">
    {% include carousel.html %}
  </div>
</div>
</div>
<div class="row feature">
      <div class="span3">
        <a href="{{ BASE_PATH }}/technology/#Spatial-Features">
          <div class="bug">
            <div class="row">
              <div class="header">
                <h3><img src="{{ BASE_PATH }}/assets/img/features.png">
                  <span>Spatial&nbsp;Features</span>
                </h3>
              </div>
              <div class="text">
                <p>define, sketch, share</p>
              </div>
            </div>
          </div>
        </a>
      </div>
      <div class="span3">
          <a href="{{ BASE_PATH }}/technology/#Data-Layers">
          <div class="bug">
            <div class="row">
              <div class="header">
                <h3><img src="{{ BASE_PATH }}/assets/img/layers.png">
                  <span>Data Layers</span>
                </h3>
              </div>
              <div class="text">
                <p>public and private</p>
              </div>
            </div>
          </div>
        </a>
      </div>
      <div class="span3">
        <a href="{{ BASE_PATH }}/technology/#Collaboration">
          <div class="bug">
            <div class="row">
              <div class="header">
                <h3><img src="{{ BASE_PATH }}/assets/img/collaboration.png"><span class="wide">Collaboration</span></h3>
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
                <h3><img src="{{ BASE_PATH }}/assets/img/analysis.png"><span class="wide">Flexible Analysis</span></h3>
              </div>
              <div class="text">
                <p>visualize and report</p>
              </div>
            </div>
          </div>
        </a>
      </div>
</div>
<script>
  $(window).load(function() {
    $('.carousel').carousel({
      interval: 8000
    })
    
  });
</script>