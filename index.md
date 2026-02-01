---
layout: default
title: Ana Sayfa | AEK Analiz
---

<div style="text-align: center; padding: 25px 0;">
  <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Logo" style="width: 150px !important; height: auto !important; display: block; margin: 0 auto;">
  <h1 style="color: #8b0000; margin-top: 15px; font-size: 1.8rem;">// GÜNCEL PROJE ANALİZLERİ //</h1>
  <p style="font-style: italic; color: #666; margin-top: -10px;">Tarih, Teknoloji ve Stratejinin Kesişim Noktası</p>
</div>

{% include market-ticker.html %}

---

<h2 style="margin-bottom: 30px; border-bottom: 2px solid #8b0000; display: inline-block;">Son Analizler & Raporlar</h2>

<div class="post-list">
  {% for post in site.posts %}
    <div class="post-item">
      <div class="post-meta">{{ post.date | date: "%d %B %Y" }}</div>
      <h3>
        <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      </h3>
      <p style="color: #444; font-size: 0.95rem;">
        {{ post.excerpt | strip_html | truncatewords: 25 }}
      </p>
      <a href="{{ post.url | relative_url }}" style="font-weight: bold; font-size: 0.85rem; color: #8b0000; text-transform: uppercase;">Analizi Oku →</a>
    </div>
  {% endfor %}
</div>