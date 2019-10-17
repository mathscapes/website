---
title: Mathscapes Research
layout: default
---

<img class="animated fadeInDown" src="/assets/images/process.svg" style="margin-bottom: 2em; margin-top: 2em; max-width: 500px;">

<center>
<h1 class="animated fadeInDown">Mathscapes is committed to advance in the field of algorithm design through mathematical research.</h1>
</center>

<!-- <center>
<p style="max-width:650px;">Based in Bangalore, Mathscapes study and design algorithms for computational problems. We see algorithmic complexity more than just space and time; and examine how maths may be used to discover and build on other possible parameters that contribute to this complexity.</p>
</center> -->


<center class="animated fadeIn delay-1s">
<a class="btn" href="about">Learn more</a><a class="primary-btn" href="about">Consult Mathscapes <ion-icon name="arrow-round-forward" style="color:white;"></ion-icon></a><br/>
<p class="tertiary">Not sure how we can help you? <ion-icon name="mail"></ion-icon> <a href="mailto: hello@mathscapes.xyz">Contact us</a> to talk about how we can create a unique collaboration opportunity.</p>
</center>

<hr/>

## <ion-icon name="list-box"></ion-icon> Notes
<p style="max-width: 500px;">Notes is where we publish about our current projects and activities, including insights into our design approach and practice.</p>

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