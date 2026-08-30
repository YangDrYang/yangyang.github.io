+++
# Operational problems section (Blank widget).
widget = "blank"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 15  # Order that this section will appear.

title = "Operational problems I work on"
subtitle = "Four recurring failures in space operations, and the work that addresses each."

[design]
  # In the Blank widget this only selects the heading treatment: "1" renders the title,
  # subtitle and body together, left-aligned; anything else centres the title and subtitle
  # above a full-width, left-aligned body. It does not split the body into columns.
  columns = "2"
+++

**Your tracks are too sparse and too noisy to trust an orbit.** Short arcs, gaps of days between
passes, and faint objects near the detection limit produce orbit solutions whose covariance does not
reflect reality. I build estimation and image-processing pipelines that extract usable astrometry from
marginal data and report honest uncertainty alongside the state.
→ [Optical tracking and observatory automation](/project/optical-tracking/)

**A satellite moved and you found out late.** Distinguishing a genuine manoeuvre from mismodelled
dynamics or a bad track is the difference between a real custody break and a false alarm. I develop
manoeuvre-detection and pattern-of-life methods for geostationary and geosynchronous satellites, built
on labelled optical data rather than assumptions.
→ [Satellite manoeuvre detection](/project/space-object-characterisation/)

**Your mission goes where GNSS does not reach.** Beyond geostationary orbit and around the Moon,
Earth-based positioning degrades or disappears, and ground tracking is a scarce, expensive resource. I
design navigation architectures that hold accuracy autonomously — inter-satellite links, constellation
geometry, and time synchronisation treated as one problem.
→ [Lunar and cislunar navigation](/project/space-navigation/)

**You cannot say when it comes down, or what it belongs to.** Reentry timing and conjunction screening
both degrade when atmospheric density is modelled badly, and debris fragments arrive without a parent.
I work on reduced-order density models driven by real ephemerides, and on classifiers that reconnect
fragments to their breakup event.
→ [Reentry and density prediction](/project/thermospheric-density-reentry/)
