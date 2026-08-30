---
title: "Thermospheric Density and Reentry Prediction"
summary: "Cutting the dominant error source in low-Earth-orbit prediction by learning reduced-order density models from real ephemerides."
tags:
  - Space Situational Awareness
  - Astrodynamics
date: "2025-06-01T00:00:00Z"
weight: 50  # Controls order in the homepage portfolio (low first).
draft: false

external_link: ""

authors: [admin, "ruoyan_zhao"]

image:
  caption: "Reduced-order thermospheric density modelling for reentry prediction"
  focal_point: "Smart"
---

## Problem

Below about 600 km, atmospheric drag dominates the error budget, and drag is only as good as the
density model behind it. JB2008, NRLMSIS 2.1 and DTM2020 disagree with each other and with reality,
worst during geomagnetic storms. Reentry windows stay wide until late, and conjunction screening
inherits the same uncertainty.

## Capability

Reduced-order density modelling calibrated against real orbital behaviour rather than against another
model: Starlink ephemerides assimilated through an Unscented Kalman Filter, comparing linear (POD with
DMDc) and nonlinear (diffusion maps with m-PCE) reduction, each initialised from the three empirical
baselines. The aim is a model fast enough for operational tracking and space traffic management.

## Demonstrated result

**Early stage — no published accuracy figure yet.** The framework and assimilation pipeline are built
and running as MPhil research by [Ruoyan (Arthur) Zhao](/authors/ruoyan_zhao/); the comparison against
the baselines is in progress.

<!-- TODO: once the comparison is complete, state the headline result here — improvement in density
     accuracy or in reentry epoch prediction, against which baseline, over which period. Until then this
     section deliberately claims nothing. -->

## External use

Density error is the shared root cause behind wide reentry windows and weak conjunction screening, and
it degrades orbit determination for the tracking and manoeuvre-detection work on this site.

## Next partnership opportunity

Calibrating the model against your tracking or ephemeris data, or applying it to a specific reentry
problem. Best suited to a co-funded or sponsored project while the method matures — see
[Partner with us](/partner/).
