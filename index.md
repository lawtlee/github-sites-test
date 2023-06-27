{% include navigation.html %}

# Building Websites in GitHub

## Description
{{ site.description }}
{% assign lead = site.team_members | where:"role", "project lead" | first %}
The project is led by {{ lead.name }}.
[See our full team](about#team)

Have any questions about what we do? [We'd love to hear from you!](mailto:{{ site.email }})

## Blog Posts

{% for post in site.blogposts %}
- {{ post.date | date_to_string }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
