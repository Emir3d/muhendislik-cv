---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. TEMEL AYARLAR & GİZLEMELER */
.author__avatar { display: none !important; }

:root {
  --modern-accent: #2563eb; /* Modern Mavi */
  --modern-bg-light: #f8fafc; /* Çok açık gri arka plan */
  --modern-card-light: rgba(255, 255, 255, 0.8); /* Yarı saydam beyaz kart */
  --modern-text-dark: #1e293b;
  --modern-text-muted: #64748b;
  --glass-shadow: 0 10px 30px -10px rgba(0,0,0,0.1); /* Yumuşak derin gölge */
}

body {
  background-color: var(--modern-bg-light); /* Sayfa arka planını biraz kıralım */
}

/* ==========================================
   MODERN BAŞLIKLAR (Typography)
   ========================================== */
h2.section-title {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  font-size: 1.75rem;
  font-weight: 800;
  letter-spacing: -0.5px; /* Modern sıkı harfler */
  margin: 4rem 0 2rem 0;
  color: var(--modern-text-dark);
  display: flex;
  align-items: center;
  gap: 15px;
}

/* Başlık yanındaki modern çizgi */
h2.section-title::before {
  content: "";
  display: block;
  width: 8px;
  height: 8px;
  background-color: var(--modern-accent);
  border-radius: 50%; /* Daire */
  box-shadow: 0 0 0 4px rgba(37, 99, 235, 0.2); /* Etrafında hafif halka */
}


/* ==========================================
   BÖLÜM 1: MODERN KARTLAR (Glassmorphism)
   ========================================== */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(340px, 1fr));
  gap: 30px;
  margin-bottom: 5rem;
}

.project-card {
  /* CAM EFEKTİ */
  background: var(--modern-card-light);
  backdrop-filter: blur(12px); /* Buzlu cam bulanıklığı */
  -webkit-backdrop-filter: blur(12px);
  border: 1px solid rgba(255, 255, 255, 0.3); /* Çok ince beyaz çerçeve */
  
  border-radius: 16px; /* Daha yuvarlak köşeler */
  padding: 30px;
  display: flex;
  flex-direction: column;
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275); /* Yaylı geçiş efekti */
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05), 0 2px 4px -1px rgba(0, 0, 0, 0.03); /* Çok hafif başlangıç gölgesi */
}

/* Hover Efekti: Kart yukarı süzülür ve gölge derinleşir */
.project-card:hover {
  transform: translateY(-8px) scale(1.01);
  box-shadow: var(--glass-shadow);
  border-color: rgba(37, 99, 235, 0.3); /* Kenarlık hafif mavi olur */
}

/* Kategori */
.card-category {
  font-size: 0.75rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 1.2px;
  color: var(--modern-accent);
  margin-bottom: 10px;
  display: block;
}

/* Başlık */
.card-title {
  font-size: 1.35rem;
  font-weight: 800;
  margin-bottom: 15px;
  color: var(--modern-text-dark);
  line-height: 1.3;
}

/* Açıklama */
.card-desc {
  font-size: 1rem;
  line-height: 1.7;
  color: var(--modern-text-muted);
  flex-grow: 1;
}
.card-desc ul { padding-left: 20px; margin-bottom: 20px; }
.card-desc li { margin-bottom: 10px; }


/* ==========================================
   MODERN HAP ROZETLER (Pill Badges)
   ========================================== */
.card-footer {
  margin-top: auto; /* En alta it */
  padding-top: 20px;
  display: flex;
  flex-wrap: wrap;
  gap: 10px;
}

.tech-tag {
  font-size: 0.7rem;
  font-weight: 600;
  padding: 6px 14px; /* Daha geniş iç boşluk */
  background-color: rgba(100, 116, 139, 0.1); /* Çok hafif gri */
  color: var(--modern-text-dark);
  border-radius: 50px; /* TAM YUVARLAK (Hap şeklinde) */
  transition: all 0.3s ease;
}

/* Önemli yazılımlar için özel renkler (Pastel Tonlar) */
.tag-ansys { background-color: rgba(245, 158, 11, 0.15); color: #b45309; } /* Turuncu */
.tag-matlab { background-color: rgba(59, 130, 246, 0.15); color: #1d4ed8; } /* Mavi */
.tag-solid { background-color: rgba(239, 68, 68, 0.15); color: #b91c1c; } /* Kırmızı */
.tag-inventor { background-color: rgba(16, 185, 129, 0.15); color: #047857; } /* Yeşil */

.tech-tag:hover {
  transform: translateY(-2px); /* Rozetler de hafifçe kalkar */
}


/* ==========================================
   BÖLÜM 2: MODERN GALERİ
   ========================================== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  margin-bottom: 4rem;
}

.gallery-item {
  border-radius: 16px;
  overflow: hidden;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);
  transition: all 0.4s ease;
  background: #fff;
}

.gallery-item:hover {
  transform: translateY(-8px);
  box-shadow: var(--glass-shadow);
}

.gallery-img-box {
  height: 240px; /* Biraz daha yüksek */
  overflow: hidden;
  position: relative;
}

.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.5s cubic-bezier(0.4, 0, 0.2, 1);
}

/* Resim Hover: Hafif zoom ve parlaklık */
.gallery-item:hover .gallery-img-box img {
  transform: scale(1.08);
  filter: brightness(1.05);
}

/* Galeri Metin Alanı */
.gallery-info {
  padding: 25px;
  background: #fff;
}

.gallery-info h3 {
  font-size: 1.2rem;
  font-weight: 800;
  margin: 0 0 8px 0;
  color: var(--modern-text-dark);
}

.gallery-info p {
  font-size: 0.9rem;
  color: var(--modern-text-muted);
  font-weight: 500;
  margin: 0;
}

/* ==========================================
   🌙 KOYU MOD (DARK MODE) - NEON GLASS
   ========================================== */
@media (prefers-color-scheme: dark) {
  :root {
    --modern-bg-light: #0f172a; /* Koyu arka plan */
    --modern-card-light: rgba(30, 41, 59, 0.7); /* Koyu yarı saydam kart */
    --modern-text-dark: #f8fafc;
    --modern-text-muted: #94a3b8;
    --glass-shadow: 0 10px 30px -10px rgba(0,0,0,0.5); /* Daha koyu gölge */
  }
  
  body { background-color: var(--modern-bg-light); }
  
  .project-card, .gallery-item {
    border-color: rgba(255, 255, 255, 0.08); /* Çok ince açık çerçeve */
  }
  
  .gallery-item, .gallery-info { background: var(--modern-card-light); }

  /* Koyu modda rozetler daha parlak olsun */
  .tech-tag { background-color: rgba(255,255,255,0.1); color: #e2e8f0; }
  .tag-ansys { background-color: rgba(245, 158, 11, 0.2); color: #fbbf24; }
  .tag-matlab { background-color: rgba(59, 130, 246, 0.2); color: #60a5fa; }
  .tag-solid { background-color: rgba(239, 68, 68, 0.2); color: #f87171; }
}
</style>

<h2 class="section-title">Mühendislik Analizleri & Ar-Ge</h2>

<div class="projects-grid">

  <div class="project-card">
    <span class="card-category">Akademik Araştırma</span>
    <h3 class="card-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    <div class="card-desc">
      <ul>
        <li>Euler-Timoshenko teorilerinin kıyaslanması.</li>
        <li>Farklı fiber dizilim açılarının kritik burkulma yüküne etkisi.</li>
        <li>FEM analizi ve analitik doğrulama.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-ansys">ANSYS ACP</span>
      <span class="tech-tag tag-ansys">Static Structural</span>
      <span class="tech-tag tag-matlab">MATLAB</span>
    </div>
  </div>

  <div class="project-card">
    <span class="card-category">Yazılım Geliştirme</span>
    <h3 class="card-title">Mohr Çemberi Analiz Aracı</h3>
    <div class="card-desc">
      <ul>
        <li>Mukavemet hesapları için otomatik Mohr çemberi çizen GUI tasarımı.</li>
        <li>Asal gerilmeler ve maksimum kayma gerilmesi hesabı.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-matlab">MATLAB App Designer</span>
      <span class="tech-tag">GUI / Algoritma</span>
    </div>
  </div>

  <div class="project-card">
    <span class="card-category">TÜBİTAK 2209-A</span>
    <h3 class="card-title">Özel Asansör Tasarımı (VİSA SÖR)</h3>
    <div class="card-desc">
      <ul>
        <li>Takım liderliği ve proje yönetimi.</li>
        <li>Mekanik boyutlandırma ve güvenlik sistemi optimizasyonu.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag tag-ansys">Mekanik Analiz</span>
    </div>
  </div>

  <div class="project-card">
    <span class="card-category">Bitirme Tezi</span>
    <h3 class="card-title">Francis Tipi Türbin Tasarımı</h3>
    <div class="card-desc">
      <ul>
        <li>Keban Barajı verileriyle hidrodinamik boyutlandırma.</li>
        <li>Çark ve salyangoz geometrisinin belirlenmesi.</li>
      </ul>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag">Hidrodinamik / CFD</span>
    </div>
  </div>

</div>

<h2 class="section-title">3D Tasarım & Render Galerisi</h2>

<div class="gallery-grid">

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Konsept Uçak Tasarımı</h3>
      <p>Inventor Pro / Render</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>M16 Piyade Tüfeği</h3>
      <p>Inventor Pro / Montaj</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Turbo-Jet Motoru</h3>
      <p>SolidWorks / Makine Elemanları</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Alpagu-X İHA</h3>
      <p>Inventor / Havacılık</p>
    </div>
  </div>
  
    <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>Manifold Mesh Ağı</h3>
      <p>ANSYS / CFD</p>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="gallery-info">
      <h3>3D Superman Logosu</h3>
      <p>3DS MAX / Poligon Modelleme</p>
    </div>
  </div>

</div>
