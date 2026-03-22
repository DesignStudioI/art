---
layout: single
title: Прилавок
permalink: /merch/
---

<style>

.merch-grid{
  display:grid;
  grid-template-columns:repeat(auto-fill,minmax(220px,1fr));
  gap:25px;
  margin-top:30px;
}

.merch-card{
  display:block;
  text-decoration:none;
  border:1px solid #ddd;
  border-radius:8px;
  overflow:hidden;
  background:white;
  transition:0.2s;
}

.merch-card:hover{
  transform:translateY(-4px);
  box-shadow:0 10px 25px rgba(0,0,0,0.15);
}

.merch-image{
  width:100%;
  height:220px;
  overflow:hidden;
}

.merch-image img{
  width:100%;
  height:100%;
  object-fit:cover;
}

.merch-text{
  padding:12px;
}

.merch-text h3{
  font-size:16px;
  margin:0;
}

.merch-text p{
  margin:6px 0 0;
  font-weight:bold;
}

</style>

<div class="merch-grid">
  {% for item in site.data.merch %}
    <a href="/merch/item/?id={{ item.slug }}" class="merch-card">
      <div class="merch-image"><img src="{{ item.image | relative_url }}"></div>
      <div class="merch-text">
        <h3>{{ item.title }}</h3>
        <p>{{ item.price }}</p>
      </div>
    </a>
  {% endfor %}
</div>
