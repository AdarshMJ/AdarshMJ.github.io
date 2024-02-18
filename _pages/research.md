---
layout: page
title: Research
permalink: /research/
order: 5
---
My research interests include Graph Representation Learning and Geometric Deep Learning. More specifically, I am interested in leveraging ideas from differential geometry and/or physics to design better representation learning algorithms for graphs.

### Papers

{% for paper in site.data.publications %}
* [{{ paper.title }}]({{ paper.url }}) <br>
  {% for author in paper.authors %}{% if author == "Adarsh Jamadandi" %}**{{ author }}**{% else %}{{ author }}{% endif %}{% if forloop.last %}{% else %}, {% endif %}{% endfor %}.
  {{ paper.venue }}, {{ paper.year }}.
{% endfor %}

