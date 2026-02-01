---
layout: post
title: "AI Ethics: The Decision Paradox"
author: Adem Evren Kır
date: 2026-02-01
permalink: /en/ai-ethics/
lang: en
---

# The Moral Responsibility of Algorithms

Artificial Intelligence (AI) is no longer just a tool for processing data; it has become an actor making autonomous decisions. However, the "ethical framework" behind these decisions remains a gray area. As I emphasize in my academic studies at Istanbul Medipol University, the legal and economic responsibility for these decisions will be the biggest debate of the future.

## Data Bias and Justice

An AI model tends to copy human biases in the data it is trained on. If there is historical discrimination in the data set, the algorithm may legitimize this discrimination under the name of "optimization." This situation carries serious risks, especially in international trade and credit scoring systems.

#### Human vs. AI Trust in Decision Making
The following radar chart visualizes the gap between public trust in humans and trust in algorithms in complex ethical dilemmas:

<canvas id="ethicsChartEn" width="400" height="200" style="background: #fff; border: 1px solid #eee; padding: 15px; border-radius: 8px; margin: 20px 0;"></canvas>

<script>
document.addEventListener("DOMContentLoaded", function() {
    const ctx = document.getElementById('ethicsChartEn').getContext('2d');
    new Chart(ctx, {
        type: 'radar',
        data: {
            labels: ['Speed', 'Impartiality', 'Empathy', 'Logic', 'Accountability'],
            datasets: [{
                label: 'Human Decision Making',
                data: [40, 50, 95, 60, 90],
                backgroundColor: 'rgba(44, 62, 80, 0.2)',
                borderColor: '#2c3e50',
                borderWidth: 2
            },
            {
                label: 'AI (Current)',
                data: [100, 80, 5, 95, 30],
                backgroundColor: 'rgba(139, 0, 0, 0.2)',
                borderColor: '#8b0000',
                borderWidth: 2
            }]
        },
        options: {
            elements: { line: { tension: 0.1 } },
            plugins: { title: { display: true, text: 'Decision Making Competency Comparison' } }
        }
    });
});
</script>

## Who is Responsible?

When an autonomous vehicle crashes or an AI algorithm gives wrong financial investment advice, should the responsibility be sought in the developer, the user, or the algorithm itself? The answer to this question will determine the future of international trade law.

---

### References
[^1]: Kır, A. E. (2026). *Algorithmic Justice and the Future of Law*, History and Analysis Blog.
[^2]: IEEE Global Initiative on Ethics of Autonomous and Intelligent Systems.