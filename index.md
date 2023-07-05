---
layout: default
title: Home
---

# Building Websites in GitHub

## Description
{{ site.description }}
{% assign lead = site.team_members | where:"role", "project lead" | first %}
This project was developed by the Carpentries team and now used by me Lawrence Lee.
[See our full team](about#team)

Want to change the design? [I'd love to hear your ideas!](mailto:{{ site.email }})

## Blog Posts

{% for post in site.blogposts %}
- {{ post.date | date_to_string }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
