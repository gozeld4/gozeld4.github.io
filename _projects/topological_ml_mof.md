---
layout: page
title: "Topological Feature-Driven Machine Learning for Mechanically Stable MOF Discovery"
description: "Using persistent homology descriptors and ML to predict mechanical stability of metal-organic frameworks from topology alone."
img:
importance: 4
category: ml & ai
year: 2024
pdf: kulik_lab.pdf
---

Conducted in the Kulik Lab at MIT, this project addresses a key bottleneck in high-throughput MOF discovery: identifying which of the millions of hypothetical framework structures are mechanically viable before committing to costly synthesis or DFT calculations. The Kulik group's expertise in ML-accelerated materials screening and first-principles computation provided the foundation for developing a topology-driven stability predictor.

The approach encodes multi-scale structural features — ring systems, pore geometry, node connectivity — as persistence diagrams via persistent homology, then vectorizes them as persistence images for use in supervised ML models. Random forest, gradient boosting, and graph neural network architectures were trained on a DFT-computed dataset of MOF elastic properties (bulk modulus, shear modulus) and benchmarked against conventional descriptor sets. Topological features capture geometric stability signals that chemistry-based fingerprints systematically miss, achieving competitive predictive performance with substantially lower computational cost per inference.

The resulting model enables rapid pre-screening of large hypothetical MOF libraries, directing synthesis resources toward structurally robust candidates and advancing the Kulik lab's broader agenda of replacing expensive quantum calculations with accurate ML surrogates.

{% include pdf_embed.liquid %}
