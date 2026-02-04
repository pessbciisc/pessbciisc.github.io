---
layout: default
title: Events
permalink: /events/
---

# Events

{% for e in site.data.events %}
<div class="card">
  <div class="card-title">{{ e.title }}</div>
  <div class="card-meta">{{ e.date }} · {{ e.venue }} · {{ e.status }}</div>
  {% if e.url %}<div><a href="{{ e.url }}">Details</a></div>{% endif %}
</div>
{% endfor %}
