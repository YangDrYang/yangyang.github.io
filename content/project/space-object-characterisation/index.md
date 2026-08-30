---
title: "Satellite Manoeuvre Detection and Pattern of Life"
summary: "Telling a real manoeuvre apart from mismodelled dynamics or a bad track, across the GEO belt, using labelled optical data rather than assumptions."
tags:
  - Space Situational Awareness
  - Astrodynamics
date: "2024-11-01T00:00:00Z"
weight: 20  # Controls order in the homepage portfolio (low first).
draft: false

# Optional external URL for the project (replaces project detail page).
external_link: ""

authors: [admin, "michael_ling"]

image:
  caption: "Pattern of life identification for geosynchronous satellites"
  focal_point: "Smart"
---

## Problem

A geostationary satellite changes its behaviour and the people responsible for the catalogue find out
late, or not at all. The hard part is not seeing that the residuals moved — it is deciding whether that
movement was a real manoeuvre, a mismodelled solar radiation pressure, or simply a bad track. Get that
call wrong in one direction and you lose custody of the object; get it wrong in the other and you
generate alarms nobody trusts.

Doing this at the scale of the GEO belt makes it worse. Analyst-led assessment does not scale to
hundreds of objects observed nightly, and detectors trained on assumed dynamics degrade quietly as the
population and operating practices change around them.

## Capability

We build manoeuvre detection and pattern-of-life identification for geostationary and geosynchronous
satellites, grounded in observational data rather than simulated behaviour. Three parts:

- **A labelled optical dataset.** The Optical Pattern of Life Analysis and Library (OPAL) dataset gives
  detectors something real to train and be evaluated against.
- **Detection methods.** Image-based and time-series transformer models for identifying manoeuvres,
  benchmarked against conventional residual-threshold approaches.
- **A pattern-of-life framework.** Integrating the above so that individual detections become a
  behavioural characterisation of an object over time, which is what an operator actually acts on.

Related characterisation work — satellite polarimetry through the UNSW Observatory, the ongoing PhD
project of [Asad Rizvi](/authors/asad_rizvi/) — supplies independent evidence about attitude and
surface state to corroborate a detection.

The work is carried out by [Michael Ling](/authors/michael_ling/), research assistant on the NSW Space
Research Network project, together with several students on supervised thesis projects covering
manoeuvre modelling, track association and object characterisation.

<!-- TODO: name the current thesis students working on this project, and link their author pages once
     created (see content/authors/ for the existing pattern). Only Michael Ling and Asad Rizvi are
     named above because they are the two with profiles in the repo. -->

## Demonstrated result

- **Competitively funded as a NSW Space Research Network Pilot Research Project for 2025–2026**,
  *Pattern of Life Identification for Geosynchronous Satellites Using Transformer-Based AI Foundation
  Models*, in collaboration with Macquarie University and the University of Adelaide.
- **A dedicated research position stood up** to deliver the GEO pattern-of-life characterisation work.
- **Method development presented externally**, including transformers and deep learning for satellite
  manoeuvre detection at the UNSW AI Symposium
  ([slides](/slides/Satellite_Manoeuvre_Detection_DRYYang.pdf)).
- **Complementary manoeuvre-modelling work** on factor graph optimisation for orbit determination with
  Gaussian approximation of impulsive manoeuvres, developed as a supervised thesis project.

<!-- TODO: once the OPAL dataset and detector are evaluated, state the headline detection performance
     here — detection rate, false-alarm rate, and the baseline it was measured against. This is the
     single most persuasive number for the manoeuvre-detection pilot. -->

## External use

The project is co-delivered with **Macquarie University** under NSW
Space Research Network funding, and it feeds the NSW Space Research Network white paper on Space Domain
Awareness. 

<!-- TODO: name any operator or agency already evaluating the detector or the OPAL dataset, if that can
     be stated publicly. -->

## Next partnership opportunity

A **manoeuvre and pattern-of-life assessment** on your GEO or LEO time series: a labelled event list
over the period you care about, and detection performance benchmarked against your current baseline,
with false-alarm behaviour stated openly. See [Partner with us](/partner/).
