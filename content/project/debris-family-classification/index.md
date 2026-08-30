---
title: "Debris Family Classification"
summary: "Reconnecting fragmentation debris to the event that produced it, by widening the orbital fingerprint a classifier can see."
tags:
  - Space Situational Awareness
date: "2025-12-10T00:00:00Z"
weight: 40  # Controls order in the homepage portfolio (low first).
# Hidden from the site. Set back to false to restore it; the inbound links from
# content/home/problems.md and content/publication/_index.md were removed at the same
# time and would need restoring too.
draft: false

external_link: ""

authors: [admin, "michael_ling"]

image:
  caption: "Classification of LEO debris families using multi-set proper elements"
  focal_point: "Smart"
---

## Problem

When a satellite breaks up, the fragments enter the catalogue as hundreds of unattributed objects.
Reconnecting them to their parent event matters for attribution, for understanding how the breakup
happened, and for predicting where the cloud goes next.

Machine-learning methods using proper elements have made progress on this, but they inherit a quiet
failure mode: a model trained on an outdated representation of the debris environment degrades as the
population evolves around it. There is also a specific technical trap — normalising quaternion-set
features for a neural network destroys the orbital size information the classifier needs, and the loss
is invisible until accuracy is measured.

## Capability

A computational pipeline that generates synthetic fragmentation data from explosive breakup events
using a Standard Breakup Model, propagates it under a high-fidelity dynamical model, and extracts proper
elements across three representations — modified equinoctial (MEE), Poincaré (PNC) and quaternion (QTN)
sets. Neural networks are then trained on combinations of those element sets to decide whether a pair of
fragments shares a parent.

Extending beyond the modified-equinoctial space used by previous approaches widens the dynamical
fingerprint available to the classifier. The pipeline also includes an augmented quaternion
representation, QTNp, which explicitly restores the semi-latus rectum lost during feature
normalisation.

## Demonstrated result

- **ROC-AUC improved from 0.789 to 0.858** in synthetic Starlink-like LEO experiments, comparing the
  joint MEE + PNC + QTN feature set against the MEE-only baseline, with corresponding gains in accuracy
  and F1.
- **The QTNp augmentation lifted quaternion-set accuracy from 0.31 to 0.60**, by restoring the orbital
  size information that standard normalisation discards — identifying and closing a failure mode that
  had not previously been characterised.
- **Published as a preprint**, [arXiv:2512.08495](https://arxiv.org/abs/2512.08495), led by
  undergraduate researcher Michael Ling, and presented at the Australian Space Research Conference 2025
  ([slides](/slides/Classification_of_LEO_debris_family_Dr_YYang.pdf)).

## External use

The method addresses a recognised gap in space sustainability and space domain awareness: maintaining
attribution of fragmentation debris as the circumterrestrial environment evolves. The preprint is
openly available, and the finding about quaternion-set normalisation applies to any classifier built on
that representation, not only to this pipeline.

<!-- TODO: note any catalogue maintainer or agency that has taken up the method or the QTNp
     representation, if that can be stated publicly. -->

## Next partnership opportunity

Applying the classifier to a real breakup event of interest to you, or extending it from synthetic
training data to your catalogue. This fits most naturally as a sponsored thesis or co-funded project —
see [Partner with us](/partner/).
