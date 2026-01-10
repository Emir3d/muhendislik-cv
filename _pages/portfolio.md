---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. SOL MENÜ GİZLEME (Tam ekran deneyimi için) */
.author__avatar { display: none !important; }
.sidebar { display: none !important; } /* Yan menüyü tamamen kaldırıyoruz ki geniş tasarım sığsın */
.page__content { width: 100% !important; max-width: 100% !important; padding: 0 !important; }

/* ===============================
   GLOBAL MODERN THEME
   =============================== */
body {
  background: radial-gradient(1200px at 10% 10%, #0f172a, #020617) !important;
  color: #e5e7eb;
  font-family: 'Inter', sans-serif;
}

/* Sayfa içeriği kapsayıcısı */
.portfolio-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
}

/* ===============================
   SECTION HEADERS
   =============================== */
.section-title {
  font-size: 2.2rem;
  font-weight: 800;
  color: #e5e7eb;
  margin: 5rem 0 3rem;
  letter-spacing: -1px;
  position: relative;
  display: inline-block;
}

.section-title::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -14px;
  width: 100%; /* Çizgiyi başlık kadar uzat */
  max-width: 120px;
  height: 4px;
  background: linear-gradient(90deg, #22d3ee, #38bdf8);
  box-shadow: 0 0 20px rgba(56,189,248,.6);
  border-radius: 2px;
}

/* ===============================
   PROJECT GRID – VITRIN
   =============================== */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 32px;
  margin-bottom: 5rem;
}

/* ===============================
   PROJECT CARD – BASE
   =============================== */
.project-card {
  grid-column: span 4; /* Standart kartlar 4 birim yer kaplar */
  background: rgba(255,255,255,.03);
  border-radius: 22px;
  overflow: hidden;
  position: relative;
  backdrop-filter: blur(14px);
  -webkit-backdrop-filter: blur(14px);
  border: 1px solid rgba(255,255,255,.08);
  transition: .5s cubic-bezier(.4,0,.2,1);
  display: flex;
  flex-direction: column;
}

/* ===============================
   FEATURED PROJECT (ÖNE ÇIKAN)
   =============================== */
.project-card.featured {
  grid-column: span 8; /* Geniş kart */
  min-height: 380px;
  background: linear-gradient(145deg, rgba(255,255,255,0.05), rgba(255,255,255,0.01));
  border: 1px solid rgba(56,189,248,0.2); /* Hafif mavi çerçeve */
}

.project-card::before {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(120deg, transparent 40%, rgba(56,189,248,.1), transparent 60%);
  opacity: 0;
  transition: .6s;
  pointer-events: none;
}

.project-card:hover::before {
  opacity: 1;
}

/* ===============================
   CARD BODY
   =============================== */
.card-body {
  padding: 36px;
  color: #e5e7eb;
  flex-grow: 1;
}

.card-category {
  color: #38bdf8;
  font-weight: 700;
  letter-spacing: 1px;
  font-size: 0.8rem;
  text-transform: uppercase;
  margin-bottom: 10px;
  display: block;
}

.card-title {
  font-size: 1.5rem;
  font-weight: 800;
  margin: 10px 0 15px 0;
  line-height: 1.3;
  color: #f1f5f9;
}

.card-desc {
  font-size: .95rem;
  color: #94a3b8; /* Biraz daha sönük gri */
  line-height: 1.6;
}
.card-desc ul { padding-left: 20px; margin: 0; }
.card-desc li { margin-bottom: 5px; }

/* ===============================
   TECH TAGS – NEON
   =============================== */
.card-footer {
  padding: 0 36px 32px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.tech-tag {
  font-size: 0.75rem;
  padding: 6px 12px;
  border-radius: 8px;
  font-weight: 600;
  background: rgba(56,189,248,.1);
  border: 1px solid rgba(56,189,248,.3);
  color: #67e8f9; /* Camgöbeği Neon */
  box-shadow: 0 0 15px rgba(56,189,248,.1);
  transition: all 0.3s ease;
}

.tech-tag:hover {
  background: rgba(56,189,248,.2);
  box-shadow: 0 0 20px rgba(56,189,248,.4);
}

/* ===============================
   HOVER MOTION
   =============================== */
.project-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 20px 80px -10px rgba(56,189,248,.15);
  border-color: rgba(56,189,248,.4);
}

/* ===============================
   GALLERY – CINEMATIC
   =============================== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 28px;
  margin-bottom: 5rem;
}

.gallery-item {
  grid-column: span 4;
  border-radius: 26px;
  overflow: hidden;
  position: relative;
  background: #0f172a;
  border: 1px solid rgba(255,255,255,0.1);
  transition: all 0.4s ease;
}

/* Sinematik Geniş Görseller */
.gallery-item.cinematic {
  grid-column: span 6;
}

.gallery-img-box {
  height: 300px;
  width: 100%;
  overflow: hidden;
}

.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.6s ease;
  filter: saturate(1.1) contrast(1.1); /* Renkleri patlat */
}

/* Resim üzeri gradient kaplama */
.gallery-item::after {
  content: "";
  position: absolute;
  inset: 0;
  background: linear-gradient(to top, rgba(2,6,23,0.95) 0%, transparent 60%);
  pointer-events: none;
}

.gallery-item:hover {
  transform: scale(1.02);
  border-color: #38bdf8;
  box-shadow: 0 0 30px rgba(56,189,248,0.3);
}

.gallery-item:hover .gallery-img-box img {
  transform: scale(1.1);
}

/* Galeri Yazıları (Resmin üstüne biner) */
.gallery-info {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  padding: 25px;
  z-index: 2;
}

.gallery-info h3 {
  margin: 0;
  font-size: 1.2rem;
  color: #fff;
  text-shadow: 0 2px 10px rgba(0,0,0,0.5);
}

.gallery-info p {
  margin: 5px 0 0 0;
  font-size: 0.85rem;
  color: #38bdf8;
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* ===============================
   MOBILE
   =============================== */
@media(max-width:900px){
  .projects-grid, .gallery-grid { grid-template-columns: 1fr; }
  .project-card, .gallery-item, .project-card.featured, .gallery-item.cinematic { grid-column: span 12; }
}
</style>

<div class="portfolio-container">

  <h2 class="section-title">Mühendislik Analizleri</h2>

  <div class="projects-grid">

    <div class="project-card featured">
      <div class="card-body">
        <span class="card-category">Akademik Araştırma</span>
        <h3 class="card-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
        <div class="card-desc">
          <ul>
            <li>Euler-Timoshenko teorilerinin kıyaslanması ve analitik çözümler.</li>
            <li>Farklı fiber dizilim açılarının (stacking sequence) kritik burkulma yüküne etkisinin incelenmesi.</li>
            <li>ANSYS ACP modülü ile Sonlu Elemanlar (FEM) doğrulaması.</li>
          </ul>
        </div>
      </div>
      <div class="card-footer">
        <span class="tech-tag">ANSYS ACP</span>
        <span class="tech-tag">Static Structural</span>
        <span class="tech-tag">MATLAB</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-body">
        <span class="card-category">Yazılım Geliştirme</span>
        <h3 class="card-title">Mohr Çemberi Aracı</h3>
        <div class="card-desc">
          Mukavemet hesapları için otomatik Mohr çemberi çizen, asal gerilmeleri hesaplayan MATLAB GUI tasarımı.
        </div>
      </div>
      <div class="card-footer">
        <span class="tech-tag">MATLAB GUI</span>
        <span class="tech-tag">Algoritma</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-body">
        <span class="card-category">TÜBİTAK 2209-A</span>
        <h3 class="card-title">VİSA SÖR Asansör</h3>
        <div class="card-desc">
          Engelli bireyler için özel asansör tasarımı. Mekanik boyutlandırma ve güvenlik optimizasyonu.
        </div>
      </div>
      <div class="card-footer">
        <span class="tech-tag">SolidWorks</span>
        <span class="tech-tag">Mekanik Analiz</span>
      </div>
    </div>

    <div class="project-card">
      <div class="card-body">
        <span class="card-category">Bitirme Tezi</span>
        <h3 class="card-title">Francis Türbin Tasarımı</h3>
        <div class="card-desc">
          Keban Barajı verileriyle hidrodinamik boyutlandırma. Çark ve salyangoz geometrisinin CFD tasarımı.
        </div>
      </div>
      <div class="card-footer">
        <span class="tech-tag">CFD / Akış</span>
        <span class="tech-tag">SolidWorks</span>
      </div>
    </div>
    
     <div class="project-card">
      <div class="card-body">
        <span class="card-category">Gönüllü Proje</span>
        <h3 class="card-title">Müsilaj Sorunu</h3>
        <div class="card-desc">
          Müsilaj oluşum mekanizmaları ve akışkanlar mekaniği temelli çözüm önerileri üzerine disiplinlerarası çalışma.
        </div>
      </div>
      <div class="card-footer">
        <span class="tech-tag">Akışkanlar Mekaniği</span>
        <span class="tech-tag">Araştırma</span>
      </div>
    </div>

  </div>

  <h2 class="section-title">3D Tasarım & Render</h2>

  <div class="gallery-grid">

    <div class="gallery-item cinematic">
      <div class="gallery-img-box">
        <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400/0f172a/38bdf8?text=UCAK+RENDER';">
      </div>
      <div class="gallery-info">
        <h3>Konsept Uçak Tasarımı</h3>
        <p>Inventor Pro / Render</p>
      </div>
    </div>

    <div class="gallery-item cinematic">
      <div class="gallery-img-box">
        <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400/0f172a/38bdf8?text=ALPAGU+IHA';">
      </div>
      <div class="gallery-info">
        <h3>Alpagu-X İHA</h3>
        <p>Havacılık Tasarımı</p>
      </div>
    </div>

    <div class="gallery-item">
      <div class="gallery-img-box">
        <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300/0f172a/38bdf8?text=M16';">
      </div>
      <div class="gallery-info">
        <h3>M16 Piyade Tüfeği</h3>
        <p>Montaj Modelleme</p>
      </div>
    </div>

    <div class="gallery-item">
      <div class="gallery-img-box">
        <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300/0f172a/38bdf8?text=JET+MOTOR';">
      </div>
      <div class="gallery-info">
        <h3>Turbo-Jet Motoru</h3>
        <p>SolidWorks</p>
      </div>
    </div>
    
    <div class="gallery-item">
      <div class="gallery-img-box">
        <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300/0f172a/38bdf8?text=LOGO';">
      </div>
      <div class="gallery-info">
        <h3>3D Superman Logosu</h3>
        <p>3DS MAX</p>
      </div>
    </div>

    <div class="gallery-item">
      <div class="gallery-img-box">
        <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300/0f172a/38bdf8?text=CFD+MESH';">
      </div>
      <div class="gallery-info">
        <h3>Manifold Mesh Ağı</h3>
        <p>ANSYS Meshing</p>
      </div>
    </div>

  </div>

</div>
