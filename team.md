---
layout: default
title: Charlottesville Racing Club Teams
permalink: /team/
---

## {{ page.title }}

The Charlottesville Racing Club competes in numerous categories, and there is at least one captain for each. Many members participate in more than one discipline. In addition to official races, team captains often organize one group ride per month. If you interested, reach out to the captain and consider [joining]({{site.baseurl}}/join) CRC.

<ul>
{% for page in site.team %}
{% assign sorted = site.team | sort:"order" %}
	<div class="row section">
	    <div class="col-md-3 text-center">
		{% if page.image %}
		<img src="{{site.baseurl}}/images/{{page.image}}" alt="{{page.title}}" class="block-image"/>
		{% endif %}        
	    </div>
	    <div class="col-md-9">
		<h4>{{page.title}}</h4>
		<p>{{page.description}}</p>
	    </div>
	</div>
{% endfor %}
</ul>
