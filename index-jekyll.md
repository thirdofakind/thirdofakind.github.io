---
layout: page
title: Home
---

# Hadley Edwards
Designer & AI/Data — I build visual systems and practical tools.

<div class="grid cols-3">
  {% assign featured = site.projects | sort: 'weight' %}
  {% for p in featured limit:6 %}
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

<p style="margin-top:1rem">
  <a class="btn" href="{{ '/work' | relative_url }}">See all projects →</a>
  <a class="btn" href="{{ '/about' | relative_url }}">About →</a>
</p>
