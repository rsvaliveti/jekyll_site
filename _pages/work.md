---
permalink: /work/
title: "Work Experience"
layout: home
author_profile: true
#modified: 2022-03-21
---


{% for job in site.data.cv.work %}
<h2>{{ job.position }}, <em>{{ job.company }}</em>. 
({{ job.startDate | date: "%b %Y" }} - 
{% if job.endDate %}{{ job.endDate | date: "%b %Y" }}{% else %}Present{% endif %})
</h2>
<ul>
	{% for highlight in job.highlights %}
	<li> {{ highlight }} </li>
	{% endfor %}
</ul>
{% endfor %}
