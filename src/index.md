---
title: Some Title or Other
layout: base.njk
cut: "- [{{ post.data. title }}]({{ post.url | url }})"
---
# Headline
In principio erat Verbum ...

<ul>
{% for post in collections.posts %}
<li><a href="{{ post.url }}">{{ post.data.title }}</a>

{%- endfor %}
</ul>