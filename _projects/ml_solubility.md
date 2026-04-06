---
layout: page
title: "Machine Learning for Small Molecule Solubility Prediction in Drug Discovery"
description: "Benchmarking and developing ML models to predict aqueous solubility of drug candidates from molecular structure."
img:
importance: 3
category: ml & ai
year: 2024
---

Aqueous solubility is one of the earliest and most critical physicochemical properties evaluated during drug discovery, directly impacting bioavailability and formulation feasibility. Experimental measurement is resource-intensive, making reliable computational prediction essential for high-throughput screening pipelines. This project benchmarks and develops machine learning models for solubility prediction using curated datasets of small molecules with measured logS values.

Multiple descriptor strategies are compared: traditional physicochemical features (RDKit), extended-connectivity fingerprints (ECFP), and graph-level representations processed by message-passing neural networks. Model performance is evaluated with rigorous train/test splitting strategies designed to assess generalization across chemical space, not just interpolation within training domains.

The best-performing models achieve state-of-the-art RMSE while maintaining interpretability. Feature attribution analysis highlights the dominant structural motifs governing solubility, consistent with established SAR knowledge and offering direct utility for medicinal chemistry decision-making.
