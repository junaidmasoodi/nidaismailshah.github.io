---
layout: blogpage
title: Blog
permalink: /blog/
---

<ul class="posts">
    {% for post in site.posts %}
      <li>
        <!--<span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>-->
        <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
         {{post.excerpt}}
      </li>
    {% endfor %}
  </ul>
  