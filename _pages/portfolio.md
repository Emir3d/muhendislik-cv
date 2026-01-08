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
   GENEL KART AYARLARI
   ========================================== */
.projects-grid, .gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
  margin-top: 2rem;
  margin-bottom: 4rem;
}

.project-card, .gallery-item {
  background-color: #ffffff;
  border: 1px solid rgba(128, 128, 128, 0.2);
  border-radius: 8px;
  overflow: hidden;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
  display: flex;
  flex-direction: column; /* İçeriği dikey diz */
}

.project-card:hover, .gallery-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0,0,0,0.08);
}

/* KART İÇERİĞİ */
.card-body {
  padding: 25px;
  flex-grow: 1; /* Alanı doldur */
}

.card-category {
  font-size: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 1px;
  color: #666;
  margin-bottom: 10px;
  display: block;
  font-weight: 700;
}

.card-title {
  font-size: 1.15rem;
  font-weight: 700;
  margin-bottom: 10px;
  color: #111;
  line-height: 1.4;
}

.card-desc {
  font-size: 0.9rem;
  color: #555;
  line-height: 1.6;
}
.card-desc ul { padding-left: 15px; margin-bottom: 0; }
.card-desc li { margin-bottom: 5px; }

/* ==========================================
   🚀 YENİ ÖZELLİK: YAZILIM ROZETLERİ (BADGES)
   ========================================== */
.card-footer {
  padding: 15px 25px;
  background-color: #f9fafb;
  border-top: 1px solid rgba(128,128,128,0.1);
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.tech-tag {
  font-size: 0.75rem;
  font-weight: 600;
  padding: 3px 10px;
  border-radius: 12px;
  color: #333;
  background-color: #e5e7eb; /* Varsayılan Gri */
}

/* Özel Renkler */
.tag-ansys { background-color: #fef08a; color: #854d0e; } /* Sarı */
.tag-matlab { background-color: #dbeafe; color: #1e40af; } /* Mavi */
.tag-solid { background-color: #fee2e2; color: #991b1b; } /* Kırmızı */
.tag-inventor { background-color: #d1fae5; color: #065f46; } /* Yeşil */
.tag-3ds { background-color: #f3e8ff; color: #6b21a8; } /* Mor */

/* ==========================================
   GÖRSEL GALERİ AYARLARI
   ========================================== */
h2.section-title {
  border-bottom: 1px solid rgba(128,128,128,0.2);
  padding-bottom: 10px;
  margin: 3rem 0 1.5rem 0;
  font-weight: 700;
}

.gallery-img-box {
  width: 100%;
  height: 200px;
  background-color: #f3f4f6;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  border-bottom: 1px solid rgba(128,128,128,0.1);
}
.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.5s ease;
}
.gallery-item:hover .gallery-img-box img {
  transform: scale(1.1);
}

/* KOYU MOD */
@media (prefers-color-scheme: dark) {
  .project-card, .gallery-item { background-color: #1f2937; border-color: #374151; }
  .card-title { color: #f3f4f6; }
  .card-desc { color: #d1d5db; }
  .card-category { color: #9ca3af; }
  .card-footer { background-color: #111827; border-color: #374151; }
  .tech-tag { background-color: #374151; color: #e5e7eb; }
  /* Koyu modda rozetler biraz daha pastel olsun */
  .tag-ansys { background-color: #422006; color: #fde047; }
  .tag-matlab { background-color: #172554; color: #93c5fd; }
  .tag-solid { background-color: #450a0a; color: #fca5a5; }
  .tag-inventor { background-color: #064e3b; color: #6ee7b7; }
  .tag-3ds { background-color: #3b0764; color: #d8b4fe; }
}
</style>

<h2 class="section-title">🔬 Mühendislik Analizleri & Ar-Ge</h2>

<div class="projects-grid">

  <div class="project-card">
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
      <span class="tech-tag tag-ansys">ANSYS ACP</span>
      <span class="tech-tag tag-ansys">Static Structural</span>
      <span class="tech-tag tag-matlab">MATLAB</span>
    </div>
  </div>

  <div class="project-card">
    <div class="card-body">
      <span class="card-category">Yazılım Geliştirme</span>
      <h3 class="card-title">Mohr Çemberi Analiz Aracı</h3>
      <div class="card-desc">
        <ul>
          <li>Mukavemet hesapları için otomatik Mohr çemberi çizen GUI tasarımı.</li>
          <li>Asal gerilmeler ve maksimum kayma gerilmesi hesabı.</li>
        </ul>
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-matlab">MATLAB App Designer</span>
      <span class="tech-tag tag-matlab">GUI</span>
    </div>
  </div>

  <div class="project-card">
    <div class="card-body">
      <span class="card-category">TÜBİTAK 2209-A</span>
      <h3 class="card-title">Özel Asansör Tasarımı (VİSA SÖR)</h3>
      <div class="card-desc">
        <ul>
          <li>Takım liderliği ve proje yönetimi.</li>
          <li>Mekanik boyutlandırma ve güvenlik sistemi optimizasyonu.</li>
        </ul>
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag tag-ansys">Mekanik Analiz</span>
    </div>
  </div>

  <div class="project-card">
    <div class="card-body">
      <span class="card-category">Bitirme Tezi</span>
      <h3 class="card-title">Francis Tipi Türbin Tasarımı</h3>
      <div class="card-desc">
        <ul>
          <li>Keban Barajı verileriyle hidrodinamik boyutlandırma.</li>
          <li>Çark ve salyangoz geometrisinin belirlenmesi.</li>
        </ul>
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag">Hidrodinamik</span>
      <span class="tech-tag">CFD</span>
    </div>
  </div>

  <div class="project-card">
    <div class="card-body">
      <span class="card-category">Teknik Çeviri</span>
      <h3 class="card-title">CFD & Kavitasyon Teknik Çeviri</h3>
      <div class="card-desc">
         Vanalarda iki fazlı akış ve kavitasyon üzerine teknik literatür çevirisi.
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag">Akademik İngilizce</span>
      <span class="tech-tag">CFD Teorisi</span>
    </div>
  </div>
  
   <div class="project-card">
    <div class="card-body">
      <span class="card-category">Gönüllü Proje</span>
      <h3 class="card-title">Müsilaj Sorunu Araştırması</h3>
      <div class="card-desc">
        Müsilaj oluşum mekanizmaları ve akışkanlar mekaniği temelli çözüm önerileri üzerine disiplinlerarası çalışma.
      </div>
    </div>
    <div class="card-footer">
      <span class="tech-tag">Akışkanlar Mekaniği</span>
      <span class="tech-tag">Çevre Müh.</span>
    </div>
  </div>

</div>

<h2 class="section-title">🎨 3D Tasarım & Render Galerisi</h2>

<div class="gallery-grid">

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">Konsept Uçak Tasarımı</h3>
      <div class="card-desc">Özgün konsept tasarım ve gerçekçi render çalışması.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-inventor">Inventor Pro</span>
      <span class="tech-tag">Render</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">M16 Piyade Tüfeği</h3>
      <div class="card-desc">Detaylı parça ve montaj modellemesi.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-inventor">Inventor Pro</span>
      <span class="tech-tag">Montaj</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">3D Superman Logosu</h3>
      <div class="card-desc">Poligon modelleme teknikleri ile ikonik logo çalışması.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-3ds">3DS MAX</span>
      <span class="tech-tag">Poligon Modelleme</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">Turbo-Jet Motoru</h3>
      <div class="card-desc">Motor bileşenlerinin detaylı CAD modellemesi.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-solid">SolidWorks</span>
      <span class="tech-tag">Makine Elemanları</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">Alpagu-X İHA</h3>
      <div class="card-desc">İnsansız hava aracı konsept tasarımı.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-inventor">Inventor</span>
      <span class="tech-tag">Havacılık</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Top" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">Şahi Top Modeli</h3>
      <div class="card-desc">Tarihi savunma sisteminin 3D rekonstrüksiyonu.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-inventor">Inventor</span>
      <span class="tech-tag">Tarihi Modelleme</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/kilic.png" alt="Kılıç" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">Witcher-3 Kılıcı</h3>
      <div class="card-desc">Oyun referanslı detaylı yüzey modelleme.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-inventor">Inventor</span>
      <span class="tech-tag">Yüzey Modelleme</span>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
    <div class="card-body">
      <h3 class="card-title">Manifold Mesh Ağı</h3>
      <div class="card-desc">Karmaşık geometriler için CFD'ye uygun ağ yapısı.</div>
    </div>
    <div class="card-footer">
      <span class="tech-tag tag-ansys">Solidworks</span>
      <span class="tech-tag">Photoshop</span>
    </div>
  </div>

</div>
