---
layout: default
title: Bidragsytere 
nav_order: 2
---
{% for people_hash in site.data.people %}
{% assign people = people_hash[1] %}
{% for person in people %}

### {{ person.author }}

{{ person.social }}

{{ person.crypto }}

```
{{ person.gpg }}
```

{% endfor %}
{% endfor %}
