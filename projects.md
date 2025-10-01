---
layout: page
title: Projects
permalink: /projects/
---

<ul>
{% for project in site.projects %}
  <li>
    <a href="{{ project.url | relative_url }}">{{ project.title }}</a>
    {% if project.date %} <small>— {{ project.date | date: "%b %Y" }}</small>{% endif %}
  </li>
{% endfor %}
</ul>
