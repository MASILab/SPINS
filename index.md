---
layout: default
title: SPINS
---

<style>
@import url('https://fonts.googleapis.com/css2?family=Source+Serif+4:ital,wght@0,300;0,400;0,600;1,300;1,400&family=IBM+Plex+Mono:wght@400;500&family=DM+Sans:wght@300;400;500&display=swap');

.spins-home {
  --ink: #1a1a2e;
  --ink-mid: #3d3d5c;
  --ink-muted: #7a7a9a;
  --rule: #e0dff0;
  --surface: #f7f6fb;
  --accent: #2d4fa0;
  --accent-light: #e8edf8;
  --accent-mid: #5070c0;
  --teal: #0f7c6e;
  --teal-light: #e2f4f2;
  --amber: #a05a00;
  --amber-light: #faf0e0;
  --serif: 'Source Serif 4', Georgia, serif;
  --sans: 'DM Sans', system-ui, sans-serif;
  --mono: 'IBM Plex Mono', monospace;
  font-family: var(--sans);
  color: var(--ink);
  max-width: 860px;
  margin: 0 auto;
  padding: 2rem 0 4rem;
  line-height: 1.6;
}

.spins-home .hero {
  display: grid;
  grid-template-columns: 1fr 220px;
  gap: 3rem;
  align-items: start;
  margin-bottom: 3rem;
}
.spins-home .hero-kicker {
  font-family: var(--mono);
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 0.18em;
  color: var(--accent-mid);
  text-transform: uppercase;
  margin-bottom: 1.1rem;
  display: flex;
  align-items: center;
  gap: 8px;
}
.spins-home .hero-kicker::before {
  content: '';
  display: inline-block;
  width: 20px;
  height: 1px;
  background: var(--accent-mid);
}
.spins-home h1 {
  font-family: var(--serif);
  font-size: 2.4rem;
  font-weight: 300;
  line-height: 1.18;
  color: var(--ink);
  margin-bottom: 1.2rem;
  letter-spacing: -0.01em;
  border: none;
  padding: 0;
}
.spins-home h1 em { font-style: italic; color: var(--accent); }
.spins-home .hero-body {
  font-size: 15px;
  font-weight: 300;
  color: var(--ink-mid);
  line-height: 1.75;
  margin-bottom: 2rem;
}
.spins-home .hero-actions { display: flex; gap: 12px; flex-wrap: wrap; }
.spins-home .btn-primary {
  font-family: var(--sans);
  font-size: 13px;
  font-weight: 500;
  padding: 9px 20px;
  background: var(--accent);
  color: #fff;
  border-radius: 4px;
  text-decoration: none;
}
.spins-home .btn-primary:hover { background: var(--accent-mid); color: #fff; }
.spins-home .btn-ghost {
  font-family: var(--sans);
  font-size: 13px;
  font-weight: 400;
  padding: 9px 20px;
  background: transparent;
  color: var(--accent);
  border: 1px solid var(--accent);
  border-radius: 4px;
  text-decoration: none;
}
.spins-home .btn-ghost:hover { background: var(--accent-light); }

.spins-home .brain-figure { display: flex; flex-direction: column; align-items: center; gap: 10px; }
.spins-home .brain-label {
  font-family: var(--mono);
  font-size: 10px;
  letter-spacing: 0.12em;
  color: var(--ink-muted);
  text-transform: uppercase;
}

.spins-home .stats-row {
  display: flex;
  border-top: 1px solid var(--rule);
  border-bottom: 1px solid var(--rule);
  margin-bottom: 3rem;
  padding: 1.5rem 0;
}
.spins-home .stat-item {
  flex: 1;
  text-align: center;
  padding: 0 1rem;
  border-right: 1px solid var(--rule);
}
.spins-home .stat-item:last-child { border-right: none; }
.spins-home .stat-number {
  font-family: var(--serif);
  font-size: 2rem;
  font-weight: 400;
  color: var(--accent);
  line-height: 1;
  margin-bottom: 5px;
}
.spins-home .stat-desc { font-size: 12px; color: var(--ink-muted); line-height: 1.4; }

.spins-home .section-eyebrow {
  font-family: var(--mono);
  font-size: 10.5px;
  font-weight: 500;
  letter-spacing: 0.16em;
  color: var(--ink-muted);
  text-transform: uppercase;
  margin-bottom: 1rem;
}

.spins-home .atlas-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
  margin-bottom: 3rem;
}
.spins-home .atlas-card {
  background: #fff;
  border: 1px solid var(--rule);
  border-radius: 6px;
  padding: 1.25rem;
  text-decoration: none;
  color: inherit;
  display: flex;
  flex-direction: column;
  gap: 10px;
  transition: border-color 0.15s, box-shadow 0.15s;
}
.spins-home .atlas-card:hover {
  border-color: #b0b8d8;
  box-shadow: 0 2px 12px rgba(45,79,160,0.08);
  text-decoration: none;
}
.spins-home .card-tag {
  display: inline-block;
  font-family: var(--mono);
  font-size: 10px;
  font-weight: 500;
  letter-spacing: 0.1em;
  text-transform: uppercase;
  padding: 3px 8px;
  border-radius: 3px;
}
.spins-home .tag-gray  { background: #eeecf8; color: #4a4880; }
.spins-home .tag-teal  { background: var(--teal-light); color: var(--teal); }
.spins-home .tag-amber { background: var(--amber-light); color: var(--amber); }
.spins-home .atlas-card h3 {
  font-family: var(--serif);
  font-size: 1.1rem;
  font-weight: 400;
  color: var(--ink);
  line-height: 1.3;
  margin: 0;
  border: none;
}
.spins-home .atlas-card p {
  font-size: 13px;
  font-weight: 300;
  color: var(--ink-muted);
  line-height: 1.6;
  flex: 1;
  margin: 0;
}
.spins-home .card-meta {
  font-family: var(--mono);
  font-size: 11px;
  color: var(--ink-muted);
  display: flex;
  align-items: center;
  gap: 6px;
}
.spins-home .card-meta::before {
  content: '';
  display: inline-block;
  width: 6px; height: 6px;
  border-radius: 50%;
  background: currentColor;
  opacity: 0.5;
}

.spins-home .about-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem;
  padding-top: 2rem;
  border-top: 1px solid var(--rule);
}
.spins-home .about-block h2 {
  font-family: var(--serif);
  font-size: 1.25rem;
  font-weight: 400;
  color: var(--ink);
  margin-bottom: 0.8rem;
  border: none;
  padding: 0;
}
.spins-home .about-block p {
  font-size: 14px;
  font-weight: 300;
  color: var(--ink-mid);
  line-height: 1.75;
  margin-bottom: 0.75rem;
}
.spins-home .pipeline-steps { display: flex; flex-direction: column; gap: 10px; margin-top: 0.5rem; }
.spins-home .pipeline-step {
  display: flex;
  align-items: flex-start;
  gap: 12px;
  padding: 10px 12px;
  background: var(--surface);
  border-radius: 4px;
  border-left: 2px solid var(--accent-mid);
}
.spins-home .step-num {
  font-family: var(--mono);
  font-size: 11px;
  font-weight: 500;
  color: var(--accent-mid);
  min-width: 16px;
  margin-top: 1px;
}
.spins-home .step-text { font-size: 13px; font-weight: 300; color: var(--ink-mid); line-height: 1.5; }

@media (max-width: 640px) {
  .spins-home .hero { grid-template-columns: 1fr; }
  .spins-home .brain-figure { display: none; }
  .spins-home .atlas-grid { grid-template-columns: 1fr; }
  .spins-home .about-grid { grid-template-columns: 1fr; }
  .spins-home .stats-row { flex-wrap: wrap; }
  .spins-home .stat-item { flex: 0 0 50%; border-right: none; border-bottom: 1px solid var(--rule); }
}
</style>

<div class="spins-home">

  <div class="hero">
    <div>
      <p class="hero-kicker">MASI Lab · Vanderbilt University</p>
      <h1>A shared public library for <em>brain atlas</em> visualization</h1>
      <p class="hero-body">
        Brain atlases are essential for interpreting neuroimaging results, yet no publicly accessible, precomputed resource for comparing regions across atlases in 3D has existed — until now. SPINS provides interactive visualizations across 210 regions spanning gray matter, white matter, and functional labels.
      </p>
      <div class="hero-actions">
        <a class="btn-primary" href="#atlases">Browse atlases</a>
        <a class="btn-ghost" href="https://github.com/MASILab/SPINS">View on GitHub</a>
      </div>
    </div>
    <div class="brain-figure">
      <img src="/SPINS/assets/images/spins_logo.png" alt="SPINS logo" style="width: 200px; height: auto;">
    </div>
  </div>

  <div class="stats-row">
    <div class="stat-item">
      <div class="stat-number">210</div>
      <div class="stat-desc">Brain regions<br>rendered</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">3</div>
      <div class="stat-desc">Atlases<br>available</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">3D</div>
      <div class="stat-desc">Glass brain<br>videos per region</div>
    </div>
    <div class="stat-item">
      <div class="stat-number">AI</div>
      <div class="stat-desc">Region overviews<br>generated</div>
    </div>
  </div>

  <p class="section-eyebrow" id="atlases">Available atlases</p>
  <div class="atlas-grid">

    <a class="atlas-card" href="https://masilab.github.io/SPINS/brainCOLOR_cortical/">
      <span class="card-tag tag-gray">Gray matter</span>
      <h3>brainCOLOR</h3>
      <p>Whole-brain parcellation covering cortical and subcortical structures across both hemispheres.</p>
      <span class="card-meta">121 regions · cortical + subcortical</span>
    </a>

    <a class="atlas-card" href="https://masilab.github.io/SPINS/Yeo17_renders/">
      <span class="card-tag tag-teal">Functional</span>
      <h3>Yeo 17-Network</h3>
      <p>Resting-state functional network parcellation. 17 bilateral networks spanning the cortex.</p>
      <span class="card-meta">17 networks · bilateral</span>
    </a>

    <a class="atlas-card" href="https://masilab.github.io/SPINS/Pandora_renders/">
      <span class="card-tag tag-amber">White matter</span>
      <h3>Pandora TractSeg</h3>
      <p>White matter tract atlas from TractSeg. Individual tract bundles rendered as binary volumes.</p>
      <span class="card-meta">72 tracts · white matter</span>
    </a>

  </div>

  <div class="about-grid">
    <div class="about-block">
      <p class="section-eyebrow">Motivation</p>
      <h2>Reducing barriers in neuroimaging research</h2>
      <p>Brain atlases are essential for interpretation of results and communication, yet atlas choice can substantially affect research conclusions. Despite this, no publicly accessible, precomputed resource to compare regions across atlases in 3D has existed.</p>
      <p>SPINS makes this comparison immediately accessible, with no software installation required. Each region page includes an AI-generated anatomical overview, rotating glass brain videos, and triplanar slice images.</p>
    </div>
    <div class="about-block">
      <p class="section-eyebrow">Pipeline</p>
      <h2>Automated rendering at scale</h2>
      <div class="pipeline-steps">
        <div class="pipeline-step">
          <span class="step-num">01</span>
          <span class="step-text">Atlas NIfTIs registered to MNI space; regions extracted per label</span>
        </div>
        <div class="pipeline-step">
          <span class="step-num">02</span>
          <span class="step-text">3D glass brain MP4s and GIFs rendered for each region</span>
        </div>
        <div class="pipeline-step">
          <span class="step-num">03</span>
          <span class="step-text">Triplanar PNG slices generated at region centroid</span>
        </div>
        <div class="pipeline-step">
          <span class="step-num">04</span>
          <span class="step-text">GPT-4o generates anatomical region descriptions</span>
        </div>
        <div class="pipeline-step">
          <span class="step-num">05</span>
          <span class="step-text">Jekyll markdown pages built and deployed to GitHub Pages</span>
        </div>
      </div>
    </div>
  </div>

</div>