---
permalink: /
title: "Mühendisliğe Analitik ve Bütüncül Bir Bakış"
excerpt: "Mekanik tasarım, analiz ve doğrulama odaklı mühendislik çalışmaları"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
header:
  overlay_image: https://emir3d.github.io/muhendislik-cv/images/header_bg.png
  overlay_filter: 0.7
---

<style>
/* 1. GLOBAL RESET (Yazı Boyutlarını Eşitleme) */
.custom-page-wrapper {
  font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
  font-size: 16px !important; /* Temel yazı boyutu sabitlendi */
  line-height: 1.6 !important;
  color: #333 !important;
}
.custom-page-wrapper h3 {
  font-size: 1.5em !important;
  margin-top: 2em !important;
  margin-bottom: 1em !important;
  font-weight: 700 !important;
  color: #222 !important;
  border-bottom: none !important; /* Temanın çizgisini kaldır */
}

/* 2. MANİFESTO KUTUSU */
.manifesto-box {
  background-color: #f8f9fa;
  border-left: 4px solid #333;
  padding: 20px;
  margin-bottom: 30px;
  font-style: italic;
  font-size: 1.1em !important;
  color: #444 !important;
}

/* 3. AKIŞ ŞEMASI (PROCESS FLOW) - ZIRHLI TASARIM */
.process-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 40px 0;
  justify-content: space-between;
}

.process-card {
  flex: 1;
  min-width: 200px;
  background-color: #ffffff !important; /* ZORLA BEYAZ */
  border: 1px solid #e0e0e0 !important;
  border-radius: 8px;
  padding: 25px;
  position: relative;
  box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  transition: transform 0.2s;
  /* Yazı rengini zorla siyah yap */
  color: #222 !important; 
}
.process-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 8px 15px rgba(0,0,0,0.1);
}

/* RENK GEÇİŞİ (SOL KENARLIKLAR - TONAL HARMONY) */
.step-1 { border-left: 6px solid #0f172a !important; } /* En Koyu Lacivert */
.step-2 { border-left: 6px solid #1e40af !important; } /* Koyu Mavi */
.step-3 { border-left: 6px solid #3b82f6 !important; } /* Açık Mavi */
.step-4 { border-left: 6px solid #60a5fa !important; } /* En Açık Mavi */

/* Kart İçindeki Yazılar */
.step-num {
  font-size: 2em !important;
  font-weight: 900;
  opacity: 0.15;
  position: absolute;
  top: 10px;
  right: 15px;
  line-height: 1;
}
/* Numara renkleri de çizgiyle aynı olsun */
.step-1 .step-num { color: #0f172a !important; }
.step-2 .step-num { color: #1e40af !important; }
.step-3 .step-num { color: #3b82f6 !important; }
.step-4 .step-num { color: #60a5fa !important; }

.step-title {
  font-size: 1.1em !important;
  font-weight: 700 !important;
  margin-bottom: 10px;
  display: block;
  color: #000 !important; /* Başlık simsiyah */
}
.step-desc {
  font-size: 0.95em !important;
  color: #555 !important; /* Açıklama koyu gri */
  margin: 0 !important;
}

/* 4. OK İŞARETİ */
.arrow-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 1.5em;
  color: #bbb;
}

/* 5. ZARİF AYRAÇ */
.custom-divider {
  width: 100%;
  height: 1px;
  background-color: #ddd !important;
  margin: 50px 0;
}

/* 6. VİZYON KARTLARI */
.vision-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
.vision-item {
  flex: 1;
  min-width: 250px;
  background: #f9f9f9 !important;
  padding: 20px;
  border-radius: 6px;
  border: 1px solid #eee;
}
.quote-text { font-style: italic; color: #555 !important; font-size: 0.95em !important; }
.quote-author { text-align: right; font-weight: bold; font-size: 0.9em !important; margin-top: 10px; color: #333 !important; }
.vision-blue { border-top: 3px solid #0f172a; }
.vision-red { border-top: 3px solid #b91c1c; }
.vision-cyan { border-top: 3px solid #0891b2; }


/* =========================================
   🌙 KARANLIK MOD (DARK MODE) ZORLA DÜZELTME
   ========================================= */
@media (prefers-color-scheme: dark) {
  .custom-page-wrapper { color: #e2e8f0 !important; }
  .custom-page-wrapper h3 { color: #ffffff !important; }
  
  /* Manifesto Kutusu */
  .manifesto-box { background-color: #1e293b !important; border-left-color: #94a3b8 !important; color: #e2e8f0 !important; }
  
  /* Kartlar SİYAH DEĞİL, KOYU GRİ OLSUN */
  .process-card { 
    background-color: #1e293b !important; 
    border-color: #334155 !important; 
  }
  .step-title { color: #f8fafc !important; }
  .step-desc { color: #cbd5e1 !important; }
  
  /* Renk geçişlerini koru ama biraz parlat */
  .step-1 { border-left-color: #60a5fa !important; }
  .step-2 { border-left-color: #3b82f6 !important; }
  .step-3 { border-left-color: #2563eb !important; }
  .step-4 { border-left-color: #1d4ed8 !important; }
  
  /* Vizyon Kartları */
  .vision-item { background-color: #1e293b !important; border-color: #334155 !important; }
  .quote-text { color: #cbd5e1 !important; }
  .quote-author { color: #f8fafc !important; }
  
  .custom-divider { background-color: #334155 !important; }
}

/* MOBİL DÜZENLEME */
@media (max-width: 768px) {
  .arrow-icon { display: none; }
  .process-grid { flex-direction: column; }
}
</style>

<div class="custom-page-wrapper">

  <div class="manifesto-box">
    "Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir."
  </div>

  <p>
    Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; <strong>analiz, modelleme, doğrulama ve üretilebilirlik</strong> ekseninde ele alan bütüncül bir yaklaşım sunuyorum.
  </p>
  <p>
    Çalışmalarımda temel amaç; mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.
  </p>

  <div class="custom-divider"></div>

  <h3>Analiz Tabanlı Tasarım Metodolojisi</h3>

  <p>
    Modern mühendislik problemleri, yalnızca deneysel yöntemlerle ya da tek boyutlu tasarım anlayışıyla sürdürülebilir biçimde çözülemez. Bu nedenle tasarım süreçlerini; <strong>yapısal analiz, sayısal modelleme ve optimizasyon</strong> adımlarıyla desteklenen analitik bir çerçevede ele alıyorum.
  </p>

  <div class="process-grid">
    
    <div class="process-card step-1">
      <div class="step-num">01</div>
      <span class="step-title">Fiziksel Tanım</span>
      <p class="step-desc">Problemin sahadaki gerçekliğinin ve sınır şartlarının belirlenmesi.</p>
    </div>

    <div class="arrow-icon">➝</div>

    <div class="process-card step-2">
      <div class="step-num">02</div>
      <span class="step-title">Matematiksel Model</span>
      <p class="step-desc">Geometrinin temizlenmesi, uygun ağ (mesh) yapısı ve sayısal kurulum.</p>
    </div>

    <div class="arrow-icon">➝</div>

    <div class="process-card step-3">
      <div class="step-num">03</div>
      <span class="step-title">Analiz & Doğrulama</span>
      <p class="step-desc">Çözümün yakınsaması, mesh bağımsızlığı ve parametrik incelemeler.</p>
    </div>

    <div class="arrow-icon">➝</div>

    <div class="process-card step-4">
      <div class="step-num">04</div>
      <span class="step-title">Mühendislik Yorumu</span>
      <p class="step-desc">Sonuçların yorumlanması ve üretilebilir tasarım kararlarının alınması.</p>
    </div>

  </div>

  <div class="custom-divider"></div>

  <h3>Sanal Doğrulama ve Sayısal Düşünme</h3>

  <p>
    Fiziksel testler mühendislikte vazgeçilmezdir; ancak doğru kurulan sayısal modeller, tasarım güvenilirliğini artırırken zaman ve maliyet açısından önemli avantajlar sağlar.
  </p>
  <p>
    Bu bağlamda, çalışmalarda <strong>Sanal Doğrulama (Virtual Verification)</strong> süreçlerini merkeze alarak, tasarımın fiziksel davranışla tutarlı olmasını hedefliyorum. Sayısal analizler, yalnızca sonuç üretmek için değil; sistemi anlamak, varsayımları sorgulamak ve model güvenilirliğini değerlendirmek için bir araç olarak ele alınmaktadır.
  </p>

  <h3>Tasarım, Davranış ve Üretilebilirlik İlişkisi</h3>

  <p>
    Bir mühendislik çözümünün başarısı, yalnızca teorik doğruluğuyla değil; üretim süreçleriyle olan uyumuyla da belirlenir.
  </p>
  <p>
    Bu nedenle tasarım, analiz ve üretim arasındaki ilişkiyi birbirinden kopuk adımlar olarak değil, tek bir mühendislik sürecinin parçaları olarak değerlendiriyorum. Bu perspektif, tasarım kararlarının gerçek dünya koşullarında uygulanabilirliğini erken aşamada görmeyi ve olası sorunları öngörmeyi mümkün kılar.
  </p>

  <div class="custom-divider"></div>

  <h3 style="text-align: center;">Mühendislik Vizyonu</h3>
  <p style="text-align: center; margin-bottom: 30px; font-style: italic;">
    "Mühendisliği; fiziksel gerçekliği anlamaya çalışan, sayısal araçları bilinçli kullanan ve her çözümü sorgulanabilir kılan bir düşünce disiplini olarak görüyorum."
  </p>

  <div class="vision-grid">
    <div class="vision-item vision-blue">
      <p class="quote-text">"Engineering is the art of directing the great sources of power in nature for the use and convenience of man."</p>
      <p class="quote-author">— Thomas Tredgold</p>
    </div>
    <div class="vision-item vision-red">
      <p class="quote-text">"Mechanics is the paradise of the mathematical sciences, because by means of it one comes to the fruits of mathematics."</p>
      <p class="quote-author">— Leonardo da Vinci</p>
    </div>
    <div class="vision-item vision-cyan">
      <p class="quote-text">"Science can amuse and fascinate us all, but it is engineering that changes the world."</p>
      <p class="quote-author">— Isaac Asimov</p>
    </div>
  </div>

</div>
