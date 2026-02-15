+++
# Display name
name = "Enbai Ji"

# Username (this should match the folder name)
authors = ["enbai_ji"]

# Force use of single template
type = "authors"
layout = "single"

# Is this the primary user of the site?
superuser = false

# Role/position
role = "MPhil Graduate"

# Organizations/Affiliations
organizations = [
  { name = "School of Mechanical and Manufacturing Engineering, UNSW Sydney", url = "https://www.unsw.edu.au" }
]

# Short bio (displayed in user profile at end of posts)
bio = "MPhil graduate specialising in autonomous orbit determination for lunar navigation satellites using inter-satellite link frameworks."

# List of user groups this user belongs to
user_groups = ["Alumni"]

# Weight for ordering within group (higher numbers appear later)
weight = 10

interests = ["Autonomous Orbit Determination", "Lunar Navigation Systems", "Inter-Satellite Links", "Cislunar PNT Infrastructure"]

# Education
education = [
  { course = "Master of Philosophy in Mechanical and Manufacturing Engineering", institution = "UNSW Sydney", year = "2025" },
]

# Thesis information
thesis_title = "Autonomous Orbit Determination of Lunar Navigation Satellites Based on Inter–Satellite Links"
+++

Enbai Ji is a recent MPhil graduate from the School of Mechanical and Manufacturing Engineering at UNSW Sydney. His research focused on developing autonomous orbit determination frameworks for lunar navigation satellites, contributing to the advancement of cislunar positioning, navigation and timing (PNT) infrastructure.

## Master's Thesis

**Title:** Autonomous Orbit Determination of Lunar Navigation Satellites Based on Inter–Satellite Links

**Abstract:** To support a future lunar navigation satellite system, this study proposes and validates an inter–satellite link (ISL)–centric framework for autonomous orbit determination. The simulation employs one–way range and range–rate satellite–to–satellite tracking (SST) between relay satellites in distant retrograde orbits (DROs) and navigation satellites in elliptical lunar frozen orbits (ELFOs), with a customised unscented Kalman filter that estimates their orbital and clock states without direct ground support to the navigation satellite. 

Performance is assessed under both a simplified circular restricted three–body problem (CR3BP) model and a high–fidelity dynamic model; first–order uncertainty from the relay satellite is introduced in the filter to improve its adaptability, robustness, consistency and hence overall estimation performance. Monte Carlo method and NEES/NIS checks are conducted for validations. 

In the CR3BP case, three evenly phased DRO relays substantially accelerate convergence and improve accuracy; the navigation satellite attains ~11 m 3–D position and 1.58 mm/s velocity accuracy, with position performance reaching that of the relays. In the high–fidelity case, two scenarios are examined: (i) a 2–day initial ground–tracking handover followed by SST only, and (ii) SST–only throughout, showing that the handover strategy expedites convergence and stabilises estimation, yielding ~1 km 3–D position and 10 mm/s velocity accuracy for the navigation satellite. 

Sensitivity analyses highlight the roles of measurement baseline, update interval, and filter tuning. Overall, the approach is feasible and scalable, laying groundwork for a resilient, autonomous cislunar positioning, navigation and timing (PNT) infrastructure and related deep–space missions.
