---
layout: archive
permalink: /
title: ""
---

<div class="tiles">
{% for page in site.pages %}
    {% if page.layout == 'example' %}
    	{% include example-grid.html %}
    {% endif %}
{% endfor %}
</div><!-- /.tiles -->
