---
layout: default
title: Archive
permalink: /archive
---
# Archive

<ul class="post-list archive-ul">
  {% for post in site.categories.page %}
    <li class="archive-li">
      <h3>
        {{ post.date| date: "%m-%d-%Y" }} - 
        p.{{post.number}}: 
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h3>
    </li>
  {% endfor %}
</ul>