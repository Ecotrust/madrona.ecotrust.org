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
								{% if post.complete %}
								<a href="{{ post.url}} "><img class="thumbnail" src="{{ BASE_PATH }}{{ post.image }}"/></a>
								{% else %}
								<img class="thumbnail" src="{{ BASE_PATH }}{{ post.image }}"/>
								{% endif %}
							</div>
							<div class="span4">
								<h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
								<p>{{ post.blurb }}	
									{% if post.complete %}						
										<a href="{{ post.url }}" class="pull-right btn btn-mini">Read More...</a>
									{% endif %}
								</p>
								<dl>
									{% if post.application %}
									<dt>Application</dt>
										<dd><a href="{{ post.application }}">{{ post.application }}</a></dd>
									{% endif %}
									{% if post.repo %}
									<dt>Source code</dt>
										<dd><a href="{{ post.repo }}">{{ post.repo }}</a></dd>
									{% endif %}
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