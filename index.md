---
title: Mathscapes Research
layout: default
---

# Mathscapes Research is committed to advance in the field of algorithm design through mathematical research.

[Learn more](about)

<hr/>

## Notes

<div class="posts">
<table style="width=100%">
  {% for post in site.posts %}
    {% include post_preview.html %}
  {% endfor %}
</table>
</div>

### Browse by Tags

<div>
{% for tag in site.tags %}
  <a href="{{ site.baseurl }}/notes/tag/{{ tag | first | downcase }}">#{{ tag | first }}</a>{% unless forloop.last %} &nbsp; {% endunless %}
{% endfor %}
</div>

<!-- ## Authors

<div>
{% for author in site.authors %}
  <a href="{{ author.url }}">{{ author.name }}</a>{% unless forloop.last %} &nbsp; {% endunless %}
{% endfor %}
</div> -->