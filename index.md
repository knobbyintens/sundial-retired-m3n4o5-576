---
layout: default
title: Home
---
# Turn every route decision into a margin you can see

Harborline Analytics gives mid-market logistics teams a clear view of what
each route and dock window actually costs.

[See what we make]({{ '/products/' | relative_url }})

## Products

{% for product in site.products %}
- [{{ product.title }}]({{ product.url | relative_url }}) — {{ product.summary }}
{% endfor %}

## What customers say

{% for item in site.data.testimonials %}
> "{{ item.quote }}" — {{ item.author }}
{% endfor %}

## Latest news

{% for post in site.posts limit:2 %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%B %d, %Y" }}
{% endfor %}
