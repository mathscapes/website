---
title: Home
layout: default
---
<img src="assets/images/logo.svg" width="200px">
<h1>Mathscapes Research is committed to advance in the field of algorithm design through mathematical research.</h1>

<hr/>
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

        <h2 class="home"><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
        <p class="date">
        {{ post.author }} /
        {{ post.date | date: "%B %e, %Y" }} /
        Posted in {{ post.categories }} /
        Tagged as 
        {% for c in post.tags %}
            {% if forloop.last == false %}
            {{ c }},
            {% else %}
            {{ c }}
            {% endif %}
        {% endfor %}
        </p>

    </article>
  {% endfor %}
</div>