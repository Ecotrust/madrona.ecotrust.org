---
layout: page
title: madrona spatial planning framework
active: experience
---
{% include JB/setup %}
<div class="row experience">
	<div class="span8">
		<h2>Madrona Projects</h2>
		<p>Madrona is at the heart of a growing number of planning tools.  In each case it has been customized for a specific audience, process, and scale.  The science of decision making and stakeholder engagement is as important as the technology itself.</p>
		<div class="row">
			<div class="span8">
				{% for post in site.categories.experience reversed %}
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
								<h3>									
									{{ post.title }}
								</h3>
								<p>{{ post.blurb }}	
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
								{% if post.complete %}						
									<a href="{{ post.url }}" class="pull-right btn btn-mini">Read More...</a>
								{% endif %}
							</div>
						</div>
					</div>
				{% endfor %}
			</div>
		</div>
	</div>
	<div class="span4">
		<div class="row">
			<div class="span3 offset1">
			<!--{% include experience/accordion.html %}-->
			</div>
		</div>
	</div>
</div>