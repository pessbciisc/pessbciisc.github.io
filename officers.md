---
layout: default
title: Officers
permalink: /officers/
---

# Officers

{% for p in site.data.officers %}
<div class="card">
  <div class="card-title">{{ p.role }} ({{ p.term }})</div>
  <div class="card-meta">{{ p.name }}</div>
  {% if p.email %}<div><a href="mailto:{{ p.email }}">{{ p.email }}</a></div>{% endif %}
</div>
{% endfor %}
