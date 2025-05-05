---
title: "Catálogo de Camisetas"
layout: single
permalink: /catalogo/
---

{% for product in site.data.products %}
  <div class="product">
    <h2>{{ product.name }}</h2>
    <img src="/assets/images/{{ product.image }}" alt="{{ product.name }}" width="200">
    <p>{{ product.description }}</p>
    <p><strong>Precio:</strong> {{ product.price }}</p>
  </div>
{% endfor %}