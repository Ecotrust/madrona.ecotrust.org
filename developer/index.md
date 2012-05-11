---
layout: page
title: madrona spatial planning framework
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
                  <img  src="{{ BASE_PATH }}/assets/img/github.png">
                </div>
                <div class="pull-left">
                  <h4>Madrona on Github</h4>
                  <p>define, sketch, share</p>
                </div>
              </div>
            </div>
          </a>
        </div>
        <div class="span3">
          <a href="http://ecotrust.github.com/madrona/docs/">
            <div class="bug">
              <div class="row">
                <div class="pull-left icon">
                  <img src="{{ BASE_PATH }}/assets/img/documentation.png">
                </div>
                <div class="pull-left">
                  <h4>Documentation</h4>
                  <p>public and private</p>
                </div>
              </div>
            </div>
          </a>
        </div>
      </div>
    </div>
    <div class="row">
      <div class="span6">
      </div>
    </div>
  </div>
  <div class="span6">
    <h3>Commits</h3>
     <table id="commits-table" class="table table-striped table-condensed table-bordered">
      <tbody data-bind="foreach: $data">
        <tr>
          <td><span data-bind="text: author.login"></span></td>
          <td><a data-bind="attr: { href: url }"><span data-bind="text: commit.message"></span></a></td>
          <td><span data-bind="text: formatDate(commit.author.date())"></span></td>
        </tr>
      </tbody>
    </table>
    <h3>Issues</h3>
     <table id="issues-table" class="table table-striped table-condensed table-bordered">
      <tbody data-bind="foreach: $data">
        <tr>
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

window.formatDate = function(dateString) {
  var date = new Date(Date.parse(dateString));
  return [ date.getMonth() + 1, date.getDate(), date.getFullYear()].join('/');
}


$(document).ready(function () {

  
  $.ajax({
    url: 'https://api.github.com/repos/ecotrust/madrona/commits?per_page=5',
    method: 'GET',
    dataType: 'jsonp',
    success: function (res) {
      viewModel.commits = ko.mapping.fromJS(res.data);
      ko.applyBindings(viewModel.commits, document.getElementById('commits-table'));
    }});
  $.ajax({
    url: 'https://api.github.com/repos/ecotrust/madrona/issues?per_page=5',
    method: 'GET',
    dataType: 'jsonp',
    success: function (res) {
      viewModel.issues = ko.mapping.fromJS(res.data);
      ko.applyBindings(viewModel.issues, document.getElementById('issues-table'));
    }});


})
</script>