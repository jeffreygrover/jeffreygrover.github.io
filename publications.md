---
layout: page
permalink: /publications/
title: publications
description: A listing of my scientific publications
---

<ul class="post-list">
{% for poem in site.publications reversed %}
    <li>
        <h2><a class="poem-title" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a></h2>
        <p class="post-meta">{{ poem.date | date: '%B %-d, %Y — %H:%M' }}</p>
      </li>
{% endfor %}
</ul>
