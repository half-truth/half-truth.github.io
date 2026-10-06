---
layout: default
---


<h1>What I Read</h1>

<div class="posts">
  {% for post in site.posts %}
    <article class="post">

   
      <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>

 
      <small>{{ post.date | date: "%-d %B %Y" }}</small>

     
      <div class="entry">
        {{ post.content }}
      </div>

     
      <hr>

    </article>
  {% endfor %}
</div>
