---
permalink: /
title: "Mühendisliğe Analitik ve Bütüncül Bir Bakış"
excerpt: "Analiz, modelleme ve doğrulama temelli mühendislik yaklaşımı"
author_profile: false
header:
  overlay_image: https://emir3d.github.io/muhendislik-cv/images/header_bg.png
  overlay_filter: 0.6
---

<style>
/* ======================================================
   GLOBAL ARKA PLAN — AÇIK / KOYU MOD
   ====================================================== */
:root {
  --bg-main: #f8fafc;
  --bg-card: #ffffff;
  --text-main: #111827;
  --text-soft: #374151;
  --border-main: #d1d5db;
  --accent: #334155;
}

@media (prefers-color-scheme: dark) {
  :root {
    --bg-main: #020617;
    --bg-card: #020617;
    --text-main: #e5e7eb;
    --text-soft: #cbd5e1;
    --border-main: #334155;
    --accent: #64748b;
  }
}

/* SAYFA ZEMİNİ */
body,
.initial-content,
.page__content {
  background-color: var(--bg-main) !important;
}

/* ======================================================
   YAZI RENKLERİNİ ZORLA
   ====================================================== */
.page__content,
.page__content * {
  color: var(--text-main) !important;
}

.page__content p {
  font-size: 1.05rem;
  line-height: 1.8;
  color: var(--text-soft) !important;
  max-width: 760px;
}

/* ======================================================
   HERO
   ====================================================== */
.page__hero--overlay .page__title,
.page__hero--overlay .page__lead {
  color: #f8fafc !important;
}

/* ======================================================
   MANİFESTO
   ====================================================== */
.manifesto {
  text-align: center;
  font-size: 1.15rem;
  font-style: italic;
  max-width: 760px;
  margin: 3rem auto;
  color: var(--text-soft);
}

/* ======================================================
   AYRAÇ
   ====================================================== */
.section-divider {
  border: none;
  height: 1px;
  background: linear-gradient(
    to right,
    transparent,
    var(--border-main),
    transparent
  );
  margin: 4rem 0;
}

/* ======================================================
   SÜREÇ AKIŞI — RENK UYUMLU
   ====================================================== */
.process-flow {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(140px, 1fr));
  gap: 1rem;
  max-width: 900px;
  margin: 3rem auto;
}

.flow-step {
  padding: 0.9rem 1rem;
  text-align: center;
  border: 1px solid var(--border-main);
  border-radius: 10px;
  background-color: var(--bg-card);
  font-size: 0.9rem;
  transition: all 0.25s ease;
}

.flow-step:hover {
  transform: translateY(-3px);
  border-color: var(--accent);
}

/* VURGU KUTUSU — AYNI PALET */
.flow-step.final {
  border-width: 2px;
  border-color: var(--accent);
  font-weight: 600;
}

/* ======================================================
   ÜNLÜ SÖZLER
   ====================================================== */
.quotes {
  max-width: 760px;
  margin: 3rem auto 0;
}

.quotes blockquote {
  border-left: 3px solid var(--border-main);
  padding-left: 1.2rem;
  margin: 2rem 0;
  font-size: 0.95rem;
  color: var(--text-soft);
}

.quotes span {
  display: block;
  margin-top: 0.4rem;
  font-size: 0.85rem;
  opacity: 0.7;
}
</style>

<div class="manifesto">
“Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme disiplinidir.”
</div>

Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; analiz, modelleme, doğrulama ve üretilebilirlik ekseninde ele alan bütüncül bir yaklaşım sunuyorum.

<hr class="section-divider">

## Analiz Tabanlı Mühendislik Yaklaşımı

<div class="process-flow">
  <div class="flow-step">Problem Tanımı</div>
  <div class="flow-step">Matematiksel Model</div>
  <div class="flow-step">Sayısal Analiz</div>
  <div class="flow-step">Doğrulama</div>
  <div class="flow-step final">Mühendislik Kararı</div>
</div>

<hr class="section-divider">

## Mühendislik Vizyonu

<div class="quotes">
  <blockquote>
    “All models are wrong, but some are useful.”
    <span>— George E. P. Box</span>
  </blockquote>

  <blockquote>
    “Science can amuse and fascinate us all, but it is engineering that changes the world.”
    <span>— Isaac Asimov</span>
  </blockquote>
</div>
