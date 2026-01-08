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
/* ================================================================
   MODERN & TEKNİK TASARIM (MINIMALIST ENGINEERING STYLE)
   ================================================================
*/

/* 1. MANİFESTO VE GİRİŞ METNİ */
.manifesto {
  text-align: center;
  font-size: 1.25rem;
  font-weight: 300; /* Daha ince, zarif font */
  font-style: italic;
  margin: 2rem 0;
  opacity: 0.9;
  line-height: 1.6;
}

/* 2. MODERN ARA ÇİZGİ (HAYALET ÇİZGİ) 
   Ortası hafif gri, kenarları yok olan modern ayraç
*/
hr.modern-split {
  border: 0;
  height: 1px;
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0));
  margin: 4rem 0;
}

/* 3. BAŞLIK TASARIMI (Technical Header) 
   Altına ince boydan boya çizgi + Sol tarafta renkli vurgu
*/
h2 {
  position: relative;
  padding-bottom: 10px;
  border-bottom: 1px solid rgba(128, 128, 128, 0.2); /* Boydan boya ince çizgi */
  margin-top: 3rem;
  font-weight: 600;
}
/* Başlığın altındaki kısa renkli çizgi (Modern Dokunuş) */
h2::after {
  content: "";
  position: absolute;
  bottom: -1px; /* Çizginin tam üstüne oturur */
  left: 0;
  width: 60px; /* Kısa çizgi */
  height: 3px;
  background-color: #2563eb; /* Mavi vurgu */
}

/* 4. SÜREÇ KUTULARI (COMPACT GRID) */
.process-wrapper {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
  margin: 2.5rem 0;
}

.process-box {
  flex: 1;
  min-width: 220px;
  padding: 1.2rem; /* Daha kompakt */
  border: 1px solid rgba(128, 128, 128, 0.2); /* Çok ince çerçeve */
  border-radius: 6px;
  background: rgba(128, 128, 128, 0.02); /* Çok hafif zemin */
}

/* Sol taraftaki renkli çizgiler (Düz ve Net) */
.step-1 { border-left: 4px solid #0f172a; }
.step-2 { border-left: 4px solid #1e40af; }
.step-3 { border-left: 4px solid #3b82f6; }
.step-4 { border-left: 4px solid #60a5fa; }

.step-title {
  display: block;
  font-weight: 700;
  font-size: 1rem;
  margin-bottom: 0.5rem;
  color: inherit; /* Temanın rengine uy */
}

/* 5. VİZYON KARTLARI (GRID) */
.quote-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
.quote-item {
  flex: 1;
  min-width: 250px;
  padding: 1.5rem;
  border: 1px solid rgba(128, 128, 128, 0.15);
  border-left-width: 4px; /* Sadece sol çizgi kalın */
  border-radius: 4px;
  background: rgba(128, 128, 128, 0.04);
}
.q-blue { border-left-color: #1e40af; }
.q-red { border-left-color: #c0392b; }
.q-cyan { border-left-color: #0891b2; }

/* DARK MODE AYARLARI (OTOMATİK GEÇİŞ)
   Karanlık modda çizgileri beyaza çevirir
*/
@media (prefers-color-scheme: dark) {
  hr.modern-split {
    background-image: linear-gradient(to right, rgba(0, 0, 0, 0), rgba(255, 255, 255, 0.3), rgba(0, 0, 0, 0));
  }
  h2 { border-bottom-color: rgba(255, 255, 255, 0.2); }
  .process-box { border-color: rgba(255, 255, 255, 0.1); background: rgba(255, 255, 255, 0.02); }
  .quote-item { border-color: rgba(255, 255, 255, 0.1); border-left-width: 4px; background: rgba(255, 255, 255, 0.02); }
}
</style>

<div class="manifesto">
“Mühendislik, yalnızca bir bileşeni tasarlamak değil; o bileşenin fiziksel dünyadaki davranışını öngörebilme, sınırlarını anlayabilme ve bu davranışı güvenilir biçimde doğrulayabilme disiplinidir.”
</div>

Bu platformda, mühendisliği geometri odaklı bir faaliyet olarak değil; **analiz, modelleme, doğrulama ve üretilebilirlik** ekseninde ele alan bütüncül bir yaklaşım sunuyorum.

Çalışmalarımda temel amaç; mühendislik problemlerini sezgisel çözümlerden bağımsız olarak, fiziksel prensiplere dayalı ve sayısal olarak doğrulanabilir yöntemlerle değerlendirmektir.

<hr class="modern-split">

## Analiz Tabanlı Mühendislik Yaklaşımı

Modern mühendislik problemleri, yalnızca deneysel yöntemlerle ya da tek boyutlu tasarım anlayışıyla sürdürülebilir biçimde çözülemez. Bu nedenle tasarım süreçlerini; **yapısal analiz, sayısal modelleme ve optimizasyon** adımlarıyla desteklenen analitik bir çerçevede ele alıyorum.

<div class="process-wrapper">
  <div class="process-box step-1">
    <span class="step-title">1. Problem Tanımı</span>
    Problemin sahadaki gerçekliğinin ve sınır şartlarının belirlenmesi.
  </div>
  
  <div class="process-box step-2">
    <span class="step-title">2. Matematiksel Model</span>
    Geometrinin temizlenmesi, uygun ağ (mesh) yapısı ve sayısal kurulum.
  </div>
  
  <div class="process-box step-3">
    <span class="step-title">3. Analiz & Doğrulama</span>
    Çözümün yakınsaması, mesh bağımsızlığı ve parametrik incelemeler.
  </div>
  
  <div class="process-box step-4">
    <span class="step-title">4. Mühendislik Yorumu</span>
    Sonuçların yorumlanması ve üretilebilir tasarım kararlarının alınması.
  </div>
</div>

Bu yaklaşım, sistem davranışını daha tasarım aşamasında öngörebilmeyi, kritik sınır koşullarını doğru şekilde tanımlamayı ve mühendislik kararlarını nicel verilere dayandırmayı mümkün kılar.

<hr class="modern-split">

## Sanal Doğrulama ve Sayısal Düşünme

Fiziksel testler mühendislikte vazgeçilmezdir; ancak doğru kurulan sayısal modeller, tasarım güvenilirliğini artırırken zaman ve maliyet açısından önemli avantajlar sağlar.

Bu bağlamda, **Sanal Doğrulama (Virtual Verification)** süreçlerini merkeze alarak, tasarımın fiziksel davranışla tutarlı olmasını hedefliyorum.

<hr class="modern-split">

## Tasarım, Davranış ve Üretilebilirlik İlişkisi

Bir mühendislik çözümünün başarısı, yalnızca teorik doğruluğuyla değil; üretim süreçleriyle olan uyumuyla da belirlenir. Bu nedenle tasarım, analiz ve üretim arasındaki ilişkiyi birbirinden kopuk adımlar olarak değil, tek bir mühendislik sürecinin parçaları olarak değerlendiriyorum.

<hr class="modern-split">

## Mühendislik Vizyonu

Mühendisliği; fiziksel gerçekliği anlamaya çalışan, sayısal araçları bilinçli kullanan ve her çözümü sorgulanabilir kılan bir düşünce disiplini olarak görüyorum.

<div class="quote-grid">
  <div class="quote-item q-blue">
    <i>“Engineering is the art of directing the great sources of power in nature for the use and convenience of man.”</i>
    <br><br><b>— Thomas Tredgold</b>
  </div>

  <div class="quote-item q-red">
    <i>“Mechanics is the paradise of the mathematical sciences, because by means of it one comes to the fruits of mathematics."</i>
    <br><br><b>— Leonardo da Vinci</b>
  </div>

  <div class="quote-item q-cyan">
    <i>“Science can amuse and fascinate us all, but it is engineering that changes the world.”</i>
    <br><br><b>— Isaac Asimov</b>
  </div>
</div>
