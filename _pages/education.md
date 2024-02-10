---
permalink: /education/
title: "Education"
layout: home
author_profile: true
#modified: 2022-03-21
---


<h2> Education </h2>
<ul>
{% for study in site.data.cv.education %}
<li>
    <strong>{{ study.degree }}</strong> ({{ study.area }}). 
    {{ study.school }}; {{ study.location }} ({{ study.endDate }})
</li>
{% endfor %}
</ul>

<h2> Awards </h2>
<ul>
{% for award in site.data.cv.awards %}
<li>
    {{ award.title }} (Awarded by {{ award.awarder }}) - ({{ award.date }}) 
</li>
{% endfor %}
</ul>

