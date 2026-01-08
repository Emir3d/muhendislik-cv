---
permalink: /projects/
title: "Engineering Projects"
excerpt: "Analysis-driven mechanical engineering portfolio"
author_profile: false
---

<style>
:root {
  --text-main: #1f2933;
  --text-sub: #4b5563;
  --card-bg: #ffffff;
  --border: #e5e7eb;
  --accent: #2563eb;
}

@media (prefers-color-scheme: dark) {
  :root {
    --text-main: #e5e7eb;
    --text-sub: #9ca3af;
    --card-bg: #0f172a;
    --border: #1e293b;
    --accent: #60a5fa;
  }
}

body {
  color: var(--text-main);
}

.portfolio-intro {
  max-width: 820px;
  margin-bottom: 3em;
}

.portfolio-intro h1 {
  font-size: 2.1em;
  margin-bottom: 0.4em;
}

.portfolio-intro p {
  font-size: 1.05em;
  color: var(--text-sub);
  line-height: 1.6;
}

.project-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 24px;
}

.project-card {
  background: var(--card-bg);
  border: 1px solid var(--border);
  border-radius: 10px;
  padding: 22px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.project-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 10px 25px rgba(0,0,0,0.12);
}

.project-title {
  font-size: 1.15em;
  font-weight: 700;
  margin-bottom: 0.3em;
}

.project-meta {
  font-size: 0.85em;
  color: var(--accent);
  margin-bottom: 0.8em;
}

.project-desc {
  font-size: 0.95em;
  color: var(--text-sub);
  line-height: 1.5;
  margin-bottom: 1em;
}

.project-tags {
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.project-tag {
  font-size: 0.75em;
  padding: 4px 8px;
  border-radius: 4px;
  background: rgba(37,99,235,0.1);
  color: var(--accent);
  border: 1px solid rgba(37,99,235,0.25);
}
</style>

<div class="portfolio-intro">
  <h1>Engineering Projects</h1>
  <p>
    Bu sayfa, yürütülen mühendislik çalışmalarını yalnızca sonuç odaklı değil;
    <strong>problem tanımı, analiz yaklaşımı ve mühendislik yorumu</strong>
    çerçevesinde sunmak amacıyla hazırlanmıştır.
  </p>
</div>

<div class="project-grid">

  <div class="project-card">
    <div class="project-title">Buckling Analysis of Composite Plates</div>
    <div class="project-meta">Structural Analysis · FEM · Theory</div>
    <div class="project-desc">
      Tabakalı kompozit plakaların burkulma davranışının
      Euler–Timoshenko–HSDT teorileri ve sonlu elemanlar yöntemi ile karşılaştırmalı analizi.
    </div>
    <div class="project-tags">
      <span class="project-tag">ANSYS</span>
      <span class="project-tag">Composite Mechanics</span>
      <span class="project-tag">Buckling</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-title">Shell Element Selection Study</div>
    <div class="project-meta">Modeling · Verification</div>
    <div class="project-desc">
      İnce cidarlı yapıların analizinde kullanılan kabuk elemanlarının
      yakınsama, doğruluk ve hesaplama maliyeti açısından değerlendirilmesi.
    </div>
    <div class="project-tags">
      <span class="project-tag">Shell281</span>
      <span class="project-tag">Mesh Independence</span>
      <span class="project-tag">Verification</span>
    </div>
  </div>

  <div class="project-card">
    <div class="project-title">CFD-Based Flow Optimization</div>
    <div class="project-meta">Fluid Dynamics · Simulation</div>
    <div class="project-desc">
      İç akış geometrilerinde basınç kaybının azaltılması amacıyla
      sayısal akış analizi ve parametrik optimizasyon çalışmaları.
    </div>
    <div class="project-tags">
      <span class="project-tag">ANSYS Fluent</span>
      <span class="project-tag">CFD</span>
      <span class="project-tag">Optimization</span>
    </div>
  </div>

</div>
