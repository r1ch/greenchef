---
layout: default
---


{% for recipe in site.recipes %}
  {{recipe | jsonify}}
{% endfor %}
