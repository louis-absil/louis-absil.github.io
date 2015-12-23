---
layout: default
title: Enregistrements
nav: Enregistrements
permalink: /files/
---

<!-- Timeline
================================================== -->
<h2>Enregistrements</h2>
<ul class="timeline">
{% for file in site.files %}
    <li class="timeline-inverted">
      <div class="timeline-badge danger"><i class="glyphicon glyphicon-music"></i></div>
      <div class="timeline-panel">
       <div class="timeline-heading">
       <a href="{{ file.url | prepend: site.baseurl }}"><h4 class="timeline-title">{{ file.title }}</h4></a>
       </div>
       <div class="timeline-body" background-color="white">
         {% if file.comment %}<p>{{ file.comment }}</p>{% endif %}
       </div>
      </div>
    </li>
{% endfor %}
</ul>
