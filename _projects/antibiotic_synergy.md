---
layout: page
title: "Predicting Antibiotic-Compound Synergy Against MDR Bacteria Using Machine Learning"
description: "ML framework to predict drug-compound synergy against multidrug-resistant bacteria, accelerating antibiotic discovery."
img:
importance: 1
category: science
selected: true
year: 2025
pdf: antibiotic_project.pdf
---

Multidrug-resistant (MDR) bacteria represent one of the most urgent threats in global public health, with existing antibiotics losing efficacy faster than new ones are developed. Identifying effective antibiotic combinations through traditional wet-lab screening is slow and expensive. This project builds a machine learning framework to predict synergistic interactions between antibiotics and adjuvant compounds against MDR strains, sharply reducing the experimental search space.

The model integrates molecular fingerprints, physicochemical descriptors, and bacterial genomic features to predict synergy outcomes across multiple drug-bacteria pairings. Gradient boosting and neural network architectures are benchmarked against standard synergy metrics (Loewe additivity, Bliss independence). SHAP-based feature importance analysis surfaces interpretable molecular drivers of synergy, providing actionable guidance for medicinal chemists.

This work demonstrates how supervised ML can accelerate antibiotic discovery pipelines with direct implications for clinical AMR response strategies.

{% include pdf_embed.liquid %}
