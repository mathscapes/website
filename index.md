---
title: Home
layout: default
---

# Mathscapes Research is committed to advance in the field of algorithm design through mathematical research.

[Learn more](about)

<hr/>

## Notes

<!-- <div class="tags">
  {% for tag in site.tags %}
    <a href = "{{ site.url }}/notes/tag/{{ tag | first }}">#{{ tag | first }}</a> 
  {% endfor %}
</div> -->

<div class="posts">
<table style="width=100%">
  {% for post in site.posts %}
    {% include post_preview.html %}
  {% endfor %}
</table>
</div>