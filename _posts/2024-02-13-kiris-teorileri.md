---
title: "Kiriş Teorileri Karşılaştırması: Euler vs. Timoshenko vs. HSDT"
date: 2024-02-13
tags: [Mekanik, Teorik, FEA, Kompozit]
excerpt: "Kiriş analizlerinde doğru teoriyi seçmek hayati önem taşır. Euler-Bernoulli, Timoshenko ve HSDT arasındaki temel farklar ve L/h oranına göre seçim kriterleri."
header:
  overlay_color: "#1e293b"
sidebar:
  nav: false
---

<style>
  /* 1. SAYFA DÜZENİ */
  .author__avatar, .sidebar { display: none !important; }
  .page__content { width: 100% !important; padding-right: 0 !important; }
  
  /* 2. TABLO TASARIMI (Responsive & Modern) */
  table {
    width: 100%;
    border-collapse: collapse;
    margin: 30px 0;
    font-size: 0.95rem;
    border-radius: 8px;
    overflow: hidden; /* Köşeleri yuvarlatır */
    box-shadow: 0 4px 6px rgba(0,0,0,0.05);
  }

  /* AYDINLIK MOD (Varsayılan) */
  th {
    background-color: #f1f5f9; /* Çok açık gri */
    color: #0f172a; /* Koyu lacivert yazı */
    font-weight: 800;
    text-transform: uppercase;
    font-size: 0.85rem;
    letter-spacing: 0.5px;
    padding: 15px;
    text-align: left;
    border-bottom: 2px solid #e2e8f0;
  }
  
  td {
    padding: 15px;
    border-bottom: 1px solid #e2e8f0;
    color: #334155;
  }
  
  /* Satır Arası Renklendirme (Zebra) */
  tr:nth-child(even) { background-color: #f8fafc; }
  tr:hover { background-color: #e2e8f0; transition: 0.2s; }

  /* 3. KOYU MOD (DARK MODE UYUMU) */
  @media (prefers-color-scheme: dark) {
    table { box-shadow: none; border: 1px solid #334155; }
    
    th {
      background-color: #1e293b; /* Koyu arka plan */
      color: #f1f5f9; /* Beyaz yazı */
      border-bottom: 2px solid #334155;
    }
    
    td {
      border-bottom: 1px solid #334155;
      color: #cbd5e1; /* Açık gri yazı */
    }
    
    tr:nth-child(even) { background-color: #0f172a; } /* Daha koyu satır */
    tr:hover { background-color: #334155; }
  }

  /* 4. SLOGAN KUTUSU */
  .slogan-box {
    padding: 20px;
    border-left: 5px solid #3b82f6;
    background-color: #f8fafc;
    color: #1e293b;
    font-size: 1.1rem;
    margin-top: 40px;
    border-radius: 4px;
  }
  
  /* Slogan Kutusu Koyu Mod */
  @media (prefers-color-scheme: dark) {
    .slogan-box {
      background-color: #1e293b;
      color: #e2e8f0;
      border-left-color: #60a5fa;
    }
  }
</style>

Kiriş teorileri arasındaki temel fark, yapının fiziksel davranışını ne ölçüde doğru temsil edebildikleridir. Bu bölümde, yaygın olarak kullanılan yaklaşımların varsayımları ve mühendislik açısından seçim kriterleri karşılaştırmalı olarak ele alınmıştır.

## Temel Varsayımlar

### 1. Euler-Bernoulli Teorisi
* Kesitler deformasyon sonrasında da **düz kalır**.
* Kesitler deformasyon sonrasında da **tarafsız eksene dik kalır**.
* **Kayma deformasyonu (Shear Deformation) YOKTUR.**
* Küçük şekil değiştirmeler için geçerlidir.

### 2. Timoshenko Teorisi
* Kesitler deformasyon sonrasında **düz kalır**.
* Ancak kesitler, **tarafsız eksene dik kalmak zorunda değildir.**
* **Kayma deformasyonu VARDIR.**
* Kesit boyunca sabit bir kayma dağılımı varsayar (Düzeltme katsayısı gerekir).

---

## L/h Oranlarına Göre Seçim Kriterleri

Uzunluk (L) ve Kalınlık (h) oranı, hangi teorinin kullanılması gerektiğini belirleyen en önemli faktördür.

| L/h Oranı | Kiriş Tipi | Uygun Teori | Sonuç Durumu |
| :--- | :--- | :--- | :--- |
| **> 20-25** | İnce Kiriş | **Euler Yeterli** | Euler ≈ Timoshenko ≈ HSDT |
| **10 - 20** | Orta Kalınlık | **Timoshenko** | Kayma etkileri başlar |
| **< 10** | Kalın Kiriş | **HSDT / 3D** | HSDT en gerçekçi sonucu verir |

### Kritik Karşılaştırma:
* **L/h > 20 olduğunda:** Euler, Timoshenko ve HSDT sonuçları birbirine çok yakındır. Basit olduğu için Euler tercih edilebilir.
* **L/h < 10 olduğunda:**
    * Euler: Aşırı rijit davranır, kritik burkulma yükünü **yüksek (hatalı)** verir.
    * Timoshenko: Kaymayı hesaba kattığı için Euler'den **daha düşük** sonuç verir.
    * HSDT: Kesit çarpılmasını modellediği için **en gerçekçi** sonucu verir.

---

## Teorilerin Özeti

* **Euler–Bernoulli:** *"Kaymayı yok sayar."* İnce elemanlarda hızlı sonuç verir ancak kalın kirişlerde iyimser (olması gerekenden yüksek) burkulma tahmini yapar.

* **Timoshenko:** *"Kaymayı düzeltir."* Kayma deformasyonunu bir katsayı ile hesaba katar. Orta kalınlıktaki kirişlerde güvenilirdir.

* **HSDT (Higher Order Shear Deformation Theory):** *"Kaymayı gerçekten modeller."* Kayma gerilmesini kesit boyunca parabolik (doğal) dağılımıyla yakalar. Kalın ve özellikle **hibrit kompozit** yapılar için en doğru sonuçları verir.

* **Kaynak:** Reddy,2004 

<div class="slogan-box">
  <strong><em>“Euler görmez, Timoshenko tahmin eder, HSDT gerçekten görür.”</em></strong>
</div>
