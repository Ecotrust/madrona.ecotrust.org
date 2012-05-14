---
layout: page
title: Prioritizing Aquatic Conservation
category: [experience]
application: http://aquatic-priorities.apps.ecotrust.org/
source: https://github.com/Ecotrust/aquatic-priorities
blurb: U.S. Fish and Wildlife Service wanted to see the big picture of conservation and restoration work at the sub-basin scale across the Pacific Northwest.
image: /assets/img/experience/aqua-priorities.png
technology: ["Madrona framework", "Google Earth", "Marxan conservation planning software"]
name: Mike Mertens
phone: 503-467-0775
email: mikem@ecotrust.org
---
<div class="row">
	<div class="span8">
		<h1>Prioritizing Aquatic Conservation</h1>
		<p>{{page.blurb}}</p>
		<div class="row">
			<div class="span4">
				<h3>The Challenges</h3>
				<p>How might U.S. Fish and Wildlife Service (USFWS) prioritize conservation and restoration activities across a broad geography?</p>
				<p>Could technology help the agency evaluate and compare the potential effects of climate change and invasive species on multiple species?</p>
				<p>Could the platform enable iterative and adaptive analysis and decision making?</p>
			</div>
			<div class="span4">
				<a href="{{ page.application }}"><img class="thumbnail" src="{{ BASE_PATH }}{{ page.image }}"/></a>
			</div>
		</div>
		<h3>Our Approach</h3>
		<p>Ecotrust and USFWS sought out and incorporated the work of numerous collaborators, including USDA Forest Service, NOAA Fisheries, and the Oregon Watershed Enhancement Board. We compiled existing data on aquatic species of interest, watershed conditions, climate change projections, and the spread of invasive species. We developed a decision support model, and used the Madrona framework as an interface for users to query the model. The platform allows users to adjust input parameters as they analyze, map, and share the results. We also developed an online tutorial to guide users through the process of prioritization.</p>
		<div class="row">
			<div class="span4">
				<h3>Technology</h3>
				<ul>
					{% for tech in page.technology %}
					<li>{{tech}}</li>
					{% endfor %}
				</ul>
			</div>
			<div class="span4">
				<dl>
					<dt>Application</dt>
						<dd><a href="{{ page.application }}">{{ page.application }}</a></dd>
					<dt>Source code</dt>
						<dd><a href="{{ page.source }}">{{ page.source }}</a></dd>
				</dl>
			</div>
		</div>
		<h3>Contact</h3>
		<p>For more information, email {{ page.name }} at <a href="{{ page.email }}">{{ page.email }}</a> or call {{ page.phone }}.</p>
	</div>
	<div class="span4">
		{% include experience/accordion.html %}
	</div>
</div>