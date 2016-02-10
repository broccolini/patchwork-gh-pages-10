---
layout: page
title: Blog
permalink: /blog/
---

  <ul class="post-list">
    {% for post in site.posts %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
        <p class="post-excerpt"><em>{{ post.excerpt }}</em></p>
      </li>
    {% endfor %}
  </ul>

  <p class="rss-subscribe">Subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
