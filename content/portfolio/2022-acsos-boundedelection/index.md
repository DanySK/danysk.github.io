---
title: Self-stabilising Priority-Based Multi-Leader Election and Network Partitioning
date: "2022-10-01"
jobDate: 2022
work: [2022 IEEE International Conference on Autonomic Computing and Self Organizing Systems (ACSOS)]
#techs: [ protelis ]
designs: [Danilo Pianini, Roberto Casadei, Mirko Viroli]
thumbnail: 2022-acsos-boundedelection/boundedelection.gif
projectUrl: https://doi.org/10.1109/ACSOS55765.2022.00026
# testimonial:
#   name: John Doe
#   role: CEO @Example
#   image: sample-project/john.jpg
#   text: Prow scuttle parrel provost Sail ho shrouds spirits boom mizzenmast yardarm. Pinnace holystone mizzenmast quarter crow's nest nipperkin
---

#### [Slides](https://danysk.github.io/Slides-2022-ACSOS-BoundedElection/)

#### Abstract

A common task in situated distributed systems is the self-organising election of leaders. These leaders can be devices or software agents appointed, for instance, to coordinate the activities of other agents or processes. In this work, we focus on the multi-leader election problem in networks of asynchronous message-passing devices, which are a common model in self-organisation approaches like aggregate computing. Specifically, we introduce a novel algorithm for space- and priority-based leader election and compare it with the state of the art. We call the algorithm Bounded Election since it leverages bounding (i.e. minimisation or maximisation) of candidacy messages to drop or promote candidate leaders and ensure stabilisation. The proposed algorithm is formally proven to be self-stabilising, allows for leader prioritisation, and performs on-the-fly network partitioning (namely, as a side effect of the leader election process, the areas regulated by the leaders are also established). Also, we experimentally compare its performance together with the state of the art of leader election in aggregate computing in a variety of synthetic scenarios, showing benefits in terms of convergence time and resilience.
