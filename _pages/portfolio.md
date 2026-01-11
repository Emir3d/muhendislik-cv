---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. PROFİL RESMİ GİZLEME */
.author__avatar { display: none !important; }

/* 2. SAYFA GENİŞLİĞİ AYARI */
.page__content { 
  width: 100% !important; 
  padding-right: 0 !important; 
  max-width: 100% !important;
}

/* 3. RENK DEĞİŞKENLERİ */
:root {
  --border-color: #e2e8f0;
  --accent-color: #2563eb;
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
  color: inherit;
}
.section-title::after {
  content: "";
  flex-grow: 1;
  height: 2px;
  background: #e5e7eb;
}

/* ===============================
   PROJE LİSTESİ (Project Stack)
   =============================== */
.projects-stack {
  display: flex;
  flex-direction: column;
  gap: 15px;
  margin-bottom: 5rem;
}

.project-row {
  background: #ffffff;
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 20px 25px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer;
  transition: all 0.2s ease;
  box-shadow: 0 2px 5px rgba(0,0,0,0.02);
  position: relative;
  z-index: 1;
}

/* Koyu mod desteği */
@media (prefers-color-scheme: dark) {
  .project-row { background: #1e293b; border-color: #334155; }
  .row-info h3 { color: #f1f5f9 !important; }
}

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

/* Gizli Detaylar */
.hidden-details { display: none; }

/* ===============================
   GALERİ (Grid)
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
  cursor: zoom-in;
  transition: 0.3s;
  position: relative;
  z-index: 1;
}

@media (prefers-color-scheme: dark) {
  .gallery-item { background: #1e293b; border-color: #334155; }
}

.gallery-item:hover {
  transform: translateY(-5px);
  box-shadow: var(--card-hover-shadow);
}

.gallery-img-box {
  height: 220px;
  width: 100%;
  overflow: hidden;
  pointer-events: none; /* Tıklamayı engellemesin diye */
}
.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: 0.5s;
}
.gallery-item:hover img { transform: scale(1.05); }

/* Büyük Kart */
.full-width { grid-column: 1 / -1; }
.full-width .gallery-img-box { height: 400px; }


/* ===============================
   MODAL (AÇILIR PENCERE - TAMİR EDİLDİ)
   =============================== */
.modal-overlay {
  position: fixed;
  top: 0; left: 0; width: 100%; height: 100%;
  background: rgba(0, 0, 0, 0.9);
  z-index: 2147483647; /* Mümkün olan en yüksek sayı */
  display: none; /* JS ile flex yapılacak */
  justify-content: center;
  align-items: center;
  padding: 20px;
  backdrop-filter: blur(5px);
}

/* Aktif Sınıfı */
.modal-overlay.active { 
  display: flex !important; 
  animation: fadeIn 0.3s ease-out forwards;
}

@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

/* METİN KUTUSU */
.modal-text-content {
  background: #fff;
  width: 100%;
  max-width: 700px;
  padding: 40px;
  border-radius: 15px;
  position: relative;
  display: none;
}
@media (prefers-color-scheme: dark) {
  .modal-text-content { background: #1e293b; color: #fff; }
  .modal-text-content h2 { color: #60a5fa !important; }
  .modal-text-content #modalDesc { color: #cbd5e1 !important; }
}
.modal-text-content.active { display: block; }

/* RESİM KUTUSU */
.modal-image-content {
  width: auto;
  height: auto;
  max-width: 95%;
  max-height: 95vh;
  position: relative;
  display: none;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.modal-image-content.active { display: flex; }

.modal-image-content img {
  max-width: 100%;
  max-height: 85vh;
  border-radius: 8px;
  box-shadow: 0 0 50px rgba(0,0,0,0.5);
  object-fit: contain;
  background: transparent;
}

.modal-caption {
  color: #fff;
  margin-top: 15px;
  font-size: 1.1rem;
  font-weight: 600;
  text-shadow: 0 2px 4px rgba(0,0,0,0.8);
  text-align: center;
}

/* KAPAT BUTONLARI */
.close-btn {
  position: absolute;
  top: 15px; right: 20px;
  font-size: 2rem;
  color: #64748b;
  cursor: pointer;
  z-index: 10;
  line-height: 1;
}
.close-btn-white {
  position: absolute;
  top: -50px; right: 0;
  font-size: 3rem;
  color: #fff;
  cursor: pointer;
  z-index: 10;
  font-weight: bold;
  text-shadow: 0 2px 5px rgba(0,0,0,0.5);
}

/* Etiketler */
#modalTitle { color: var(--accent-color); margin-top: 0; }
#modalDesc { line-height: 1.6; color: #334155; font-size: 1.05rem; }
#modalTags { margin-top: 25px; display: flex; gap: 10px; flex-wrap: wrap; }
.modal-tag {
  background: #eff6ff;
  color: var(--accent-color);
  padding: 5px 12px;
  border-radius: 50px;
  font-size: 0.8rem;
  border: 1px solid #bfdbfe;
  font-weight: 600;
}
@media (prefers-color-scheme: dark) {
  .modal-tag { background: #172554; color: #93c5fd; border-color: #1e40af; }
}
</style>

<h2 class="section-title">Mühendislik Analizleri</h2>

<div class="projects-stack">

  <div class="project-row" onclick="window.openTextModal('p1')">
    <div class="row-info">
      <span>Akademik Araştırma</span>
      <h3>Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p1" class="hidden-details">
      <div class="m-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</div>
      <div class="m-desc">
        Bu çalışmada, hibrit kompozit kirişlerin burkulma davranışları incelenmiştir.
        <ul>
          <li>Euler-Timoshenko teorilerinin kıyaslanması yapıldı.</li>
          <li>Farklı fiber dizilim açılarının (stacking sequence) kritik burkulma yüküne etkisi araştırıldı.</li>
          <li>ANSYS ACP modülü kullanılarak Sonlu Elemanlar (FEM) doğrulaması gerçekleştirildi.</li>
        </ul>
      </div>
      <div class="m-tags">ANSYS ACP, Static Structural, MATLAB</div>
    </div>
  </div>

  <div class="project-row" onclick="window.openTextModal('p2')">
    <div class="row-info">
      <span>Yazılım Geliştirme</span>
      <h3>Mohr Çemberi Hesaplama Aracı</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p2" class="hidden-details">
      <div class="m-title">Mohr Çemberi Hesaplama Aracı</div>
      <div class="m-desc">Mukavemet hesaplamaları için geliştirilen bu araç, kullanıcıdan alınan gerilme verileriyle otomatik Mohr çemberi çizer. Asal gerilmeleri ve maksimum kayma gerilmesini hesaplayarak grafiksel arayüzde sunar.</div>
      <div class="m-tags">MATLAB GUI, Algoritma, Mukavemet</div>
    </div>
  </div>

  <div class="project-row" onclick="window.openTextModal('p3')">
    <div class="row-info">
      <span>TÜBİTAK 2209-A</span>
      <h3>VİSA SÖR Asansör Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p3" class="hidden-details">
      <div class="m-title">VİSA SÖR Asansör Tasarımı</div>
      <div class="m-desc">Engelli bireylerin erişilebilirliğini artırmak için tasarlanan özel asansör sistemi. Proje kapsamında mekanik boyutlandırma, motor seçimi ve güvenlik freni optimizasyonu yapılmıştır.</div>
      <div class="m-tags">SolidWorks, Mekanik Tasarım, Proje Yönetimi</div>
    </div>
  </div>

  <div class="project-row" onclick="window.openTextModal('p4')">
    <div class="row-info">
      <span>Bitirme Tezi</span>
      <h3>Francis Tipi Türbin Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    <div id="p4" class="hidden-details">
      <div class="m-title">Francis Tipi Türbin Tasarımı</div>
      <div class="m-desc">Keban Barajı verileri referans alınarak yapılan hidrodinamik tasarım çalışması. Çark (runner) ve salyangoz (volute) geometrisinin CFD analizleri ile optimizasyonu.</div>
      <div class="m-tags">SolidWorks, CFD, Hidrodinamik</div>
    </div>
  </div>

</div>

<h2 class="section-title">3D Tasarım & Render</h2>

<div class="gallery-grid">

  <div class="gallery-item" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/ucak.jpg', 'Konsept Uçak Tasarımı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg', 'Alpagu-X İHA Tasarımı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/m16.jpg', 'M16 Piyade Tüfeği Montajı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/jet.png', 'Turbo-Jet Motoru')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>
  
  <div class="gallery-item" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/superman.png', '3D Superman Logosu')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/manifold.jpg', 'Manifold CFD Mesh Ağı')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item full-width" onclick="window.openImageModal('https://emir3d.github.io/muhendislik-cv/images/top.jpg', 'Şahi Top Modeli - Tarihi Modelleme')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Top" onerror="this.src='https://via.placeholder.com/800x400';">
    </div>
  </div>

</div>


<div id="universalModal" class="modal-overlay" onclick="window.closeModal(event)">
  
  <div id="textModalBody" class="modal-text-content">
    <span class="close-btn" onclick="window.closeModal(event)">×</span>
    <h2 id="modalTitle">Başlık</h2>
    <div id="modalDesc">Açıklama...</div>
    <div id="modalTags"></div>
  </div>

  <div id="imageModalBody" class="modal-image-content">
    <span class="close-btn-white" onclick="window.closeModal(event)">×</span>
    <img id="modalImgTag" src="" alt="">
    <div id="modalImgCaption" class="modal-caption"></div>
  </div>

</div>

<script>
// Fonksiyonları window nesnesine ekleyerek global yapıyoruz
window.openTextModal = function(id) {
  var modal = document.getElementById('universalModal');
  var textBody = document.getElementById('textModalBody');
  var imgBody = document.getElementById('imageModalBody');

  imgBody.classList.remove('active');
  textBody.classList.add('active');
  
  var dataDiv = document.getElementById(id);
  if(!dataDiv) return;

  var title = dataDiv.querySelector('.m-title').innerHTML;
  var desc = dataDiv.querySelector('.m-desc').innerHTML;
  var tags = dataDiv.querySelector('.m-tags').innerText.split(',');

  document.getElementById('modalTitle').innerHTML = title;
  document.getElementById('modalDesc').innerHTML = desc;
  
  var tagHTML = '';
  tags.forEach(function(tag) {
    if(tag.trim() !== '') {
      tagHTML += '<span class="modal-tag">' + tag.trim() + '</span>';
    }
  });
  document.getElementById('modalTags').innerHTML = tagHTML;

  modal.classList.add('active');
}

window.openImageModal = function(imgSrc, imgTitle) {
  var modal = document.getElementById('universalModal');
  var textBody = document.getElementById('textModalBody');
  var imgBody = document.getElementById('imageModalBody');

  textBody.classList.remove('active');
  imgBody.classList.add('active');

  document.getElementById('modalImgTag').src = imgSrc;
  document.getElementById('modalImgCaption').innerText = imgTitle;

  modal.classList.add('active');
}

window.closeModal = function(event) {
  if (
      event.target.classList.contains('modal-overlay') || 
      event.target.classList.contains('close-btn') ||
      event.target.classList.contains('close-btn-white')
     ) {
    document.getElementById('universalModal').classList.remove('active');
  }
}
</script>
