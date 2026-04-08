---
layout: page
title: "SolvaNET: Predicting Solvation Free Energies with Machine Learning"
description: "Gradient boosting model combining Morgan fingerprints and RDKit descriptors to predict logK for solute-solvent pairs, achieving R² = 0.973 on cross-validation."
img:
importance: 5
category: ml & ai
year: 2024
skills: [Python, Machine Learning, RDKit, Morgan Fingerprints, Gradient Boosting, Random Forest, Graph Neural Networks, Cheminformatics, Feature Engineering, Cross-validation]
---

<div class="project-meta-badges">
  <span class="project-badge">MIT ML4MolEng</span>
  <span class="project-badge">Spring 2024</span>
</div>

<div class="project-stats">
  <div class="project-stat">
    <span class="project-stat-value">R² = 0.973</span>
    <span class="project-stat-label">CV performance</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">~500</span>
    <span class="project-stat-label">solvent-solute pairs</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">5 models</span>
    <span class="project-stat-label">benchmarked</span>
  </div>
</div>

<div class="project-sections">

<div class="project-section-card">
<h4>The Problem</h4>
<p>Predicting solvation free energies (logK) for solute-solvent pairs — a key property in chemistry that quantifies how well a molecule dissolves in a given solvent. The dataset comes from the Solv@TUM database and contains ~500 solvent-solute pairs in SMILES format.</p>
</div>

<div class="project-section-card">
<h4>The Approach</h4>
<p>Feature engineering using two complementary molecular representations: <strong>RDKit descriptors</strong> (molecular weight, TPSA, H-bond donors, rotatable bonds, etc.) and <strong>Morgan fingerprints</strong> — 512-bit circular fingerprints (radius 2) encoding local atomic environments. Features were computed independently for both solvent and solute, then concatenated. Multiple models were evaluated: Linear Regression (baseline), Random Forest, Gradient Boosting, MLP, and Graph Neural Networks. Hyperparameter tuning and 5-fold cross-validation were used throughout.</p>
</div>

<div class="project-section-card">
<h4>Results</h4>
<table class="project-results-table">
  <thead>
    <tr><th>Model</th><th>CV R²</th></tr>
  </thead>
  <tbody>
    <tr><td>Linear Regression</td><td>0.816</td></tr>
    <tr><td>Random Forest</td><td>0.959</td></tr>
    <tr class="project-results-best"><td>Gradient Boosting</td><td><strong>0.973</strong></td></tr>
  </tbody>
</table>
<p>The winning model was Gradient Boosting with combined Morgan fingerprint + RDKit features (training R² = 0.996). The key insight: combining fingerprint-based and physicochemical descriptors outperformed either alone.</p>
</div>

</div>

<div class="project-github-links">
  <a class="project-github-btn" href="https://github.com/gozeld4/SolvaNET" target="_blank">
    <i class="fa-brands fa-github"></i>
    <span class="project-github-btn-title">SolvaNET</span>
    <span class="project-github-btn-sub">Full notebook & code</span>
  </a>
</div>
