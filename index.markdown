---
layout: default
---

{% for file in site.static_files %}
  {% if file.extname == ".json" -%}
     [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
     <button type="button" class="btn btn-primary">Primary</button>
  {%- endif %}
{% endfor %}

<div class="alert alert-primary" role="alert">
  A simple primary alert—check it out!
</div>