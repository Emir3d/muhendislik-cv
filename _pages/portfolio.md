---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* ==========================================
   BÖLÜM 1: ANALİZ KARTLARI (Teknik Detay)
   ========================================== */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
  margin-top: 2rem;
  margin-bottom: 4rem;
}

.project-card {
  background-color: #ffffff;
  border: 1px solid rgba(128, 128, 128, 0.2);
  border-radius: 8px;
  padding: 25px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
  overflow: hidden;
  border-left: 5px solid #2563eb; /* Varsayılan Mavi */
}

.project-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 20px rgba(0,0,0,0.08);
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
  font-size: 1.2rem;
  font-weight: 700;
  margin-bottom: 10px;
  color: #111;
}

.card-desc {
  font-size: 0.95rem;
  color: #444;
  line-height: 1.6;
}
.card-desc li { margin-bottom: 5px; }

/* Renk Kodları */
.type-research { border-left-color: #2563eb; } /* Mavi: Ar-Ge */
.type-design { border-left-color: #d97706; }   /* Turuncu: Tasarım */
.type-cfd { border-left-color: #059669; }      /* Yeşil: Akışkanlar/Yazılım */

/* ==========================================
   BÖLÜM 2: GÖRSEL GALERİ (Renderlar)
   ========================================== */
h2.gallery-title {
  border-bottom: 1px solid rgba(128,128,128,0.2);
  padding-bottom: 10px;
  margin-bottom: 25px;
}

.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 20px;
}

.gallery-item {
  background: #fff;
  border: 1px solid rgba(128,128,128,0.2);
  border-radius: 8px;
  overflow: hidden;
  transition: transform 0.2s ease;
}
.gallery-item:hover { transform: scale(1.02); }

/* Resim Alanı */
.gallery-img-box {
  width: 100%;
  height: 200px; /* Sabit yükseklik, düzgün dursun */
  background-color: #f3f4f6;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
}
.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover; /* Resmi kutuya sığdır */
}

.gallery-content { padding: 15px; }
.g-title { font-size: 1.1rem; font-weight: bold; margin-bottom: 5px; color: #111; }
.g-desc { font-size: 0.9rem; color: #555; }

/* KOYU MOD */
@media (prefers-color-scheme: dark) {
  .project-card, .gallery-item { background-color: #1f2937; border-color: #374151; }
  .card-title, .g-title { color: #f3f4f6; }
  .card-desc, .g-desc { color: #d1d5db; }
  .card-category { color: #9ca3af; }
}
</style>

## 🔬 Mühendislik Analizleri ve Ar-Ge Projeleri

<div class="projects-grid">

  <div class="project-card type-research">
    <span class="card-category">Devam Eden Araştırma / ANSYS ACP</span>
    <h3 class="card-title">Tabakalı ve Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    <div class="card-desc">
      <ul>
        [cite_start]<li>Euler-Timoshenko teorilerinin karşılaştırılması[cite: 5].</li>
        <li>Analitik modelleme, sonlu elemanlar analizi (FEM) ve sayısal çözümler.</li>
        [cite_start]<li><strong>Ansys ACP</strong> modülü ile detaylı katman analizi[cite: 5].</li>
      </ul>
    </div>
  </div>

  <div class="project-card type-cfd">
    <span class="card-category">Yazılım Geliştirme / MATLAB</span>
    <h3 class="card-title">MATLAB ile Mohr Çemberi Analiz Aracı</h3>
    <div class="card-desc">
      <ul>
        [cite_start]<li>Mukavemet hesaplamaları için Mohr çemberini otomatik çizen grafiksel arayüz (GUI)[cite: 57, 63].</li>
        [cite_start]<li>Asal gerilmelerin (Sigma max/min) ve maksimum kayma gerilmelerinin hesaplanması[cite: 100, 101].</li>
        [cite_start]<li>Kullanıcı dostu arayüz ile veri girişi ve görselleştirme[cite: 92].</li>
      </ul>
    </div>
  </div>

  <div class="project-card type-design">
    <span class="card-category">TÜBİTAK 2209-A / Tasarım</span>
    <h3 class="card-title">Asansör Tasarımı (VİSA SÖR)</h3>
    <div class="card-desc">
      <ul>
        [cite_start]<li>Dubleks ve tripleks yapılar için özel asansör sistem tasarımı[cite: 5].</li>
        [cite_start]<li><strong>Takım Lideri</strong> olarak proje yönetimi[cite: 5].</li>
        [cite_start]<li>Mekanik boyutlandırma, güvenlik hesapları ve sistem optimizasyonu[cite: 5].</li>
      </ul>
    </div>
  </div>

  <div class="project-card type-design">
    <span class="card-category">Bitirme Tezi / Hidrodinamik</span>
    <h3 class="card-title">Francis Tipi Türbin Tasarımı</h3>
    <div class="card-desc">
      <ul>
        [cite_start]<li>Keban Barajı verilerine uygun Francis tipi hidroelektrik türbin tasarımı[cite: 5].</li>
        [cite_start]<li>Türbin geometrisinin belirlenmesi ve hidrodinamik boyutlandırma hesapları[cite: 5].</li>
        [cite_start]<li>Enerji dönüşüm prensipleri ve verimlilik analizi[cite: 5].</li>
      </ul>
    </div>
  </div>

  <div class="project-card type-cfd">
    <span class="card-category">Teknik Literatür / CFD</span>
    <h3 class="card-title">CFD Teknik Kitap Çevirisi Projesi</h3>
    <div class="card-desc">
      <ul>
        [cite_start]<li>Danışman: Dr. Nuray Kayakol (CFDEXPLAINED)[cite: 5].</li>
        [cite_start]<li>Vanalarda iki fazlı akış ve kavitasyon üzerine teknik doküman çevirisi[cite: 5].</li>
        [cite_start]<li>Teknik terminoloji ve akademik yazım diline hakimiyet[cite: 5].</li>
      </ul>
    </div>
  </div>

  <div class="project-card type-cfd">
    <span class="card-category">Sosyal Sorumluluk / Çevre</span>
    <h3 class="card-title">Gönüllü Müsilaj Projesi</h3>
    <div class="card-desc">
      <ul>
        [cite_start]<li>Müsilaj oluşumunun nedenleri ve çözüm yöntemleri üzerine araştırma[cite: 5].</li>
        [cite_start]<li>Akışkanlar mekaniği temelli yaklaşımlarla problem analizi[cite: 5].</li>
        [cite_start]<li>Çevresel mühendislik problemlerine disiplinlerarası bakış[cite: 5].</li>
      </ul>
    </div>
  </div>

</div>


<h2 class="gallery-title">🎨 3D Tasarım & Render Galerisi</h2>

<div class="gallery-grid">

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Konsept Uçak" onerror="this.src='https://via.placeholder.com/400x300?text=Ucak+Resmi';">
    </div>
    <div class="gallery-content">
      <div class="g-title">Konsept Uçak Tasarımı</div>
      [cite_start]<div class="g-desc">Autodesk Inventor ile modellenen özgün uçak konsepti ve render çalışması[cite: 55].</div>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Turbo Jet" onerror="this.src='https://via.placeholder.com/400x300?text=Resim+Yukle';">
    </div>
    <div class="gallery-content">
      <div class="g-title">Turbo-Jet Motoru</div>
      [cite_start]<div class="g-desc">SolidWorks ile detaylı modelleme ve yüksek çözünürlüklü render çalışması[cite: 104].</div>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu İHA" onerror="this.src='https://via.placeholder.com/400x300?text=Resim+Yukle';">
    </div>
    <div class="gallery-content">
      <div class="g-title">Alpagu-X İHA Tasarımı</div>
      [cite_start]<div class="g-desc">Autodesk Inventor kullanılarak özgün konsept tasarım ve görselleştirme[cite: 51].</div>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Şahi Top" onerror="this.src='https://via.placeholder.com/400x300?text=Resim+Yukle';">
    </div>
    <div class="gallery-content">
      <div class="g-title">Şahi Top Modellemesi</div>
      [cite_start]<div class="g-desc">Tarihi savunma sisteminin Inventor ortamında 3D modellenmesi[cite: 48].</div>
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/kilic.png" alt="Witcher Sword" onerror="this.src='https://via.placeholder.com/400x300?text=Resim+Yukle';">
    </div>
    <div class="gallery-content">
      <div class="g-title">Witcher-3 Kılıç Replikası</div>
      [cite_start]<div class="g-desc">Oyun içi modelin referans alınarak CAD ortamına aktarılması ve renderı[cite: 108].</div>
    </div>
  </div>

   <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold Mesh" onerror="this.src='https://via.placeholder.com/400x300?text=Resim+Yukle';">
    </div>
    <div class="gallery-content">
      <div class="g-title">Manifold Mesh Çalışması</div>
      [cite_start]<div class="g-desc">ANSYS ortamında karmaşık geometri için ağ (mesh) yapısının oluşturulması[cite: 115].</div>
    </div>
  </div>

</div>
