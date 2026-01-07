---
permalink: /
title: "Mühendisliğe Analitik ve Bütüncül Bir Bakış"
excerpt: "Analiz, modelleme ve doğrulama odaklı mühendislik yaklaşımı"
author_profile: true
redirect_from:
  - /about/
  - /about.html
header:
  overlay_image: https://emir3d.github.io/muhendislik-cv/images/header_bg.png
  overlay_filter: 0.7
---

<style>
/* --------------------------------------------------
   1) SOL MENÜDEKİ KIRIK AVATAR GİZLE
-------------------------------------------------- */
.author__avatar {
  display: none !important;
}

/* --------------------------------------------------
   2) SIDEBAR STICKY (PROFESYONEL DAVRANIŞ)
-------------------------------------------------- */
.sidebar {
  position: sticky;
  top: 90px;
}

/* --------------------------------------------------
   3) RENK DEĞİŞKENLERİ (LIGHT MODE)
-------------------------------------------------- */
:root {
  --text-main: #1f2937;
  --text-sub: #4b5563;
  --bg-card: #ffffff;
  --border-soft: #e5e7eb;
  --divider: #d1d5db;
}

/* --------------------------------------------------
   4) RENK DEĞİŞKENLERİ (DARK MODE)
-------------------------------------------------- */
@media (prefers-color-scheme: dark) {
  :root {
    --text-main: #e5e7eb;
    --text-sub: #cbd5e1;
    --bg-card: #0f172a;
    --border-soft: #334155;
    --divider: #475569;
  }
}

/* --------------------------------------------------
   5) SADECE ANA İÇERİK TİPOGRAFİ
-------------------------------------------------- */
.page__content p,
.page__content li {
  color: var(--text-main);
  font-size: 1rem;
  line-height: 1.7;
  margin-bottom: 1.2em;
}

.page__content h2 {
  font-size: 1.6rem;
  margin-top: 3em;
  margin-bottom: 0.8em;
  color: var(--text-main);
}

.page__content h3 {
  font-size: 1.3rem;
  margin-top: 2.5em;
  margin-bottom: 0.8em;
  color: var(--text-main);
}

/* --------------------------------------------------
   6) MANIFESTO METNİ
-------------------------------------------------- */
.manifesto-text {
  text-align: center;
  font-size: 1.2em;
  font-style: italic;
  font-family: Georgia, serif;
  margin: 2.5em auto;
  max-width: 700px;
  color: var(--text-main);
  opacity: 0.9;
}

/* --------------------------------------------------
   7) ZARİF BÖLÜM AYRACI
-------------------------------------------------- */
hr.elegant-divider {
  border: none;
  height: 1px;
  width: 60%;
  margin: 4em auto;
  background: linear-gradient(
    to right,
    transparent,
    var(--divider),
    transparent
  );
}

/* --------------------------------------------------
   8) SÜREÇ KUTULARI (PROCESS GRID)
-------------------------------------------------- */
.process-grid-container {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 20px;
  margin: 3em 0;
}

.p-card {
  background: var(--bg-card);
  border: 1px solid var(--border-soft);
  padding: 20px;
  border-radius: 8px;
  position: relative;
  transition: transform 0.2s ease;
}

.p-card:hover {
  transform: translateY(-4px);
}

/* SOL ŞERİTLER */
.style-1 { border-left: 4px solid #0f172a; }
.style-2 { border-left: 4px solid #1e3a8a; }
.style-3 { border-left: 4px solid #2563eb; }
.style-4 { border-left: 4px solid #60a5fa; }

/* KUTU METİNLERİ */
.p-num {
  position: absolute;
  top: 10px;
  right: 15px;
  font-size: 1.4em;
  font-weight: 800;
  opacity: 0.12;
  color: var(--text-main);
}

.p-title {
  font-weight: 600;
  margin-bottom: 6px;
  color: var(--text-main);
}

.p-desc {
  font-size: 0.9em;
  color: var(--text-sub);
  line-height: 1.5;
}

/* --------------------------------------------------
   9) VİZYON / ALINTI KARTLARI
-------------------------------------------------- */
.vision-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 20px;
}

.v-card {
  background: var(--bg-card);
  border: 1px solid var(--border-soft);
  border-radius: 6px;
  padding: 20px;
}

.border-blue { border-top: 3px solid #0f172a; }
.border-red { border-top: 3px solid #991b1b; }
.border-cyan { border-top: 3px solid #0891b2; }

.v-quote {
  font-style: italic;
  font-size: 0.95em;
  color: var(--text-sub);
}

.v-author {
  margin-top: 10px;
  text-align: right;
  font-weight: 600;
  font-size: 0.9em;
  color: var(--text-main);
}

/* --------------------------------------------------
   10) MOBİL UYUM
-------------------------------------------------- */
@media (max-width: 900px) {
  .process-grid-container {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="manifesto-text">
“Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir.”
</div>

<p>
Bu platformda mühendisliği; <strong>analiz, modelleme, doğrulama ve üretilebilirlik</strong> ekseninde ele alan bütüncül bir yaklaşım sunuyorum.
</p>

<p>
Amaç, mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.
</p>

<hr class="elegant-divider">

<h2>Analiz Tabanlı Tasarım Metodolojisi</h2>

<div class="process-grid-container">
  <div class="p-card style-1">
    <div class="p-num">01</div>
    <div class="p-title">Fiziksel Tanım</div>
    <div class="p-desc">Problemin gerçek davranışının ve sınır şartlarının belirlenmesi.</div>
  </div>

  <div class="p-card style-2">
    <div class="p-num">02</div>
    <div class="p-title">Sayısal Model</div>
    <div class="p-desc">Geometri, ağ yapısı ve çözüm parametrelerinin kurulması.</div>
  </div>

  <div class="p-card style-3">
    <div class="p-num">03</div>
    <div class="p-title">Analiz & Doğrulama</div>
    <div class="p-desc">Yakınsama, parametrik inceleme ve model güvenilirliği.</div>
  </div>

  <div class="p-card style-4">
    <div class="p-num">04</div>
    <div class="p-title">Mühendislik Yorumu</div>
    <div class="p-desc">Sonuçların değerlendirilmesi ve uygulanabilir kararlar.</div>
  </div>
</div>

<hr class="elegant-divider">

<h3 style="text-align:center;">Mühendislik Vizyonu</h3>

<div class="vision-grid">
  <div class="v-card border-blue">
    <p class="v-quote">“Engineering is the art of directing the great sources of power in nature.”</p>
    <p class="v-author">— Thomas Tredgold</p>
  </div>
  <div class="v-card border-red">
    <p class="v-quote">“Mechanics is the paradise of the mathematical sciences.”</p>
    <p class="v-author">— Leonardo da Vinci</p>
  </div>
  <div class="v-card border-cyan">
    <p class="v-quote">“It is engineering that changes the world.”</p>
    <p class="v-author">— Isaac Asimov</p>
  </div>
</div>
