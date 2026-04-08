---
layout: page
title: "Optimizing Solar Panel Waste Recycling Facility Placement in Massachusetts"
description: "Geospatial optimization model using p-median and coverage formulations to site solar panel recycling facilities across Massachusetts for minimal transport cost and equitable access."
img:
importance: 6
category: ml & ai
year: 2025
pdf: Optimization_project.pdf
skills: [Python, Gurobi, Julia, Optimization, Geospatial Analysis, Data Analysis, Environmental Engineering, Operations Research, p-median, Facility Location]
---

<div class="project-meta-badges">
  <span class="project-badge">MIT 15.C57</span>
  <span class="project-badge">Operations Research</span>
  <span class="project-badge">Environmental Policy</span>
</div>

<div class="project-sections">

<div class="project-section-card">
<h4>The Problem</h4>
<p>As solar energy adoption accelerates across New England, end-of-life photovoltaic panels are becoming a significant waste challenge. Solar panels contain hazardous materials including lead and cadmium, making unmanaged disposal an environmental and public health risk. Massachusetts currently lacks dedicated recycling infrastructure, and with projected panel retirements growing rapidly, siting decisions made now will shape cost and equity outcomes for decades.</p>
</div>

<div class="project-section-card">
<h4>The Approach</h4>
<p>Built a geospatial facility location optimization model combining <strong>p-median</strong> and <strong>coverage formulations</strong> to minimize total transport distance while maintaining coverage requirements across the state. Panel waste volume projections were derived from state-level solar installation data to account for both current and future recycling demand. Sociodemographic weighting was incorporated to ensure equitable facility access across income and population-density gradients. Candidate facility sites were evaluated via geospatial clustering against town-level demand nodes.</p>
</div>

<div class="project-section-card">
<h4>Results</h4>
<p>The model identified facility configurations that minimize total transport distance while satisfying coverage constraints — producing concrete, actionable siting recommendations for policymakers and waste management planners. Sensitivity analysis showed that a small number of well-placed facilities can serve the majority of projected panel waste volume, with equitable access achievable at minimal additional cost relative to cost-only optimization.</p>
</div>

</div>

<div class="project-github-links">
  <a class="project-github-btn" href="https://github.com/nilay-mishra/15c57_project" target="_blank">
    <i class="fa-brands fa-github"></i>
    <span class="project-github-btn-title">15c57_project</span>
    <span class="project-github-btn-sub">Optimization models & analysis</span>
  </a>
</div>

{% include pdf_embed.liquid %}
