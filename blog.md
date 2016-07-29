---
layout: page
title: Blog Posts / Articles
permalink: /blog/
---
<hr>
<div class="posts">
  {% for post in site.posts %}
    <article class="post">
    	<b>{{ post.title }}</b> 
    	<span class="date-post"> Written on {{ post.date | date: "%B %e, %Y" }} by Chris Joy.</span>
     
      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>

    </article>
  {% endfor %}
</div>
