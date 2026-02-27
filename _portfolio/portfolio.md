---
layout: archive
title: "Lab"
permalink: /portfolio/
author_profile: true
---

<style>
/* ── Typography & Variables ───────────────────────────── */
@import url('https://fonts.googleapis.com/css2?family=Lora:ital,wght@0,400;0,600;1,400&family=Source+Sans+3:wght@300;400;600&display=swap');

:root {
  --green-deep:   #2c4a2e;
  --green-mid:    #4a7c59;
  --green-light:  #8db89a;
  --cream:        #f7f4ef;
  --sand:         #e8e0d0;
  --text-dark:    #1e2820;
  --text-mid:     #4a5040;
  --accent:       #c17f3a;
}

.lab-page {
  font-family: 'Source Sans 3', sans-serif;
  color: var(--text-dark);
}

/* ── PI / Research Group Banner ───────────────────────── */
.lab-banner {
  background: var(--green-deep);
  color: #fff;
  border-radius: 6px;
  padding: 2rem 2.5rem;
  margin-bottom: 2.5rem;
  display: flex;
  gap: 2rem;
  align-items: flex-start;
}
.lab-banner-text h2 {
  font-family: 'Lora', serif;
  font-size: 1.5rem;
  font-weight: 600;
  margin: 0 0 0.4rem;
  color: #fff;
  border: none;
}
.lab-banner-text .lab-affil {
  font-size: 0.95rem;
  color: var(--green-light);
  margin-bottom: 0.8rem;
}
.lab-banner-text p {
  font-size: 0.95rem;
  line-height: 1.6;
  color: #d4e8da;
  margin: 0;
}
.lab-banner-links {
  margin-top: 1rem;
  display: flex;
  gap: 0.8rem;
  flex-wrap: wrap;
}
.lab-banner-links a {
  background: rgba(255,255,255,0.12);
  color: #fff;
  border: 1px solid rgba(255,255,255,0.25);
  border-radius: 3px;
  padding: 0.3rem 0.8rem;
  font-size: 0.85rem;
  text-decoration: none;
  transition: background 0.2s;
}
.lab-banner-links a:hover {
  background: rgba(255,255,255,0.22);
}

/* ── Section Headers ──────────────────────────────────── */
.lab-section-title {
  font-family: 'Lora', serif;
  font-size: 1.3rem;
  font-weight: 600;
  color: var(--green-deep);
  border-bottom: 2px solid var(--sand);
  padding-bottom: 0.4rem;
  margin: 2.5rem 0 1.5rem;
}

/* ── Research Project Cards ───────────────────────────── */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
  gap: 1.5rem;
  margin-bottom: 2rem;
}
.project-card {
  border: 1px solid var(--sand);
  border-radius: 6px;
  overflow: hidden;
  background: #fff;
  transition: box-shadow 0.2s, transform 0.2s;
}
.project-card:hover {
  box-shadow: 0 6px 20px rgba(44,74,46,0.12);
  transform: translateY(-2px);
}
.project-card-img {
  width: 100%;
  height: 170px;
  object-fit: cover;
  background: var(--sand);
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2.5rem;
}
.project-card-body {
  padding: 1.1rem 1.2rem 1.3rem;
}
.project-card-tag {
  font-size: 0.72rem;
  font-weight: 600;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  color: var(--green-mid);
  margin-bottom: 0.4rem;
}
.project-card-title {
  font-family: 'Lora', serif;
  font-size: 1rem;
  font-weight: 600;
  color: var(--text-dark);
  margin: 0 0 0.5rem;
  line-height: 1.35;
}
.project-card-desc {
  font-size: 0.88rem;
  color: var(--text-mid);
  line-height: 1.55;
  margin: 0;
}

/* ── Photo Gallery ────────────────────────────────────── */
.photo-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 0.75rem;
  margin-bottom: 2rem;
}
.photo-cell {
  aspect-ratio: 4/3;
  background: var(--sand);
  border-radius: 4px;
  overflow: hidden;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--green-light);
  font-size: 0.8rem;
  text-align: center;
  font-style: italic;
  position: relative;
}
.photo-cell img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}
.photo-cell .photo-caption {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: rgba(28,40,32,0.65);
  color: #fff;
  font-size: 0.72rem;
  padding: 0.3rem 0.5rem;
  font-style: normal;
}

/* ── Methods / Equipment ──────────────────────────────── */
.methods-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
  gap: 1rem;
  margin-bottom: 2rem;
}
.method-chip {
  background: var(--cream);
  border: 1px solid var(--sand);
  border-left: 4px solid var(--green-mid);
  border-radius: 4px;
  padding: 0.7rem 1rem;
  font-size: 0.88rem;
  color: var(--text-dark);
  line-height: 1.4;
}
.method-chip strong {
  display: block;
  font-size: 0.8rem;
  text-transform: uppercase;
  letter-spacing: 0.06em;
  color: var(--green-mid);
  margin-bottom: 0.2rem;
}

/* ── Collaborators ────────────────────────────────────── */
.collab-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
  gap: 1rem;
  margin-bottom: 2rem;
}
.collab-card {
  background: var(--cream);
  border: 1px solid var(--sand);
  border-radius: 5px;
  padding: 1rem 1.1rem;
}
.collab-card .collab-name {
  font-family: 'Lora', serif;
  font-weight: 600;
  font-size: 0.95rem;
  color: var(--green-deep);
  margin-bottom: 0.15rem;
}
.collab-card .collab-inst {
  font-size: 0.82rem;
  color: var(--text-mid);
  margin-bottom: 0.3rem;
}
.collab-card .collab-topic {
  font-size: 0.8rem;
  color: var(--accent);
  font-style: italic;
}

/* ── Photo upload note ────────────────────────────────── */
.photo-upload-note {
  background: #fffbf4;
  border: 1px dashed var(--accent);
  border-radius: 4px;
  padding: 0.7rem 1rem;
  font-size: 0.82rem;
  color: var(--accent);
  margin-bottom: 1.2rem;
}
</style>

<div class="lab-page">

<!-- ══ PI / RESEARCH GROUP ══════════════════════════════ -->
<div class="lab-banner">
  <div class="lab-banner-text">
    <h2>Daane Lab — UC Berkeley / UCANR Kearney REC</h2>
    <div class="lab-affil">University of California, Berkeley &nbsp;·&nbsp; USDA-ARS Kearney Research & Extension Center, Parlier, CA</div>
    <p>The Daane Lab investigates the ecology and management of arthropod pests in specialty crops, with particular emphasis on biological control, integrated pest management, and vineyard agroecosystems. Research spans the Central Valley, Central Coast, and Pacific Northwest, addressing pests of grapes, tree fruits, and berry crops.</p>
    <div class="lab-banner-links">
      <a href="https://nature.berkeley.edu/daanelab/" target="_blank" rel="noopener noreferrer">Lab Website</a>
      <a href="mailto:jamestbrown5@berkeley.edu">Contact Me</a>
      <a href="https://scholar.google.com/citations?user=PS_CX0AAAAAJ" target="_blank" rel="noopener noreferrer">Google Scholar</a>
    </div>
  </div>
</div>

<!-- ══ CURRENT RESEARCH PROJECTS ════════════════════════ -->
<div class="lab-section-title">Current Research Projects</div>

<div class="projects-grid">

  <div class="project-card">
    <div class="project-card-img">🪰</div>
    <div class="project-card-body">
      <div class="project-card-tag">Classical Biological Control</div>
      <div class="project-card-title">Biocontrol of Spotted-Wing Drosophila Using <em>Ganaspis kimorum</em></div>
      <p class="project-card-desc">Evaluating host-range, field establishment, and parasitism efficacy of the larval parasitoid <em>Ganaspis kimorum</em> as a sustainable suppression strategy for <em>Drosophila suzukii</em> in California berry and grape systems.</p>
    </div>
  </div>

  <div class="project-card">
    <div class="project-card-img">🍇</div>
    <div class="project-card-body">
      <div class="project-card-tag">IPM · Viticulture</div>
      <div class="project-card-title">Vine Mealybug Management in Wine Grapes</div>
      <p class="project-card-desc">Comparing drip- and foliar-applied insecticide programs, application intervals, and novel active ingredients for control of <em>Planococcus ficus</em> under Central Valley field conditions.</p>
    </div>
  </div>

  <div class="project-card">
    <div class="project-card-img">🌿</div>
    <div class="project-card-body">
      <div class="project-card-tag">Agroecology</div>
      <div class="project-card-title">Pest Management Across Conventional, Organic & Natural Systems</div>
      <p class="project-card-desc">Assessing how land management type shapes <em>D. suzukii</em> population dynamics and the efficacy of IPM interventions, with the goal of developing cross-system management recommendations.</p>
    </div>
  </div>

  <div class="project-card">
    <div class="project-card-img">🔬</div>
    <div class="project-card-body">
      <div class="project-card-tag">Insecticide Evaluation</div>
      <div class="project-card-title">Novel Insecticide Efficacy Trials — Specialty Crops</div>
      <p class="project-card-desc">Field evaluation of new and reduced-risk insecticide chemistries for mealybug and stink bug management in grapes and pomegranates, contributing data to pest management guidelines for California growers.</p>
    </div>
  </div>

</div>

<!-- ══ FIELD & LAB PHOTOS ════════════════════════════════ -->
<div class="lab-section-title">Field & Lab Work</div>

<div class="photo-upload-note">
  📷 Photos coming soon — to add your own, upload images to <code>/images/lab/</code> in your repo and replace the placeholder cells below with <code>&lt;img src="/images/lab/your-photo.jpg"&gt;</code>.
</div>

<div class="photo-grid">
  <div class="photo-cell">Vineyard field trial<br><em>Central Valley, CA</em></div>
  <div class="photo-cell">Mealybug sampling<br><em>Grapevine trunk</em></div>
  <div class="photo-cell"><em>Ganaspis kimorum</em><br>parasitoid rearing</div>
  <div class="photo-cell">SWD monitoring trap<br><em>Blueberry field</em></div>
  <div class="photo-cell">Insecticide drip trial<br><em>Kearney REC</em></div>
  <div class="photo-cell">Cover crop arthropod<br>sampling, N. Florida</div>
</div>

<!-- ══ METHODS & EQUIPMENT ═══════════════════════════════ -->
<div class="lab-section-title">Methods & Equipment</div>

<div class="methods-grid">
  <div class="method-chip"><strong>Field Ecology</strong>Trap-based monitoring, sweep netting, visual scouting, population density estimation</div>
  <div class="method-chip"><strong>Insecticide Trials</strong>Randomized complete block designs, foliar & drip application, residue efficacy assessment</div>
  <div class="method-chip"><strong>Biocontrol Assays</strong>Parasitoid rearing, host-range bioassays, no-choice and choice tests</div>
  <div class="method-chip"><strong>Molecular</strong>DNA extraction, PCR, species identification via sequencing</div>
  <div class="method-chip"><strong>Analytical Chemistry</strong>Lipid extraction and quantification (GC-based), gravimetric analysis</div>
  <div class="method-chip"><strong>Microbiology</strong>Aseptic fruit surface sterilization, microbiome manipulation for behavioral assays</div>
</div>

<!-- ══ COLLABORATORS ══════════════════════════════════════ -->
<div class="lab-section-title">Collaborators & Partners</div>

<div class="collab-grid">

  <div class="collab-card">
    <div class="collab-name">Dr. Kent Daane</div>
    <div class="collab-inst">UC Berkeley / UCANR Kearney REC</div>
    <div class="collab-topic">Postdoctoral supervisor — vineyard IPM, biological control, specialty crops</div>
  </div>

  <div class="collab-card">
    <div class="collab-name">Dr. Oscar Liburd</div>
    <div class="collab-inst">University of Florida</div>
    <div class="collab-topic">PhD advisor — <em>Drosophila suzukii</em> ecology and IPM in berry crops</div>
  </div>

  <div class="collab-card">
    <div class="collab-name">Dr. Dan Hahn</div>
    <div class="collab-inst">University of Florida</div>
    <div class="collab-topic">MS advisor — insect diapause physiology, lipid metabolism</div>
  </div>

  <div class="collab-card">
    <div class="collab-name">Dr. Robert Meagher</div>
    <div class="collab-inst">USDA-ARS, Gainesville, FL</div>
    <div class="collab-topic">Pathways internship supervisor — cover crop ecology, fall armyworm, carabid communities</div>
  </div>

</div>
</div>
