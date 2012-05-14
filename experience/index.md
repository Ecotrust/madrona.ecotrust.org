---
layout: page
title: madrona spatial planning framework
active: experience
---
{% include JB/setup %}
<div class="row experience">
	<div class="span8">
		<h2>Madrona Projects</h2>
		<p>The Madrona framework has been used to build planning tools for a variety of environments.</p>
		<div class="row">
			<div class="span8">
				{% for post in site.posts %}
					{% if post.category contains "experience" %}
					<div class="project">
						<div class="row">
							<div class="span4">
								<a href="{{ post.url}} "><img class="thumbnail" src="{{ BASE_PATH }}{{ post.image }}"/></a>
							</div>
							<div class="span4">
								<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
								<p>{{ post.blurb }}							
									<a href="{{ post.url }}" class="pull-right btn btn-mini">Read More...</a>
								</p>
								<dl>
									<dt>Application</dt>
										<dd><a href="{{ post.application }}">{{ post.application }}</a></dd>
									<dt>Source code</dt>
										<dd><a href="{{ post.source }}">{{ post.source }}</a></dd>
								</dl>
							</div>
						</div>
					</div>
					{% endif %}
				{% endfor %}
			</div>
		</div>
	</div>
	<div class="span4">
		{% include experience/accordion.html %}
	</div>
</div>