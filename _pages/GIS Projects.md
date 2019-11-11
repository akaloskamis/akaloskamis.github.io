---
layout: GIS Projects
permalink: /GIS/
title: "GIS projects"
author_profile: true
header:
  image: "/images/Fotolia_108919730_M.jpg"
---


{% include base_path %}
{% include group-by-array collection=site.posts field="tags" %}

{% for tag in group_names %}
  {% assign posts = group_items[forloop.index0] %}
  <h2 id="{{ tag | slugify }}" class="archive__subtitle">{{ tag }}</h2>
  {% for post in posts %}
    {% include archive-single.html %}
  {% endfor %}
{% endfor %}
