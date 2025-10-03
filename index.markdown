---
layout: home
title: Son Analizler ve Gündem # Ana sayfa başlığı olarak görünecek
---

{% for post in site.posts %}
  <div class="post-item">
    <h2 class="post-title">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h2>
    <p class="post-meta">
      <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time>
      {% if post.author %} - Yazar: {{ post.author }}{% endif %}
      {% if post.categories.size > 0 %} | Kategori: {{ post.categories | join: ", " }} {% endif %}
    </p>
    
    {% comment %} 
      Bu kısım, makalenin ilk paragrafını özet olarak gösterecek.
      Eğer makalenizde `` etiketi kullanırsanız, o etikete kadar olan kısmı gösterir.
    {% endcomment %}
    {{ post.excerpt }}
    <a href="{{ post.url | relative_url }}"> [Devamını Oku]</a>
    
    <hr>
  </div>
{% endfor %}