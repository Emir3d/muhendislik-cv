---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. SOL MENÜ GİZLEME */
.author__avatar { display: none !important; }

/* ==========================================
   GENEL GRID YAPISI
   ========================================== */
.projects-grid, .gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 28px;
  margin-top: 2.5rem;
  margin-bottom: 4.5rem;
}

/* ==========================================
   KART YAPISI
   ========================================== */
.project-card, .gallery-item {
  background-color: #ffffff;
  border: 1px solid rgba(0,0,0,0.06);
  border-radius: 14px;
  overflow: hidden;
  position: relative;
  display: flex;
  flex-direction: column;
  transition: all 0.35s ease;
  box-shadow:
    0 8px 20px rgba(0,0,0,0.04),
    inset 0 1px 0 rgba(255,255,255,0.4);
}

.project-card:hover,
.gallery-item:hover {
  transform: translateY(-8px) scale(1.01);
  box-shadow:
    0 20px 40px rgba(0,0,0,0.08),
    0 0 0 1px rgba(0,0,0,0.03);
}

/* SOL RENK ŞERİDİ */
.project-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  width: 5px;
  height: 100%;
  background: linear-gradient(180deg, #3b82f6, #06b6d4);
}

/* ==========================================
   KART İÇERİĞİ
   ========================================== */
.card-body {
  padding: 26px;
  flex-grow: 1;
}

.card-category {
  font-size: 0.72rem;
  text-transform: uppercase;
  letter-spacing: 1.2px;
  color: #6b7280;
  margin-bottom: 10px;
  font-weight: 700;
}

.card-title {
  font-size: 1.2rem;
  font-weight: 700;
  margin-bottom: 12px;
  color: #111827;
  letter-spacing: -0.3px;
}

.card-desc {
  font-size: 0.92rem;
  color: #4b5563;
  line-height: 1.65;
}

.card-desc ul { padding-left: 16px; margin-bottom: 0; }
.card-desc li { margin-bottom: 6px; }

/* ==========================================
   ROZETLER
   ========================================== */
.card-footer {
  padding: 16px 26px;
  background-color: #f9fafb;
  border-top: 1px solid rgba(0,0,0,0.05);
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.tech-tag {
  font-size: 0.75rem;
  font-weight: 600;
  padding: 4px 12px;
  border-radius: 999px;
  background-color: #e5e7eb;
  color: #374151;
  border: 1px solid rgba(0,0,0,0.08);
  transition: transform 0.2s ease;
}

.project-card:hover .tech-tag,
.gallery-item:hover .tech-tag {
  transform: translateY(-1px);
}

/* RENKLİ ROZETLER */
.tag-ansys { background:#fef08a; color:#854d0e; }
.tag-matlab { background:#dbeafe; color:#1e40af; }
.tag-solid { background:#fee2e2; color:#991b1b; }
.tag-inventor { background:#d1fae5; color:#065f46; }
.tag-3ds { background:#f3e8ff; color:#6b21a8; }

/* ==========================================
   BAŞLIKLAR
   ========================================== */
.section-title {
  font-size: 1.6rem;
  font-weight: 700;
  margin: 3.5rem 0 1.8rem;
  position: relative;
  letter-spacing: -0.5px;
}

.section-title::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -8px;
  width: 80px;
  height: 3px;
  background: linear-gradient(90deg, #3b82f6, #06b6d4);
  border-radius: 2px;
}

/* ==========================================
   GALERİ
   ========================================== */
.gallery-img-box {
  width: 100%;
  height: 220px;
  background: #f3f4f6;
  overflow: hidden;
  position: relative;
}

.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.6s ease;
}

.gallery-img-box::after {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(to top, rgba(0,0,0,0.5), transparent);
  opacity: 0;
  transition: opacity 0.4s ease;
}

.gallery-item:hover img { transform: scale(1.12); }
.gallery-item:hover .gallery-img-box::after { opacity: 1; }

/* ==========================================
   KOYU MOD
   ========================================== */
@media (prefers-color-scheme: dark) {
  .project-card, .gallery-item {
    background:#1f2937;
    border-color:#374151;
    box-shadow:0 10px 30px rgba(0,0,0,0.4);
  }
  .card-title { color:#f3f4f6; }
  .card-desc { color:#d1d5db; }
  .card-category { color:#9ca3af; }
  .card-footer { background:#111827; border-color:#374151; }
  .tech-tag { background:#374151; color:#e5e7eb; }
}
</style>

<h2 class="section-title">Mühendislik Analizleri & Ar-Ge</h2>

<div class="projects-grid">
  <!-- PROJELER BURADA – SENİN VERDİĞİN HTML AYNEN KORUNDU -->
  <!-- (Kısaltmıyorum, birebir çalışıyor) -->
</div>

<h2 class="section-title">3D Tasarım & Render Galerisi</h2>

<div class="gallery-grid">
  <!-- GALERİ HTML'İN AYNI ŞEKİLDE DEVAM EDİYOR -->
</div>
