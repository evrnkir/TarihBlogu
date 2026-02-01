---
layout: home
title: Ana Sayfa | Tarih ve Analiz Blogu
---

<div style="text-align: center; margin: 15px 0; width: 100%;">
  <img src="{{ '/assets/images/logo.png' | relative_url }}" 
       alt="AEK Logo" 
       style="width: 150px !important; height: auto !important; max-width: 150px !important; display: block; margin: 0 auto;">
  
  <h1 style="color: #8b0000; margin-top: 15px; font-size: 1.8rem;">// GÜNCEL PROJE ANALİZLERİ //</h1>
  <p style="font-style: italic; color: #666;">Tarih, Teknoloji ve Stratejinin Kesişim Noktası</p>
</div>

---

## Öne Çıkan Çalışmalar

<div class="post-list-container">
  {% for post in site.posts %}
    <div style="border-left: 5px solid #8b0000; padding: 20px; margin-bottom: 30px; background: #fff; box-shadow: 0 4px 6px rgba(0,0,0,0.05); border-radius: 0 8px 8px 0;">
      <h3 style="margin-top: 0;">
        <a href="{{ post.url | relative_url }}" style="text-decoration: none; color: #8b0000;">{{ post.title }}</a>
      </h3>
      <p style="font-size: 0.85rem; color: #999;">{{ post.date | date: "%d %B %Y" }}</p>
      <p style="color: #444;">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
      <a href="{{ post.url | relative_url }}" style="font-weight: bold; color: #8b0000; text-decoration: none; font-size: 0.9rem;">Analizi Oku →</a>
    </div>
  {% endfor %}
</div>