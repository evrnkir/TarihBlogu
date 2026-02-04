---
layout: default
title: AEK Analiz | Stratejik Vizyon
---

<header style="text-align: center; padding: 60px 0 30px 0;">
  <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="AEK Logo" style="width: 140px; opacity: 0.95;">
  <h1 style="font-size: 2.6rem; color: #1a1a1a; margin-top: 30px; font-weight: 800; letter-spacing: -1.5px;">// STRATEJİK ANALİZ //</h1>
  <p style="color: #666; font-size: 1.25rem; max-width: 700px; margin: 15px auto 0; font-style: italic;">
    Küresel piyasalar, jeopolitik tarih ve finansal stratejiler üzerine derinlemesine incelemeler.
  </p>
</header>

<div style="background: #fff; border-radius: 50px; padding: 5px; box-shadow: 0 10px 30px rgba(0,0,0,0.04); margin-bottom: 50px; border: 1px solid #f0f0f0; overflow: hidden; display: flex; align-items: center; justify-content: center;">
  <div style="width: 100%; border-radius: 45px; overflow: hidden;">
    {% include market-ticker.html %}
  </div>
</div>

---

<div class="post-list">
  <h2 style="font-size: 1.3rem; text-transform: uppercase; letter-spacing: 3px; color: #bbb; margin-bottom: 40px; text-align: center;">Son Raporlar & Yayınlar</h2>
  
  {% for post in site.posts %}
    <article class="post-item">
      <div class="post-meta">{{ post.date | date: "%d %B %Y" }}</div>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <p style="color: #555;">{{ post.excerpt | strip_html | truncatewords: 25 }}</p>
      <a href="{{ post.url | relative_url }}" class="read-more">ANALİZİ DERİNLEŞTİR →</a>
    </article>
  {% endfor %}
</div>