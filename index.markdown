---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
title: Home 
---




<section class="recent-posts">
  <h2>Recent Posts</h2>

  {% for post in site.posts limit:5 %}
    <div class="post-preview">
      <a href="{{ post.url }}">{{ post.title }}</a>
      <small>{{ post.date | date: "%Y-%m-%d" }}</small>
      <p>{{ post.excerpt }}</p>
    </div>
  {% endfor %}
</section>
