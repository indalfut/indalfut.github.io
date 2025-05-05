---
title: "Inicio"
layout: page
---

# ¡Bienvenido a mi catálogo!

{% for item in site.data.products %}
<div class="producto">
  <h3>{{ item.name }}</h3>
  <img src="{{ site.baseurl }}/assets/img/{{ item.image }}" width="200">
  <p>{{ item.description }}</p>
  <p>Precio: {{ item.price }}</p>
</div>
{% endfor %}