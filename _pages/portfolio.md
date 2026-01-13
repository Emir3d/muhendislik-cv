---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. Kırık Profil Resmini Gizle */
.author__avatar { display: none !important; }

/* 2. Temel Renkler */
:root {
  --tech-blue: #2563eb;
  --tech-bg: #ffffff;
  --tech-border: #e2e8f0;
}

/* 3. Başlıklar */
.section-title {
  font-size: 1.8rem;
  font-weight: 800;
  margin: 3rem 0 2rem;
  display: flex;
  align-items: center;
  gap: 15px;
  color: inherit;
  border-bottom: 2px solid #e5e7eb;
  padding-bottom: 10px;
}

/* ===============================
   PROJE KARTLARI (LİNK YAPISI)
   =============================== */
.projects-container {
  display: flex;
  flex-direction: column;
  gap: 20px;
  margin-bottom: 5rem;
}

.project-card-link {
  text-decoration: none !important;
  color: inherit !important;
  display: block;
}

.project-row {
  background: #ffffff;
  border: 1px solid var(--tech-border);
  border-radius: 12px;
  padding: 25px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
}

@media (prefers-color-scheme: dark) {
  .project-row { background: #1e293b; border-color: #334155; }
  .row-title { color: #f1f5f9 !important; }
}

.project-row:hover {
  transform: translateX(10px);
  border-color: var(--tech-blue);
  box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
}

.row-info { display: flex; flex-direction: column; gap: 5px; }

.row-category {
  font-size: 0.75rem;
  color: var(--tech-blue);
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.row-title {
  font-size: 1.2rem;
  font-weight: 800;
  color: #1e293b;
  margin: 0;
}

.row-arrow {
  font-size: 1.5rem;
  color: #cbd5e1;
  transition: 0.2s;
}

.project-row:hover .row-arrow {
  color: var(--tech-blue);
  transform: translateX(5px);
}

/* ===============================
   MODAL PENCERE TASARIMI
   =============================== */
.modal-overlay {
  display: none; 
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  background: rgba(0, 0, 0, 0.85);
  z-index: 99999;
  justify-content: center;
  align-items: center;
  padding: 20px;
  backdrop-filter: blur(5px);
}

.modal-overlay:target {
  display: flex;
}

.modal-content {
  background: #fff;
  width: 100%;
  max-width: 800px; /* Kutu genişliğini biraz artırdık */
  max-height: 90vh;
  overflow-y: auto;
  padding: 40px;
  border-radius: 15px;
  position: relative;
  box-shadow: 0 0 50px rgba(0,0,0,0.5);
  animation: slideDown 0.3s ease;
}

@media (prefers-color-scheme: dark) {
  .modal-content { background: #1e293b; color: #fff; }
  .modal-desc { color: #cbd5e1 !important; }
  .modal-title { color: #60a5fa !important; }
}

@keyframes slideDown {
  from { transform: translateY(-50px); opacity: 0; }
  to { transform: translateY(0); opacity: 1; }
}

.close-link {
  position: absolute;
  top: 15px; right: 20px;
  font-size: 2rem;
  color: #94a3b8;
  text-decoration: none !important;
  line-height: 1;
  z-index: 10;
}
.close-link:hover { color: #ef4444; }

.modal-backdrop-close {
  position: absolute;
  top: 0; left: 0; width: 100%; height: 100%;
  cursor: default;
}

/* ✅ MODAL İÇİ GÖRSEL AYARLARI (DÜZELTİLDİ) ✅ */
.modal-banner {
  width: 100%;
  height: auto;         /* Sabit yükseklik yerine otomatik */
  max-height: 600px;    /* Çok uzarsa diye güvenlik sınırı */
  object-fit: contain;  /* Resmi kesme, tamamını göster */
  border-radius: 8px;
  margin-bottom: 25px;
  box-shadow: 0 4px 15px rgba(0,0,0,0.1);
  display: block;
  background-color: #f8fafc; /* Resim yüklenirken veya şeffafsa arka plan */
}

.modal-title {
  margin-top: 0;
  color: var(--tech-blue);
  font-size: 1.5rem;
  border-bottom: 1px solid #e2e8f0;
  padding-bottom: 15px;
  margin-bottom: 15px;
}

.modal-desc {
  line-height: 1.7;
  font-size: 1.05rem;
  color: #334155;
}

.modal-tags {
  margin-top: 25px;
  display: flex;
  gap: 10px;
  flex-wrap: wrap;
}

.tag-badge {
  background: #eff6ff;
  color: var(--tech-blue);
  padding: 5px 12px;
  border-radius: 50px;
  font-size: 0.8rem;
  border: 1px solid #bfdbfe;
  font-weight: 600;
}
@media (prefers-color-scheme: dark) {
  .tag-badge { background: #172554; color: #93c5fd; border-color: #1e40af; }
}

/* ===============================
   GALERİ
   =============================== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}

.gallery-card {
  background: #fff;
  border: 1px solid var(--tech-border);
  border-radius: 12px;
  overflow: hidden;
  transition: 0.3s;
}

@media (prefers-color-scheme: dark) {
  .gallery-card { background: #1e293b; border-color: #334155; }
}

.gallery-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
}

.img-box {
  height: 220px;
  width: 100%;
  overflow: hidden;
}

.img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: 0.5s;
}

.gallery-card:hover img { transform: scale(1.05); }

.full-width { grid-column: 1 / -1; }
.full-width .img-box { height: 400px; }
</style>


<h2 class="section-title">Mühendislik Analizleri</h2>

<div class="projects-container">

  <a href="#proje-1" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">Akademik Araştırma</span>
        <h3 class="row-title">Tabakalı ve hibrit kompozit kirişler için burkulma analizi</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-2" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">Yazılım Geliştirme</span>
        <h3 class="row-title">Mohr Çemberi Hesaplama Aracı</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-3" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">TÜBİTAK 2209-A</span>
        <h3 class="row-title">Asansör Tasarımı (VİSA SÖR)</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-4" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">Bitirme Tezi</span>
        <h3 class="row-title">Francis Tipi Türbinlerin Tasarımı</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-5" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">Gönüllü Çalışma</span>
        <h3 class="row-title">CFD Teknik Kitap Çevirisi Projesi</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-6" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">Gönüllü Araştırma</span>
        <h3 class="row-title">Gönüllü Müsilaj Projesi</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-7" class="project-card-link">
    <div class="project-row">
      <div class="row-info">
        <span class="row-category">Sertifika / Eğitim</span>
        <h3 class="row-title">Akbank Python ve Yapay Zeka Bootcamp</h3>
      </div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

</div>


<h2 class="section-title">3D Tasarım & Render</h2>

<div class="gallery-grid">

  <div class="gallery-card">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-card">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-card">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-card">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>
  
  <div class="gallery-card">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-card">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-card full-width">
    <div class="img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Top" onerror="this.src='https://via.placeholder.com/800x400';">
    </div>
  </div>

</div>


<div id="proje-1" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    
    <img src="https://emir3d.github.io/muhendislik-cv/images/matlab.jpg" class="modal-banner" onerror="this.style.display='none'"> 
    
    <h3 class="modal-title">Tabakalı ve hibrit kompozit kirişler için burkulma analizi</h3>
    <div class="modal-desc">
      <p>Devam Eden Araştırma Çalışması</p>
      <ul>
        <li>Euler-Timoshenko teorilerinin karşılaştırılması.</li>
        <li>Analitik modelleme, sonlu elemanlar analizi ve MATLAB tabanlı sayısal çözümler.</li>
        <li>Ansys ACP modülü.</li>
        <li>Kullanıcı dostu grafiksel Matlab arayüz.</li>
        <li>Makale yazım süreci devam etmektedir.</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">ANSYS ACP</span>
      <span class="tag-badge">MATLAB</span>
      <span class="tag-badge">FEM</span>
    </div>
  </div>
</div>

<div id="proje-2" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Mohr Çemberi Hesaplama Aracı</h3>
    <div class="modal-desc">
      <p>Mukavemet hesaplamaları için geliştirilen bu araç, kullanıcıdan alınan gerilme verileriyle otomatik Mohr çemberi çizer.</p>
      <ul>
        <li>Asal gerilmelerin (σ1, σ2) hesaplanması.</li>
        <li>Maksimum kayma gerilmesinin (τmax) tespiti.</li>
        <li>Matlab tasarımı ve grafiksel gösterim (GUI).</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">MATLAB GUI</span>
      <span class="tag-badge">Mukavemet</span>
    </div>
  </div>
</div>

<div id="proje-3" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Asansör Tasarımı (VİSA SÖR)</h3>
    <div class="modal-desc">
      <p>TÜBİTAK 2209-A – Üniversite Öğrencileri Araştırma Projeleri Desteği</p>
      <ul>
        <li>Dubleks ve tripleks yapılar için asansör sistem tasarımı.</li>
        <li>Projede takım lideri olarak görev alındı.</li>
        <li>Mekanik tasarım, boyutlandırma ve analiz çalışmalarının yürütülmesi.</li>
        <li>Tasarım sürecinde mühendislik hesapları ve sistem optimizasyonu.</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">SolidWorks</span>
      <span class="tag-badge">Mekanik Tasarım</span>
    </div>
  </div>
</div>

<div id="proje-4" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Francis Tipi Türbinlerin Tasarımı</h3>
    <div class="modal-desc">
      <p>Bitirme Tezi</p>
      <ul>
        <li>Keban Barajı için Francis tipi hidroelektrik türbin tasarımı.</li>
        <li>Türbin geometrisinin belirlenmesi ve boyutlandırma hesapları.</li>
        <li>Enerji dönüşüm prensipleri ve hidrodinamik tasarım kriterlerinin uygulanması.</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">SolidWorks</span>
      <span class="tag-badge">CFD</span>
      <span class="tag-badge">Hidrodinamik</span>
    </div>
  </div>
</div>

<div id="proje-5" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">CFD Teknik Kitap Çevirisi Projesi</h3>
    <div class="modal-desc">
  
      <ul>
        <li>CFD teori denklemleri ve modelleme yöntemleri üzerine teknik doküman çevirisi.</li>
        <li>Vanalarda iki fazlı akış ve kavitasyon konularını içeren akademik içeriklerin Türkçeye kazandırılması.</li>
        <li>4 ay süren proje kapsamında çeviri grubunun aktif üyesi.</li>
        <li>Teknik terminolojiye ve akademik yazım diline hâkimiyet kazanımı.</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">CFD</span>
      <span class="tag-badge">Teknik Çeviri</span>
      <span class="tag-badge">Akademik</span>
    </div>
  </div>
</div>

<div id="proje-6" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Gönüllü Müsilaj Projesi</h3>
    <div class="modal-desc">
      
      <ul>
        <li>Müsilaj oluşumunun nedenleri ve çözüm yöntemleri üzerine araştırma.</li>
        <li>Akışkanlar mekaniği ve CFD temelli yaklaşımlarla problem analizi.</li>
        <li>Çevresel mühendislik problemlerine disiplinlerarası bakış açısı kazanımı.</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">CFD</span>
      <span class="tag-badge">Araştırma</span>
      <span class="tag-badge">Akışkanlar Mekaniği</span>
    </div>
  </div>
</div>

<div id="proje-7" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Akbank Python ve Yapay Zeka Bootcamp</h3>
    <div class="modal-desc">
      <p>Global AI Hub Sponsorluğu</p>
      <ul>
        <li>Python programlama ve yapay zekâ temelleri eğitimi.</li>
        <li>Sürücüsüz Metro Simülasyonu (Rota Optimizasyonu) projesinin gerçekleştirilmesi.</li>
        <li>Algoritmik düşünme ve optimizasyon problemleri üzerine uygulamalar.</li>
      </ul>
    </div>
    <div class="modal-tags">
      <span class="tag-badge">Python</span>
      <span class="tag-badge">Yapay Zeka</span>
      <span class="tag-badge">Algoritma</span>
    </div>
  </div>
</div>
