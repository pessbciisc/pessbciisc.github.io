---
layout: default
---

<div class="hero">
  <h1>{{ site.data.chapter.name }}</h1>
  <p class="kv">{{ site.data.chapter.tagline }}</p>
</div>

## Upcoming events
{% assign upcoming = site.data.events | where: "status", "upcoming" %}
{% for e in upcoming %}
<div class="card">
  <div class="card-title">{{ e.title }}</div>
  <div class="card-meta">{{ e.date }} · {{ e.venue }}</div>
  {% if e.url %}<div><a href="{{ e.url }}">Details / Registration</a></div>{% endif %}
</div>
{% endfor %}
