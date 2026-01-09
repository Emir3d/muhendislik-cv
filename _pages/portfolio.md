---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. TEMEL AYARLAR & GİZLEMELER */
.author__avatar { display: none !important; } /* Sol menü resmi gizle */

:root {
  --hud-primary: #0ea5e9; /* Elektrik Mavisi - Ana Vurgu Rengi */
  --hud-dark: #0f172a;    /* Çok Koyu Lacivert (Arka Plan) */
  --hud-card: #1e293b;    /* Kart Rengi (Koyu Mod) */
  --hud-text: #e2e8f0;    /* Açık Yazı Rengi */
  --hud-muted: #94a3b8;   /* Sönük Yazı Rengi */
  --hud-font-tech: "SF Mono", "Roboto Mono", Menlo, monospace; /* Teknik Font */
}

/* ==========================================
   YENİ NESİL BAŞLIKLAR (Tech Headers)
   ========================================== */
h2.section-title {
  font-family: var(--hud-font-tech);
  text-transform: uppercase;
  letter-spacing: 2px;
  font-size: 1.5rem;
  font-weight: 800;
  margin: 4rem 0 2rem 0;
  padding-bottom: 15px;
  position: relative;
  color: #111; /* Açık mod rengi */
  display: flex;
  align-items: center;
}

/* Başlık Altındaki Teknik Çizgi */
h2.section-title::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 2px;
  background: linear-gradient(90deg, var(--hud-primary), transparent); /* Maveden şeffafa geçiş */
}

/* Başlık Önündeki Yanıp Sönen İmleç Efekti */
h2.section-title::before {
  content: "▐";
  margin-right: 10px;
  color: var(--hud-primary);
  animation: blink 1s step-end infinite;
}
@keyframes blink { 50% { opacity: 0; } }


/* ==========================================
   BÖLÜM 1: ANALİZ KARTLARI (Data Modules)
   ========================================== */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
  gap: 30px;
  margin-bottom: 5rem;
}

.project-card {
  background-color: #fff; /* Açık mod zemin */
  border: 1px solid #e2e8f0;
  border-top: 4px solid var(--hud-primary); /* Üstte mavi şerit */
  border-radius: 4px;
  padding: 25px;
  position: relative;
  overflow: hidden;
  transition: all 0.3s ease;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

/* Hover Efekti: Kart yukarı kalkar ve gölge maviye döner */
.project-card:hover {
  transform: translateY(-7px);
  box-shadow: 0 20px 25px -5px rgba(14, 165, 233, 0.15), 0 0 0 1px var(--hud-primary);
}

/* Kartın içindeki teknik detaylar */
.card-category {
  font-family: var(--hud-font-tech);
  font-size: 0.7rem;
  text-transform: uppercase;
  color: var(--hud-primary);
  letter-spacing: 1px;
  margin-bottom: 8px;
  display: block;
  font-weight: 700;
}

.card-title {
  font-size: 1.25rem;
  font-weight: 700;
  margin-bottom: 15px;
  line-height: 1.3;
}

.card-desc {
  font-size: 0.95rem;
  line-height: 1.6;
  color: #555;
}
.card-desc ul { padding-left: 18px; margin-bottom: 15px; }
.card-desc li { margin-bottom: 8px; position: relative; list-style: none; }
/* Liste maddelerinin başına teknik ok işareti koyalım */
.card-desc li::before {
  content: "►";
  font-size: 0.7rem;
  color: var(--hud-primary);
  position: absolute;
  left: -18px;
  top: 4px;
}

/* ==========================================
   YENİ NESİL ROZETLER (Tech Badges v2)
   ========================================== */
.card-footer {
  margin-top: 20px;
  padding-top: 15px;
  border-top: 1px dashed rgba(128,128,128,0.3); /* Kesik çizgili ayraç */
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.tech-tag {
  font-family: var(--hud-font-tech);
  font-size: 0.65rem;
  font-weight: 700;
  text-transform: uppercase;
  padding: 4px 10px;
  border: 1px solid #e2e8f0;
  background-color: #f8fafc;
  color: #475569;
  border-radius: 2px; /* Daha köşeli, teknik görünüm */
  letter-spacing: 0.5px;
}

/* Önemli yazılımlar için özel vurgu */
.tag-ansys, .tag-matlab, .tag-solid, .tag-inventor {
  border-color: var(--hud-primary);
  color: var(--hud-dark);
  background-color: rgba(14, 165, 233, 0.05); /* Çok hafif mavi zemin */
}


/* ==========================================
   BÖLÜM 2: GALERİ (CAD Viewport Style)
   ========================================== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 30px;
  margin-bottom: 4rem;
}

.gallery-item {
  position: relative;
  background: #fff;
  border: 1px solid #e2e8f0;
  transition: all 0.3s ease;
}

/* Hover Efekti: Çerçeve mavi yanar */
.gallery-item:hover {
  border-color: var(--hud-primary);
  box-shadow: 0 0 15px rgba(14, 165, 233, 0.2);
}

.gallery-img-box {
  height: 220px;
  background-color: #f1f5f9;
  overflow: hidden;
  position: relative;
  /* CAD ekranı gibi köşe çizgileri ekleyelim */
}

/* CAD Köşe Efektleri */
.gallery-img-box::after {
  content: "";
  position: absolute;
  top: 10px; left: 10px; right: 10px; bottom: 10px;
  border: 1px solid rgba(14, 165, 233, 0.3); /* İnce mavi iç çerçeve */
  pointer-events: none;
  z-index: 2;
}

.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);
  filter: grayscale(30%); /* Varsayılan olarak biraz teknik/soluk dursun */
}

.gallery-item:hover .gallery-img-box img {
  transform: scale(1.1);
  filter: grayscale(0%); /* Üzerine gelince renkler canlansın */
}

/* Galeri Metin Alanı */
.gallery-info {
  padding: 20px;
  border-top: 2px solid var(--hud-primary); /* Resimle metni ayıran kalın çizgi */
  background: #fff;
}

.gallery-info h3 {
  font-size: 1.1rem;
  font-weight: 700;
  margin: 0 0 5px 0;
}

.gallery-info p {
  font-size: 0.9rem;
  color: #666;
  margin: 0;
}

/* ==========================================
   🌙 KOYU MOD (DARK MODE) - GERÇEK HUD DENEYİMİ
   ========================================== */
@media (prefers-color-scheme: dark) {
  /* Başlıklar */
  h2.section-title { color: var(--hud-text); }
  
  /* Analiz Kartları */
  .project-card {
    background-color: var(--hud-card);
    border-color: #334155;
  }
  .project-card:hover {
    box-shadow: 0 20px 25px -5px rgba(14, 165, 233, 0.1), 0 0 0 1px var(--hud-primary);
  }
  .card-title { color: var(--hud-text); }
  .card-desc { color: var(--hud-muted); }
  .card-footer { border-top-color: rgba(255,255,255,0.1); }
  
  /* Rozetler (Koyu Mod) */
  .tech-tag {
    background-color: #334155;
    border-color: #475569;
    color: var(--hud-muted);
  }
  .tag-ansys, .tag-matlab, .tag-solid, .tag-inventor {
    background-color: rgba(14, 165, 233, 0.1);
    color: var(--hud-primary);
  }

  /* Galeri (Koyu Mod) */
  .gallery-item {
    background-color: var(--hud-card);
    border-color: #334155;
  }
  .gallery-item:hover { border-color: var(--hud-primary); }
  .gallery-info { background-color: var(--hud-card); }
  .gallery-info h3 { color: var(--hud-text); }
  .gallery-info p { color: var(--hud-muted); }
  .gallery-img-box { background-color: #000; }
}
</style>

<h2 class="section-title">Mühendislik Analizleri & Ar-Ge Verileri</h2>

<div class="projects-grid">

  <div class="project-card">
    <span class="card-category">Akademik Araştırma / FEA</span>
    <h3 class="card-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    <div class="card-desc">
      <ul>
        <li>Euler-Timoshenko teorilerinin kıyaslanmalı analizi.</li>
        <li>Fiber dizilim açılarının (stacking sequence) kritik burkulma yüküne etkisi.</li>
        <li>Sonlu Elemanlar Yöntemi (FEM) ile analitik doğrulama.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-ansys">ANSYS ACP</span>
      <span class="tech-tag tag-ansys">Static Structural</span>
      <span class="tech-tag tag-matlab">MATLAB</span>
    </div>
  </div>

  <div class="project-card">
    <span class="card-category">Yazılım Geliştirme / GUI</span>
    <h3 class="card-title">Mohr Çemberi Hesaplama Aracı</h3>
    <div class="card-desc">
      <ul>
        <li>Mukavemet hesapları için interaktif Mohr çemberi çizen arayüz tasarımı.</li>
        <li>Asal gerilmeler (σ1, σ2) ve maksimum kayma gerilmesi (τmax) hesabı.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-matlab">MATLAB App Designer</span>
      <span class="tech-tag">Algoritma</span>
    </div>
  </div>

  <div class="project-card">
    <span class="card-category">TÜBİTAK 2209-A Projesi</span>
    <h3 class="card-title">Özel Asansör Tasarımı (VİSA SÖR)</h3>
    <div class="card-desc">
      <ul>
        <li>Takım liderliği ve proje yaşam döngüsü yönetimi.</li>
        <li>Mekanik sistem boyutlandırması ve güvenlik optimizasyonu.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag tag-ansys">Mekanik Analiz</span>
    </div>
  </div>

  <div class="project-card">
    <span class="card-category">Bitirme Tezi / Hidrodinamik</span>
    <h3 class="card-title">Francis Tipi Türbin Tasarımı</h3>
    <div class="card-desc">
      <ul>
        <li>Keban Barajı verileri referans alınarak hidrodinamik boyutlandırma.</li>
        <li>Çark (runner) ve salyangoz (volute) geometrisinin CFD odaklı tasarımı.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag">CFD Teorisi</span>
    </div>
  </div>

</div>

<h2 class="section-title">3D CAD Tasarım & Render Çıktıları</h2>

<div class="gallery-grid">

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak Tasarımı" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Konsept Uçak Tasarımı</h3>
      <p>Inventor Pro / Yüzey Modelleme & Render</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16 Tüfeği" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>M16 Piyade Tüfeği</h3>
      <p>Inventor Pro / Detaylı Parça & Montaj</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet Motoru" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Turbo-Jet Motor Montajı</h3>
      <p>SolidWorks / Makine Elemanları Modelleme</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="İHA Tasarımı" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Alpagu-X İHA Konsepti</h3>
      <p>Inventor / Havacılık Tasarımı</p>
    </div>
  </div>
  
    <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="CFD Mesh" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Manifold CFD Mesh Ağı</h3>
      <p>ANSYS Meshing / Akışkanlar Dinamiği</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman Logo" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>3D Superman Logosu</h3>
      <p>3DS MAX / Poligon Modelleme</p>
    </div>
  </div>

</div>
