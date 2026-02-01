---
layout: home
title: Ana Sayfa
---

<div class="posts-list">
  <h2 style="color: #8b0000; border-bottom: 2px solid #8b0000; padding-bottom: 10px;">
    // GÜNCEL PROJE ANALİZLERİ //
  </h2>
  <p style="font-style: italic; color: #666; margin-bottom: 40px;">
    Tarih, Teknoloji ve Stratejinin Kesişim Noktası
  </p>
<style>
  .post-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
    list-style: none;
    padding: 0;
  }
  .post-card {
    border: 1px solid #eee;
    padding: 20px;
    border-radius: 8px;
    transition: transform 0.2s;
  }
  .post-card:hover {
    transform: translateY(-5px);
    border-color: #8b0000;
  }
</style>
  {% for post in site.posts %}
    <article class="post-item" style="margin-bottom: 50px; padding: 25px; border-left: 5px solid #8b0000; background: #fff; box-shadow: 0 4px 6px rgba(0,0,0,0.05);">
      <h2 class="post-title" style="margin-top: 0;">
        <a href="{{ post.url | relative_url }}" style="color: #8b0000; text-decoration: none; font-weight: bold; font-family: 'Lora', serif;">
          {{ post.title }}
        </a>
      </h2>

      <div class="post-meta" style="font-style: italic; color: #888; margin-bottom: 15px; font-size: 0.9em;">
        <time datetime="{{ post.date | date_to_xmlschema }}">
          {{ post.date | date: "%d %B %Y" }}
        </time>
        {% if post.categories.size > 0 %}
          | <strong>Kategoriler:</strong> {{ post.categories | join: ", " }}
        {% endif %}
      </div>

      <div class="post-excerpt" style="line-height: 1.7; color: #444;">
        {{ post.excerpt | strip_html | truncatewords: 45 }}
      </div>

      <div style="margin-top: 20px;">
        <a href="{{ post.url | relative_url }}" style="color: #8b0000; font-weight: bold; text-decoration: none; border-bottom: 1px solid #8b0000;">
          Analizin Tamamını Oku →
        </a>
      </div>
    </article>
  {% else %}
    <div style="padding: 40px; text-align: center; background: #f9f9f9; border: 1px dashed #ccc;">
      <p>Henüz yayınlanmış bir analiz bulunamadı.</p>
      <p style="font-size: 0.9em; color: #777;">Lütfen <strong>_posts</strong> klasöründe en az bir markdown dosyası olduğundan emin olun.</p>
    </div>
  {% endfor %}
</div>