---
layout: page
title: Education
permalink: /education/
---

# Education

<ul>
{% for education in site.education %}
  <li>
    <h3>{{ education.institution }}</h3>
    <h4>{{ education.degree }}</h4>
    <p>{{ education.date | date: "%B %d, %Y" }}</p>
    {{ education.content | markdownify }}
  </li>
{% endfor %}
</ul>
