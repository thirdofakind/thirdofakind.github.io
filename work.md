---
layout: page
title: Work
permalink: /work/
---

A mix of brand systems, motion, and data tooling.

<div class="grid cols-3">
  {% assign sorted = site.projects | sort: 'weight' %}
  {% for p in sorted %}
  <a class="card" href="{{ p.url | relative_url }}">
    {% if p.hero %}
      <img class="card-thumb" src="{{ p.hero | relative_url }}" alt="{{ p.title }} thumbnail">
    {% else %}
      <div class="card-thumb"></div>
    {% endif %}
    <div class="card-body">
      <h3 class="card-title">{{ p.title }}</h3>
      <p class="card-summary">{{ p.summary }}</p>
    </div>
  </a>
  {% endfor %}
</div>
