{% assign pages_list = site.pages | where_exp: "item", "item.url contains '/latest/'" %}
{% for node in pages_list %}
  {% unless node.name == "README.md"%}
    {% unless node.name == "index.md" %}
      {% unless node.name == "info.md" %}
<a href="{{ node.url }}">{{ node.name }}</a>
      {% endunless %}
    {% endunless %}
  {% endunless %}
{% endfor %}