---
layout: default
---
{% for file in site.static_files %}
  {{file}}
  {{file.path}}
  {% if file.path contains 'recipe' %}
      <a href="{{ file.path }}">
        {{file.path}}
      </a>
  {% endif %}
{% endfor %}

{% for file in site.recipes %}
  {{file}}
  {{file.path}}
  {% if file.path contains 'recipe' %}
      <a href="{{ file.path }}">
        {{file.path}}
      </a>
  {% endif %}
{% endfor %}
