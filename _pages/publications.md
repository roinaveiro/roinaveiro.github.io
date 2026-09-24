---
layout: minimal
title: "Research"
permalink: /publications/
author_profile: false
description: "Selected publications by Roi Naveiro on Bayesian statistics, machine learning, optimization, decision theory, and their applications."
---

I develop statistical and computational methods for learning and decision-making under uncertainty. My interests span Bayesian inference, probabilistic machine learning, optimization, and decision theory.

I enjoy working across disciplines on exciting applications with practical impact, including molecular and materials design, health, and automated driving. Robustness and adversarial machine learning are also part of my research.

## Selected publications

The papers below give a selection of this work. For the full list, see [Google Scholar]({{ site.author.googlescholar }}).

<ul class="reading-list">
{% for paper in site.data.selected_publications %}
  <li>
    <h3><a href="{{ paper.url }}">{{ paper.title }}</a></h3>
    <p class="paper-authors">{{ paper.authors }}</p>
    <p class="paper-venue"><em>{{ paper.venue }}</em><span class="paper-year">{{ paper.year | default: paper.status }}</span></p>
    {% if paper.preprint %}<p class="paper-links"><a href="{{ paper.preprint }}">Open preprint</a></p>{% endif %}
  </li>
{% endfor %}
</ul>
