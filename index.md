---
layout: page
title: Computing Bits and Bytes
---

<div class="latest-post">
  {% if site.posts.size > 0 %}
    {% assign latest_post = site.posts.first %}
    <article>
      <h1>{{ latest_post.title }}</h1>
      <p class="post-meta">Published on {{ latest_post.date | date: "%B %d, %Y" }}</p>
      <div class="excerpt">
        {{ latest_post.content | truncatewords: 150 | markdownify }}
      </div>
      <a class="read-more" href="{{ latest_post.url }}">Read More</a>
    </article>
  {% else %}
    <p>No posts available yet. Check back soon!</p>
  {% endif %}
</div>