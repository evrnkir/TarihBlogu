---
layout: post
title: "Antik Roma'da Para Değeri: Dinaris'ten Hiper Enflasyona Giden Yol"
author: Evren Yazar
date: 2025-10-04 10:00:00 +0300
categories: [analiz, ekonomi, tarih]
---

# Roma Ekonomisinin Gümüş Sırrı

Antik Roma, gücünün zirvesindeyken ekonomik istikrarını **denarius** adı verilen gümüş sikkelere borçluydu.
Ancak imparatorluk büyüdükçe ve harcamalar arttıkça, hükümdarlar kolay bir yola başvurdular: **paranın değerini düşürmek.**

---

## Sikke Basım Merkezleri ve Etki Alanları (Harita)

Bu interaktif harita, Roma İmparatorluğu'nun ekonomik yayılımını göstermektedir.

<iframe 
    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d154446.04018335968!2d12.37894336582572!3d41.90998606402484!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x132f6196f9928ebb%3A0x6de9a202bfb8d234!2sRoma%2C%20%C4%B0talya!5e0!3m2!1str!2str!4v1709214041724!5m2!1str!2str" 
    width="100%" 
    height="450" 
    style="border:0;" 
    allowfullscreen="" 
    loading="lazy" 
    referrerpolicy="no-referrer-when-downgrade">
</iframe>

---

## Gümüş İçeriği ve Yıkım

M.S. 1. yüzyılda, bir denarius'taki gümüş oranı yaklaşık %95'ti. Ancak Nero ve sonraki imparatorlar, askerlerin maaşlarını ödemek ve kamu harcamalarını karşılamak için sikkelerin içindeki gümüş miktarını sürekli azalttılar.

* **M.S. 2. Yüzyıl:** Gümüş oranı %50'ye düştü.
* **M.S. 3. Yüzyıl:** Gümüş oranı neredeyse %5'e düştü (bronz sikke haline geldi).
<canvas id="enflasyonChart" width="400" height="200"></canvas>
<script>
const ctx = document.getElementById('enflasyonChart').getContext('2d');
const myChart = new Chart(ctx, {
    type: 'line',
    data: {
        labels: ['M.Ö 27', 'M.S 180', 'M.S 211', 'M.S 270'],
        datasets: [{
            label: 'Denarius Gümüş Oranı (%)',
            data: [95, 75, 50, 5],
            borderColor: 'rgba(139, 0, 0, 1)',
            tension: 0.1
        }]
    }
});
</script>