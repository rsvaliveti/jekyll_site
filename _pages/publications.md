---
title: "Publications"
permalink: /publications/
layout: home
author_profile: true
---

{% if site.author.googlescholar %}
  You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.
{% endif %}


<h2> Refereed journal articles </h2>
{% bibliography --query @article %}

<h2> Refereed conference proceedings </h2>
{% bibliography --query @inproceedings %}

