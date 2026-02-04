---
layout: page
title: Events
permalink: /events/
---

{% for e in site.data.events %}
<div class="card">
  <div><strong>{{ e.title }}</strong></div>
  <div class="kv">{{ e.date }} · {{ e.venue }} · {{ e.status }}</div>
  {% if e.url %}<div><a href="{{ e.url }}">Details / Registration</a></div>{% endif %}
</div>
{% endfor %}
