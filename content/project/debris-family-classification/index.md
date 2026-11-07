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
  caption: "AI-generated schematic summarising the published IEEE TAES workflow and results. Metrics describe a synthetic, atmospheric-drag-free LEO benchmark; F1 and recall use posthoc evaluation-set thresholds, not deployment-ready estimates."
  caption_below: true
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
using a Standard Breakup Model, propagates it under an atmospheric-drag-free dynamical model, and extracts proper
elements across three representations — modified equinoctial (MEE), Poincaré (PNC) and quaternion (QTN)
sets. Neural networks are then trained on combinations of those element sets to decide whether a pair of
fragments shares a parent.

Extending beyond the modified-equinoctial space used by previous approaches widens the dynamical
fingerprint available to the classifier. The pipeline also includes an augmented quaternion
representation, QTNp, which appends an explicit orbital-size proxy. The journal results show that
physically complete representations matter more than simply adding element sets.

## Demonstrated result

- **QTNp achieved the highest positive-class F1 of 0.1245**, compared with 0.1023 for standard QTN;
  recall increased from 0.156 to 0.263. These are same-parent fragment-pair classification results,
  not overall accuracy.
- **MEE + QTNp achieved the highest ROC-AUC of 0.656.** QTNp, MEE + QTNp and MEE + PNC + QTNp
  shared the highest PR-AUC of 0.071. Adding more element sets did not consistently improve
  positive-class F1, and difference-based features provided no consistent advantage.
- **Published in IEEE Transactions on Aerospace and Electronic Systems**, volume 62 (2026):
  *Supervised Classification of Synthetic LEO Debris Families Using Multiset Proper Elements Under
  Atmospheric-Drag-Free Dynamics*, by Michael Ling and Yang Yang.
  [Read the journal paper](https://doi.org/10.1109/TAES.2026.3737763).
  Earlier work was presented at the Australian Space Research Conference 2025
  ([presentation slides](/slides/Classification_of_LEO_debris_family_Dr_YYang.pdf)).

These results apply to a **synthetic, atmospheric-drag-free LEO benchmark**, not operational
classification of real debris. Positive-class F1 and recall were evaluated at thresholds selected
posthoc on the same evaluation set, so they are descriptive operating-point summaries rather than
deployment-ready performance estimates.

## External use

The method addresses a recognised gap in space sustainability and space domain awareness: maintaining
attribution of fragmentation debris as the circumterrestrial environment evolves. The
[journal paper](https://doi.org/10.1109/TAES.2026.3737763) establishes a controlled benchmark for
comparing representations. Transfer to real LEO debris requires drag-aware descriptors and independent
validation; performance in other orbital regimes has not been established.

<!-- TODO: note any catalogue maintainer or agency that has taken up the method or the QTNp
     representation, if that can be stated publicly. -->

## Next partnership opportunity

Applying the classifier to a real breakup event of interest to you, or extending it from synthetic
training data to your catalogue. This fits most naturally as a sponsored thesis or co-funded project —
see [Partner with us](/partner/).
