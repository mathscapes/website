---
title: Mathscapes Research
layout: default
---

# Mathscapes Research is committed to advance in the field of algorithm design through mathematical research.
Based in Bangalore, Mathscapes study and design algorithms for computational problems. We see algorithmic complexity more than just space and time; and examine how maths may be used to discover and build on other possible parameters that contribute to this complexity.

<img src="{{ site.url }}/assets/images/process.svg" width="80%" style="margin-bottom: 3em; margin-top: 3em;">

[Learn more about Mathscapes](about)

<hr/>

## <ion-icon name="list-box"></ion-icon> Notes
Notes is where we publish about our current projects and activities, including insights into our design approach and practice.

<div class="posts">
<table style="width=100%">
  {% for post in site.posts %}
    {% include post_preview.html %}
  {% endfor %}
</table>
</div>

### <ion-icon name="pricetags"></ion-icon> Browse by Tags

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