---
title: Blog Posts
permalink: /blog/
profile: true 
---

# Blog Posts

<ul id="post-list">
    {% for post in site.posts %}
        <li>
            <a href="{{ site.baseurl }}{{ post.url | remove_first: '/' }}"><aside class="dates">{{ post.date | date:"%b %d, %Y" }}</aside></a>
            <a href="{{ site.baseurl }}{{ post.url | remove_first: '/' }}">{{ post.title }} {{ post.description }}</a>
        </li>
    {% endfor %}
</ul>
 
{% include footer.html %}
