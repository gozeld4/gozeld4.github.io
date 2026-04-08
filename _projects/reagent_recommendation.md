---
layout: page
title: "Reaction-Aware Agent Prediction via Local Neural Models"
description: "Reaction class-specific D-MPNN and FFN models trained on 15M patent reactions for chemical agent prediction, achieving ~20% improvement over global baselines."
img:
importance: 2
category: ml & ai
selected: true
year: 2025
pdf: coley_lab.pdf
skills: [Python, PyTorch, Graph Neural Networks, Chemprop, RDKit, Multi-label Classification, Beam Search, Data Augmentation, HPC, Machine Learning]
---

<div class="project-meta-badges">
  <span class="project-badge">Coley Lab @ MIT</span>
  <span class="project-badge">Drug Discovery</span>
</div>

<div class="project-stats">
  <div class="project-stat">
    <span class="project-stat-value">~15M</span>
    <span class="project-stat-label">patent reactions</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">1,376</span>
    <span class="project-stat-label">agent vocabulary</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">~20% better</span>
    <span class="project-stat-label">over global model</span>
  </div>
</div>

<div class="project-sections">

<div class="project-section-card">
<h4>Data Processing</h4>
<p>Leveraged a preprocessed dataset of ~15 million patent reactions from the Pistachio database, with a curated agent vocabulary of 1,376 chemical species. Partitioned data by reaction class to enable training of class-specific local models.</p>
</div>

<div class="project-section-card">
<h4>Model Training</h4>
<p>Trained reaction class-specific local models using two neural network architectures — a graph-based D-MPNN and a fingerprint-based FFN — to predict chemical agent identities as a multi-label classification task. Applied data augmentation to handle the unordered nature of agent sets, encouraging order-invariant predictions. By specializing models on individual reaction classes rather than training a single global model, achieved a ~20% improvement in agent prediction performance.</p>
</div>

<div class="project-section-card">
<h4>Inference & Results</h4>
<p>Agents are decoded autoregressively via beam search, capturing inter-agent dependencies without enforcing a fixed output structure. Reaction class-specific specialization yielded a ~20% performance improvement over the global model, with the largest gains observed in condition-sensitive reaction classes.</p>
</div>

</div>

{% include pdf_embed.liquid %}
