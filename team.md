---
layout: page
title: Team
---
# Team

{% for member in site.team %}
## {{ member.title }}

{{ member.role }}

{{ member.content }}
{% endfor %}
