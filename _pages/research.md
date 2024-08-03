---
layout: page
title: Research
permalink: /research/
order: 5
---
My research interests broadly encompass geometric deep learning and graph representation learning. I am driven by questions such as - Can we design deep learning models that can naturally encode symmetries without explicit guidance? How can we introduce non-Euclidean spaces as geometrical inductive biases for learning efficient representations of the data, especially graphs? I am also interested in finding interesting applications for modeling molecular data and biological networks. I am currently working on improving the generalization ability of GNNs by tackling problems like over-squashing and over-smoothing.





### Papers

{% for paper in site.data.publications %}
* [{{ paper.title }}]({{ paper.url }}) <br>
  {% for author in paper.authors %}{% if author == "Adarsh Jamadandi" %}**{{ author }}**{% else %}{{ author }}{% endif %}{% if forloop.last %}{% else %}, {% endif %}{% endfor %}.
  {{ paper.venue }}, {{ paper.year }}.
{% endfor %}

