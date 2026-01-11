---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* 1. PROFİL RESMİ GİZLEME */
.author__avatar { display: none !important; }

/* ===============================
   RENK PALETİ (OTOMATİK KOYU MOD)
   =============================== */
:root {
  --bg-color: #f8fafc;
  --card-bg: #ffffff;
  --text-main: #1e293b;
  --text-sub: #64748b;
  --border-color: #e2e8f0;
  --accent-color: #3b82f6; /* Mavi */
  --highlight-shadow: rgba(59, 130, 246, 0.15);
}

/* 🌙 CİHAZ KOYU MOD İSE OTOMATİK DEVREYE GİRER */
@media (prefers-color-scheme: dark) {
  :root {
    --bg-color: #0f172a; /* Slate 900 (Koyu Lacivert) */
    --card-bg: #1e293b;  /* Slate 800 */
    --text-main: #f1f5f9;
    --text-sub: #94a3b8;
    --border-color: #334155;
    --accent-color: #38bdf8; /* Açık Mavi (Neon) */
    --highlight-shadow: rgba(56, 189, 248, 0.2);
  }
}

/* GLOBAL AYARLAR */
body {
  background-color: var(--bg-color) !important;
  color: var(--text-main);
  transition: background-color 0.3s ease, color 0.3s ease;
  font-family: 'Inter', sans-serif;
}

.page__content { width: 100% !important; padding-right: 0 !important; }

/* ===============================
   BAŞLIKLAR
   =============================== */
.section-title {
  font-size: 1.8rem;
  font-weight: 800;
  margin: 3rem 0 2rem;
  color: var(--text-main);
  display: flex;
  align-items: center;
  gap: 15px;
}
.section-title::after {
  content: "";
  flex-grow: 1;
  height: 2px;
  background: linear-gradient(90deg, var(--accent-color), transparent);
}

/* ===============================
   YENİ DÜZEN: "STACK" (ÜST ÜSTE) LİSTE
   =============================== */
.projects-stack {
  display: flex;
  flex-direction: column;
  gap: 15px; /* Kartlar arası boşluk */
  margin-bottom: 5rem;
}

/* Proje Kartı (Satır Halinde) */
.project-row {
  background: var(--card-bg);
  border: 1px solid var(--border-color);
  border-radius: 12px;
  padding: 20px 25px;
  display: flex;
  justify-content: space-between; /* Yazı solda, etiket sağda */
  align-items: center;
  cursor: pointer; /* Tıklanabilir el işareti */
  transition: all 0.2s ease;
  position: relative;
}

/* Hover Efekti */
.project-row:hover {
  transform: translateX(10px); /* Hafif sağa kayar */
  border-color: var(--accent-color);
  box-shadow: 0 4px 20px var(--highlight-shadow);
}

/* Sol Taraf: Bilgiler */
.row-info h3 {
  margin: 0 0 5px 0;
  font-size: 1.1rem;
  font-weight: 700;
  color: var(--text-main);
}
.row-info span {
  font-size: 0.8rem;
  color: var(--accent-color);
  font-weight: 600;
  text-transform: uppercase;
  letter-spacing: 1px;
}

/* Sağ Taraf: Ok İşareti */
.row-arrow {
  font-size: 1.2rem;
  color: var(--text-sub);
  opacity: 0.5;
  transition: 0.2s;
}
.project-row:hover .row-arrow {
  opacity: 1;
  color: var(--accent-color);
  transform: translateX(5px);
}

/* Gizli Detaylar (Modal İçin) */
.hidden-details { display: none; }


/* ===============================
   GALERİ (GRID)
   =============================== */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 20px;
}

.gallery-item {
  background: var(--card-bg);
  border: 1px solid var(--border-color);
  border-radius: 12px;
  overflow: hidden;
  cursor: pointer;
  transition: 0.3s;
}

.gallery-item:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 30px var(--highlight-shadow);
}

.gallery-img-box {
  height: 200px;
  width: 100%;
  overflow: hidden;
}
.gallery-img-box img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: 0.5s;
}
.gallery-item:hover img { transform: scale(1.1); }

/* Özel Büyük Kartlar (Top ve Manifold) */
.full-width { grid-column: 1 / -1; }
.full-width .gallery-img-box { height: 350px; }


/* ===============================
   MODAL (AÇILIR PENCERE) - SİHİR BURADA ✨
   =============================== */
.modal-overlay {
  position: fixed;
  top: 0; left: 0; width: 100%; height: 100%;
  background: rgba(0, 0, 0, 0.8); /* Arka planı karart */
  backdrop-filter: blur(5px); /* Arka planı bulanıklaştır */
  z-index: 9999;
  display: none; /* Varsayılan gizli */
  justify-content: center;
  align-items: center;
  padding: 20px;
  opacity: 0;
  transition: opacity 0.3s ease;
}

.modal-content {
  background: var(--card-bg);
  width: 100%;
  max-width: 700px;
  padding: 40px;
  border-radius: 20px;
  position: relative;
  border: 1px solid var(--accent-color);
  box-shadow: 0 0 50px var(--highlight-shadow);
  transform: scale(0.9);
  transition: transform 0.3s ease;
}

/* Modal Açılınca Efekt */
.modal-overlay.active { display: flex; opacity: 1; }
.modal-overlay.active .modal-content { transform: scale(1); }

/* Kapat Butonu */
.close-btn {
  position: absolute;
  top: 15px; right: 20px;
  font-size: 2rem;
  color: var(--text-sub);
  cursor: pointer;
}
.close-btn:hover { color: var(--accent-color); }

/* Modal İçindeki Yazılar */
#modalTitle { color: var(--accent-color); margin-top: 0; }
#modalDesc { line-height: 1.6; font-size: 1rem; color: var(--text-main); }
#modalTags { margin-top: 20px; display: flex; gap: 10px; flex-wrap: wrap; }

.modal-tag {
  background: rgba(59, 130, 246, 0.1);
  color: var(--accent-color);
  padding: 5px 12px;
  border-radius: 50px;
  font-size: 0.8rem;
  font-weight: 600;
  border: 1px solid var(--accent-color);
}
</style>

<h2 class="section-title">Mühendislik Analizleri</h2>

<div class="projects-stack">

  <div class="project-row" onclick="openModal('p1')">
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
          <li>ANSYS ACP modülü ile Sonlu Elemanlar (FEM) doğrulaması ve analitik sonuçlarla karşılaştırma.</li>
        </ul>
      </div>
      <div class="m-tags">ANSYS ACP, Static Structural, MATLAB</div>
    </div>
  </div>

  <div class="project-row" onclick="openModal('p2')">
    <div class="row-info">
      <span>Yazılım Geliştirme</span>
      <h3>Mohr Çemberi Hesaplama Aracı</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div id="p2" class="hidden-details">
      <div class="m-title">Mohr Çemberi Hesaplama Aracı</div>
      <div class="m-desc">Mukavemet hesaplamaları için geliştirilen bu araç, kullanıcıdan alınan gerilme verileriyle (sigma x, sigma y, tau) otomatik olarak Mohr çemberini çizer, asal gerilmeleri ve maksimum kayma gerilmesini hesaplar. MATLAB App Designer kullanılarak oluşturulmuştur.</div>
      <div class="m-tags">MATLAB GUI, Algoritma, Mukavemet</div>
    </div>
  </div>

  <div class="project-row" onclick="openModal('p3')">
    <div class="row-info">
      <span>TÜBİTAK 2209-A</span>
      <h3>VİSA SÖR Asansör Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div id="p3" class="hidden-details">
      <div class="m-title">VİSA SÖR Asansör Tasarımı</div>
      <div class="m-desc">Engelli bireylerin erişilebilirliğini artırmak amacıyla tasarlanan özel asansör sistemi. Proje kapsamında mekanik boyutlandırma, motor seçimi ve güvenlik freni optimizasyonu yapılmıştır.</div>
      <div class="m-tags">SolidWorks, Mekanik Tasarım, Proje Yönetimi</div>
    </div>
  </div>

  <div class="project-row" onclick="openModal('p4')">
    <div class="row-info">
      <span>Bitirme Tezi</span>
      <h3>Francis Tipi Türbin Tasarımı</h3>
    </div>
    <div class="row-arrow">➔</div>
    
    <div id="p4" class="hidden-details">
      <div class="m-title">Francis Tipi Türbin Tasarımı</div>
      <div class="m-desc">Keban Barajı'nın hidrolik verileri referans alınarak yapılan hidrodinamik tasarım çalışması. Çark (runner), salyangoz (volute) ve dağıtıcı kanatların tasarımı CFD analizleri göz önünde bulundurularak yapılmıştır.</div>
      <div class="m-tags">SolidWorks, CFD Teorisi, Hidrodinamik</div>
    </div>
  </div>

</div>

<h2 class="section-title">3D Tasarım & Render</h2>

<div class="gallery-grid">

  <div class="gallery-item" onclick="alert('Görsel odaklama özelliği yakında!')">
    <div class="gallery-img-box">
      <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Uçak" onerror="this.src='https://via.placeholder.com/600x400';">
    </div>
  </div>

  <div class="gallery-item" onclick="alert('Görsel odaklama özelliği yakında!')">
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


<div id="projectModal" class="modal-overlay" onclick="closeModal(event)">
  <div class="modal-content">
    <span class="close-btn" onclick="closeModal(event)">×</span>
    <h2 id="modalTitle">Proje Başlığı</h2>
    <div id="modalDesc">Proje açıklaması buraya gelecek...</div>
    <div id="modalTags"></div>
  </div>
</div>

<script>
// Modal Açma Fonksiyonu
function openModal(id) {
  var dataDiv = document.getElementById(id);
  
  // İçerikleri çek
  var title = dataDiv.querySelector('.m-title').innerHTML;
  var desc = dataDiv.querySelector('.m-desc').innerHTML;
  var tags = dataDiv.querySelector('.m-tags').innerText.split(',');

  // Modala yaz
  document.getElementById('modalTitle').innerHTML = title;
  document.getElementById('modalDesc').innerHTML = desc;
  
  // Etiketleri oluştur
  var tagHTML = '';
  tags.forEach(function(tag) {
    tagHTML += '<span class="modal-tag">' + tag.trim() + '</span>';
  });
  document.getElementById('modalTags').innerHTML = tagHTML;

  // Modalı Göster
  document.getElementById('projectModal').classList.add('active');
}

// Modal Kapatma Fonksiyonu
function closeModal(event) {
  // Sadece siyah alana veya çarpıya basınca kapat (İçeriğe basınca kapanmasın)
  if (event.target.classList.contains('modal-overlay') || event.target.classList.contains('close-btn')) {
    document.getElementById('projectModal').classList.remove('active');
  }
}
</script>
