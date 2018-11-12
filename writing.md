---
title: Writing
permalink: /writing/
---

<div class="content">
  {% if site.posts.size > 0 %}
    {% for post in site.posts %}
      <div class="post-list">
        <h2 class="post-title">
        <a href="{{ post.url }}">{{ post.title }}</a>
      </h2> {% if post.description %}
        <p>{{ post.description }}</p>
        {% endif %}
        <div class="post-date">
            <time>{{ post.date | date_to_string }}</time>
        </div>
      </div>
    {% endfor %}
  {% else %}  
    <h2>No post found</h2> 
  {% endif %}
</div>
