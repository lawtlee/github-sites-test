---
layout: default
title: Blogs
---

Hello these are the most recent blogs:


{% for post in site.blogposts %}
- {{ post.date | date_to_string }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}