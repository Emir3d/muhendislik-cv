---
permalink: /portfolio/
title: "Portfolyo & Projeler"
excerpt: "Mühendislik analizleri, simülasyonlar ve tasarım çalışmaları."
author_profile: true
---

<style>
.author__avatar{display:none!important}

.projects-grid,.gallery-grid{
  display:grid;
  grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
  gap:28px;
  margin:2.5rem 0 4.5rem
}

.project-card,.gallery-item{
  background:#fff;
  border:1px solid rgba(0,0,0,.06);
  border-radius:14px;
  overflow:hidden;
  display:flex;
  flex-direction:column;
  position:relative;
  transition:.35s;
  box-shadow:0 8px 20px rgba(0,0,0,.04)
}

.project-card:hover,.gallery-item:hover{
  transform:translateY(-8px) scale(1.01);
  box-shadow:0 20px 40px rgba(0,0,0,.08)
}

.project-card::before{
  content:"";
  position:absolute;
  left:0;top:0;
  width:5px;height:100%;
  background:linear-gradient(180deg,#3b82f6,#06b6d4)
}

.card-body{padding:26px;flex-grow:1}

.card-category{
  font-size:.72rem;
  text-transform:uppercase;
  letter-spacing:1.2px;
  color:#6b7280;
  margin-bottom:10px;
  font-weight:700
}

.card-title{
  font-size:1.2rem;
  font-weight:700;
  margin-bottom:12px;
  color:#111827
}

.card-desc{
  font-size:.92rem;
  color:#4b5563;
  line-height:1.65
}
.card-desc ul{padding-left:16px;margin-bottom:0}
.card-desc li{margin-bottom:6px}

.card-footer{
  padding:16px 26px;
  background:#f9fafb;
  border-top:1px solid rgba(0,0,0,.05);
  display:flex;
  flex-wrap:wrap;
  gap:8px
}

.tech-tag{
  font-size:.75rem;
  font-weight:600;
  padding:4px 12px;
  border-radius:999px;
  background:#e5e7eb;
  color:#374151;
  border:1px solid rgba(0,0,0,.08)
}

.tag-ansys{background:#fef08a;color:#854d0e}
.tag-matlab{background:#dbeafe;color:#1e40af}
.tag-solid{background:#fee2e2;color:#991b1b}
.tag-inventor{background:#d1fae5;color:#065f46}
.tag-3ds{background:#f3e8ff;color:#6b21a8}

.section-title{
  font-size:1.6rem;
  font-weight:700;
  margin:3.5rem 0 1.8rem;
  position:relative
}
.section-title::after{
  content:"";
  position:absolute;
  left:0;bottom:-8px;
  width:80px;height:3px;
  background:linear-gradient(90deg,#3b82f6,#06b6d4)
}

.gallery-img-box{
  height:220px;
  overflow:hidden
}
.gallery-img-box img{
  width:100%;
  height:100%;
  object-fit:cover;
  transition:.6s
}
.gallery-item:hover img{transform:scale(1.12)}

@media(prefers-color-scheme:dark){
  .project-card,.gallery-item{background:#1f2937;border-color:#374151}
  .card-title{color:#f3f4f6}
  .card-desc{color:#d1d5db}
  .card-category{color:#9ca3af}
  .card-footer{background:#111827;border-color:#374151}
  .tech-tag{background:#374151;color:#e5e7eb}
}
</style>

<h2 class="section-title">Mühendislik Analizleri & Ar-Ge</h2>
<div class="projects-grid">

<div class="project-card">
  <div class="card-body">
    <span class="card-category">Akademik Araştırma</span>
    <h3 class="card-title">Hibrit Kompozit Kirişlerde Burkulma Analizi</h3>
    <div class="card-desc">
      <ul>
        <li>Euler–Timoshenko teorilerinin kıyaslanması</li>
        <li>Fiber dizilim açılarının kritik burkulma yüküne etkisi</li>
        <li>FEM analizi ve analitik doğrulama</li>
      </ul>
    </div>
  </div>
  <div class="card-footer">
    <span class="tech-tag tag-ansys">ANSYS ACP</span>
    <span class="tech-tag tag-ansys">Static Structural</span>
    <span class="tech-tag tag-matlab">MATLAB</span>
  </div>
</div>

<div class="project-card">
  <div class="card-body">
    <span class="card-category">Yazılım Geliştirme</span>
    <h3 class="card-title">Mohr Çemberi Analiz Aracı</h3>
    <div class="card-desc">
      <ul>
        <li>Otomatik Mohr çemberi çizen GUI</li>
        <li>Asal ve maksimum kayma gerilmesi hesabı</li>
      </ul>
    </div>
  </div>
  <div class="card-footer">
    <span class="tech-tag tag-matlab">MATLAB App Designer</span>
    <span class="tech-tag tag-matlab">GUI</span>
  </div>
</div>

<div class="project-card">
  <div class="card-body">
    <span class="card-category">TÜBİTAK 2209-A</span>
    <h3 class="card-title">Özel Asansör Tasarımı (VİSA SÖR)</h3>
    <div class="card-desc">
      <ul>
        <li>Takım liderliği ve proje yönetimi</li>
        <li>Mekanik boyutlandırma ve güvenlik optimizasyonu</li>
      </ul>
    </div>
  </div>
  <div class="card-footer">
    <span class="tech-tag tag-solid">SolidWorks</span>
    <span class="tech-tag tag-ansys">Mekanik Analiz</span>
  </div>
</div>

<div class="project-card">
  <div class="card-body">
    <span class="card-category">Bitirme Tezi</span>
    <h3 class="card-title">Francis Tipi Türbin Tasarımı</h3>
    <div class="card-desc">
      <ul>
        <li>Keban Barajı verileriyle hidrodinamik tasarım</li>
        <li>Çark ve salyangoz geometrisi</li>
      </ul>
    </div>
  </div>
  <div class="card-footer">
    <span class="tech-tag tag-solid">SolidWorks</span>
    <span class="tech-tag">CFD</span>
  </div>
</div>

<div class="project-card">
  <div class="card-body">
    <span class="card-category">Teknik Çeviri</span>
    <h3 class="card-title">CFD & Kavitasyon Teknik Çeviri</h3>
    <div class="card-desc">
      Vanalarda iki fazlı akış ve kavitasyon literatürü çevirisi
    </div>
  </div>
  <div class="card-footer">
    <span class="tech-tag">Akademik İngilizce</span>
    <span class="tech-tag">CFD</span>
  </div>
</div>

<div class="project-card">
  <div class="card-body">
    <span class="card-category">Gönüllü Proje</span>
    <h3 class="card-title">Müsilaj Sorunu Araştırması</h3>
    <div class="card-desc">
      Akışkanlar mekaniği temelli çevresel çözüm çalışması
    </div>
  </div>
  <div class="card-footer">
    <span class="tech-tag">Akışkanlar Mekaniği</span>
    <span class="tech-tag">Çevre</span>
  </div>
</div>

</div>

<h2 class="section-title">3D Tasarım & Render Galerisi</h2>
<div class="gallery-grid">

<div class="gallery-item">
  <div class="gallery-img-box">
    <img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg">
  </div>
  <div class="card-body">
    <h3 class="card-title">Konsept Uçak Tasarımı</h3>
    <div class="card-desc">Özgün konsept ve render</div>
  </div>
</div>

<div class="gallery-item">
  <div class="gallery-img-box">
    <img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg">
  </div>
  <div class="card-body">
    <h3 class="card-title">M16 Piyade Tüfeği</h3>
    <div class="card-desc">Detaylı montaj modeli</div>
  </div>
</div>

<div class="gallery-item">
  <div class="gallery-img-box">
    <img src="https://emir3d.github.io/muhendislik-cv/images/superman.png">
  </div>
  <div class="card-body">
    <h3 class="card-title">3D Superman Logosu</h3>
  </div>
</div>

<div class="gallery-item">
  <div class="gallery-img-box">
    <img src="https://emir3d.github.io/muhendislik-cv/images/jet.png">
  </div>
  <div class="card-body">
    <h3 class="card-title">Turbo Jet Motoru</h3>
  </div>
</div>

</div>
