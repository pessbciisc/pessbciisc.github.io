---
layout: default
---

# {{ site.data.chapter.name }}
<p class="kv">{{ site.data.chapter.tagline }}</p>

## Upcoming events
{% assign upcoming = site.data.events | where: "status", "upcoming" %}
{% for e in upcoming %}
<div class="card">
  <div><strong>{{ e.title }}</strong></div>
  <div class="kv">{{ e.date }} · {{ e.venue }}</div>
  {% if e.url %}<div><a href="{{ e.url }}">Event link</a></div>{% endif %}
</div>
{% endfor %}
