---
layout: default
title: Blogs
category: blogs
---

<div class="posts">
  {% for post in site.posts %}
    {% if post.categories contains 'blogs' %}

    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

    <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>


    <!-- added by dummys */ -->
    <div class="line-separator"></div>

    {% endif %}
    {% endfor %}

</div>
