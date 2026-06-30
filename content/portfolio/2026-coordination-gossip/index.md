---
title: "A Self-stabilizing Min-Max Consensus via Path-Loop Detection"
date: "2026-06-21"
jobDate: 2026
work: [Coordination Models and Languages (Lecture Notes in Computer Science 16590)]
designs: [Angela Cortecchia, Danilo Pianini, Mirko Viroli]
thumbnail: 2026-coordination-gossip/gossip.gif
projectUrl: https://doi.org/10.1007/978-3-032-28358-0_5
---

#### Abstract

In large-scale distributed systems, such as the Internet of Things (IoT), min-max consensus algorithms provide a mechanism for collective coordination by enabling nodes to converge on a “best” value produced by one of the participants in the computation. However, min-max consensus algorithms are monotonic and non-self-stabilizing by nature: once a value is merged into the aggregate it cannot be retracted, leading to propagation of stale or incorrect data in the presence of transient faults or topology changes. In this work, we propose a novel self-stabilizing min-max consensus algorithm ensuring convergence to the best available value in the network by propagating information along shortest valid paths. Each gossip message carries a value and path of nodes that have acknowledged it, enabling loop-freedom and natural pruning of obsolete contributions. We rely on field-based coordination and specifically the Aggregate Computing paradigm to present the algorithm, prove self-stabilization, and provide an implementation as a reusable library for the *Collektive* DSL. This work contributes a foundational building block for resilient coordination in pervasive computing systems, paving the way to more complex, self-stabilizing distributed applications.

#### [Slides and interactive playground](https://danysk.github.io/slides-2026-coordination-gossip/#/)
