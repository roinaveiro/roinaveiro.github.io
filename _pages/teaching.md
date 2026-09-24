---
layout: minimal
title: "Teaching"
permalink: /teaching/
author_profile: false
description: "Open teaching materials by Roi Naveiro in machine learning, Bayesian methods, data analysis, and stochastic processes."
---

Selected courses with open teaching materials. My [CV](/cv/) includes further teaching experience.

<ul class="course-list">
{% for course in site.data.teaching %}
  <li>
    <h3>{{ course.title }}</h3>
    <p class="course-meta">{{ course.institution }} · {{ course.date }}</p>
    <p>{{ course.description }}</p>
    <p class="course-links">{% for link in course.links %}<a href="{{ link.url }}">{{ link.label }}</a>{% endfor %}</p>
  </li>
{% endfor %}
</ul>
