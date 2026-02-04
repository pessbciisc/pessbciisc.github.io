---
layout: page
title: Officers
permalink: /officers/
---

{% for p in site.data.officers %}
<div class="card">
  <div><strong>{{ p.role }}</strong> ({{ p.term }})</div>
  <div>{{ p.name }}</div>
  {% if p.email %}<div class="kv"><a href="mailto:{{ p.email }}">{{ p.email }}</a></div>{% endif %}
</div>
{% endfor %}
