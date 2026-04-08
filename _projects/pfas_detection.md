---
layout: page
title: "Resistivity-Based PFAS Detection via Fluorous Polyaniline Lateral Flow Sensor"
description: "F-PANI sensor on nitrocellulose membranes for field-deployable PFAS detection, with transport modeling reducing assay time to ~13.6 minutes."
img:
importance: 5
category: science
year: 2025
pdf: polymer_ice_class.pdf
skills: [Chemical Synthesis, Environmental Monitoring, Sensor Systems, Materials Characterization, Electrochemistry, Transport Modeling, Polymer Science]
---

<div class="project-meta-badges">
  <span class="project-badge">Environmental Sensing</span>
  <span class="project-badge">PFAS Detection</span>
  <span class="project-badge">Transport Modeling</span>
</div>

<div class="project-stats">
  <div class="project-stat">
    <span class="project-stat-value">1 ppt</span>
    <span class="project-stat-label">EPA drinking water limit</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">~13.6 min</span>
    <span class="project-stat-label">optimized assay time</span>
  </div>
  <div class="project-stat">
    <span class="project-stat-value">400 ppt</span>
    <span class="project-stat-label">current detection limit</span>
  </div>
</div>

<div class="project-sections">

<div class="project-section-card">
<h4>The Problem</h4>
<p>PFAS — "forever chemicals" — are persistent environmental contaminants linked to cancer, liver damage, and hormonal disruption. The U.S. EPA has set drinking water limits as low as 1 ppt, but gold-standard detection methods like LC-MS are expensive, complex, and confined to centralized labs. Existing portable electrical lateral flow assays (e-LFAs) offer a promising path to field deployment, but suffer from response times exceeding 30 minutes due to poor capillary transport across hydrophobic sensing lines — limiting their practical utility.</p>
</div>

<div class="project-section-card">
<h4>The Approach</h4>
<p>The sensor uses <strong>fluorous polyaniline (F-PANI)</strong> printed on nitrocellulose membranes to detect PFAS via resistivity changes. The mechanism exploits reversible acid-base doping of polyaniline: when anionic PFAS molecules partition into the fluorous polymer layer, they donate protons that convert the polymer from an insulating base to a conductive salt — producing a measurable resistance drop. To accelerate response time, Washburn's capillary flow analysis and dimensionless transport modeling (Reynolds, Damköhler, and Péclet numbers) were applied to identify physical parameters — pore radius, membrane length, contact angle — that can be tuned to speed up analyte delivery without sacrificing selectivity.</p>
</div>

<div class="project-section-card">
<h4>Results</h4>
<p>Modeling decomposed total sensor response time into capillary flow, external mass transfer, internal diffusion, and reaction kinetics. Optimizing the test strip to a 2 cm distance with a 0.50 μm pore radius membrane reduced the total assay time to <strong>~13.6 minutes</strong> — competitive with commercial rapid tests. The current limit of detection (400 ppt for PFOA) remains above the EPA's 4 ppt target, but the analysis identifies minimizing transport distance as the most impactful lever for future improvement, providing a clear design roadmap for field-deployable PFAS monitoring at the community level.</p>
</div>

</div>

{% include pdf_embed.liquid %}
