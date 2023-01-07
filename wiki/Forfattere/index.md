---
layout: default
title: Bidragsytere 
nav_order: 2
---
{% for people_hash in site.data.people %}
{% assign people = people_hash[1] %}
{% for person in people %}

### {{ person.author }}

#### Kontakt

- {{ person.email }}
- [GPG](/assets/gpg/{{ person.gpg }})


#### Sosial

{% for website in person.social %}
- [{{ website }}](https://www.{{ website }})
{% endfor %}

#### Donasjon

- {{ person.donation }}

{% endfor %}
{% endfor %}
