---
layout: default
title: AEK Analiz | Stratejik Bakış
---

<header style="text-align: center; padding: 40px 0 20px 0;">
  <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="AEK Logo" style="width: 130px; opacity: 0.9;">
  <h1 style="font-size: 2.2rem; color: #1a1a1a; margin-top: 20px; font-weight: 800; letter-spacing: -1px;">// STRATEJİK PORTFÖY //</h1>
  <p style="color: #888; font-size: 1.1rem; max-width: 600px; margin: 0 auto; line-height: 1.5;">Ekonomik tarih, finansal piyasalar ve teknoloji üzerine derinlemesine raporlar.</p>
</header>

<div style="background: #fff; border-radius: 50px; padding: 5px 20px; box-shadow: 0 5px 15px rgba(0,0,0,0.02); margin-bottom: 40px;">
  {% include market-ticker.html %}
</div>

---

<div class="post-list">
  <h2 style="font-size: 1.2rem; text-transform: uppercase; letter-spacing: 2px; color: #999; margin-bottom: 30px; text-align: center;">Güncel Raporlar</h2>
  
  {% for post in site.posts %}
    <article class="post-item">
      <div class="post-meta">{{ post.date | date: "%d %B %Y" }}</div>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <p style="color: #666; font-size: 1rem; margin-bottom: 0;">{{ post.excerpt | strip_html | truncatewords: 22 }}</p>
      <a href="{{ post.url | relative_url }}" class="read-more">ANALİZİ İNCELE →</a>
    </article>
  {% endfor %}
</div>