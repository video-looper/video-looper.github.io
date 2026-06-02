# Gallery

{% for page in site.pages %}
  {% if page.path contains "gallery/" and page.name != "index.md" %}
- [{{ page.title }}]({{ page.url | relative_url }})
  {% endif %}
{% endfor %}
