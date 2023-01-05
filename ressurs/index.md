---
layout: home 
---
{: .note }
> 1. Alle prøver, eller oppgave ark som blir sendt inn– MÅ være en PDF eller markdown
> 2. PDF filene skal ha format \[DATO\]\[SKOLE\]\[FAG\].pdf


{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
      {% for pdf in site.data.pdf %}
      <li>{{ pdf.date }} {{ pdf.author }} <a href="/assets/pdf/{{ pdf.name }}">{{ pdf.title }}</a></li>
      {% endfor %}
  </ul>
{% endfor %}
