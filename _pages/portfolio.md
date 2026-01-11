---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. PROFİL RESMİ GİZLEME (Kırık ikon sorunu için) */
.author__avatar { display: none !important; }

/* ===============================
   GLOBAL AYARLAR (Tema Rengine Dokunmuyoruz)
   =============================== */
/* Body rengine MÜDAHALE ETMİYORUZ. Tema neyse o kalsın. */

.page__content { width: 100% !important; padding-right: 0 !important; }

/* Renk Değişkenleri */
:root {
  --border-color: #e2e8f0;
  --accent-color: #2563eb; /* Standart Mavi */
  --card-hover-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1);
}

/* ===============================
   BAŞLIKLAR
   =============================== */
.section-title {
  font-size: 1.8rem;
  font-weight: 800;
  margin: 3rem 0 2rem;
  display: flex;
  align-items: center;
  gap: 15px;
}
.section-title::after {
  content: "";
  flex-grow: 1;
  height: 2px;
  background: #e5e7eb; /* İnce gri çizgi */
}

/* ===============================
   YAZILI PROJELER (LİSTE GÖRÜNÜMÜ)
   =============================== */
.projects-stack {
  display: flex;
  flex-direction: column;
  gap: 15px;
  margin-bottom: 5rem;
}

.project-row {
  background: #ffffff; /* Kart içi beyaz olsun */
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 20px 25px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
  transition: all 0.2s ease;
  box-shadow: 0 2px 5px rgba(0,0,0,0.02);
}

/* Hover Efekti */
.project-row:hover {
  transform: translateX(10px);
  border-color: var(--accent-color);
  box-shadow: var(--card-hover-shadow);
}

.row-info h3 {
  margin: 0 0 5px 0;
  font-size: 1.1rem;
  font-weight: 700;
  color: #1e293b;
}
.row-info span {
  font-size: 0.8rem;
  color: var(--accent-color);
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1px;
}

.row-arrow {
  font-size: 1.2rem;
  color: #94a3b8;
  transition: 0.2s;
}
.project-row:hover .row-arrow {
  color: var(--accent-color);
  transform: translateX(5px);
}

.hidden-details { display: none; }

/* ===============================
   GÖRSEL GALERİ (GRID)
   =============================== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}

.gallery-item {
  background: #fff;
  border: 1px solid var(--border-color);
  border-radius: 12px;
  overflow: hidden;
  cursor: zoom-in; /* Büyüteç ikonu çıkar */
  transition: 0.3s;
  position: relative;
}

.gallery-item:hover {
  transform: translateY(-5px);
  box-shadow: var(--card-hover-shadow);
}

.gallery-img-box {
  height: 220px;
  width: 100%;
  overflow: hidden;
}
.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: 0.5s;
}
.gallery-item:hover img { transform: scale(1.05); }

/* Büyük Kartlar */
.full-width { grid-column: 1 / -1; }
.full-width .gallery-img-box { height: 400px; }


/* ===============================
   MODAL (AÇILIR PENCERE - ORTAK)
   =============================== */
.modal-overlay {
  position: fixed;
  top: 0; left: 0; width: 100%; height: 100%;
  background: rgba(0, 0, 0, 0.85); /* Arka plan koyu */
  z-index: 9999;
  display: none;
  justify-content: center;
  align-items: center;
  padding: 20px;
  opacity: 0;
  transition: opacity 0.3s ease;
  backdrop-filter: blur(5px);
}

.modal-overlay.active { display: flex; opacity: 1; }

/* 1. METİN MODALI İÇERİĞİ */
.modal-text-content {
  background: #fff;
  width: 100%;
  max-width: 700px;
  padding: 40px;
  border-radius: 15px;
  position: relative;
  transform: scale(0.9);
  transition: transform 0.3s ease;
  display: none; /* Varsayılan gizli */
}
.modal-overlay.active .modal-text-content.active { display: block; transform: scale(1); }

/* 2. RESİM MODALI İÇERİĞİ */
.modal-image-content {
  max-width: 90%;
  max-height: 90vh;
  position: relative;
  display: none; /* Varsayılan gizli */
  text-align: center;
}
.modal-overlay.active .modal-image-content.active { display: flex; flex-direction: column; }

.modal-image-content img {
  max-width: 100%;
  max-height: 80vh;
  border-radius: 8px;
  box-shadow: 0 0 50px rgba(0,0,0,0.5);
  object-fit: contain;
}
.modal-caption {
  color: #fff;
  margin-top: 15px;
  font-size: 1.1rem;
  font-weight: 600;
}

/* Kapat Butonları */
.close-btn {
  position: absolute;
  top: 15px; right: 20px;
  font-size: 2rem;
  color: #64748b;
  cursor: pointer;
  z-index: 10;
}
.close-btn-white {
  position: absolute;
  top: -40px; right: 0;
  font-size: 2rem;
  color: #fff;
  cursor: pointer;
}

/* Modal İç Yazı Stilleri */
#modalTitle { color: var(--accent-color); margin-top: 0; }
#modalDesc { line-height: 1.6; color: #334155; }
#modalTags { margin-top: 20px; display: flex; gap: 10px; flex-wrap: wrap; }
.modal-tag {
  background: #eff6ff;
  color: var(--accent-color);
  padding: 5px 12px;
  border-radius: 50px;
  font-size: 0.8rem;
  border: 1px solid #bfdbfe;
}
</style>

<h2 class="section-title">Mühendislik Analizleri</h2>

<div class="projects-stack">

  <div class="project-row" onclick="openTextModal('p1')">
    <div class="row-info">
      <span>Akademik Araştırma</span>
      <h3>Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p1" class="hidden-details">
      <div class="m-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</div>
      <div class="m-desc">
        <ul>
          <li>Euler-Timoshenko teorilerinin kıyaslanması.</li>
          <li>Farklı fiber dizilim açılarının (stacking) kritik burkulma yüküne etkisi.</li>
          <li>ANSYS ACP modülü ile Sonlu Elemanlar (FEM) doğrulaması.</li>
        </ul>
      </div>
      <div class="m-tags">ANSYS ACP, Static Structural, MATLAB</div>
    </div>
  </div>

  <div class="project-row" onclick="openTextModal('p2')">
    <div class="row-info">
      <span>Yazılım Geliştirme</span>
      <h3>Mohr Çemberi Hesaplama Aracı</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p2" class="hidden-details">
      <div class="m-title">Mohr Çemberi Hesaplama Aracı</div>
      <div class="m-desc">Mukavemet hesaplamaları için geliştirilen bu araç, kullanıcıdan alınan gerilme verileriyle otomatik Mohr çemberi çizer ve asal gerilmeleri hesaplar.</div>
      <div class="m-tags">MATLAB GUI, Algoritma, Mukavemet</div>
    </div>
  </div>

  <div class="project-row" onclick="openTextModal('p3')">
    <div class="row-info">
      <span>TÜBİTAK 2209-A</span>
      <h3>VİSA SÖR Asansör Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p3" class="hidden-details">
      <div class="m-title">VİSA SÖR Asansör Tasarımı</div>
      <div class="m-desc">Engelli bireyler için tasarlanan asansör sistemi. Mekanik boyutlandırma, motor seçimi ve güvenlik freni optimizasyonu.</div>
      <div class="m-tags">SolidWorks, Mekanik Tasarım</div>
    </div>
  </div>

  <div class="project-row" onclick="openTextModal('p4')">
    <div class="row-info">
      <span>Bitirme Tezi</span>
      <h3>Francis Tipi Türbin Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p4" class="hidden-details">
      <div class="m-title">Francis Tipi Türbin Tasarımı</div>
      <div class="m-desc">Keban Barajı verileriyle hidrodinamik boyutlandırma. Çark ve salyangoz geometrisinin CFD analizleri.</div>
      <div class="m-tags">SolidWorks, CFD, Hidrodinamik</div>
    </div>
  </div>

</div>

<h2 class="section-title">3D Tasarım & Render</h2>

<div class="gallery-grid">

  <div class="gallery-item" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/ucak.jpg', 'Konsept Uçak Tasarımı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg', 'Alpagu-X İHA Tasarımı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/m16.jpg', 'M16 Piyade Tüfeği Montajı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/jet.png', 'Turbo-Jet Motoru')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>
  
  <div class="gallery-item" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/superman.png', '3D Superman Logosu')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/manifold.jpg', 'Manifold CFD Mesh Ağı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item full-width" onclick="openImageModal('https://emir3d.github.io/muhendislik-cv/images/top.jpg', 'Şahi Top Modeli - Tarihi Modelleme')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Top" onerror="this.src='https://via.placeholder.com/800x400';">
    </div>
  </div>

</div>


<div id="universalModal" class="modal-overlay" onclick="closeModal(event)">
  
  <div id="textModalBody" class="modal-text-content">
    <span class="close-btn" onclick="closeModal(event)">×</span>
    <h2 id="modalTitle">Başlık</h2>
    <div id="modalDesc">Açıklama...</div>
    <div id="modalTags"></div>
  </div>

  <div id="imageModalBody" class="modal-image-content">
    <span class="close-btn-white" onclick="closeModal(event)">×</span>
    <img id="modalImgTag" src="" alt="">
    <div id="modalImgCaption" class="modal-caption"></div>
  </div>

</div>

<script>
// METİN MODALI AÇMA
function openTextModal(id) {
  // Önce temizlik
  document.getElementById('imageModalBody').classList.remove('active');
  document.getElementById('textModalBody').classList.add('active');
  
  var dataDiv = document.getElementById(id);
  
  var title = dataDiv.querySelector('.m-title').innerHTML;
  var desc = dataDiv.querySelector('.m-desc').innerHTML;
  var tags = dataDiv.querySelector('.m-tags').innerText.split(',');

  document.getElementById('modalTitle').innerHTML = title;
  document.getElementById('modalDesc').innerHTML = desc;
  
  var tagHTML = '';
  tags.forEach(function(tag) {
    tagHTML += '<span class="modal-tag">' + tag.trim() + '</span>';
  });
  document.getElementById('modalTags').innerHTML = tagHTML;

  document.getElementById('universalModal').classList.add('active');
}

// RESİM MODALI AÇMA (ZOOM)
function openImageModal(imgSrc, imgTitle) {
  // Önce temizlik
  document.getElementById('textModalBody').classList.remove('active');
  document.getElementById('imageModalBody').classList.add('active');

  document.getElementById('modalImgTag').src = imgSrc;
  document.getElementById('modalImgCaption').innerText = imgTitle;

  document.getElementById('universalModal').classList.add('active');
}

// MODAL KAPATMA
function closeModal(event) {
  // Sadece siyah alana veya çarpıya basınca kapat
  if (
      event.target.classList.contains('modal-overlay') || 
      event.target.classList.contains('close-btn') ||
      event.target.classList.contains('close-btn-white')
     ) {
    document.getElementById('universalModal').classList.remove('active');
  }
}
</script>
