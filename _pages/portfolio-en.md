---
permalink: /en/portfolio/
title: "Portfolio & Projects"
excerpt: "Engineering analyses, simulations, and design studies."
author_profile: true
---

<style>
/* 1. Kırık Profil Resmini Gizle */
.author__avatar { display: none !important; }

/* 2. DİL SEÇİCİ */
.lang-switcher { display: flex; justify-content: flex-end; gap: 10px; margin-bottom: 20px; }
.lang-btn { padding: 6px 16px; border: 1px solid #3b82f6; border-radius: 50px; text-decoration: none !important; font-weight: 700; font-size: 0.85rem; transition: all 0.3s ease; color: #3b82f6 !important; }
.lang-btn.active { background-color: #3b82f6; color: #ffffff !important; box-shadow: 0 4px 10px rgba(59, 130, 246, 0.3); }
.lang-btn:hover:not(.active) { background-color: rgba(59, 130, 246, 0.1); }

/* Temel Renkler ve Başlıklar */
:root { --tech-blue: #2563eb; --tech-bg: #ffffff; --tech-border: #e2e8f0; }
.section-title { font-size: 1.8rem; font-weight: 800; margin: 3rem 0 2rem; display: flex; align-items: center; gap: 15px; color: inherit; border-bottom: 2px solid #e5e7eb; padding-bottom: 10px; }

/* PROJE KARTLARI */
.projects-container { display: flex; flex-direction: column; gap: 20px; margin-bottom: 5rem; }
.project-card-link { text-decoration: none !important; color: inherit !important; display: block; }
.project-row { background: #ffffff; border: 1px solid var(--tech-border); border-radius: 12px; padding: 25px; display: flex; justify-content: space-between; align-items: center; transition: transform 0.2s ease, box-shadow 0.2s ease; position: relative; }
@media (prefers-color-scheme: dark) { .project-row { background: #1e293b; border-color: #334155; } .row-title { color: #f1f5f9 !important; } }
.project-row:hover { transform: translateX(10px); border-color: var(--tech-blue); box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1); }
.row-info { display: flex; flex-direction: column; gap: 5px; }
.row-category { font-size: 0.75rem; color: var(--tech-blue); font-weight: 700; text-transform: uppercase; letter-spacing: 1px; }
.row-title { font-size: 1.2rem; font-weight: 800; color: #1e293b; margin: 0; }
.row-arrow { font-size: 1.5rem; color: #cbd5e1; transition: 0.2s; }
.project-row:hover .row-arrow { color: var(--tech-blue); transform: translateX(5px); }

/* MODAL PENCERE */
.modal-overlay { display: none; position: fixed; top: 0; left: 0; width: 100%; height: 100%; background: rgba(0, 0, 0, 0.85); z-index: 99999; justify-content: center; align-items: center; padding: 20px; backdrop-filter: blur(5px); }
.modal-overlay:target { display: flex; }
.modal-content { background: #fff; width: 100%; max-width: 800px; max-height: 90vh; overflow-y: auto; padding: 40px; border-radius: 15px; position: relative; box-shadow: 0 0 50px rgba(0,0,0,0.5); animation: slideDown 0.3s ease; }
@media (prefers-color-scheme: dark) { .modal-content { background: #1e293b; color: #fff; } .modal-desc { color: #cbd5e1 !important; } .modal-title { color: #60a5fa !important; } }
@keyframes slideDown { from { transform: translateY(-50px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
.close-link { position: absolute; top: 15px; right: 20px; font-size: 2rem; color: #94a3b8; text-decoration: none !important; line-height: 1; z-index: 10; }
.close-link:hover { color: #ef4444; }
.modal-backdrop-close { position: absolute; top: 0; left: 0; width: 100%; height: 100%; cursor: default; }

.modal-banner { width: 100%; height: auto; max-height: 600px; object-fit: contain; border-radius: 8px; margin-bottom: 25px; box-shadow: 0 4px 15px rgba(0,0,0,0.1); display: block; background-color: #f8fafc; }
.modal-title { margin-top: 0; color: var(--tech-blue); font-size: 1.5rem; border-bottom: 1px solid #e2e8f0; padding-bottom: 15px; margin-bottom: 15px; }
.modal-desc { line-height: 1.7; font-size: 1.05rem; color: #334155; }
.modal-tags { margin-top: 25px; display: flex; gap: 10px; flex-wrap: wrap; }
.tag-badge { background: #eff6ff; color: var(--tech-blue); padding: 5px 12px; border-radius: 50px; font-size: 0.8rem; border: 1px solid #bfdbfe; font-weight: 600; }
@media (prefers-color-scheme: dark) { .tag-badge { background: #172554; color: #93c5fd; border-color: #1e40af; } }

/* GALERİ */
.gallery-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
.gallery-card { background: #fff; border: 1px solid var(--tech-border); border-radius: 12px; overflow: hidden; transition: 0.3s; }
@media (prefers-color-scheme: dark) { .gallery-card { background: #1e293b; border-color: #334155; } }
.gallery-card:hover { transform: translateY(-5px); box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.1); }
.img-box { height: 220px; width: 100%; overflow: hidden; }
.img-box img { width: 100%; height: 100%; object-fit: cover; transition: 0.5s; }
.gallery-card:hover img { transform: scale(1.05); }
.full-width { grid-column: 1 / -1; } .full-width .img-box { height: 400px; }
</style>

<div class="lang-switcher">
  <a href="/muhendislik-cv/portfolio/" class="lang-btn">TR</a>
  <a href="/muhendislik-cv/en/portfolio/" class="lang-btn active">EN</a>
</div>

<h2 class="section-title">Engineering Analyses</h2>

<div class="projects-container">

  <a href="#proje-1" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">Academic Research</span><h3 class="row-title">Buckling analysis for laminated and hybrid composite beams</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-2" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">Software Development</span><h3 class="row-title">Mohr's Circle Calculator Tool</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-3" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">TÜBİTAK 2209-A</span><h3 class="row-title">Elevator System Design (VİSA SÖR)</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-4" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">Graduation Thesis</span><h3 class="row-title">Design of Francis Type Turbines</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-5" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">Volunteer Work</span><h3 class="row-title">CFD Technical Book Translation Project</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-6" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">Volunteer Research</span><h3 class="row-title">Volunteer Mucilage Project</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

  <a href="#proje-7" class="project-card-link">
    <div class="project-row">
      <div class="row-info"><span class="row-category">Certificate / Training</span><h3 class="row-title">Akbank Python & AI Bootcamp</h3></div>
      <div class="row-arrow">➔</div>
    </div>
  </a>

</div>

<h2 class="section-title">3D Design & Render</h2>

<div class="gallery-grid">
  <div class="gallery-card"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/ucak.jpg" alt="Plane" onerror="this.src='https://via.placeholder.com/600x400';"></div></div>
  <div class="gallery-card"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/alpagu.jpg" alt="Alpagu" onerror="this.src='https://via.placeholder.com/600x400';"></div></div>
  <div class="gallery-card"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/m16.jpg" alt="M16" onerror="this.src='https://via.placeholder.com/400x300';"></div></div>
  <div class="gallery-card"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/jet.png" alt="Jet" onerror="this.src='https://via.placeholder.com/400x300';"></div></div>
  <div class="gallery-card"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/superman.png" alt="Superman" onerror="this.src='https://via.placeholder.com/400x300';"></div></div>
  <div class="gallery-card"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/manifold.jpg" alt="Manifold" onerror="this.src='https://via.placeholder.com/400x300';"></div></div>
  <div class="gallery-card full-width"><div class="img-box"><img src="https://emir3d.github.io/muhendislik-cv/images/top.jpg" alt="Cannon" onerror="this.src='https://via.placeholder.com/800x400';"></div></div>
</div>

<div id="proje-1" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <img src="https://emir3d.github.io/muhendislik-cv/images/matlab.jpg" class="modal-banner" onerror="this.style.display='none'"> 
    <h3 class="modal-title">Buckling analysis for laminated and hybrid composite beams</h3>
    <div class="modal-desc">
      <p>Ongoing Research Study</p>
      <ul>
        <li>Comparison of Euler-Timoshenko theories.</li>
        <li>Analytical modeling, finite element analysis (FEA), and MATLAB-based numerical solutions.</li>
        <li>ANSYS ACP module implementation.</li>
        <li>Literature review and article drafting processes are ongoing.</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">ANSYS ACP</span><span class="tag-badge">MATLAB</span><span class="tag-badge">FEA</span></div>
  </div>
</div>

<div id="proje-2" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Mohr's Circle Calculator Tool</h3>
    <div class="modal-desc">
      <p>Developed for strength of materials calculations, this tool automatically draws Mohr's circle using user-provided stress data.</p>
      <ul>
        <li>Calculation of principal stresses (σ1, σ2).</li>
        <li>Determination of maximum shear stress (τmax).</li>
        <li>User-friendly graphical interface (GUI).</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">MATLAB GUI</span><span class="tag-badge">Solid Mechanics</span></div>
  </div>
</div>

<div id="proje-3" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Elevator System Design (VİSA SÖR)</h3>
    <div class="modal-desc">
      <p>TÜBİTAK 2209-A – University Students Research Projects Support</p>
      <ul>
        <li>Elevator system design for duplex and triplex structures.</li>
        <li>Served as the team leader in the project.</li>
        <li>Execution of mechanical design, sizing, and analysis studies.</li>
        <li>Engineering calculations and system optimization during the design process.</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">SolidWorks</span><span class="tag-badge">Mechanical Design</span></div>
  </div>
</div>

<div id="proje-4" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Design of Francis Type Turbines</h3>
    <div class="modal-desc">
      <p>Graduation Thesis</p>
      <ul>
        <li>Francis type hydroelectric turbine design for Keban Dam.</li>
        <li>Determination of turbine geometry and sizing calculations.</li>
        <li>Application of energy conversion principles and hydrodynamic design criteria.</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">SolidWorks</span><span class="tag-badge">CFD</span><span class="tag-badge">Hydrodynamics</span></div>
  </div>
</div>

<div id="proje-5" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">CFD Technical Book Translation Project</h3>
    <div class="modal-desc">
      <p>Advisor: Dr. Nuray Kayakol</p>
      <ul>
        <li>Technical document translation on CFD theory equations and modeling methods.</li>
        <li>Translation of academic content regarding two-phase flow and cavitation in valves into Turkish.</li>
        <li>Active member of the translation group during the 4-month project.</li>
        <li>Gained mastery in technical terminology and academic writing style.</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">CFD</span><span class="tag-badge">Technical Translation</span></div>
  </div>
</div>

<div id="proje-6" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Volunteer Mucilage Project</h3>
    <div class="modal-desc">
      <p>Advisor: Dr. Nuray Kayakol – CFDEXPLAINED</p>
      <ul>
        <li>Research on the causes of mucilage formation and solution methods.</li>
        <li>Problem analysis using fluid mechanics and CFD-based approaches.</li>
        <li>Gained an interdisciplinary perspective on environmental engineering problems.</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">CFD</span><span class="tag-badge">Fluid Mechanics</span></div>
  </div>
</div>

<div id="proje-7" class="modal-overlay">
  <a href="#_" class="modal-backdrop-close"></a>
  <div class="modal-content">
    <a href="#_" class="close-link">&times;</a>
    <h3 class="modal-title">Akbank Python & AI Bootcamp</h3>
    <div class="modal-desc">
      <p>Sponsored by Global AI Hub</p>
      <ul>
        <li>Training in Python programming and artificial intelligence fundamentals.</li>
        <li>Implementation of Driverless Metro Simulation (Route Optimization) project.</li>
        <li>Applications focusing on algorithmic thinking and optimization problems.</li>
      </ul>
    </div>
    <div class="modal-tags"><span class="tag-badge">Python</span><span class="tag-badge">AI</span><span class="tag-badge">Algorithms</span></div>
  </div>
</div>
