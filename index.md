---
layout: page
description: Course website for Fundamentals of eDNA
---

<img src="img/favicon.png" alt="drawing" width="150"/>

This is the course website for Fundamentals of eDNA offered Srping 2021 at the University of Maine.

## Recent Reflections

<!-- Posts -->
<ul id="posts">

	{% for post in site.posts limit:3 %}

	  <li class="post">
	  	<h3><a href="{% if site.baseurl == "/" %}{{ post.url }}{% else %}{{ post.url | prepend: site.baseurl }}{% endif %}">{%if post.header %}{{ post.header }}{% else %}{{ post.title }}{% endif %}</a></h3><time datetime="{{ post.date | date_to_xmlschema }}" class="by-line"> <i>{{ post.date | date_to_string }}</i> </time>
	  	<span>{{ post.content | strip_html | truncatewords:50 }}</span>
	  </li>

    {% endfor %}

</ul>


#### Head to the Reflections tab for more!
