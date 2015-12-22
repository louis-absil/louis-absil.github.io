---
layout: default
title: Enregistrements
nav: Enregistrements
permalink: /files/
---

<h2> Enregistrements </h2>

<div class="list-group">
{% for file in site.files %}
  <a href="{{ file.url }}" class="list-group-item">
  <h4 class="list-group-item-heading">{{ file.title }}</h4>
    {% if file.description %}<p class="list-group-item-text">{{ file.description }}</p>{% endif %}</a>
{% endfor %}
</div>

