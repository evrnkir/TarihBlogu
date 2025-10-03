---
layout: post
title: "Antik Roma'da Para Değeri: Dinaris'ten Hiper Enflasyona Giden Yol"
author: Evren Yazar
date: 2025-10-04 10:00:00 +0300
categories: [analiz, ekonomi, tarih]
---

# Roma Ekonomisinin Gümüş Sırrı

Antik Roma, gücünün zirvesindeyken ekonomik istikrarını **denarius** adı verilen gümüş sikkelere borçluydu. Ancak imparatorluk büyüdükçe ve harcamalar arttıkça, hükümdarlar kolay bir yola başvurdular: **paranın değerini düşürmek.**

## Gümüş İçeriği ve Yıkım

M.S. 1. yüzyılda, bir denarius'taki gümüş oranı yaklaşık %95'ti. Ancak Nero ve sonraki imparatorlar, askerlerin maaşlarını ödemek ve kamu harcamalarını karşılamak için sikkelerin içindeki gümüş miktarını sürekli azalttılar.

* **M.S. 2. Yüzyıl:** Gümüş oranı %50'ye düştü.
* **M.S. 3. Yüzyıl:** Gümüş oranı neredeyse %5'e düştü (bronz sikke haline geldi).

---

## Sikke Basım Merkezleri ve Etki Alanları (Harita)

Bu interaktif harita, Roma İmparatorluğu'nun ekonomik yayılımını göstermektedir.

{% raw %}
<div id="roma-harita" style="height: 400px; width: 100%;"></div>

<script>
    // 1. Haritayı Başlatma
    var map = L.map('roma-harita').setView([41.9028, 12.4964], 5);

    // 2. Harita Katmanını Ekleme (OpenStreetMap)
    L.tileLayer('https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png', {
        attribution: '&copy; <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors'
    }).addTo(map);

    // 3. Markör Ekleme: Roma
    L.marker([41.9028, 12.4964]).addTo(map)
        .bindPopup('**Roma Şehri:** Siyasi Merkez.')
        .openPopup();

    // 4. Markör Ekleme: Sikke Merkezi (Atina)
    L.marker([37.9838, 23.7275]).addTo(map) 
        .bindPopup('**Atina:** Ticaret ve Sikke Merkezi.')
</script>
{% endraw %}