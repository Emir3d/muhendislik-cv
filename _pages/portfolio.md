---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. KIRIK PROFİL RESMİNİ GİZLEME (İşaretlediğin Yer) */
.author__avatar {
  display: none !important;
}

/* ===============================
   GLOBAL: HIGH-END TECH THEME
   =============================== */
body {
  background-color: #f8fafc !important; /* Çok hafif teknik gri zemin */
  color: #1e293b;
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, sans-serif;
}

/* Sayfa içeriği kapsayıcısı */
.page__content {
  padding-right: 0 !important;
  width: 100% !important;
}

/* ===============================
   BAŞLIK TASARIMI (FUTURE HEADER)
   =============================== */
.section-title {
  font-size: 2rem;
  font-weight: 900;
  color: #0f172a;
  margin: 4rem 0 2.5rem;
  letter-spacing: -1px;
  position: relative;
  display: inline-block;
}

.section-title::after {
  content: "";
  display: block;
  width: 60px;
  height: 6px;
  background: linear-gradient(90deg, #3b82f6, #06b6d4); /* Mavi-Turkuaz Gradyan */
  border-radius: 3px;
  margin-top: 10px;
  box-shadow: 0 0 15px rgba(6, 182, 212, 0.5); /* Neon Parlama */
}

/* ===============================
   GRID SİSTEMİ
   =============================== */
.projects-grid, .gallery-grid {
  display: grid;
  grid-template-columns: repeat(12, 1fr);
  gap: 30px;
  margin-bottom: 5rem;
}

/* ===============================
   KART TASARIMI: WHITE NEON
   =============================== */
.project-card {
  grid-column: span 6; /* 2 Sütun */
  background: #ffffff;
  border-radius: 20px;
  position: relative;
  overflow: hidden;
  border: 1px solid rgba(226, 232, 240, 0.8);
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  display: flex;
  flex-direction: column;
}

/* Öne Çıkan Kart (Featured) - SADECE GENİŞLİK KALDI, KENARLIK GİTTİ */
.project-card.featured {
  grid-column: span 12; /* Tam genişlik */
  /* border-left: 6px solid #3b82f6;  <-- BU SATIRI SİLDİK */
}

/* 🔥 HOVER EFEKTİ: NEON PARLAMA 🔥 */
.project-card:hover {
  transform: translateY(-10px) scale(1.02);
  border-color: #3b82f6;
  /* KARTI KALDIRIP ALTINA MAVİ IŞIK VERİYORUZ */
  box-shadow: 0 20px 40px -10px rgba(59, 130, 246, 0.4);
  z-index: 10;
}

/* Kartın içine hafif mavi bir sis efekti */
.project-card::before {
  content: "";
  position: absolute;
  top: 0; left: 0; width: 100%; height: 100%;
  background: linear-gradient(135deg, rgba(59,130,246,0.05) 0%, transparent 100%);
  opacity: 0;
  transition: opacity 0.4s;
}
.project-card:hover::before { opacity: 1; }

/* ===============================
   KART İÇERİĞİ
   =============================== */
.card-body {
  padding: 30px;
  flex-grow: 1;
  z-index: 2; /* Efektin üstünde kalsın */
}

.card-category {
  color: #06b6d4; /* Turkuaz */
  font-weight: 800;
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 1.5px;
  margin-bottom: 10px;
  display: block;
}

.card-title {
  font-size: 1.4rem;
  font-weight: 800;
  margin: 5px 0 15px 0;
  color: #1e293b;
  line-height: 1.3;
}

.card-desc {
  font-size: 1rem;
  color: #64748b;
  line-height: 1.6;
}
.card-desc ul { padding-left: 18px; margin: 0; }
.card-desc li { margin-bottom: 6px; }

/* ===============================
   ETİKETLER (NEON HAPLAR)
   =============================== */
.card-footer {
  padding: 0 30px 30px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
  z-index: 2;
}

.tech-tag {
  font-size: 0.75rem;
  padding: 6px 14px;
  border-radius: 50px; /* Tam yuvarlak */
  font-weight: 700;
  background: rgba(241, 245, 249, 1);
  color: #475569;
  border: 1px solid #e2e8f0;
  transition: all 0.3s ease;
}

/* Hover olunca etiketler de parlasın */
.project-card:hover .tech-tag {
  background: rgba(59, 130, 246, 0.1);
  color: #2563eb;
  border-color: rgba(59, 130, 246, 0.3);
}

/* ===============================
   GALERİ TASARIMI
   =============================== */
.gallery-item {
  grid-column: span 6;
  background: #fff;
  border-radius: 20px;
  overflow: hidden;
  border: 1px solid #e2e8f0;
  transition: all 0.4s ease;
  position: relative;
}

/* 🔥 ŞAHİ TOP (EN ALTA, BÜYÜK VE ORTADA) 🔥 */
.gallery-item.full-width {
  grid-column: span 12;
  margin-top: 20px;
  box-shadow: 0 10px 30px rgba(0,0,0,0.1); /* Varsayılan olarak gölgeli */
}

.gallery-img-box {
  height: 260px;
  width: 100%;
  overflow: hidden;
  position: relative;
}

/* Top görseli daha yüksek */
.gallery-item.full-width .gallery-img-box { height: 450px; }

.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.6s cubic-bezier(0.25, 0.46, 0.45, 0.94);
}

/* Hover Efekti */
.gallery-item:hover {
  transform: translateY(-8px);
  box-shadow: 0 20px 50px -10px rgba(6, 182, 212, 0.3); /* Turkuaz Neon Gölge */
  border-color: #06b6d4;
}

.gallery-item:hover .gallery-img-box img {
  transform: scale(1.08);
}

.gallery-info {
  padding: 25px;
  background: #fff;
  border-top: 1px solid #f1f5f9;
  position: relative;
  z-index: 5;
}

.gallery-info h3 {
  margin: 0;
  font-size: 1.15rem;
  font-weight: 800;
  color: #0f172a;
}
.gallery-info p {
  margin: 5px 0 0;
  font-size: 0.85rem;
  color: #06b6d4;
  font-weight: 700;
  text-transform: uppercase;
}

/* MOBİL AYARLARI */
@media(max-width: 900px){
  .project-card, .gallery-item { grid-column: span 12 !important; }
}
</style>

<h2 class="section-title">Mühendislik Analizleri</h2>

<div class="projects-grid">

  <div class="project-card featured">
    <div class="card-body">
      <span class="card-category">Akademik Araştırma</span>
      <h3 class="card-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
      <div class="card-desc">
        <ul>
          <li>Euler-Timoshenko teorilerinin kıyaslanması.</li>
          <li>Farklı fiber dizilim açılarının (stacking) kritik burkulma yüküne etkisi.</li>
          <li>FEM analizi ve analitik doğrulama.</li>
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
        Mukavemet hesapları için otomatik Mohr çemberi çizen MATLAB GUI tasarımı ve gerilme analizi.
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag">MATLAB App Designer</span>
    </div>
  </div>

  <div class="project-card">
    <div class="card-body">
      <span class="card-category">TÜBİTAK 2209-A</span>
      <h3 class="card-title">VİSA SÖR Asansör</h3>
      <div class="card-desc">
        Özel asansör tasarımı, mekanik boyutlandırma ve güvenlik sistemi optimizasyonu.
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
      <span class="tech-tag">SolidWorks</span>
      <span class="tech-tag">CFD</span>
    </div>
  </div>
  
  <div class="project-card">
    <div class="card-body">
      <span class="card-category">Gönüllü Proje</span>
      <h3 class="card-title">Müsilaj Sorunu Araştırması</h3>
      <div class="card-desc">
        Müsilaj oluşum mekanizmaları ve akışkanlar mekaniği temelli çözüm önerileri.
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

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
    <div class="gallery-info">
      <h3>Konsept Uçak Tasarımı</h3>
      <p>Inventor Pro / Render</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
    <div class="gallery-info">
      <h3>Alpagu-X İHA</h3>
      <p>Havacılık Tasarımı</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>M16 Piyade Tüfeği</h3>
      <p>Montaj Modelleme</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Turbo-Jet Motoru</h3>
      <p>SolidWorks</p>
    </div>
  </div>
  
  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>3D Superman Logosu</h3>
      <p>3DS MAX</p>
    </div>
  </div>
  
  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Manifold CFD Mesh Ağı</h3>
      <p>ANSYS Meshing</p>
    </div>
  </div>

  <div class="gallery-item full-width">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Top" onerror="this.src='https://via.placeholder.com/800x400';">
    </div>
    <div class="gallery-info">
      <h3>Şahi Top Modeli</h3>
      <p>Inventor / Tarihi Modelleme</p>
    </div>
  </div>

</div>
