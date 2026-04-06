---
layout: page
title: "Data-Driven Reagent Recommendation for Organic Synthesis and Drug Discovery"
description: "ML pipeline for recommending optimal reagents and reaction conditions to accelerate retrosynthetic planning and drug synthesis."
img:
importance: 2
category: ml & ai
selected: true
year: 2025
pdf: coley_lab.pdf
---

Developed in the Coley Lab at MIT, this project advances the group's mission of making computer-aided synthesis planning practically useful for real-world drug discovery. Selecting optimal reagents and reaction conditions for a given transformation is one of the highest-expertise tasks in synthesis, and one where ML systems trained on large reaction databases can offer substantial leverage — particularly for chemists exploring unfamiliar reaction classes or novel substrates.

The system is trained on curated reaction datasets (USPTO, Reaxys-derived) using transformer-based reaction encoders that embed chemical context into rich representations for condition prediction. A retrieval-augmented architecture surfaces historically successful reagent-condition combinations for analogous transformations, while a ranking model scores candidates by predicted yield, selectivity, and practical accessibility. Active learning components prioritize experimental validation of high-uncertainty predictions, enabling continuous model improvement from laboratory feedback with minimal annotation overhead.

Evaluation on held-out reaction classes demonstrates strong generalization to underrepresented transformations — a key requirement given the long-tail distribution of reaction types in synthesis databases. The system integrates with retrosynthesis planning tools developed within the Coley Lab ecosystem, positioning reagent recommendation as a practical decision-support layer within an end-to-end computer-aided synthesis planning pipeline.

{% include pdf_embed.liquid %}
