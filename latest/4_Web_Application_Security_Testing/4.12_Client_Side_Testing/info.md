{% assign pages_list = site.pages | where_exp: "item", "item.url contains '/latest/'" %}
{% for node in pages_list %}
  {% unless node.name == "README.md"%}
    {% unless node.name == "index.md" %}
      {% unless node.name == "info.md" %}
        {% if node.url == page.url %}
{{ node.name | remove_first: '.md' }}
        {% elsif node.url != page.url %}
<a href="{{ site.baseurl }}{{ node.url }}">{{ node.name | remove_first: '.md' }}</a>
        {% endif %}
      {% endunless %}
    {% endunless %}
  {% endunless %}
{% endfor %}