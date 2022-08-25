---
layout: default
---

{% for file in site.static_files %}
        <h2>{{ file | jsonify }}</h2>
<a href = '{{file.path}}'>File</a>
        {% for item in site.static_files[file] %}
            {{item}}
            <a href = '{{file.path}}'>{{item}}</a>
        {% endfor %}
{% endfor %}
