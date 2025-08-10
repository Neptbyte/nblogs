---
layout: default
title: My Awesome Website
---

# Hello, World!

Welcome to my personal website, powered by GitHub Pages and the elegant Cayman theme.

This is a great place to showcase my projects, share my thoughts, and connect with the community.

## About this Site

- **Easy to set up:** Thanks to Jekyll and the `remote_theme` feature, getting this site up and running was a breeze.
- **Clean design:** The Cayman theme provides a simple, responsive, and professional look.
- **Markdown-based:** All content is written in Markdown, making it easy to create and update posts.

### Latest Blog Posts

{% for post in site.posts %}
  <div class="post-item">
    <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
    <p class="post-meta">
      <span class="post-date">{{ post.date | date_to_string }}</span>
      {% if post.author %}
        <span> by {{ post.author }}</span>
      {% endif %}
    </p>
    <div class="post-excerpt">
      {{ post.excerpt }}
    </div>
  </div>
{% endfor %}

Happy reading!
