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
  /* İç sayfa düzeni */
  .author__avatar, .sidebar { display: none !important; }
  .page__content { width: 100% !important; padding-right: 0 !important; }
  
  /* Özel Tablo Tasarımı */
  table { width: 100%; border-collapse: collapse; margin: 25px 0; font-size: 0.95rem; box-shadow: 0 0 20px rgba(0, 0, 0, 0.05); }
  th { background-color: #2563eb; color: #ffffff; text-align: left; padding: 12px 15px; }
  td { padding: 12px 15px; border-bottom: 1px solid #dddddd; }
  tr:nth-of-type(even) { background-color: #f3f4f6; }
  tr:last-of-type { border-bottom: 2px solid #2563eb; }
</style>

Mühendislik analizlerinde kullanılan kiriş teorileri, problemin fiziğini ne kadar doğru modelledikleriyle ayrışır. Aşağıda temel varsayımlar ve seçim kriterleri karşılaştırılmıştır.

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

<br>
<div style="background:#f8fafc; border-left:5px solid #2563eb; padding:20px; font-size:1.2rem; color:#1e293b; border-radius:4px;">
<strong><em>“Euler görmez, Timoshenko tahmin eder, HSDT gerçekten görür.”</em></strong>
<strong><em>“Kaynak: Reddy, 2004.”</em></strong>
</div>
