---
layout: page
title: madrona spatial planning framework
active: developer
---
<h1>Developer</h1>
<div class="row">
  <div class="span8">
    <div class="bugs developer">
      <div class="row">
        <div class="span8">
          <p>Take the latest Madrona release for a test drive with our VirtualBox appliance or get up and running from scratch on Windows, Linux or Mac.  Let our step-by-step tutorials guide you.</p>
        </div>
      </div>
      <div class="row">        
        <div class="span4">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3>
                    <img  src="{{ BASE_PATH }}/assets/img/download.png"><span> Download</span>
                  </h3>
                </div>
                <div class="text">
                  <ul class="unstyled">
                    <li><a href="{{ BASE_PATH }}/developer/appliance">Madrona appliance</a></li>
                    <li><a href="https://github.com/Ecotrust/madrona/downloads">4.0 Release</a></li>
                  </ul>
                </div>
              </div>
            </div>
        </div>
        <div class="span4">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><a href="http://ecotrust.github.com/madrona/docs/tutorial.html"><img src="{{ BASE_PATH }}/assets/img/tutorials.png"><span> Tutorials</span></a></h3>
                </div>
                <div class="text">
                  <ul class="unstyled">
                    <li><a href="http://ecotrust.github.com/madrona/docs/tutorial_appgen.html">Madrona appliance</a></li>
                    <li><a href="http://ecotrust.github.com/madrona/docs/tutorial_create.html">Your first Madrona project</a></li>
                  </ul>
                </div>
              </div>
            </div>
        </div>
      </div>
      <div class="row">
        <div class="span8">
          <p>Madrona is an open book and there's always room for more authors.  Follow along and collaborate with us using powerful community tools.</p>
        </div>        
        <div class="span4">            
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3>
                    <img  src="{{ BASE_PATH }}/assets/img/github.png"><span> Madrona on Github</span>
                  </h3>
                </div>
                <div class="text">
                  <ul class="unstyled">
                    <li><a href="http://www.github.com/ecotrust/madrona">Source Code</a></li>
                    <li><a href="http://www.github.com/ecotrust/madrona/issues">Issues</a></li>
                  </ul>
                </div>
              </div>
            </div>
        </div>      
        <div class="span4">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><img src="{{ BASE_PATH }}/assets/img/hourglass.png"><span> Project Status</span></h3>
                </div>
                <div class="text">
                  <ul class="unstyled">
                    <li><a href="{{ BASE_PATH }}/developer/roadmap.html">Roadmap</a></li>
                    <li><a href="{{ BASE_PATH }}/developer/roadmap.html">Open Source License</a></li>                                       
                  </ul>
                </div>
              </div>
            </div>
        </div>
      </div>
      <div class="row">        
        <div class="span8">
          <p>Many aspects of Madrona have been meticulously documented and tested.  It's worth the time to dig in.  If you're looking for a way to contribute this is a great place.</p>
        </div>        
        <div class="span4">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><a href="http://ecotrust.github.com/madrona/docs/index.html"><img src='{{ BASE_PATH }}/assets/img/documentation.png'/><span> Documentation</span></a></h3>
                </div>
                <div class="text">
                  <ul class="unstyled">
                    <li><a href="http://ecotrust.github.com/madrona/docs/deployment.html">Deployment</a></li>
                    <li><a href="http://ecotrust.github.com/madrona/docs/#api">API</a></li>                                       
                  </ul>
                </div>
              </div>
            </div>
        </div>
        <div class="span4">
            <div class="bug">
              <div class="row">
                <div class="header">
                  <h3><img src="{{BASE_PATH}}/assets/img/testing.png"/><span> Testing</span></h3>
                </div>
                <div class="text">
                  <ul class="unstyled">
                    <li><a href="http://ecotrust.github.com/madrona/docs/coverage/index.html">Unit tests</a></li>
                    <li>&nbsp;</li>                                       
                  </ul>
                </div>  
              </div>
            </div>
        </div>                
      </div>      
    </div>
    <div class="row">
      <div class="span4">
      </div>
    </div>
  </div>
  <div class="span4">
    <h3>Recent Commits</h3>
     <table id="commits-table" class="table table-striped table-condensed table-bordered">
      <tbody data-bind="foreach: $data">
        <tr class="commits-row" data-bind="attr: { 'data-content': commit.message }">
          <td><span data-bind="text: author.login"></span></td>
          <td><a data-bind="attr: { href: getCommitUrl(url()) }"><span data-bind="text: commit.message"></span></a></td>
          <td><span data-bind="text: formatDate(commit.author.date())"></span></td>
        </tr>
      </tbody>
    </table>
    <h3>Recent Issues</h3>
     <table id="issues-table" class="table table-striped table-condensed table-bordered">
      <tbody data-bind="foreach: $data">
        <tr class="issue-row" data-bind="attr: { 'data-content': body, 'data-original-title': 'Issue Text' }">
          <td><span data-bind="text: user.login"></span></td>
          <td><a data-bind="attr: { href: html_url } "><span data-bind="text: title"></span></a></td>
          <td><span data-bind="text: formatDate(updated_at())"></span></td>
        </tr>
      </tbody>
    </table>
   </div>
</div>


<script>
var viewModel = {};

window.getCommitUrl = function(url) {
  var base = 'https://github.com/Ecotrust/madrona/commit/',
      urlParts = url.split('/');
      return base + urlParts[urlParts.length-1];
}

window.formatDate = function(dateString) {
  var date = new Date(Date.parse(dateString));
  return [ date.getMonth() + 1, date.getDate(), date.getFullYear()].join('/');
}


$(document).ready(function () {
  var popoverOptions = {
    placement: 'bottom',
    html: true
  }
  
  $.ajax({
    url: 'https://api.github.com/repos/ecotrust/madrona/commits?per_page=5',
    method: 'GET',
    dataType: 'jsonp',
    success: function (res) {
      viewModel.commits = ko.mapping.fromJS(res.data);
      ko.applyBindings(viewModel.commits, document.getElementById('commits-table'));
      // $(".commits-row").popover(popoverOptions);
    }});
  $.ajax({
    url: 'https://api.github.com/repos/ecotrust/madrona/issues?per_page=5',
    method: 'GET',
    dataType: 'jsonp',
    success: function (res) {
      viewModel.issues = ko.mapping.fromJS(res.data);
      ko.applyBindings(viewModel.issues, document.getElementById('issues-table'));
      $(".issue-row").popover(popoverOptions);

    }});


})
</script>