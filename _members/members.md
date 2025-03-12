---
layout: default
title: Miembros del Equipo
---

<h1>Miembros del Equipo</h1>
<ul>
  {% for member in site.members %}
    <li>
      <a href={{ member.url }}>{{ member.name }}</a> - <a href={{ member.github }}>GitHub</a>
    </li>
  {% endfor %}
</ul>

