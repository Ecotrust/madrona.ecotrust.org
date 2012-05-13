---
layout: page
title: madrona spatial planning framework
active: developer
---
{% include JB/setup %}
<div class="row">
  <div class="span6">
    <div class="bugs">
      <div class="row">
        <div class="span6">
          <p>Take the latest Madrona release for a test drive with our VirtualBox appliance or get up and running from scratch.  Let our step-by-step tutorials guide you.</p>
        </div>
      </div>
      <div class="row">        
        <div class="span3">
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <a href="http://www.github.com/ecotrust/madrona">
                    <img  src="{{ BASE_PATH }}/assets/img/download.png">
                  </a>
                </div>
                <div class="pull-left">
                  <h4><a href="https://github.com/Ecotrust/madrona/downloads">Download</a></h4>
                  <ul class="unstyled">
                    <li><a href="https://github.com/Ecotrust/madrona/wiki/Madrona-Virtual-Machine">Madrona Appliance</a></li>
                    <li><a href="https://github.com/Ecotrust/madrona/downloads">4.0 Release</a></li>
                  </ul>
                </div>
              </div>
            </div>
        </div>
        <div class="span3">
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <a href="http://ecotrust.github.com/madrona/docs/"><img src="{{ BASE_PATH }}/assets/img/documentation.png"></a>
                </div>
                <div class="pull-left">
                  <h4><a href="http://ecotrust.github.com/madrona/docs/">Documentation</a></h4>
                  <ul class="unstyled">
                    <li><a href="http://ecotrust.github.com/madrona/docs/tutorial_appgen.html">Tutorial - appliance</a></li>
                    <li><a href="http://ecotrust.github.com/madrona/docs/tutorial_scratch.html">Tutorial - from scratch</a></li>
                  </ul>
                </div>
              </div>
            </div>
        </div>
      </div>
      <div class="row">
        <div class="span6">
          <p>Madrona is an open book and there's always room for more authors.  Follow along and collaborate with us using powerful community tools.</p>
        </div>        
        <div class="span3">            
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <a href="http://www.github.com/ecotrust/madrona">
                    <img  src="{{ BASE_PATH }}/assets/img/github.png">
                  </a>
                </div>
                <div class="pull-left">
                  <h4><a href="http://www.github.com/ecotrust/madrona">Madrona on Github</a></h4>
                  <ul class="unstyled">
                    <li><a href="http://www.github.com/ecotrust/madrona">Source Code</a></li>
                    <li><a href="http://www.github.com/ecotrust/madrona/issues">Issues</a></li>
                  </ul>
                </div>
              </div>
            </div>
        </div>      
        <div class="span3">
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <a href="http://ecotrust.github.com/madrona/docs/"><img src="{{ BASE_PATH }}/assets/img/hourglass.png"></a>
                </div>
                <div class="pull-left">
                  <h4><a href="http://ecotrust.github.com/madrona/docs/">Project Status</a></h4>
                  <ul class="unstyled">
                    <li><a href="{{ BASE_PATH }}/experience/history.html">History</a></li>
                    <li><a href="{{ BASE_PATH }}/developer/roadmap.html">Roadmap</a></li>
                    <li><a href="{{ BASE_PATH }}/developer/roadmap.html">Open Source License</a></li>                                        
                  </ul>
                </div>
              </div>
            </div>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="span6">
      </div>
    </div>
  </div>
  <div class="span6">
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