---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{% for file in site.static_files %}
  {% if file.extname == ".jpg" -%}
     * [{{ file.path }}]({{ site.baseurl }}{{ file.path }})
  {%- endif %}
{% endfor %}

{% for image in site.images %}
     {% if image.extname == 'jpg' %}
         <img src="{{ file.url }}" />
     {% endif %}
{% endfor %}
