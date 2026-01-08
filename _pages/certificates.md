---
permalink: /certificates/
title: "Sertifikalar & Eğitimler"
excerpt: "Mesleki yetkinlik belgeleri, teknik eğitimler ve kurslar."
author_profile: true
---

<style>
/* 1. SOL MENÜ GİZLEME */
.author__avatar { display: none !important; }

/* 2. ANA AYARLAR */
body, .page__content {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
}

/* 3. BAŞLIK TASARIMI (Senin Beğendiğin Hafif Renkli Stil) */
h3.cert-category {
  margin-top: 2.5rem;
  margin-bottom: 1.2rem;
  font-size: 1.2rem;
  font-weight: 700;
  letter-spacing: 0.5px;
  
  /* Arka plan: Slate-100 (Çok açık gri-mavi) */
  background: #f1f5f9; 
  
  /* Sol Çizgi */
  border-left: 5px solid #2563eb; 
  padding: 10px 15px;
  border-radius: 0 6px 6px 0;
  
  /* Alt çizgi */
  border-bottom: 1px solid rgba(128, 128, 128, 0.1);
  
  /* Yazı Rengi: Temadan miras alsın (Siyah/Beyaz) */
  color: inherit; 
}

/* 4. LİSTE YAPISI */
.cert-list {
  display: flex;
  flex-direction: column;
  gap: 0;
  margin-bottom: 2rem;
}

.cert-item {
  display: flex;
  flex-direction: column;
  padding: 12px 10px;
  border-bottom: 1px solid rgba(128, 128, 128, 0.1);
  /* Animasyon ayarı */
  transition: all 0.2s cubic-bezier(0.4, 0, 0.2, 1);
  border-left: 3px solid transparent; /* Gizli sol çizgi */
}
.cert-item:last-child { border-bottom: none; }

/* Sertifika Adı */
.cert-name {
  font-size: 1rem;
  font-weight: 600;
  margin-bottom: 3px;
  display: block;
  transition: color 0.2s ease;
}

/* Kurum Adı */
.cert-issuer {
  font-size: 0.9rem;
  opacity: 0.85; /* Hafif transparanlık yeterli */
  font-weight: 400;
}

/* 🔥 DÜZELTİLEN KISIM: HOVER EFEKTİ 🔥 */
/* Arka plan rengini DEĞİŞTİRMİYORUZ. Sadece kayma ve çizgi. */
.cert-item:hover {
  background-color: transparent !important; /* Arka plan değişmesin */
  padding-left: 18px; /* Sağa kaydır */
  border-left-color: #2563eb; /* Sol tarafta mavi çizgi çıkar */
}

/* Hover olunca başlık mavi olsun */
.cert-item:hover .cert-name {
  color: #2563eb !important; 
}

/* 5. KOYU MOD UYUMLULUĞU */
@media (prefers-color-scheme: dark) {
  h3.cert-category {
    background: #1e293b; /* Koyu modda başlık zemini */
    color: #f3f4f6;
    border-bottom: none;
  }
  .cert-item { border-bottom-color: rgba(255,255,255,0.1); }
  
  /* Koyu modda yazı renklerini garantiye al */
  .cert-name { color: #e2e8f0; }
  .cert-issuer { color: #94a3b8; }
  
  /* Hover durumunda başlık açık mavi olsun */
  .cert-item:hover .cert-name { color: #60a5fa !important; }
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
