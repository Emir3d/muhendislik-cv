---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. Kırık Profil Resmini Gizle */
.author__avatar { display: none !important; }

/* 2. Genişlik Ayarı */
.page__content { 
  width: 100% !important; 
  padding-right: 0 !important; 
  max-width: 100% !important;
}

/* 3. Renkler */
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
   PROJE LİSTESİ (TIKLANABİLİR)
   =============================== */
.projects-stack {
  display: flex;
  flex-direction: column;
  gap: 15px;
  margin-bottom: 5rem;
}

/* Tıklanabilir Proje Satırı */
.project-trigger {
  background: #ffffff;
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 20px 25px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  cursor: pointer; /* Tıklanabilir el işareti */
  transition: all 0.2s ease;
  box-shadow: 0 2px 5px rgba(0,0,0,0.02);
  position: relative;
  z-index: 1;
}

/* Koyu Mod Desteği */
@media (prefers-color-scheme: dark) {
  .project-trigger { background: #1e293b; border-color: #334155; }
  .row-info h3 { color: #f1f5f9 !important; }
}

.project-trigger:hover {
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
.project-trigger:hover .row-arrow {
  color: var(--accent-color);
  transform: translateX(5px);
}

/* Gizli Veri Deposu (CSS ile gizlenir) */
.data-storage { display: none !important; }

/* ===============================
   GALERİ (SADECE GÖRÜNÜM)
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
  /* cursor: zoom-in; SİLDİK - Tıklama yok */
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
}
.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: 0.5s;
}
.gallery-item:hover img { transform: scale(1.05); }

/* Büyük Kart (Top) */
.full-width { grid-column: 1 / -1; }
.full-width .gallery-img-box { height: 400px; }


/* ===============================
   MODAL (SADECE PROJELER İÇİN)
   =============================== */
.modal-overlay {
  position: fixed;
  top: 0; left: 0; width: 100%; height: 100%;
  background: rgba(0, 0, 0, 0.9);
  z-index: 9999999; /* En üst katman */
  display: none;
  justify-content: center;
  align-items: center;
  padding: 20px;
  backdrop-filter: blur(5px);
}

/* JS ile 'active' sınıfı eklenince görünür olur */
.modal-overlay.active { display: flex !important; animation: fadeIn 0.3s forwards; }

@keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }

/* İçerik Kutusu (Metin) */
.modal-text-box {
  background: #fff;
  width: 100%;
  max-width: 700px;
  padding: 40px;
  border-radius: 15px;
  position: relative;
  /* display: none; SİLDİK - Zaten overlay gizli */
}
@media (prefers-color-scheme: dark) {
  .modal-text-box { background: #1e293b; color: #fff; }
  .modal-text-box h2 { color: #60a5fa !important; }
  .modal-text-box #modal-desc-area { color: #cbd5e1 !important; }
}

/* Kapat Butonu */
.close-btn {
  position: absolute;
  top: 15px; right: 20px;
  font-size: 2rem;
  color: #64748b;
  cursor: pointer;
  line-height: 1;
}
.close-btn:hover { color: #ef4444; }

/* Modal Etiketleri */
#modal-tags-area { margin-top: 25px; display: flex; gap: 10px; flex-wrap: wrap; }
.modal-tag-item {
  background: #eff6ff;
  color: var(--accent-color);
  padding: 5px 12px;
  border-radius: 50px;
  font-size: 0.8rem;
  border: 1px solid #bfdbfe;
  font-weight: 600;
}
@media (prefers-color-scheme: dark) {
  .modal-tag-item { background: #172554; color: #93c5fd; border-color: #1e40af; }
}
</style>


<h2 class="section-title">Mühendislik Analizleri</h2>

<div class="projects-stack">

  <div class="project-trigger">
    <div class="row-info">
      <span>Akademik Araştırma</span>
      <h3>Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div class="data-storage">
      <div class="d-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</div>
      <div class="d-desc">
        Bu çalışmada, hibrit kompozit kirişlerin burkulma davranışları incelenmiştir.
        <ul>
          <li>Euler-Timoshenko teorilerinin kıyaslanması yapıldı.</li>
          <li>Farklı fiber dizilim açılarının (stacking sequence) kritik burkulma yüküne etkisi araştırıldı.</li>
          <li>ANSYS ACP modülü kullanılarak Sonlu Elemanlar (FEM) doğrulaması gerçekleştirildi.</li>
        </ul>
      </div>
      <div class="d-tags">ANSYS ACP, Static Structural, MATLAB</div>
    </div>
  </div>

  <div class="project-trigger">
    <div class="row-info">
      <span>Yazılım Geliştirme</span>
      <h3>Mohr Çemberi Hesaplama Aracı</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div class="data-storage">
      <div class="d-title">Mohr Çemberi Hesaplama Aracı</div>
      <div class="d-desc">Mukavemet hesaplamaları için geliştirilen bu araç, kullanıcıdan alınan gerilme verileriyle otomatik Mohr çemberi çizer. Asal gerilmeleri ve maksimum kayma gerilmesini hesaplayarak grafiksel arayüzde sunar.</div>
      <div class="d-tags">MATLAB GUI, Algoritma, Mukavemet</div>
    </div>
  </div>

  <div class="project-trigger">
    <div class="row-info">
      <span>TÜBİTAK 2209-A</span>
      <h3>VİSA SÖR Asansör Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div class="data-storage">
      <div class="d-title">VİSA SÖR Asansör Tasarımı</div>
      <div class="d-desc">Engelli bireylerin erişilebilirliğini artırmak için tasarlanan özel asansör sistemi. Proje kapsamında mekanik boyutlandırma, motor seçimi ve güvenlik freni optimizasyonu yapılmıştır.</div>
      <div class="d-tags">SolidWorks, Mekanik Tasarım, Proje Yönetimi</div>
    </div>
  </div>

  <div class="project-trigger">
    <div class="row-info">
      <span>Bitirme Tezi</span>
      <h3>Francis Tipi Türbin Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div class="data-storage">
      <div class="d-title">Francis Tipi Türbin Tasarımı</div>
      <div class="d-desc">Keban Barajı verileri referans alınarak yapılan hidrodinamik tasarım çalışması. Çark (runner) ve salyangoz (volute) geometrisinin CFD analizleri ile optimizasyonu.</div>
      <div class="d-tags">SolidWorks, CFD, Hidrodinamik</div>
    </div>
  </div>

</div>


<h2 class="section-title">3D Tasarım & Render</h2>

<div class="gallery-grid">

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>
  
  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';">
    </div>
  </div>

  <div class="gallery-item full-width">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Top" onerror="this.src='https://via.placeholder.com/800x400';">
    </div>
  </div>

</div>


<div id="main-modal" class="modal-overlay">
  
  <div id="text-box" class="modal-text-box">
    <span class="close-btn">&times;</span>
    <h2 id="modal-title">Başlık</h2>
    <div id="modal-desc-area">Açıklama...</div>
    <div id="modal-tags-area"></div>
  </div>

</div>

<script>
document.addEventListener("DOMContentLoaded", function() {
  
  // Elemanları Seç
  const modal = document.getElementById("main-modal");
  const modalTitle = document.getElementById("modal-title");
  const modalDesc = document.getElementById("modal-desc-area");
  const modalTags = document.getElementById("modal-tags-area");

  // KAPATMA FONKSİYONU
  function closeModal() {
    modal.classList.remove("active");
  }

  // Kapatma butonunu dinle
  document.querySelector(".close-btn").addEventListener("click", closeModal);

  // Dışarıya tıklayınca kapat
  modal.addEventListener("click", function(e) {
    if (e.target === modal) closeModal();
  });


  // PROJE KARTLARINI DİNLE
  const projects = document.querySelectorAll(".project-trigger");
  
  projects.forEach(p => {
    p.addEventListener("click", function() {
      // Verileri gizli kutudan çek
      const dataDiv = this.querySelector(".data-storage");
      const title = dataDiv.querySelector(".d-title").innerHTML;
      const desc = dataDiv.querySelector(".d-desc").innerHTML;
      const tags = dataDiv.querySelector(".d-tags").innerText.split(",");

      // Modala yaz
      modalTitle.innerHTML = title;
      modalDesc.innerHTML = desc;

      // Etiketleri oluştur
      let tagHTML = "";
      tags.forEach(tag => {
        if(tag.trim()) tagHTML += '<span class="modal-tag-item">' + tag.trim() + '</span>';
      });
      modalTags.innerHTML = tagHTML;

      // Göster
      modal.classList.add("active");
    });
  });

});
</script>
