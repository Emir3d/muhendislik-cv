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
   TEMEL RENK SİSTEMİ (AYDINLIK / KOYU MOD)
   ====================================================== */
:root {
  /* AYDINLIK MOD (Varsayılan) */
  --text-primary: #111827; /* Ana başlıklar (Simsiyah) */
  --text-body: #374151;    /* Gövde metni (Koyu Gri) */
  --bg-card: #f9fafb;      /* Kutu arka planı (Çok açık gri) */
  --border-color: #e5e7eb; /* İnce çerçeveler */
  
  /* Tonal Renk Geçişi (Koyudan Açığa Mavi) */
  --tone-1: #0f172a;
  --tone-2: #1e40af;
  --tone-3: #3b82f6;
  --tone-4: #60a5fa;
  --tone-final: #2563eb;
}

@media (prefers-color-scheme: dark) {
  :root {
    /* KOYU MOD */
    --text-primary: #f9fafb; /* Ana başlıklar (Beyaz) */
    --text-body: #d1d5db;    /* Gövde metni (Açık Gri) */
    --bg-card: #1f2937;      /* Kutu arka planı (Koyu Gri) */
    --border-color: #374151; /* İnce çerçeveler (Daha koyu) */

    /* Tonal Renk Geçişi (Karanlıkta parlayan maviler) */
    --tone-1: #1e40af;
    --tone-2: #3b82f6;
    --tone-3: #60a5fa;
    --tone-4: #93c5fd;
    --tone-final: #3b82f6;
  }
}

/* ======================================================
   YAZI RENKLERİNİ ZORLA DÜZELTME (Fix)
   ====================================================== */
/* Temanın beyaz dayatmasını kırıyoruz */
body, .page__content, p, li {
  color: var(--text-body) !important;
}

h1, h2, h3, h4, h5, h6 {
  color: var(--text-primary) !important;
}

/* Hero (Üst Resim) üzerindeki yazılar hep beyaz kalsın */
.page__hero--overlay .page__title,
.page__hero--overlay .page__lead {
  color: #ffffff !important;
}

/* ======================================================
   TİPOGRAFİ & DÜZEN
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
  color: var(--text-primary) !important; /* Başlık rengiyle aynı olsun */
  opacity: 0.9;
}

/* Zarif Ayraç */
.section-divider {
  border: none;
  height: 1px;
  background: linear-gradient(to right, transparent, var(--border-color), transparent);
  margin: 4rem 0;
  opacity: 0.7;
}

/* ======================================================
   SÜREÇ AKIŞI — RENK UYUMLU KUTULAR (Harmony Box)
   ====================================================== */
.process-flow {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr)); /* Mobilde alt alta, pc'de yan yana */
  gap: 1.2rem;
  max-width: 900px;
  margin: 3rem auto;
}

.flow-step {
  padding: 1.2rem 1rem;
  text-align: center;
  background-color: var(--bg-card); /* Tema uyumlu arka plan */
  border: 1px solid var(--border-color);
  border-left-width: 5px; /* Sol taraf kalın renkli çizgi */
  border-radius: 8px;
  font-size: 0.95rem;
  font-weight: 600;
  color: var(--text-primary) !important; /* Kutu içi yazı rengi */
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  box-shadow: 0 2px 4px rgba(0,0,0,0.05);
}

.flow-step:hover {
  transform: translateY(-4px);
  box-shadow: 0 8px 16px rgba(0,0,0,0.1);
}

/* Tonal Renk Atamaları */
.step-1 { border-left-color: var(--tone-1); }
.step-2 { border-left-color: var(--tone-2); }
.step-3 { border-left-color: var(--tone-3); }
.step-4 { border-left-color: var(--tone-4); }
.step-final { 
  border-left-color: var(--tone-final);
  font-weight: 700;
}

/* Koyu modda gölgeyi düzelt */
@media (prefers-color-scheme: dark) {
  .flow-step { box-shadow: 0 2px 4px rgba(0,0,0,0.3); }
}

/* ======================================================
   ÜNLÜ SÖZLER (Quotes)
   ====================================================== */
.quotes {
  max-width: 760px;
  margin: 3rem auto 0;
  display: grid;
  gap: 1.5rem;
}

.quote-box {
    background: var(--bg-card);
    border-left: 4px solid var(--border-color);
    padding: 1.5rem;
    border-radius: 0 8px 8px 0;
}

.quote-text {
  font-style: italic;
  font-size: 1rem;
  color: var(--text-body) !important;
  margin-bottom: 0.8rem;
}

.quote-author {
  display: block;
  text-align: right;
  font-size: 0.9rem;
  font-weight: bold;
  color: var(--text-primary) !important;
}
/* Renkli vurgular */
.q-blue { border-left-color: var(--tone-2); }
.q-red { border-left-color: #c0392b; }
.q-cyan { border-left-color: #0891b2; }
</style>

<div class="manifesto">
“Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir.”
</div>

<p>
Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; <strong>analiz, modelleme, doğrulama ve üretilebilirlik</strong> ekseninde ele alan bütüncül bir yaklaşım sunuyorum.
</p>
<p>
Çalışmalarımda temel amaç; mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.
</p>

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

<p>
Bu yaklaşım, sistem davranışını daha tasarım aşamasında öngörebilmeyi, kritik sınır koşullarını doğru şekilde tanımlamayı ve mühendislik kararlarını nicel verilere dayandırmayı mümkün kılar.
</p>

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
