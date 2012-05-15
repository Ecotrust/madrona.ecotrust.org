---
layout: page
title: madrona spatial planning framework
---
{% include JB/setup %}

<div class="row">
  <div class="span6">
    <div class="row">
      <div class="span6">
        <p>A framework for building spatial planning tools at any scale.</p>
      </div>
    </div>
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
    </div>
    <div class="row">
      <div class="span6">
        <p class="madrona-text">Madrona offers a flexible set of building blocks and design patterns for software development. Our support services can help you develop and implement cutting-edge tools for effective place-based decision making.</p>
      </div>
    </div>
  </div>
  <div class="span6">
    {% include carousel.html %}
   </div>
</div>
<script>
  $(window).load(function() {
    $('.carousel').carousel({
      interval: 8000
    })
    
  });
</script>