<div style="font-size:0.9em">
{% assign pages_list = site.pages | sort: 'url' | where_exp: "item", "item.url contains '/latest/'" %}
{% for node in pages_list %}
  {% unless node.name == 'README.md' %}
      {% unless node.name == 'info.md' %}
        {% unless node.url == '/latest/' %}
          {% if node.url == page.url %}
&#42; {{ node.dir | remove_first: '/latest/' | replace: '_', ' ' | replace: '-', ' - '}}{{ node.name | 
remove_first: '.md' | remove_first: 'index' | replace: '_', ' ' | replace: '-', ' - ' }} <br>
          {% elsif node.url != page.url %}
&#42; <a href="{{ site.baseurl }}{{ node.url }}">{{ node.dir | remove_first: '/latest/' | replace: '_', ' ' | 
replace: '-', ' - ' }}{{ node.name | remove_first: '.md' | remove_first: 'index' | replace: '_', ' ' | replace: '-', ' - ' }}</a> <br>
          {% endif %}
        {% endunless %}
      {% endunless %}
  {% endunless %}
{% endfor %}
</div>