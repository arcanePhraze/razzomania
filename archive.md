---
layout: default
title: Archive
permalink: /archive
---
# Archive

<ul class="post-list archive-ul">
  {% for post in site.categories.page %}
    <li class="archive-li">
      <h2>
        {{ post.date| date: "%m-%d-%Y" }} - 
        Page {{post.page}}: 
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
      </h2>
    </li>
  {% endfor %}
</ul>