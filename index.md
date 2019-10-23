---
title: Mathscapes Research
layout: default
---

<img class="animated fadeInDown" src="/assets/images/process.svg" style="margin-bottom: 2em; margin-top: 2em; max-width: 500px;">

<center>
<h1 class="animated fadeInDown">Mathscapes is committed to advance in the field of <i>algorithm design</i> through <i>mathematical research</i>.</h1>
</center>

<center class="animated fadeIn delay-1s">
<a class="btn" href="about">Learn more</a><a class="primary-btn" href="about">Consult Mathscapes <ion-icon name="open" style="color:white;"></ion-icon></a><br/>
<p class="tertiary">Not sure how we can help you? <ion-icon name="mail"></ion-icon> <a href="mailto: hello@mathscapes.xyz">Contact us</a> to talk about how we can create a unique collaboration opportunity.</p>
</center>

<hr/>

## <ion-icon name="list-box"></ion-icon> Notes
<p>Notes is where we publish about our current projects and activities, including insights into our design approach and practice.</p>

<div class="posts">
<table style="width=100%">
  {% for post in site.posts %}
    {% include post_preview.html %}
  {% endfor %}
</table>
</div>

### <ion-icon name="pricetags"></ion-icon> Browse by Tags

<!-- <div>
{% for tag in site.tags %}
  <a class="tag" href="{{ site.baseurl }}/notes/tag/{{ tag | first | downcase | replace: ' ','-' }}">{{ tag | first }}</a>{% unless forloop.last %}{% endunless %}
{% endfor %}
</div> -->

<div>
{% capture site_tags %}{% for tag in site.tags %}{{ tag[1].size }}#{{ tag | first | downcase }}#{{ tag | first }}{% unless forloop.last %},{% endunless %}{% endfor %}{% endcapture %}
{% assign tag_hashes = site_tags | split:',' | sort %}

{% for hash in tag_hashes reversed%}
  {% assign keyValue = hash | split: '#' %}
  {% capture tag_word %}{{ keyValue[2] | strip_newlines }}{% endcapture %}
    <a class="tag" href="{{ site.baseurl }}/notes/tag/{{ tag_word | downcase | replace: ' ','-' }}">
      {{ tag_word }} <span class="count">{{ site.tags[tag_word].size }}</span>
    </a>
{% endfor %}
</div>

<!-- ## Authors

<div>
{% for author in site.authors %}
  <a href="{{ author.url }}">{{ author.name }}</a>{% unless forloop.last %} &nbsp; {% endunless %}
{% endfor %}
</div> -->