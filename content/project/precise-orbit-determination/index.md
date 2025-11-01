---
title: Precise Orbit Determination Using Advanced Filtering
summary: Development of robust orbit determination algorithms using higher-order unscented Kalman estimators for enhanced tracking of low Earth orbit satellites.
tags:
  - POD
  - Orbit Determination
  - HOUSE
  - Space Tracking
date: "2024-04-27T00:00:00Z"
draft: true

# Optional external URL for project (replaces project detail page).
external_link:

image:
  caption: Precision orbit determination workflow
  focal_point: Smart

links:
  - icon: github
    icon_pack: fab
    name: HOUSE Implementation
    url: https://github.com/YangDrYang/orbDetHOUSE
  - icon: external-link-alt
    icon_pack: fas
    name: IEEE Paper
    url: https://doi.org/10.1109/TAES.2024.3423851

authors: [admin]
---

## Project Overview

This research project focuses on developing advanced orbit determination techniques using the novel Higher-Order Unscented Kalman Estimator (HOUSE) framework. The work addresses critical challenges in space surveillance and tracking, particularly for satellites in low Earth orbit (LEO).

## Key Achievements

### Square-Root HOUSE (w-HOUSE) Development
Our breakthrough research has led to the development of the w-HOUSE filter, which represents a significant advancement in nonlinear filtering for orbit determination applications. This work was published in **IEEE Transactions on Aerospace and Electronic Systems** in 2024.

### Performance Improvements
The w-HOUSE filter demonstrates:
- **Superior Accuracy**: 3D root-mean-square errors of less than 60 metres over three-day tracking scenarios
- **Enhanced Robustness**: Better handling of outlier-contaminated measurements compared to traditional methods
- **Computational Efficiency**: Square-root formulation ensures numerical stability

## Technical Approach

### Challenges Addressed
- **Limited Measurement Time**: Short visible arcs from ground-based optical tracking
- **Non-Gaussian Data**: Presence of outliers in observational data
- **Nonlinear Dynamics**: Highly perturbative orbit dynamics in LEO environment
- **Sparse Observations**: Irregular measurement availability

### Methodology
1. **Higher-Order Unscented Transformation**: Enhanced sigma point selection for better nonlinear approximation
2. **Square-Root Implementation**: Improved numerical stability and computational efficiency
3. **Robust Parameter Estimation**: Advanced techniques for handling measurement uncertainties
4. **Multi-Sensor Integration**: Fusion of angle-only measurements with other sensor data

## Validation and Results

### Real-World Testing
The algorithm has been validated using:
- **Synthetic Datasets**: Comprehensive Monte Carlo simulations
- **Real Measurements**: Optical tracking data from Sentinel-6A satellite
- **Comparative Analysis**: Performance benchmarking against UKF, CUT filters, and precise GNSS-based solutions

### Performance Metrics
- Positioning accuracy: **< 60m RMS error** over 3 days
- Robustness to outliers: **30% improvement** over traditional methods
- Computational efficiency: **Real-time capable** implementation

## Applications

This research has direct applications in:
- **Space Situational Awareness**: Enhanced tracking of space debris and active satellites
- **Mission Operations**: Improved spacecraft navigation and collision avoidance
- **Scientific Missions**: Precise orbit determination for Earth observation satellites
- **Commercial Space**: Supporting the growing commercial satellite industry

## Code Availability

The implementation of the HOUSE algorithms is available on GitHub, supporting reproducible research and enabling the space community to benefit from these advances.

## Future Work

Ongoing developments include:
- Extension to higher-altitude orbits
- Multi-object tracking capabilities
- Integration with machine learning approaches
- Real-time implementation on space-qualified hardware
