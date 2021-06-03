---
layout: layout
title: "关于"
---

<!-- You can edit this whole page, remove it, or use it as basis for any non-post pages you have. -->
<section class="content">

# {{ site.name }}

<ul class="listing">
<li>
<span>2020-2021学期</span><a href="{{ site.url }}/upcoming.html">下期组会</a>
</li>
  {% assign upcoming = (site.posts | where: "category" , "upcoming") %}
  {% for post in upcoming reversed %}
    {% if forloop.first %}
    <li style="text-indent: 2em;">
	<span>{{ post.date | date: "%B %e, %Y" }}</span> Next topic: <a href="{{ site.url }}{{ post.url }}">{{ post.title }}</a>
	</li>
    {% endif %}
  {% endfor %}
<li>
<a href="{{ site.url }}/previous.html">Previous Topics</a>
</li>
</ul>


## What:

同济大学-华中师范大学联合理论组会



</section>
