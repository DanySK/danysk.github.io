---
title: "A Field-Based Approach for Runtime Replanning in Swarm Robotics Missions"
date: "2025-09-01"
jobDate: 2025
work: [2025 IEEE International Conference on Autonomic Computing and Self-Organizing Systems (ACSOS)]
designs: [Gianluca Aguzzi, Martina Baiardi, Angela Cortecchia, Branko Miloradovic, Alessandro Papadopoulos, Danilo Pianini, Mirko Viroli]
thumbnail: 2025-acsos-swarm-replanning/thumb.png
projectUrl: https://doi.org/10.1109/ACSOS66086.2025.00017
---

🏆 **Best Student Paper — ACSOS 2025**

#### Abstract

Ensuring mission success for multi-robot systems operating in unpredictable environments
requires robust mechanisms to react to unpredictable events,
such as robot failures, by adapting plans in real-time.
Adaptive mechanisms are especially needed for large teams deployed in areas with unreliable network infrastructure,
for which centralised control is impractical and where network segmentation is frequent.

This work advances the state of the art by proposing a field-based runtime replanning approach
grounded in aggregate programming.
Through this paradigm,
the mission and the environment are represented by continuously evolving fields,
enabling robots to make decentralised decisions and collectively adapt the ongoing plan.

The proposed approach is compared with a simple late-stage replanning strategy
and an oracle-supported centralised continuous replanner.
Experimental evidence shows that the proposed approach achieves performance close to the oracle
when communication range is sufficient,
while significantly outperforming the baseline even under sparse communication,
and scaling well with the number of robots.
