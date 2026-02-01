---
layout: default
title: Ana Sayfa | AEK Analiz
---

<div style="text-align: center; padding: 20px 0;">
  <img src="{{ '/assets/images/logo.png' | relative_url }}" alt="Logo" style="width: 150px !important; height: auto !important; display: block; margin: 0 auto;">
  <h1 style="color: #8b0000; margin-top: 15px; font-size: 1.8rem;">// GÜNCEL PROJE ANALİZLERİ //</h1>
</div>

<div class="tradingview-widget-container" style="margin: 20px 0; border-bottom: 1px solid #eee;">
  <div class="tradingview-widget-container__widget"></div>
  <script type="text/javascript" src="https://s3.tradingview.com/external-embedding/embed-widget-ticker-tape.js" async>
  {
    "symbols": [
      { "proName": "BIST:XU100", "title": "BIST 100" },
      { "proName": "FX_IDC:XAUUSD", "title": "Altın" },
      { "proName": "FOREXCOM:SPX3500", "title": "S&P 500" },
      { "proName": "FX:USDTRY", "title": "USD/TRY" }
    ],
    "showSymbolLogo": true,
    "colorTheme": "light",
    "locale": "tr"
  }
  </script>
</div>

---

## Son Analizler
<div class="post-list">
  {% for post in site.posts %}
    <div style="margin-bottom: 20px;">
      <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
      <p>{{ post.date | date: "%d.%m.%Y" }}</p>
    </div>
  {% endfor %}
</div>