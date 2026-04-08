---
layout: page
title: "Topological Feature-Driven Machine Learning for Mechanically Stable MOF Discovery"
description: "ML framework predicting MOF bulk modulus from topology, chemistry, and geometry features — screening ~435k candidates with 75% MD-validated accuracy."
img:
importance: 4
category: ml & ai
year: 2026
pdf: kulik_lab.pdf
skills: [Python, Machine Learning, MD Simulations, Random Forest, Gradient Boosting, Kernel Ridge Regression, Materials Science, Topological Features, MOFs, Transformers, Uncertainty Quantification]
---

<div class="project-meta-badges">
  <span class="project-badge">Kulik Lab @ MIT</span>
  <span class="project-badge">Published 2026</span>
  <a class="project-badge project-badge-link" href="https://pubs.rsc.org/en/content/articlelanding/2026/ta/d5ta08080k" target="_blank"><i class="fa-solid fa-book-open"></i> J. Mater. Chem. A</a>
</div>

<div class="project-stats">
  <div class="project-stat">
    <span class="project-stat-value">~435k</span>
    <span class="project-stat-label">MOFs screened</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">R² = 0.79</span>
    <span class="project-stat-label">test performance</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">22,609</span>
    <span class="project-stat-label">stable candidates found</span>
  </div>
</div>

<div class="project-sections">

<div class="project-section-card">
<h4>The Problem</h4>
<p>MOFs are promising for gas storage, water harvesting, and separation, but many collapse under pressure — and with millions of possible structures, experimental or simulation-based testing is intractable. Prior ML models couldn't generalize across the diverse topologies found in real MOF databases, because one-hot encoding of net topology treats each topology as entirely unrelated to all others.</p>
</div>

<div class="project-section-card">
<h4>The Approach</h4>
<p>Trained multiple ML architectures (random forest, gradient boosting, kernel ridge regression, and ANNs) on 7,330 ultrastable MOFs, using a novel feature set combining topological descriptors (normalized cycle-length frequencies derived from net theory), revised autocorrelations (RACs) for local atom chemistry, and Zeo++ geometric descriptors. Cycle-length features encode properties of nets rather than identities, enabling the model to reason about unseen topologies. Also fine-tuned MOFormer, a pretrained transformer, as a comparison baseline. Uncertainty quantification via latent space distance made the model reliable on databases far outside the training distribution.</p>
</div>

<div class="project-section-card">
<h4>Results & Publication</h4>
<p>The best model (KRR-Laplacian) achieved a test log R² of 0.79 with ~1 GPa mean absolute error. Applied to ~435k MOFs, it identified 22,609 exceptionally stable candidates — 75% validated by molecular dynamics simulation, with 6,889 passing a structural feasibility check. Published open-access in <em>Journal of Materials Chemistry A</em> (2026); data, models, and screening notebooks available on Zenodo (<a href="https://doi.org/10.5281/zenodo.17088767">10.5281/zenodo.17088767</a>).</p>
</div>

</div>

<div class="project-figures project-figures-row">
  <figure class="project-figure">
    <img src="{{ '/assets/img/topology_project_fig1.png' | relative_url }}" alt="MOF screening dataset distributions and example high-stability candidates" />
    <figcaption>K<sub>VRH</sub> distributions and example high-stability candidates.</figcaption>
  </figure>
  <figure class="project-figure">
    <img src="{{ '/assets/img/topology_project_fig2.png' | relative_url }}" alt="Predicted vs. true bulk modulus for different feature sets" />
    <figcaption>Predicted vs. true K<sub>VRH</sub> across four feature combinations (log R² 0.47 → 0.76).</figcaption>
  </figure>
</div>

<div class="project-github-links">
  <a class="project-github-btn" href="https://github.com/gozeld4/ML4MOFs" target="_blank">
    <i class="fa-brands fa-github"></i>
    <span class="project-github-btn-title">ML4MOFs</span>
    <span class="project-github-btn-sub">ML models & training example code</span>
  </a>
  <a class="project-github-btn" href="https://github.com/gozeld4/MD_Simulations" target="_blank">
    <i class="fa-brands fa-github"></i>
    <span class="project-github-btn-title">MD_Simulations</span>
    <span class="project-github-btn-sub">Molecular dynamics example code</span>
  </a>
</div>
