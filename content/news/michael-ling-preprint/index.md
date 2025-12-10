---
title: "Supervised Classification of LEO Debris Families Using Multi-Set Proper Elements"
date: "2025-12-10"
authors: ["Michael Ling", "Yang Yang", "et al."]
tags: [preprint, arxiv, undergraduate]
featured: true
links:
  - url: "https://arxiv.org/abs/2512.08495"
    icon_pack: "fas"
    icon: "file-alt"
summary: "A new preprint led by undergraduate student Michael Ling is now available on arXiv."
---

We are excited to announce a new preprint led by our undergraduate student Michael Ling:

**Title:** See arXiv link for details
**Authors:** Michael Ling, Yang Yang, et al.
**arXiv:** [https://arxiv.org/abs/2512.08495](https://arxiv.org/abs/2512.08495)

**Abstract:**
Machine learning techniques using proper elements to reconnect families of satellite fragmentation debris have recently advanced, becoming key to space sustainability and domain awareness. However, an evolving circumterrestrial environment may limit their applicability, particularly when models are trained on outdated debris representations. In this work, we devise a computational pipeline using synthetic fragmentation data from explosive breakup events, generated via a Standard Breakup Model and propagated under a high-fidelity dynamical model. Proper elements are extracted using adapted algorithms for modified equinoctial (MEE), Poincar'e (PNC), and quaternion (QTN) sets.
Extending beyond previous approaches limited to MEE space, we include PNC and QTN sets to broaden the dynamical fingerprints available to the classifier. Neural networks trained on various element combinations are used to determine if fragment pairs share a parent. Crucially, we identify a fundamental limitation when applying standard quaternion sets to neural networks: the loss of orbital size information during feature normalization. We introduce an augmented representation (QTNp) that explicitly restores the semi-latus rectum, improving accuracy from 0.31 to 0.60 compared to the standard set. In synthetic Starlink-like LEO experiments, expanding proper-element sets generally improves discrimination. The best model, using a joint feature set (MEE + PNC + QTN), achieves an ROC-AUC of 0.858 compared to 0.789 for the MEE-only baseline, alongside higher accuracy and F1 scores.

Congratulations to Michael and the team for this achievement!
