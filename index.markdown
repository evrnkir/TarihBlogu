---
# Front Matter (Değiştirmeyin)
layout: home
---

# Son Analizler ve Gündem

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
    
    {{ post.excerpt | strip_html | truncatewords: 30 }}
    <a href="{{ post.url | relative_url }}"> [Devamını Oku]</a>
    
    <hr>
  </div>
{% endfor %}