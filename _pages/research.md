---
layout: page
title: Research
permalink: /research/
order: 5
---
My research interests broadly encompass graph representation learning and geometric deep learning. I am fascinated by questions such as

#### How important is the graph structure for Graph Neural Networks?
* How critical is the input graph for the downstream task? Can we determine a priori if the input graph contains sufficient information to solve the downstream task? The input graph plays a dual role: it provides the data for the GNN model and also serves as the computational structure upon which message-passing happens. This duality brings up another question: How do we know if we have an optimal computational structure for the learning task? Is the graph structure always relevant?

#### Generalization for Graph Neural Networks.
 * What does memorization mean in the context of GNNs? Do GNNs even memorize? How can we distinguish between memorization and graph structure overfitting?

#### Applications to biomedical/modeling molecular data.
* Designing deep neural networks for biomedical applications such as modeling protein structures, chemical molecules, accelerated drug-target interaction prediction etc.


### Papers

{% for paper in site.data.publications %}
* [{{ paper.title }}]({{ paper.url }}) <br>
  {% for author in paper.authors %}{% if author == "Adarsh Jamadandi" %}**{{ author }}**{% else %}{{ author }}{% endif %}{% if forloop.last %}{% else %}, {% endif %}{% endfor %}.
  {{ paper.venue }}, {{ paper.year }}.
{% endfor %}

