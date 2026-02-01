---
layout: post
title: "Yapay Zeka Etiği: Makineler Kime Göre Karar Vermeli?"
author: Adem Evren Kır
date: 2026-02-01 11:00:00 +0300
categories: [teknoloji, etik, hukuk]
---

# Algoritmaların Ahlaki Sorumluluğu

Yapay zeka (YZ), artık sadece veri işleyen bir araç değil, otonom kararlar veren bir aktör haline gelmiştir. Ancak bu kararların arkasındaki "etik çerçeve" hala gri bir alandadır. Medipol Üniversitesi'nde sürdürdüğüm akademik çalışmalarımda da vurguladığım üzere, bu kararların hukuki ve ekonomik sorumluluğu geleceğin en büyük tartışma konusu olacaktır.

## Veri Taraflılığı ve Adalet

Bir YZ modeli, eğitildiği verideki insan önyargılarını kopyalama eğilimindedir. Eğer veri setinde tarihsel bir ayrımcılık varsa, algoritma bu ayrımcılığı "optimizasyon" adı altında meşrulaştırabilir. Bu durum, özellikle uluslararası ticaret ve kredi skorlama sistemlerinde ciddi riskler barındırmaktadır.

#### Karar Alma Süreçlerinde İnsan vs. YZ Güveni
Aşağıdaki grafik, karmaşık etik ikilemlerde toplumun insana duyduğu güven ile algoritmaya duyduğu güven arasındaki makası göstermektedir:

<canvas id="etikChart" width="400" height="200" style="background: #fff; border: 1px solid #eee; padding: 15px; border-radius: 8px; margin: 20px 0;"></canvas>

<script>
document.addEventListener("DOMContentLoaded", function() {
    const ctx = document.getElementById('etikChart').getContext('2d');
    new Chart(ctx, {
        type: 'radar',
        data: {
            labels: ['Hız', 'Tarafsızlık', 'Empati', 'Mantık', 'Sorumluluk'],
            datasets: [{
                label: 'İnsan Karar Mekanizması',
                data: [40, 50, 95, 60, 90],
                backgroundColor: 'rgba(44, 62, 80, 0.2)',
                borderColor: '#2c3e50',
                borderWidth: 2
            },
            {
                label: 'Yapay Zeka (Mevcut)',
                data: [100, 80, 5, 95, 30],
                backgroundColor: 'rgba(139, 0, 0, 0.2)',
                borderColor: '#8b0000',
                borderWidth: 2
            }]
        },
        options: {
            elements: { line: { tension: 0.1 } },
            plugins: { title: { display: true, text: 'Karar Verme Yetkinlik Karşılaştırması' } }
        }
    });
});
</script>

## Sorumluluk Kimde?

Bir otonom araç kaza yaptığında veya bir YZ algoritması yanlış bir finansal yatırım tavsiyesi verdiğinde sorumluluk yazılımcıda mı, kullanıcıda mı yoksa algoritmanın kendisinde mi aranmalıdır? Bu soruya verilecek cevap, geleceğin ticaret hukukunu belirleyecektir.

---

### Referanslar ve Notlar
[^1]: Kır, A. E. (2026). *Algoritmik Adalet ve Geleceğin Hukuku*, Tarih ve Analiz Blogu.
[^2]: IEEE Global Initiative on Ethics of Autonomous and Intelligent Systems.