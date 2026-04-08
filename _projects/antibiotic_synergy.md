---
layout: page
title: "Predicting Antibiotic-Compound Synergy Against MDR Bacteria Using Machine Learning"
description: "LightGBM + ChemBERTa classifier trained on 1.3M drug combinations to predict antibiotic synergy against multidrug-resistant bacteria, achieving 80% accuracy and AUROC of 0.88."
img:
importance: 3
category: ml & ai
selected: true
year: 2025
pdf: antibiotic_project.pdf
skills: [Python, Machine Learning, LightGBM, XGBoost, Random Forest, ChemBERTa, Morgan Fingerprints, Drug Discovery, Bioinformatics, Classification]
---

<div class="project-meta-badges">
  <span class="project-badge">Antibiotic Resistance</span>
  <span class="project-badge">High-Throughput Screening</span>
  <span class="project-badge">ML for Drug Discovery</span>
</div>

<div class="project-stats">
  <div class="project-stat">
    <span class="project-stat-value">1.3M</span>
    <span class="project-stat-label">drug combinations</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">80% / 0.88</span>
    <span class="project-stat-label">accuracy / AUROC</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">5 models</span>
    <span class="project-stat-label">benchmarked</span>
  </div>
</div>

<div class="project-sections">

<div class="project-section-card">
<h4>The Problem</h4>
<p>Antibiotic resistance contributed to approximately 1.27 million deaths in 2019, and the pipeline for antibiotics with novel mechanisms has nearly dried up. One promising path forward is combination therapy — pairing existing antibiotics with other approved compounds to potentiate their effects. But the space of possible combinations is far too large to test experimentally, making ML-driven prediction essential.</p>
</div>

<div class="project-section-card">
<h4>The Approach</h4>
<p>The study used a dataset of 1.3 million unique strain-antibiotic-compound combinations from a high-throughput droplet-based screen. Synergy was defined via a Bliss score threshold (> 0.3 = synergistic). Five model architectures were evaluated for binary classification: Logistic Regression, Random Forest, XGBoost, LightGBM, and a multi-layer perceptron (MLP). Molecular representation was compared between 1024-bit Morgan Fingerprints and ChemBERTa, a transformer-based chemical language model.</p>
</div>

<div class="project-section-card">
<h4>Results</h4>
<p>The best model was <strong>LightGBM with ChemBERTa embeddings</strong>, achieving <strong>80% accuracy and AUROC of 0.88</strong> — without using the antibiotic-only effect feature (E<sub>a</sub>), which when included pushed accuracy to 95% but conflated molecular signal with experimental artifact. The MLP underperformed across the board, and XGBoost regression showed poor correlation with continuous synergy scores. The final classifier is biased toward avoiding false positives, making it a reliable filter for prioritizing combination candidates for experimental follow-up.</p>
</div>

</div>

<div class="project-github-links">
  <a class="project-github-btn" href="https://github.com/gozeld4/antibiotics_project" target="_blank">
    <i class="fa-brands fa-github"></i>
    <span class="project-github-btn-title">antibiotics_project</span>
    <span class="project-github-btn-sub">Full notebook & saved models</span>
  </a>
</div>

{% include pdf_embed.liquid %}
