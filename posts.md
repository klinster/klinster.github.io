---
layout: page
title: Posts
permalink: /posts/
---

#### A place to put my musings down

<ul>
  {% for post in site.posts %}
    <li>
    <hr />
      <h4>
        <a href="{{ post.url | prepend: site.baseurl }}">{{ post.title | escape }}</a>
      </h4>
      <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
