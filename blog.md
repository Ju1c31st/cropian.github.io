---
layout: page
title: Blog Posts / Articles
permalink: /blog/
---
<hr>
<div class="posts">
  {% for post in site.posts %}
    <article class="post">

    <h3>
      	<a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> 
      	<span class="date-post"> Written on {{ post.date | date: "%B %e, %Y" }} </span>
	  </h3> 
      
      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>

    </article>
  {% endfor %}
</div>