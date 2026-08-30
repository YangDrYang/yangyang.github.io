---
title: Optical Tracking and Observatory Automation
summary: Turning a heritage university telescope into a taskable sensor, and marginal optical tracks into orbit solutions with honest uncertainty.
tags:
  - Space Tracking
  - Space Situational Awareness
date: "2024-10-01T00:00:00Z"
weight: 10  # Controls order in the homepage portfolio (low first).
external_link:
authors: [admin, "asad_rizvi"]
image:
  caption: Observatory automation and remote control
  focal_point: Smart
---

## Problem

Ground-based optical tracking is the cheapest way to keep custody of objects in high orbits, and the
hardest data to work with. Passes are short, gaps run to days, and the objects that matter most are
often close to the detection limit. An orbit fitted to that data can look precise and still be wrong,
because the reported covariance reflects the fit rather than the observation geometry that produced it.

## Capability

My team develop the full path from photons to orbit solutions: image processing that pulls astrometry from
faint and streaked detections, association and initial orbit determination for short arcs, and
estimation that propagates realistic uncertainty rather than an optimistic fit residual.

Alongside this, the UNSW Observatory has been automated for remote and programmatic operation, so
tracking can be tasked against a target list instead of scheduled by hand.

Satellite polarimetry extends the same sensor from tracking towards object characterisation —
inferring attitude and surface properties, not just position. This is the ongoing PhD project of
[Asad Rizvi](/authors/asad_rizvi/), and it is at an earlier stage than the tracking and automation
work above: the observing approach is being developed on the UNSW telescope, with research outputs
still to come.

{{< img src="fav1.jpg" box="640x720" caption="The UNSW Observatory telescope on its equatorial mount, with control computer, guide scope and imaging camera fitted." >}}

## Demonstrated result

- **The UNSW Observatory now runs automated, remotely controlled satellite tracking.** The automation
  and control work was delivered as an undergraduate thesis project by Tejas Margapuram
  ([slides](/slides/Observatory_Automation_and_Remote_Control.pdf)).
- **A modular three-tier control system now drives the observatory**, designed, implemented and
  deployed by undergraduate thesis student Darcy Faulkes: an ASCOM Alpaca server abstracting
  heterogeneous hardware, a backend for visibility prediction, scheduling and orchestration, and a web
  frontend. Remote control was verified against third-party clients, and **a complete satellite
  observation was carried out autonomously, with no human intervention**.
- **An end-to-end optical space surveillance and tracking pipeline** runs from raw frames to orbit
  solutions ([overview slides](/slides/Optical_SST_Pipeline_DrYYang.pdf)).
- **An automated satellite tracking control project was funded** by the NSW Space Research
  Network for 2025–2026.
- **Astrometric analysis of satellite streak images** was developed end to end as a supervised thesis
  project, extending the pipeline's usable detection range.

<!-- TODO: add the observatory's instrument specifications — aperture, sensor, limiting magnitude,
     achieved astrometric accuracy, and objects trackable per night. These are the numbers a partner
     evaluating a tracking campaign will ask for first. -->

{{< img src="fav2.png" box="1100x640" caption="The observatory tasking interface: satellites predicted to be visible on a given night, with sky track and altitude profile for the selected object and one-click schedule capture. This is the top tier of a three-tier architecture built by undergraduate thesis student **Darcy Faulkes** — an ASCOM Alpaca server abstracting the observatory's heterogeneous hardware, a backend handling visibility prediction, scheduling and orchestration, and this web frontend." >}}

## External use

The observatory is used for research and for space engineering education at UNSW, and it is the sensor
behind the tracking pilot offered to partners. 

<!-- TODO: name any external organisation already receiving tracking data or products, if that can be
     stated publicly. -->

## Next partnership opportunity

A **tracking campaign** against objects you nominate, returning astrometry, orbit solutions and a
residual and accuracy report — enough to judge whether a taskable optical sensor belongs in your
architecture. See [Partner with us](/partner/).
