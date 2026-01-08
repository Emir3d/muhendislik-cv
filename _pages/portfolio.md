---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
/* ==========================================
   PORTFOLYO KART TASARIMI
   ========================================== */

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 25px;
  margin-top: 2rem;
}

.project-card {
  background-color: #ffffff;
  border: 1px solid rgba(128, 128, 128, 0.2);
  border-radius: 8px;
  padding: 25px;
  transition: transform 0.2s ease, box-shadow 0.2s ease;
  position: relative;
  overflow: hidden;
}

/* Kartın soluna renkli çizgi */
.project-card::before {
  content: "";
  position: absolute;
  left: 0;
  top: 0;
  height: 100%;
  width: 5px;
  background-color: #2563eb; /* Varsayılan Mavi */
}

/* Hover Efekti */
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
  font-size: 1.25rem;
  font-weight: 700;
  margin-bottom: 10px;
  color: #111; /* Başlık Rengi */
}

.card-desc {
  font-size: 0.95rem;
  color: #444;
  line-height: 1.6;
  margin-bottom: 20px;
}

.card-link {
  font-size: 0.9rem;
  font-weight: 700;
  color: #2563eb;
  text-decoration: none;
  display: inline-block;
}
.card-link:hover {
  text-decoration: underline;
}

/* Kart Tipleri (Renk Kodları) */
.type-analysis::before { background-color: #2563eb; } /* Mavi: Analiz */
.type-software::before { background-color: #059669; } /* Yeşil: Yazılım/Kod */
.type-design::before { background-color: #d97706; }   /* Turuncu: Tasarım */

/* KOYU MOD AYARLARI */
@media (prefers-color-scheme: dark) {
  .project-card {
    background-color: #1f2937;
    border-color: #374151;
  }
  .card-title { color: #f3f4f6; }
  .card-desc { color: #d1d5db; }
  .card-category { color: #9ca3af; }
  .card-link { color: #60a5fa; }
}
</style>

Mühendislik problemlerine getirdiğim sayısal ve tasarımsal çözümlerden seçkiler.

<div class="projects-grid">

  <div class="project-card type-analysis">
    <span class="card-category">Yapısal Analiz / ANSYS</span>
    <h3 class="card-title">Hibrit Kompozit Plakların Burkulma Analizi</h3>
    <p class="card-desc">
      Karbon ve Aramid fiberlerin farklı dizilim açılarının (stacking sequence) kritik burkulma yüküne etkisinin ANSYS ACP modülü ile incelenmesi ve deneysel verilerle doğrulanması.
    </p>
  </div>

  <div class="project-card type-software">
    <span class="card-category">MATLAB / GUI</span>
    <h3 class="card-title">Kompozit Laminasyon Hesaplayıcı</h3>
    <p class="card-desc">
      Klasik Laminasyon Teorisi (CLT) kullanılarak, farklı katman özelliklerine sahip kompozit yapıların gerilme-şekil değiştirme matrislerini hesaplayan, kullanıcı dostu bir arayüz tasarımı.
    </p>
  </div>

  <div class="project-card type-design">
    <span class="card-category">Mekanik Tasarım</span>
    <h3 class="card-title">Endüstriyel Robot Kolu Mekanizması</h3>
    <p class="card-desc">
      6 eksenli bir robot kolunun kinematik analizlerinin yapılması, SolidWorks ortamında modellenmesi ve kritik parçaların mukavemet analizlerinin gerçekleştirilmesi.
    </p>
  </div>

  <div class="project-card type-analysis">
    <span class="card-category">Akademik Yayın</span>
    <h3 class="card-title">Nanokompozitlerin Otomotiv Uygulamaları</h3>
    <p class="card-desc">
      Otomotiv endüstrisinde ağırlık azaltma ve dayanım artırma amacıyla kullanılan nanokompozit malzemeler üzerine kapsamlı bir literatür taraması ve gelecek projeksiyonu.
    </p>
  </div>

</div>
