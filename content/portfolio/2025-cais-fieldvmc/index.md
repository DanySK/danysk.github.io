---
title: "FieldVMC: An Asynchronous Model and Platform for Self-organising Morphogenesis of Artificial Structures"
date: "2025-12-01"
jobDate: 2025
work: [Complex & Intelligent Systems]
designs: [Angela Cortecchia, Giovanni Ciatto, Roberto Casadei, Danilo Pianini]
thumbnail: 2025-cais-fieldvmc/thumb.png
projectUrl: https://doi.org/10.1007/s40747-025-02141-y
---

#### Abstract

In the field of evolutionary computing, the concept of Vascular Morphogenesis Controller (VMC)
has been proposed to model the growth of artificial structures over time,
stemming from a botanical metaphor of plant morphogenesis.
VMC entails a distributed and self-organising protocol where each node in a tree-shaped structure
is responsible for distributing resources to its children and collecting success towards its parent.

However, the original VMC model has known limitations:
it assumes a tree organisation structure and is implicitly synchronous.
These assumptions may induce abstraction gaps when VMC is used to model real-world systems,
and limit the applicability of the pattern to engineered morphogenetic systems.

To address these limitations, this work proposes *FieldVMC*:
a generalisation of the VMC model as a field-based computation,
in the spirit of the Aggregate Programming paradigm.
FieldVMC lifts the synchrony assumption and supports arbitrary network topologies,
while preserving the self-organising properties of the original model.
The approach is validated through simulation experiments demonstrating
self-construction, self-division, self-integration, self-segmentation, and self-optimisation of artificial structures.
