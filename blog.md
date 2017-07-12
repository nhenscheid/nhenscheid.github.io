---
layout: page
title: Blog
rank: 4
---

### Recent Posts
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{post.date | date: "%B %-d, %Y"}}: {{ post.title}}</a>
      {{ post.excerpt }}

    </li>
  {% endfor %}
</ul>


