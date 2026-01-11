---
permalink: /engineering-notes/
title: "Mühendislik Notları"
excerpt: "Akışkanlar dinamiği, yapısal analiz ve kodlama üzerine teknik notlar."
author_profile: true
layout: archive
---

<style>
/* =========================================
   MÜHENDİSLİK NOTLARI - ÖZEL TASARIM
   ========================================= */

/* Sayfa Genişliği */
.page__content { width: 100% !important; max-width: 100% !important; padding-right: 0 !important; }

/* 1. ÜST BİLGİ ALANI (Search & Intro) */
.notes-header {
  background: #f8fafc;
  border: 1px solid #e2e8f0;
  border-radius: 12px;
  padding: 30px;
  margin-bottom: 40px;
  text-align: center;
}

.notes-header h2 {
  margin-top: 0;
  color: #1e293b;
  font-size: 1.5rem;
}

.notes-header p {
  color: #64748b;
  max-width: 600px;
  margin: 10px auto 0;
}

/* 2. NOT KARTLARI (Grid Yapısı) */
.notes-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); /* Responsive */
  gap: 25px;
}

/* Kart Tasarımı */
.note-card {
  background: #ffffff;
  border: 1px solid #e2e8f0;
  border-radius: 12px;
  overflow: hidden;
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  position: relative;
  height: 100%; /* Kartlar eşit boyda olsun */
}

/* Kart Linki (Tıklanabilir Alan) */
.note-link {
  text-decoration: none !important;
  color: inherit !important;
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  padding: 25px;
}

/* Hover Efekti */
.note-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 15px 30px rgba(0,0,0,0.08);
  border-color: #3b82f6; /* Mavi Çerçeve */
}

/* Kart İçeriği */
.note-meta {
  font-size: 0.8rem;
  color: #94a3b8;
  margin-bottom: 10px;
  display: flex;
  align-items: center;
  gap: 10px;
}

.note-date::before {
  content: "📅 ";
}

.note-title {
  font-size: 1.25rem;
  font-weight: 800;
  color: #1e293b;
  margin: 0 0 10px 0;
  line-height: 1.4;
}

.note-excerpt {
  font-size: 0.95rem;
  color: #475569;
  line-height: 1.6;
  flex-grow: 1; /* Metni uzat */
}

/* Etiketler (Alt Kısım) */
.note-footer {
  padding: 15px 25px;
  background: #f8fafc;
  border-top: 1px solid #e2e8f0;
  display: flex;
  flex-wrap: wrap;
  gap: 8px;
}

.note-tag {
  background: #e0f2fe;
  color: #0284c7;
  font-size: 0.75rem;
  padding: 4px 10px;
  border-radius: 4px;
  font-weight: 600;
}

/* "Yeni" Rozeti */
.badge-new {
  position: absolute;
  top: 15px; right: 15px;
  background: #ef4444;
  color: #fff;
  font-size: 0.7rem;
  padding: 3px 8px;
  border-radius: 50px;
  font-weight: bold;
}

/* Koyu Mod Desteği */
@media (prefers-color-scheme: dark) {
  .notes-header { background: #1e293b; border-color: #334155; }
  .notes-header h2 { color: #f1f5f9; }
  .notes-header p { color: #cbd5e1; }
  
  .note-card { background: #1e293b; border-color: #334155; }
  .note-title { color: #f1f5f9; }
  .note-excerpt { color: #cbd5e1; }
  
  .note-footer { background: #0f172a; border-color: #334155; }
  .note-tag { background: #172554; color: #7dd3fc; }
}
</style>

<div class="notes-header">
  <h2>Teknik Dokümantasyon & Ar-Ge Günlüğü</h2>
  <p>Mühendislik problemlerine dair araştırmalarım, çözdüğüm algoritmalar ve teorik notlarımın derlemesi.</p>
</div>

<div class="notes-grid">
  {% for post in site.posts %}
    <article class="note-card">
      {% if forloop.first %}
        <span class="badge-new">YENİ</span>
      {% endif %}

      <a href="{{ post.url }}" class="note-link">
        <div class="note-meta">
          <span class="note-date">{{ post.date | date: "%d.%m.%Y" }}</span>
        </div>
        
        <h3 class="note-title">{{ post.title }}</h3>
        
        <div class="note-excerpt">
          {{ post.excerpt | strip_html | truncate: 120 }}
        </div>
      </a>

      <div class="note-footer">
        {% if post.tags.size > 0 %}
          {% for tag in post.tags limit:3 %}
            <span class="note-tag">#{{ tag }}</span>
          {% endfor %}
        {% else %}
           <span class="note-tag">#Mühendislik</span>
        {% endif %}
      </div>
    </article>
  {% endfor %}
</div>

{% if site.posts.size == 0 %}
  <div style="text-align:center; padding:50px; color:#64748b; border:2px dashed #e2e8f0; border-radius:12px;">
    <h3>Henüz not eklenmemiş.</h3>
    <p>Yakında buraya CFD, FEA ve Python üzerine teknik makaleler eklenecek.</p>
  </div>
{% endif %}
