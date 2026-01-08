---
permalink: /certificates/
title: "Sertifikalar & Eğitimler"
excerpt: "Mesleki yetkinlik belgeleri, teknik eğitimler ve kurslar."
author_profile: true
---

<style>
/* 1. SOL MENÜYÜ GİZLE */
.author__avatar { display: none !important; }

/* 2. PROFESYONEL BAŞLIK TASARIMI (GÖRÜNÜR ARKA PLAN) */
h3.cert-category {
  margin-top: 2.5rem;
  margin-bottom: 1.2rem;
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: 0.5px;
  
  /* 🎨 AYARLANAN RENK: Slate-100 (Hafif Mavimsi Gri) */
  /* Ne beyaz kadar silik, ne de koyu gri kadar sert */
  background: #f1f5f9; 
  
  /* Sol tarafa mavi teknik çizgi */
  border-left: 5px solid #2563eb; 
  padding: 10px 15px; /* İç boşluğu biraz artırdım, ferah dursun */
  border-radius: 0 6px 6px 0; /* Sağ kenarları yuvarladık */
  
  /* Altına ince çizgi */
  border-bottom: 1px solid rgba(128, 128, 128, 0.1);
  
  color: inherit; 
}

/* 3. LİSTE YAPISI */
.cert-list {
  display: flex;
  flex-direction: column;
  gap: 0;
  margin-bottom: 2rem; /* Gruplar arası mesafe */
}

.cert-item {
  display: flex;
  flex-direction: column;
  padding: 12px 10px; /* Kenar boşluğu */
  border-bottom: 1px solid rgba(128, 128, 128, 0.1);
  transition: all 0.2s ease;
}
.cert-item:last-child { border-bottom: none; }

/* Sertifika İsmi */
.cert-name {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 3px;
  display: block;
}

/* Kurum İsmi */
.cert-issuer {
  font-size: 0.9rem;
  opacity: 0.8;
  font-weight: 400;
}

/* KÜÇÜK HOVER EFEKTİ */
.cert-item:hover {
  background-color: #f8fafc; /* Üzerine gelince çok hafif renk değişimi */
  padding-left: 15px; /* Hafif sağa kayma efekti */
  border-radius: 4px;
}

/* 4. KOYU MOD AYARLARI */
@media (prefers-color-scheme: dark) {
  h3.cert-category {
    background: #1e293b; /* Koyu modda Slate-800 */
    border-bottom: none;
    color: #f3f4f6;
  }
  .cert-item { border-bottom-color: rgba(255,255,255,0.1); }
  .cert-item:hover { background-color: #334155; }
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
