---
permalink: /
title: "Mühendisliğe Analitik ve Bütüncül Bir Bakış"
excerpt: "Analiz, modelleme ve doğrulama temelli mühendislik yaklaşımı"
author_profile: false
header:
  overlay_image: https://emir3d.github.io/muhendislik-cv/images/header_bg.png
  overlay_filter: 0.65
---

<style>
/* =========================================
   1. GENEL DÜZEN AYARLARI
   ========================================= */

/* Manifesto Yazısı (Ortalanmış, İtalik) */
.manifesto {
  text-align: center;
  font-size: 1.2rem;
  font-style: italic;
  margin: 2rem 0;
  opacity: 0.9;
  line-height: 1.6;
}

/* Ayraç Çizgisi */
hr.spacer {
  margin: 3rem 0;
  border: 0;
  border-top: 1px solid rgba(128, 128, 128, 0.3);
}

/* =========================================
   2. SÜREÇ KUTULARI (Blue Cards Tasarımı)
   ========================================= */
.process-wrapper {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 2rem 0;
}

.process-box {
  flex: 1;
  min-width: 220px;
  background-color: #1e293b; /* Koyu Lacivert Arka Plan */
  color: #ffffff; /* Beyaz Yazı */
  padding: 2rem 1.5rem;
  border-radius: 12px; /* Yuvarlak Köşeler */
  text-align: center; /* Ortalanmış Yazı */
  box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  border: 1px solid #334155;
  transition: transform 0.3s ease;
}

.process-box:hover {
  transform: translateY(-5px); /* Hoverda hafif kalksın */
}

/* Mavi Numara Dairesi */
.p-circle {
  background-color: #3b82f6; /* Parlak Mavi */
  color: white;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: bold;
  font-size: 1.1rem;
  margin: 0 auto 15px; /* Ortala ve alt boşluk ver */
  box-shadow: 0 0 10px rgba(59, 130, 246, 0.5);
}

.step-title {
  font-weight: 800;
  font-size: 1.1rem;
  margin-bottom: 0.8rem;
  display: block;
  color: #fff;
}

.step-desc {
  font-size: 0.9rem;
  color: #cbd5e1; /* Hafif gri metin */
  line-height: 1.5;
}

/* =========================================
   3. ALINTI KUTULARI (Dark Quote Cards)
   ========================================= */
.quote-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}

.quote-item {
  flex: 1;
  min-width: 250px;
  background-color: #172033; /* Çok Koyu Lacivert */
  padding: 1.5rem;
  border-radius: 8px;
  border: 1px solid #334155;
  color: #e2e8f0;
  font-family: "Georgia", serif; /* Tırnaklı font (Daha şık) */
  font-style: italic;
  font-size: 1rem;
  line-height: 1.6;
}

.q-author {
  display: block;
  margin-top: 15px;
  font-family: sans-serif; /* İsim düz font olsun */
  font-style: normal;
  font-weight: 700;
  color: #38bdf8; /* Açık Mavi İsim Rengi */
  text-transform: uppercase;
  font-size: 0.85rem;
  letter-spacing: 1px;
}
</style>

<div class="manifesto">
“Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir.”
</div>

Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; **analiz, modelleme, doğrulama ve üretilebilirlik** ekseninde ele alan bütüncül bir yaklaşım sunuyorum.

Çalışmalarımda temel amaç; mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.

<hr class="spacer">

## Analiz Tabanlı Mühendislik Yaklaşımı

Modern mühendislik problemleri, yalnızca deneysel yöntemlerle ya da tek boyutlu tasarım anlayışıyla sürdürülebilir biçimde çözülemez. Bu nedenle tasarım süreçlerini; **yapısal analiz, sayısal modelleme ve optimizasyon** adımlarıyla desteklenen analitik bir çerçevede ele alıyorum.

<div class="process-wrapper">
  <div class="process-box">
    <div class="p-circle">1</div>
    <span class="step-title">Problem Tanımı</span>
    <div class="step-desc">Problemin sahadaki gerçekliğinin ve fiziksel sınır şartlarının doğru belirlenmesi.</div>
  </div>
  
  <div class="process-box">
    <div class="p-circle">2</div>
    <span class="step-title">Matematiksel Model</span>
    <div class="step-desc">Geometrinin temizlenmesi, uygun ağ (mesh) yapısı ve sayısal kurulum.</div>
  </div>
  
  <div class="process-box">
    <div class="p-circle">3</div>
    <span class="step-title">Analiz & Doğrulama</span>
    <div class="step-desc">Çözümün yakınsaması, mesh bağımsızlığı ve parametrik incelemeler.</div>
  </div>
  
  <div class="process-box">
    <div class="p-circle">4</div>
    <span class="step-title">Mühendislik Yorumu</span>
    <div class="step-desc">Sonuçların yorumlanması ve üretilebilir tasarım kararlarının alınması.</div>
  </div>
</div>

Bu yaklaşım, sistem davranışını daha tasarım aşamasında öngörebilmeyi, kritik sınır koşullarını doğru şekilde tanımlamayı ve mühendislik kararlarını nicel verilere dayandırmayı mümkün kılar.

<hr class="spacer">

## Sanal Doğrulama ve Sayısal Düşünme

Fiziksel testler mühendislikte vazgeçilmezdir; ancak doğru kurulan sayısal modeller, tasarım güvenilirliğini artırırken zaman ve maliyet açısından önemli avantajlar sağlar.

Bu bağlamda, **Sanal Doğrulama (Virtual Verification)** süreçlerini merkeze alarak, tasarımın fiziksel davranışla tutarlı olmasını hedefliyorum.

<hr class="spacer">

## Tasarım, Davranış ve Üretilebilirlik İlişkisi

Bir mühendislik çözümünün başarısı, yalnızca teorik doğruluğuyla değil; üretim süreçleriyle olan uyumuyla da belirlenir. Bu nedenle tasarım, analiz ve üretim arasındaki ilişkiyi birbirinden kopuk adımlar olarak değil, tek bir mühendislik sürecinin parçaları olarak değerlendiriyorum.

<hr class="spacer">

## Mühendislik Vizyonu

Mühendisliği; fiziksel gerçekliği anlamaya çalışan, sayısal araçları bilinçli kullanan ve her çözümü sorgulanabilir kılan bir düşünce disiplini olarak görüyorum.

<div class="quote-grid">
  <div class="quote-item">
    “Engineering is the art of directing the great sources of power in nature for the use and convenience of man.”
    <span class="q-author">— Thomas Tredgold</span>
  </div>

  <div class="quote-item">
    “Mechanics is the paradise of the mathematical sciences, because by means of it one comes to the fruits of mathematics."
    <span class="q-author">— Leonardo da Vinci</span>
  </div>

  <div class="quote-item">
    “Science can amuse and fascinate us all, but it is engineering that changes the world.”
    <span class="q-author">— Isaac Asimov</span>
  </div>
</div>
