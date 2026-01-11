---
permalink: /
title: ""
excerpt: "Makine Mühendisi - Simülasyon & Tasarım"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
/* ==============================
   ANA SAYFA "WOW" TASARIMI
   ============================== */
.page__content { width: 100% !important; max-width: 100% !important; padding: 0 !important; }
.author__avatar { display: none !important; }

/* 1. HERO BÖLÜMÜ (Devasa Arka Planlı Giriş) */
.hero-banner {
  position: relative;
  /* Arka plana senin manifold görselini koyuyoruz, üzerine koyu filtre atıyoruz */
  background: linear-gradient(rgba(15, 23, 42, 0.85), rgba(15, 23, 42, 0.9)), url('https://emir3d.github.io/muhendislik-cv/images/manifold.jpg');
  background-size: cover;
  background-position: center;
  background-attachment: fixed; /* Parallax efekti */
  padding: 100px 20px;
  text-align: center;
  color: #fff;
  border-bottom: 4px solid #2563eb;
  margin-bottom: 50px;
}

.hero-main-title {
  font-size: 3rem;
  font-weight: 900;
  letter-spacing: -1px;
  margin-bottom: 15px;
  text-shadow: 0 4px 10px rgba(0,0,0,0.5);
}

.hero-subtitle {
  font-size: 1.25rem;
  font-weight: 300;
  color: #94a3b8; /* Hafif gri */
  max-width: 800px;
  margin: 0 auto 30px;
  line-height: 1.6;
}

.hero-highlight {
  color: #38bdf8; /* Neon Mavi */
  font-weight: 700;
}

.btn-hero {
  display: inline-block;
  padding: 15px 40px;
  background: #2563eb;
  color: #fff !important;
  text-decoration: none !important;
  border-radius: 50px;
  font-weight: 700;
  font-size: 1rem;
  transition: all 0.3s ease;
  box-shadow: 0 0 20px rgba(37, 99, 235, 0.4);
}
.btn-hero:hover {
  transform: translateY(-5px);
  background: #fff;
  color: #2563eb !important;
  box-shadow: 0 0 30px rgba(255, 255, 255, 0.4);
}

/* 2. MANİFESTO KUTUSU */
.manifesto-box {
  max-width: 900px;
  margin: -80px auto 60px; /* Hero'nun içine girsin */
  background: #fff;
  padding: 40px;
  border-radius: 12px;
  box-shadow: 0 20px 50px rgba(0,0,0,0.1);
  position: relative;
  z-index: 10;
  text-align: center;
  border-top: 5px solid #2563eb;
}

.manifesto-text {
  font-size: 1.1rem;
  color: #334155;
  font-style: italic;
  line-height: 1.8;
  font-weight: 500;
}

/* 3. SÜREÇ KARTLARI (Process Flow) */
.section-header {
  text-align: center;
  font-size: 2rem;
  font-weight: 800;
  margin-bottom: 40px;
  color: #0f172a;
}

.process-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
  gap: 30px;
  max-width: 1100px;
  margin: 0 auto 80px;
  padding: 0 20px;
}

.process-card {
  background: #f8fafc;
  border: 1px solid #e2e8f0;
  border-radius: 16px;
  padding: 30px 20px;
  text-align: center;
  transition: 0.3s;
  position: relative;
}

.process-card:hover {
  transform: translateY(-10px);
  background: #fff;
  box-shadow: 0 20px 40px rgba(37, 99, 235, 0.1);
  border-color: #2563eb;
}

.p-number {
  background: #2563eb;
  color: #fff;
  width: 40px; height: 40px;
  border-radius: 50%;
  display: flex;
  align-items: center; justify-content: center;
  font-weight: 800;
  margin: 0 auto 15px;
  box-shadow: 0 5px 15px rgba(37, 99, 235, 0.3);
}

.p-title {
  font-size: 1.1rem;
  font-weight: 800;
  margin-bottom: 10px;
  color: #1e293b;
}

.p-desc {
  font-size: 0.9rem;
  color: #64748b;
  line-height: 1.5;
}

/* Ok işareti (CSS ile) */
.process-card::after {
  content: "→";
  position: absolute;
  right: -20px;
  top: 50%;
  transform: translateY(-50%);
  font-size: 2rem;
  color: #cbd5e1;
  display: none; /* Mobilde gizle */
}
/* Sadece masaüstünde ve son kart hariç okları göster */
@media(min-width: 1000px) {
  .process-card:not(:last-child)::after { display: block; }
}


/* 4. ALINTI BLOĞU (Quotes) */
.quotes-container {
  background: #0f172a; /* Koyu Lacivert */
  padding: 60px 20px;
  color: #fff;
  text-align: center;
  margin-top: 50px;
}

.quote-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 40px;
  max-width: 1000px;
  margin: 0 auto;
}

.quote-card {
  background: rgba(255,255,255,0.05);
  padding: 30px;
  border-radius: 12px;
  border: 1px solid rgba(255,255,255,0.1);
}

.q-text {
  font-size: 1.1rem;
  font-style: italic;
  margin-bottom: 20px;
  color: #cbd5e1;
  font-family: serif;
}

.q-author {
  font-weight: 700;
  color: #38bdf8;
  text-transform: uppercase;
  font-size: 0.85rem;
  letter-spacing: 1px;
}

/* Koyu Mod Uyumu (Manifesto ve Process Kartları İçin) */
@media (prefers-color-scheme: dark) {
  .manifesto-box { background: #1e293b; color: #fff; border-top-color: #38bdf8; }
  .manifesto-text { color: #e2e8f0; }
  
  .section-header { color: #f1f5f9; }
  
  .process-card { background: #1e293b; border-color: #334155; }
  .process-card:hover { background: #273549; border-color: #38bdf8; }
  .p-title { color: #f1f5f9; }
  .p-desc { color: #94a3b8; }
}
</style>

<div class="hero-banner">
  <h1 class="hero-main-title">Mühendisliğe Analitik Bakış</h1>
  <p class="hero-subtitle">
    Analiz, modelleme ve doğrulama temelli <span class="hero-highlight">Bütüncül Mühendislik Yaklaşımı</span>.<br>
    Veriyi tasarıma, tasarımı gerçeğe dönüştürüyorum.
  </p>
  <a href="/portfolio/" class="btn-hero">Projelerimi Keşfet</a>
</div>

<div class="manifesto-box">
  <p class="manifesto-text">
    "Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir."
  </p>
</div>

<h2 class="section-header">Analiz Tabanlı Yaklaşımım</h2>

<div class="process-grid">

  <div class="process-card">
    <div class="p-number">1</div>
    <div class="p-title">Problem Tanımı</div>
    <div class="p-desc">
      Problemin sahadaki gerçekliğinin ve fiziksel sınır şartlarının doğru belirlenmesi.
    </div>
  </div>

  <div class="process-card">
    <div class="p-number">2</div>
    <div class="p-title">Matematiksel Model</div>
    <div class="p-desc">
      Geometrinin temizlenmesi, uygun ağ (mesh) yapısı ve sayısal kurulum.
    </div>
  </div>

  <div class="process-card">
    <div class="p-number">3</div>
    <div class="p-title">Analiz & Doğrulama</div>
    <div class="p-desc">
      Çözümün yakınsaması, mesh bağımsızlığı ve parametrik incelemeler.
    </div>
  </div>

  <div class="process-card">
    <div class="p-number">4</div>
    <div class="p-title">Mühendislik Yorumu</div>
    <div class="p-desc">
      Sonuçların yorumlanması ve üretilebilir tasarım kararlarının alınması.
    </div>
  </div>

</div>

<div class="quotes-container">
  <h2 class="section-header" style="color:#fff; margin-bottom:10px;">Mühendislik Vizyonu</h2>
  <p style="color:#94a3b8; margin-bottom:50px;">Fiziksel gerçekliği anlamaya çalışan, sorgulanabilir bir düşünce disiplini.</p>

  <div class="quote-grid">
    <div class="quote-card">
      <div class="q-text">
        "Mühendislik, doğadaki büyük güç kaynaklarını insanın kullanımı ve rahatlığı için yönlendirme sanatıdır."
      </div>
      <div class="q-author">— Thomas Tredgold</div>
    </div>

    <div class="quote-card">
      <div class="q-text">
        "Mekanik, matematik bilimlerinin cennetidir, çünkü matematik meyvelerini orada verir."
      </div>
      <div class="q-author">— Leonardo da Vinci</div>
    </div>
    
    <div class="quote-card">
      <div class="q-text">
        "Bilim bizi büyüleyebilir, ama dünyayı değiştiren mühendisliktir."
      </div>
      <div class="q-author">— Isaac Asimov</div>
    </div>
  </div>
</div>
