---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
{% for villain in site.villains %}
  <h2><a href="{{ villain.url }}">{{ villain.title }}</a></h2>
  <p>{{ villain.content | markdownify }}</p>
{% endfor %}
