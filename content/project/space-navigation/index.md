---
title: Lunar and Cislunar Navigation
summary: Holding navigation accuracy where GNSS does not reach, by treating constellation geometry, inter-satellite links and time synchronisation as one problem.
tags:
  - Space Navigation
  - GNSS
  - Lunar Missions
date: "2024-12-01T00:00:00Z"
weight: 30  # Controls order in the homepage portfolio (low first).

# Optional external URL for project (replaces project detail page).
external_link: ""

image:
  caption: Lunar navigation satellite system architecture

url_code: ""
url_pdf: ""
url_slides: ""
url_video: ""

authors: [admin, "rameez_malik", "enbai_ji"]

# Slides (optional).
slides: ""
---

## Problem

Beyond geostationary orbit, Earth GNSS signals arrive weak, sparse and from a poor geometry; ground
tracking is a scarce, contested resource with light-time delay attached; and the lunar south pole —
where the missions are going — is among the hardest regions to cover. Without an architecture that
holds accuracy autonomously, every landing, rendezvous and surface operation waits on a deep-space
tracking slot.

## Capability

My research group design navigation architectures for cislunar space and evaluate what accuracy they
can sustain, treating constellation geometry, inter-satellite links and time synchronisation as one
coupled problem rather than three. The estimation work underneath: higher-order and square-root
unscented estimators, factor graph optimisation for orbit determination and time synchronisation, and
station-keeping models that make long-horizon constellation studies tractable.

## Demonstrated result

- **Autonomous orbit determination to approximately 11 m in 3-D position and 1.58 mm/s in velocity**
  using one-way range and range-rate inter-satellite links between three evenly phased relay satellites
  in distant retrograde orbits and navigation satellites in elliptical lunar frozen orbits, with no
  direct ground support to the navigation satellite (CR3BP case). Under a high-fidelity dynamical model,
  a two-day initial ground-tracking handover followed by inter-satellite tracking alone yielded
  approximately 1 km in position and 10 mm/s in velocity. Validated with Monte Carlo runs and NEES/NIS
  consistency checks. [Enbai Ji](/authors/enbai_ji/), MPhil thesis, UNSW Sydney, 2025:
  [*Autonomous Orbit Determination of Lunar Navigation Satellites Based on Inter-Satellite Links*](https://unsworks.unsw.edu.au/entities/publication/ef9a27ce-1bee-4219-972b-b3f8d3db42b6).
- **A lunar navigation constellation optimised for targeted south-pole coverage**, combining
  high-fidelity propagation, a semi-analytical station-keeping model and Earth-GPS integration for time
  synchronisation and ephemeris generation. [Rameez A. Malik](/authors/rameez_malik/) and Yang Yang,
  [*Lunar navigation system optimization for targeted coverage with semi-analytical station keeping model and Earth-GPS integration*](https://www.sciencedirect.com/science/article/pii/S0094576525007465),
  *Acta Astronautica* **239**, 278–293 (February 2026).
- **HALO, a high-precision analyser for lunar orbits**, presented at the Australian Space Research
  Conference ([slides](/slides/High-precision_Analyser_for_Lunar_Orbits%20(HALO)_DrYYang.pdf)).
- **Factor graph optimisation for lunar orbit determination and time synchronisation**, presented in the
  Lunar Navigation session at PNT 2026.

## External use

The work is funded as **ARC Discovery Project DP260100821** with Professor Andrew Dempster (UNSW ACSER,
lead chief investigator) and Professor Junichiro Kawaguchi. Its stated outcomes — single-satellite
Doppler positioning deployable ahead of full PNT infrastructure, autonomous on-board positioning, and
time synchronisation for lunar PNT satellites — are targeted at Australia's robotic lunar mission and at
Australia's national lunar PNT capability.

## Next partnership opportunity

A **cislunar and lunar PNT trade study** on your mission geometry: a coverage and accuracy budget across
the regimes you nominate, and an architecture recommendation with every assumption written down. See
[Partner with us](/partner/).
