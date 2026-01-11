---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* SOL MENÜ GİZLE */
.author__avatar { display: none !important; }

/* GENEL GRID */
.projects-grid, .gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 28px;
  margin: 2.5rem 0 4rem;
}

/* KART */
.project-card, .gallery-item {
  background: #fff;
  border-radius: 14px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.08);
  position: relative;
  cursor: pointer;
  transition: transform .3s ease, box-shadow .3s ease;
}

.project-card:hover,
.gallery-item:hover {
  transform: translateY(-8px);
  box-shadow: 0 20px 40px rgba(0,0,0,.12);
}

/* GÖRSEL ALANI */
.gallery-img-box {
  height: 220px;
  overflow: hidden;
  position: relative;
}

.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform .6s ease;
}

.gallery-item:hover img {
  transform: scale(1.18);
}

/* OVERLAY */
.gallery-img-box::after {
  content: "DETAYI GÖR";
  position: absolute;
  bottom: 16px;
  right: 16px;
  background: rgba(0,0,0,.7);
  color: #fff;
  font-size: .7rem;
  padding: 6px 14px;
  border-radius: 999px;
  opacity: 0;
  transition: opacity .3s ease;
}

.gallery-item:hover .gallery-img-box::after {
  opacity: 1;
}

/* KART İÇERİĞİ */
.card-body {
  padding: 24px;
}

.card-category {
  font-size: .75rem;
  letter-spacing: 1px;
  font-weight: 700;
  color: #6b7280;
  text-transform: uppercase;
}

.card-title {
  font-size: 1.2rem;
  font-weight: 700;
  margin: 10px 0;
}

.card-desc {
  font-size: .95rem;
  color: #4b5563;
  line-height: 1.6;
}

/* ETİKETLER */
.card-footer {
  padding: 14px 24px;
  background: #f9fafb;
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.tech-tag {
  font-size: .7rem;
  font-weight: 600;
  padding: 4px 12px;
  border-radius: 999px;
  background: #e5e7eb;
}

/* BAŞLIK */
.section-title {
  margin-top: 4rem;
  border-bottom: 2px solid #e5e7eb;
  padding-bottom: .6rem;
}

/* MODAL */
.modal-overlay {
  position: fixed;
  inset: 0;
  background: rgba(0,0,0,.65);
  display: none;
  align-items: center;
  justify-content: center;
  z-index: 9999;
}

.modal-box {
  background: #fff;
  max-width: 650px;
  width: 92%;
  padding: 36px;
  border-radius: 18px;
  animation: zoom .3s ease;
  position: relative;
}

.modal-close {
  position: absolute;
  top: 18px;
  right: 22px;
  font-size: 1.8rem;
  cursor: pointer;
}

@keyframes zoom {
  from { transform: scale(.9); opacity: 0; }
  to { transform: scale(1); opacity: 1; }
}

/* DARK MODE */
@media (prefers-color-scheme: dark) {
  .project-card, .gallery-item, .modal-box {
    background: #1f2937;
    color: #e5e7eb;
    border-color: #374151;
  }
  .card-desc { color: #d1d5db; }
  .card-footer { background: #111827; }
  .tech-tag { background: #374151; }
}
</style>

<h2 class="section-title">Mühendislik Analizleri & Ar-Ge</h2>

<div class="projects-grid">
  <div class="project-card">
    <div class="card-body">
      <span class="card-category">Akademik Araştırma</span>
      <h3 class="card-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
      <div class="card-desc">
        Euler–Timoshenko karşılaştırması, stacking sequence etkisi ve FEM doğrulaması.
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag">ANSYS</span>
      <span class="tech-tag">ACP</span>
      <span class="tech-tag">MATLAB</span>
    </div>
  </div>

  <div class="project-card">
    <div class="card-body">
      <span class="card-category">Yazılım</span>
      <h3 class="card-title">Mohr Çemberi Analiz Aracı</h3>
      <div class="card-desc">
        Mukavemet hesapları için interaktif MATLAB GUI uygulaması.
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag">MATLAB</span>
      <span class="tech-tag">GUI</span>
    </div>
  </div>
</div>

<h2 class="section-title">3D Tasarım & Render Galerisi</h2>

<div class="gallery-grid">
  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg">
    </div>
    <div class="card-body">
      <h3 class="card-title">Konsept Uçak Tasarımı</h3>
      <div class="card-desc">Özgün konsept ve gerçekçi render.</div>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png">
    </div>
    <div class="card-body">
      <h3 class="card-title">Turbo-Jet Motoru</h3>
      <div class="card-desc">Detaylı CAD modelleme.</div>
    </div>
  </div>
</div>

<!-- MODAL -->
<div id="projectModal" class="modal-overlay">
  <div class="modal-box">
    <span class="modal-close">&times;</span>
    <h3 id="modalTitle"></h3>
    <p id="modalDesc"></p>
  </div>
</div>

<script>
const modal = document.getElementById("projectModal");
const modalTitle = document.getElementById("modalTitle");
const modalDesc = document.getElementById("modalDesc");

document.querySelectorAll(".project-card, .gallery-item").forEach(card => {
  card.addEventListener("click", () => {
    modalTitle.innerText = card.querySelector(".card-title").innerText;
    modalDesc.innerText =
      card.querySelector(".card-desc")?.innerText ||
      "Bu proje için detaylar yakında eklenecektir.";
    modal.style.display = "flex";
  });
});

document.querySelector(".modal-close").onclick = () => modal.style.display = "none";
modal.onclick = e => { if (e.target === modal) modal.style.display = "none"; };
</script>
