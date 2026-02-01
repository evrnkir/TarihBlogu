---
layout: home
title: Ana Sayfa
---

<div class="posts-list">
  {% for post in site.posts %}
    <article class="post-item" style="margin-bottom: 40px; padding: 20px; border-left: 4px solid #8b0000; background: rgba(255,255,255,0.5);">
      <h2 class="post-title" style="margin-top: 0;">
        <a href="{{ post.url | relative_url }}" style="color: #8b0000; text-decoration: none; font-weight: bold;">
          {{ post.title }}
        </a>
      </h2>

      <div class="post-meta" style="font-style: italic; color: #666; margin-bottom: 15px; font-size: 0.9em;">
        <time datetime="{{ post.date | date_to_xmlschema }}">
          {{ post.date | date: "%d %B %Y" }}
        </time>
        {% if post.categories.size > 0 %}
          | Kategori: {{ post.categories | join: ", " }}
        {% endif %}
      </div>

      <div class="post-excerpt" style="line-height: 1.6;">
        {{ post.excerpt | strip_html | truncatewords: 40 }}
      </div>

      <div style="margin-top: 15px;">
        <a href="{{ post.url | relative_url }}" style="color: #8b0000; font-weight: bold; text-decoration: underline;">
          Analizin Devamını Oku →
        </a>
      </div>
    </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
  <p>Henüz bir analiz yazısı yayınlanmadı. İlk yazınızı eklemek için sabırsızlanıyoruz!</p>
{% endif %}