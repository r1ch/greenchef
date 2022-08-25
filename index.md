---
layout: default
---
{% for file in site.static_files %}
  {% if file.path contains 'recipe' %}
      <a href="{{ file.path }}">
        {{file.path}}
      </a>
  {% endif %}
{% endfor %}
