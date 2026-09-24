---
layout: minimal
title: "Research"
permalink: /publications/
author_profile: false
description: "Selected publications by Roi Naveiro on Bayesian inference, adversarial machine learning, optimization, and sequential decisions."
---

I study how to learn and make decisions under uncertainty, particularly when the data or the behavior of another agent may be strategic. My work includes adversarial machine learning, Bayesian optimization, and sequential games.

## Selected publications

The papers below give a selection of this work. For the full list, see [Google Scholar]({{ site.author.googlescholar }}).

<ul class="reading-list">
{% for paper in site.data.selected_publications %}
  <li>
    <h3><a href="{{ paper.url }}">{{ paper.title }}</a></h3>
    <p class="paper-authors">{{ paper.authors }}</p>
    <p class="paper-venue"><em>{{ paper.venue }}</em><span class="paper-year">{{ paper.year }}</span></p>
    {% if paper.preprint %}<p class="paper-links"><a href="{{ paper.preprint }}">Open preprint</a></p>{% endif %}
  </li>
{% endfor %}
</ul>
