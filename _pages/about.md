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
/* SADECE DÜZEN (LAYOUT) VE BOYUT AYARLARI 
   Renk kodlarına (metin/arka plan) dokunmuyoruz, site kendi halletsin.
*/

/* Manifesto Yazısı */
.manifesto {
  text-align: center;
  font-size: 1.2rem;
  font-style: italic;
  margin: 2rem 0;
  opacity: 0.9; /* Biraz daha belirgin */
}

/* Süreç Kutuları (Yan Yana Dizme) */
.process-wrapper {
  display: flex;
  flex-wrap: wrap;
  gap: 15px;
  margin: 2rem 0;
}

.process-box {
  flex: 1;
  min-width: 200px;
  /* DÜZELTME 1: Padding azaltıldı, kutular daha kibar */
  padding: 1.2rem; 
  border: 1px solid rgba(128, 128, 128, 0.3);
  border-radius: 8px;
  font-size: 0.95rem; /* Kutu içi yazı bir tık küçüldü */
}

/* Sol taraftaki renkli çizgiler */
.step-1 { border-left: 5px solid #0f172a; }
.step-2 { border-left: 5px solid #1e40af; }
.step-3 { border-left: 5px solid #3b82f6; }
.step-4 { border-left: 5px solid #60a5fa; }

.step-title {
  font-weight: bold;
  /* DÜZELTME 2: Başlık boyutu uyum için ayarlandı */
  font-size: 1.05rem; 
  margin-bottom: 0.5rem;
  display: block;
}

/* Ayraç (Daha Belirgin) */
hr.spacer {
  margin: 3rem 0;
  border: 0;
  /* DÜZELTME 3: Opaklık 0.2'den 0.5'e çıkarıldı (Karanlıkta görünür) */
  border-top: 1px solid rgba(128, 128, 128, 0.5); 
}

/* Alıntılar */
.quote-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 20px;
}
.quote-item {
  flex: 1;
  min-width: 250px;
  padding: 1rem;
  border-left: 4px solid rgba(128, 128, 128, 0.4); /* Çerçeve biraz daha belirgin */
  background: rgba(128, 128, 128, 0.08); /* Arka plan biraz daha belirgin */
  font-size: 0.95rem;
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
    <i>“Engineering is the art of directing the great sources of power in nature for the use and convenience of man.”</i>
    <br><b>— Thomas Tredgold</b>
  </div>

  <div class="quote-item">
    <i>“Mechanics is the paradise of the mathematical sciences, because by means of it one comes to the fruits of mathematics."</i>
    <br><b>— Leonardo da Vinci</b>
  </div>

  <div class="quote-item">
    <i>“Science can amuse and fascinate us all, but it is engineering that changes the world.”</i>
    <br><b>— Isaac Asimov</b>
  </div>
</div>
