---
layout: projetos_index
title: "Projetos"
permalink: /projetos/
---

<div class="equipe-grid">
  {% for projeto in site.projetos %}
    <div class="card card-projeto">
      {% if projeto.image %}
        <img class="img-projeto" src="{{ projeto.image | relative_url }}" alt="{{ projeto.title }}">
      {% endif %}
      <h3><a href="{{ projeto.url | relative_url }}">{{ projeto.title }}</a></h3>
      {% if projeto.financiador %}
        <p class="financiador-label">{{ projeto.financiador }}</p>
      {% endif %}
    </div>
  {% endfor %}
</div>



