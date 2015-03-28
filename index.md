---
layout: archive
permalink: /
title: ""
---

<div class="tiles">
{% for page in site.pages %}
    {% if page.layout == 'snippet' %}
    	{% include snippet-grid.html %}
    {% endif %}
{% endfor %}
</div><!-- /.tiles -->
