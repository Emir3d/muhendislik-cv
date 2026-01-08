---
permalink: /
title: "Mühendisliğe Analitik ve Bütüncül Bir Bakış"
excerpt: "Analiz, modelleme ve doğrulama temelli mühendislik yaklaşımı"
author_profile: false
header:
  overlay_image: https://emir3d.github.io/muhendislik-cv/images/header_bg.png
  overlay_filter: 0.65
---

<style>
/* ======================================================
   1. YAZI RENGİ GARANTİSİ (SORUN ÇÖZÜCÜ)
   ====================================================== */
/* Varsayılan (Aydınlık Mod) - Yazılar kesinlikle KOYU olsun */
body, .page__content, p, li, .manifesto, .quote-text {
  color: #222222 !important; /* Koyu Gri/Siyah */
}

h1, h2, h3, h4, h5, h6, .flow-step {
  color: #000000 !important; /* Başlıklar Simsiyah */
}

/* Hero Başlığı (Resim üzerindeki yazı) hep beyaz kalsın */
.page__hero--overlay .page__title,
.page__hero--overlay .page__lead {
  color: #ffffff !important;
}

/* ======================================================
   2. KOYU MOD (DARK MODE) AYARLARI
   ====================================================== */
@media (prefers-color-scheme: dark) {
  /* Karanlık mod algılanırsa yazıları beyaza çevir */
  body, .page__content, p, li, .manifesto, .quote-text {
    color: #e5e7eb !important; /* Açık Gri */
  }
  h1, h2, h3, h4, h5, h6, .flow-step {
    color: #ffffff !important; /* Başlıklar Beyaz */
  }
}

/* ======================================================
   3. TİPOGRAFİ & DÜZEN
   ====================================================== */
.page__content p {
  font-size: 1.05rem;
  line-height: 1.8;
  max-width: 760px;
}

.page__content h2 { font-size: 1.65rem; margin-top: 3.5rem; }
.page__content h3 { font-size: 1.35rem; margin-top: 2.5rem; }

/* Manifesto Bloğu */
.manifesto {
  text-align: center;
  font-size: 1.2rem;
  font-style: italic;
  max-width: 760px;
  margin: 3rem auto;
  opacity: 0.9;
}

/* Zarif Ayraç */
.section-divider {
  border: none;
  height: 1px;
  background: linear-gradient(to right, transparent, #ccc, transparent);
  margin: 4rem 0;
  opacity: 0.7;
}
@media (prefers-color-scheme: dark) {
  .section-divider { background: linear-gradient(to right, transparent, #555, transparent); }
}

/* ======================================================
   4. SÜREÇ AKIŞI — RENK UYUMLU KUTULAR
   ====================================================== */
.process-flow {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1.2rem;
  max-width: 900px;
  margin: 3rem auto;
}

.flow-step {
  padding: 1.2rem 1rem;
  text-align: center;
  background-color: #f9fafb; /* Aydınlık arka plan */
  border: 1px solid #e5e7eb;
  border-left-width: 5px;
  border-radius: 8px;
  font-size: 0.95rem;
  font-weight: 600;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
}

.flow-step:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 16px rgba(0,0,0,0.1);
}

/* Renk Geçişi (Tonal Harmony) */
.step-1 { border-left-color: #0f172a; } /* En Koyu */
.step-2 { border-left-color: #1e40af; }
.step-3 { border-left-color: #3b82f6; }
.step-4 { border-left-color: #60a5fa; }
.step-final { border-left-color: #2563eb; }

/* Kutuların Koyu Modu */
@media (prefers-color-scheme: dark) {
  .flow-step {
    background-color: #1f2937; /* Koyu arka plan */
    border-color: #374151;
    box-shadow: 0 2px 4px rgba(0,0,0,0.3);
  }
  /* Renkleri karanlıkta parlat */
  .step-1 { border-left-color: #1e40af; }
  .step-2 { border-left-color: #3b82f6; }
  .step-3 { border-left-color: #60a5fa; }
  .step-4 { border-left-color: #93c5fd; }
  .step-final { border-left-color: #3b82f6; }
}

/* ======================================================
   5. ÜNLÜ SÖZLER (Quotes)
   ====================================================== */
.quotes {
  max-width: 760px;
  margin: 3rem auto 0;
  display: grid;
  gap: 1.5rem;
}

.quote-box {
    background: #f9fafb;
    border-left: 4px solid #ccc;
    padding: 1.5rem;
    border-radius: 0 8px 8px 0;
}

.quote-text {
  font-style: italic;
  font-size: 1rem;
  margin-bottom: 0.8rem;
}

.quote-author {
  display: block;
  text-align: right;
  font-size: 0.9rem;
  font-weight: bold;
  opacity: 0.9;
}

/* Koyu Mod için Sözler */
@media (prefers-color-scheme: dark) {
  .quote-box { background: #1f2937; border-left-color: #555; }
}

/* Renkli vurgular */
.q-blue { border-left-color: #1e40af !important; }
.q-red { border-left-color: #c0392b !important; }
.q-cyan { border-left-color: #0891b2 !important; }
</style>

<div class="manifesto">
“Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir.”
</div>

Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; **analiz, modelleme, doğrulama ve üretilebilirlik** ekseninde ele alan bütüncül bir yaklaşım sunuyorum.

Çalışmalarımda temel amaç; mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.

<hr class="section-divider">

## Analiz Tabanlı Mühendislik Yaklaşımı

Modern mühendislik problemleri, yalnızca deneysel yöntemlerle ya da tek boyutlu tasarım anlayışıyla sürdürülebilir biçimde çözülemez. Bu nedenle tasarım süreçlerini; **yapısal analiz, sayısal modelleme ve optimizasyon** adımlarıyla desteklenen analitik bir çerçevede ele alıyorum.

<div class="process-flow">
  <div class="flow-step step-1">Problem Tanımı</div>
  <div class="flow-step step-2">Matematiksel Model</div>
  <div class="flow-step step-3">Sayısal Analiz</div>
  <div class="flow-step step-4">Doğrulama</div>
  <div class="flow-step step-final">Mühendislik Kararı</div>
</div>

Bu yaklaşım, sistem davranışını daha tasarım aşamasında öngörebilmeyi, kritik sınır koşullarını doğru şekilde tanımlamayı ve mühendislik kararlarını nicel verilere dayandırmayı mümkün kılar.

<hr class="section-divider">

## Sanal Doğrulama ve Sayısal Düşünme

Fiziksel testler mühendislikte vazgeçilmezdir; ancak doğru kurulan sayısal modeller, tasarım güvenilirliğini artırırken zaman ve maliyet açısından önemli avantajlar sağlar.

Bu bağlamda, **Sanal Doğrulama (Virtual Verification)** süreçlerini merkeze alarak, tasarımın fiziksel davranışla tutarlı olmasını hedefliyorum.

<hr class="section-divider">

## Tasarım, Davranış ve Üretilebilirlik İlişkisi

Bir mühendislik çözümünün başarısı, yalnızca teorik doğruluğuyla değil; üretim süreçleriyle olan uyumuyla da belirlenir.

Bu nedenle tasarım, analiz ve üretim arasındaki ilişkiyi birbirinden kopuk adımlar olarak değil, tek bir mühendislik sürecinin parçaları olarak değerlendiriyorum.

<hr class="section-divider">

## Mühendislik Vizyonu

Mühendisliği; fiziksel gerçekliği anlamaya çalışan, sayısal araçları bilinçli kullanan ve her çözümü sorgulanabilir kılan bir düşünce disiplini olarak görüyorum.

<div class="quotes">
  <div class="quote-box q-blue">
    <div class="quote-text">“Engineering is the art of directing the great sources of power in nature for the use and convenience of man.”</div>
    <span class="quote-author">— Thomas Tredgold</span>
  </div>

  <div class="quote-box q-red">
    <div class="quote-text">“Mechanics is the paradise of the mathematical sciences, because by means of it one comes to the fruits of mathematics."</div>
    <span class="quote-author">— Leonardo da Vinci</span>
  </div>

  <div class="quote-box q-cyan">
    <div class="quote-text">“Science can amuse and fascinate us all, but it is engineering that changes the world.”</div>
    <span class="quote-author">— Isaac Asimov</span>
  </div>
</div>
