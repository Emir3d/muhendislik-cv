---
permalink: /
title: "Mühendisliğe Analitik ve Bütüncül Bir Bakış"
excerpt: "Mekanik tasarım, analiz ve doğrulama odaklı mühendislik çalışmaları"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
header:
  overlay_image: https://emir3d.github.io/muhendislik-cv/images/header_bg.png
  overlay_filter: 0.7
---

<style>
/* 1. SOL MENÜDEKİ KIRIK RESMİ YOK ET */
.author__avatar {
  display: none !important;
}

/* 2. SAYFA YAPISINI BOZAN ETKENLERİ SIFIRLA */
/* Bu kod, içeriğin sidebar ile uyumlu durmasını sağlar */
.page__content {
  width: 100% !important;
  margin-right: 0 !important;
}

/* 3. AKILLI RENK YÖNETİMİ (LIGHT MODE - VARSAYILAN) */
:root {
  --text-color: #333333;
  --bg-card: #ffffff;
  --border-color: #e0e0e0;
  --desc-color: #555555;
  --divider-color: #cccccc;
}

/* 4. AKILLI RENK YÖNETİMİ (DARK MODE - OTOMATİK) */
@media (prefers-color-scheme: dark) {
  :root {
    --text-color: #e0e0e0;      /* Yazılar açık gri */
    --bg-card: #1e293b;         /* Kartlar koyu gri */
    --border-color: #334155;    /* Çerçeveler silik */
    --desc-color: #cbd5e1;      /* Açıklamalar beyazımsı */
    --divider-color: #444444;   /* Ayraçlar koyu */
  }
}

/* GENEL YAZI STİLLERİ (Değişkenlere Bağlı) */
body, p, li {
  color: var(--text-color) !important;
}

.manifesto-text {
  text-align: center;
  font-size: 1.25em;
  font-style: italic;
  font-family: 'Georgia', serif;
  margin-bottom: 1.5em;
  color: var(--text-color) !important;
  opacity: 0.9;
}

/* PROCESS GRID (SÜREÇ KUTULARI) */
.process-grid-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr); 
  gap: 15px;
  margin: 2em 0;
}

.p-card {
  background-color: var(--bg-card) !important;
  color: var(--text-color) !important;
  padding: 20px;
  border-radius: 8px;
  border: 1px solid var(--border-color);
  position: relative;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.2s;
}
.p-card:hover {
  transform: translateY(-5px);
}

/* RENKLİ ÇİZGİLER (SABİT) */
.style-1 { border-left: 5px solid #0f172a !important; }
.style-2 { border-left: 5px solid #1e40af !important; }
.style-3 { border-left: 5px solid #3b82f6 !important; }
.style-4 { border-left: 5px solid #60a5fa !important; }

/* KUTU İÇİ YAZILAR */
.p-num {
  font-weight: 900; 
  font-size: 1.5em; 
  opacity: 0.2; 
  position: absolute; 
  top: 10px; 
  right: 15px; 
  color: var(--text-color) !important;
}
.p-title {
  font-weight: 700; 
  font-size: 1em; 
  margin-bottom: 8px; 
  color: var(--text-color) !important;
}
.p-desc {
  font-size: 0.85em; 
  color: var(--desc-color) !important; 
  line-height: 1.4;
}

/* ZARİF AYRAÇ */
hr.elegant-divider {
  border: 0;
  height: 1px;
  background-color: var(--divider-color);
  margin: 3em 0;
}

/* VİZYON KARTLARI */
.vision-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
}
.v-card {
  background-color: var(--bg-card) !important;
  padding: 20px;
  border-radius: 6px;
  border: 1px solid var(--border-color);
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
}
.border-blue { border-top: 3px solid #0f172a; }
.border-red { border-top: 3px solid #b91c1c; }
.border-cyan { border-top: 3px solid #0891b2; }

.v-quote { font-style: italic; font-size: 0.95em; color: var(--desc-color) !important; }
.v-author { text-align: right; font-weight: bold; font-size: 0.9em; margin-top: 10px; color: var(--text-color) !important; }

/* MOBİL UYUM */
@media (max-width: 900px) {
  .process-grid-container {
    grid-template-columns: 1fr; 
  }
}
</style>

<div class="manifesto-text">
  "Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir."
</div>

<p>
  Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; <strong>analiz, modelleme, doğrulama ve üretilebilirlik</strong> ekseninde ele alan bütüncül bir yaklaşım sunuyorum.
</p>

<p>
  Çalışmalarımda temel amaç; mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.
</p>

<hr class="elegant-divider">

### Analiz Tabanlı Tasarım Metodolojisi

Modern mühendislik problemleri, yalnızca deneysel yöntemlerle ya da tek boyutlu tasarım anlayışıyla sürdürülebilir biçimde çözülemez. Bu nedenle tasarım süreçlerini; **yapısal analiz, sayısal modelleme ve optimizasyon** adımlarıyla desteklenen analitik bir çerçevede ele alıyorum.

<div class="process-grid-container">
  
  <div class="p-card style-1">
    <div class="p-num">01</div>
    <div class="p-title">Fiziksel Tanım</div>
    <div class="p-desc">Problemin sahadaki gerçekliğinin ve sınır şartlarının belirlenmesi.</div>
  </div>

  <div class="p-card style-2">
    <div class="p-num">02</div>
    <div class="p-title">Matematiksel Model</div>
    <div class="p-desc">Geometrinin temizlenmesi, uygun ağ (mesh) yapısı ve sayısal kurulum.</div>
  </div>

  <div class="p-card style-3">
    <div class="p-num">03</div>
    <div class="p-title">Analiz & Doğrulama</div>
    <div class="p-desc">Çözümün yakınsaması, mesh bağımsızlığı ve parametrik incelemeler.</div>
  </div>

  <div class="p-card style-4">
    <div class="p-num">04</div>
    <div class="p-title">Mühendislik Yorumu</div>
    <div class="p-desc">Sonuçların yorumlanması ve üretilebilir tasarım kararlarının alınması.</div>
  </div>

</div>

<hr class="elegant-divider">

### Sanal Doğrulama ve Sayısal Düşünme

Fiziksel testler mühendislikte vazgeçilmezdir; ancak doğru kurulan sayısal modeller, tasarım güvenilirliğini artırırken zaman ve maliyet açısından önemli avantajlar sağlar.

Bu bağlamda, çalışmalarda **Sanal Doğrulama (Virtual Verification)** süreçlerini merkeze alarak, tasarımın fiziksel davranışla tutarlı olmasını hedefliyorum. Sayısal analizler, yalnızca sonuç üretmek için değil; sistemi anlamak, varsayımları sorgulamak ve model güvenilirliğini değerlendirmek için bir araç olarak ele alınmaktadır.

### Tasarım, Davranış ve Üretilebilirlik İlişkisi

Bir mühendislik çözümünün başarısı, yalnızca teorik doğruluğuyla değil; üretim süreçleriyle olan uyumuyla da belirlenir.

Bu nedenle tasarım, analiz ve üretim arasındaki ilişkiyi birbirinden kopuk adımlar olarak değil, tek bir mühendislik sürecinin parçaları olarak değerlendiriyorum. Bu perspektif, tasarım kararlarının gerçek dünya koşullarında uygulanabilirliğini erken aşamada görmeyi ve olası sorunları öngörmeyi mümkün kılar.

<hr class="elegant-divider">

<h3 style="text-align: center; margin-bottom: 1em;">Mühendislik Vizyonu</h3>
<div class="manifesto-text" style="font-size: 1.1em; margin-bottom: 2em;">
  "Mühendisliği; fiziksel gerçekliği anlamaya çalışan, sayısal araçları bilinçli kullanan ve her çözümü sorgulanabilir kılan bir düşünce disiplini olarak görüyorum."
</div>

<div class="vision-grid">
  <div class="v-card border-blue">
    <p class="v-quote">"Engineering is the art of directing the great sources of power in nature for the use and convenience of man."</p>
    <p class="v-author">— Thomas Tredgold</p>
  </div>
  <div class="v-card border-red">
    <p class="v-quote">"Mechanics is the paradise of the mathematical sciences, because by means of it one comes to the fruits of mathematics."</p>
    <p class="v-author">— Leonardo da Vinci</p>
  </div>
  <div class="v-card border-cyan">
    <p class="v-quote">"Science can amuse and fascinate us all, but it is engineering that changes the world."</p>
    <p class="v-author">— Isaac Asimov</p>
  </div>
</div>
