---
permalink: /certificates/
title: "Sertifikalar & Eğitimler"
excerpt: "Mesleki yetkinlik belgeleri, teknik eğitimler ve kurslar."
author_profile: true
---

<style>
/* 1. SOL MENÜ GİZLEME */
.author__avatar { display: none !important; }

/* 2. GENEL YAZI RENGİ & TİPOGRAFİ */
body, .page__content {
  color: #222 !important;
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}

/* 3. PROFESYONEL BAŞLIK TASARIMI (Mühendislik Stili) */
h3.cert-category {
  margin-top: 3rem;
  margin-bottom: 1.5rem;
  font-size: 1.15rem;
  font-weight: 700;
  text-transform: uppercase; /* Ciddiyet için hepsi büyük harf */
  letter-spacing: 0.5px;
  color: #111 !important;
  
  /* Modern Dokunuş: Sol Çizgi ve Arka Plan */
  background: #f9fafb; /* Çok açık gri zemin */
  border-left: 5px solid #2563eb; /* Mavi "Engineering" çizgisi */
  padding: 12px 15px; /* İç boşluk */
  border-radius: 0 4px 4px 0; /* Sağ köşeleri hafif yuvarla */
}

/* 4. TEMİZ LİSTE TASARIMI */
.cert-list {
  display: flex;
  flex-direction: column;
  border-top: 1px solid #e5e7eb; /* Listenin tepesine ince çizgi */
}

.cert-item {
  display: flex;
  flex-direction: column;
  padding: 14px 10px; /* Kenarlardan biraz boşluk bırak */
  border-bottom: 1px solid #e5e7eb;
  transition: background-color 0.2s ease;
}

/* Üzerine gelince hafif vurgu */
.cert-item:hover {
  background-color: rgba(37, 99, 235, 0.03); /* Çok silik mavi */
}

.cert-item:last-child { border-bottom: none; }

/* Sertifika Adı */
.cert-name {
  font-size: 1rem;
  font-weight: 600;
  color: #000 !important;
  margin-bottom: 4px;
}

/* Kurum Adı */
.cert-issuer {
  font-size: 0.85rem;
  font-weight: 500;
  color: #666 !important;
  display: flex;
  align-items: center;
}

/* Kurum adının önüne minik gri nokta */
.cert-issuer::before {
  content: "";
  display: inline-block;
  width: 6px;
  height: 6px;
  background-color: #9ca3af;
  border-radius: 50%;
  margin-right: 8px;
}

/* 5. KOYU MOD AYARLARI */
@media (prefers-color-scheme: dark) {
  body, .page__content { color: #e5e7eb !important; }
  
  h3.cert-category { 
    background: #1f2937; /* Koyu gri zemin */
    color: #fff !important; 
    border-left-color: #60a5fa; /* Daha açık mavi */
  }
  
  .cert-list, .cert-item { border-color: #374151; }
  .cert-item:hover { background-color: rgba(255,255,255,0.03); }
  
  .cert-name { color: #f3f4f6 !important; }
  .cert-issuer { color: #9ca3af !important; }
  .cert-issuer::before { background-color: #6b7280; }
}
</style>

Mühendislik kariyerim boyunca edindiğim teknik yetkinlikler ve tamamladığım eğitim programları.

<h3 class="cert-category">Analiz ve Simülasyon (CAE)</h3>
<div class="cert-list">
  <div class="cert-item">
    <span class="cert-name">Introduction to ANSYS Fluent</span>
    <span class="cert-issuer">Numesys (Ansys Elite Channel Partner)</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Introduction to ANSYS Meshing</span>
    <span class="cert-issuer">Numesys (Ansys Elite Channel Partner)</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Temel ve İleri Düzeyde Simulink Eğitimi</span>
    <span class="cert-issuer">FİGES A.Ş. / MathWorks</span>
  </div>
</div>

<h3 class="cert-category">Tasarım ve CAD</h3>
<div class="cert-list">
  <div class="cert-item">
    <span class="cert-name">SolidWorks Montaj Eğitimi</span>
    <span class="cert-issuer">Armada Yazılım</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">SolidWorks Teknik Resim Eğitimi</span>
    <span class="cert-issuer">Armada Yazılım</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">SolidWorks 2019 2 Boyutlu Çizim Eğitimi</span>
    <span class="cert-issuer">Udemy</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">AutoCAD Eğitimi & Çizim Teknikleri</span>
    <span class="cert-issuer">Global Enstitü</span>
  </div>
</div>

<h3 class="cert-category">Havacılık ve İHA Sistemleri</h3>
<div class="cert-list">
  <div class="cert-item">
    <span class="cert-name">Havacılık Motorları Okulu</span>
    <span class="cert-issuer">TEI Akademi (TUSAŞ Motor Sanayii A.Ş.)</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">İHA-1 Sportif / Amatör Pilot Lisansı</span>
    <span class="cert-issuer">Sivil Havacılık Genel Müdürlüğü (SHGM)</span>
  </div>
</div>

<h3 class="cert-category">Yazılım ve Yapay Zeka</h3>
<div class="cert-list">
  <div class="cert-item">
    <span class="cert-name">Python and AI Introduction Bootcamp</span>
    <span class="cert-issuer">Global AI Hub & Akbank</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Yapay Zekaya İlk Adım & Uygulamalı Atölye</span>
    <span class="cert-issuer">Global AI Hub / GAİB</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Introduction to Python</span>
    <span class="cert-issuer">Business AI School</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Algoritma ve Programlamaya Giriş</span>
    <span class="cert-issuer">İSMEK</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Temel Python Eğitimi</span>
    <span class="cert-issuer">IEEE Gazi Öğrenci Topluluğu</span>
  </div>
</div>

<h3 class="cert-category">Otomotiv Endüstrisi</h3>
<div class="cert-list">
  <div class="cert-item">
    <span class="cert-name">Click4Career Programı</span>
    <span class="cert-issuer">Tofaş Türk Otomobil Fabrikası A.Ş.</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Otomotiv Yaz Kampı</span>
    <span class="cert-issuer">OİB & OSD</span>
  </div>
</div>

<h3 class="cert-category">Diğer Eğitimler</h3>
<div class="cert-list">
  <div class="cert-item">
    <span class="cert-name">Fotovoltaik Teknik Eğitim Programı</span>
    <span class="cert-issuer">CW Akademi / CW Enerji</span>
  </div>
  <div class="cert-item">
    <span class="cert-name">Microsoft Word Yetkinlik Eğitimi</span>
    <span class="cert-issuer">Güneydoğu Anadolu İhracatçı Birlikleri (GAİB)</span>
  </div>
</div>
