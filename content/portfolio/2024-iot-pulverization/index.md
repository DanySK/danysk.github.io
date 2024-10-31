---
title: "Dynamic IoT deployment reconfiguration: A global-level self-organisation approach"
date: "2024-10-28"
jobDate: 2024
work: [Internet of Things]
designs: [Nicolas Farabegoli, Danilo Pianini, Roberto Casadei, Mirko Viroli]
thumbnail: 2024-iot-pulverization/image.png
projectUrl: https://doi.org/10.1016/j.iot.2024.101412

---

#### Abstract

The edge-cloud continuum provides a heterogeneous, multi-scale, and dynamic infrastructure supporting complex deployment
profiles and trade-offs for application scenarios like those found in the Internet of Things
and large-scale cyber–physical systems domains.
To exploit the continuum, applications should be designed in a way that promotes flexibility and reconfigurability,
and proper management (sub-)systems should take care of reconfiguring them in response to changes in the environment
or non-functional requirements.
Approaches may leverage optimisation-based or heuristic-based policies,
and decision making may be centralised or distributed:
this work investigates decentralised heuristic-based approaches.
In particular, we focus on the pulverisation approach,
whereby a distributed software system is automatically partitioned (“pulverised”) into different deployment units.
In this context, we address two main research problems:
how to support the runtime reconfiguration of pulverised systems,
and how to specify decentralised reconfiguring policies by a global perspective.
To address the first problem,
we design and implement a middleware for pulverised systems separating infrastructural and application concerns.
To address the second problem, we leverage aggregate computing and exploit self-organisation patterns
to devise self-stabilising reconfiguration strategies.
By simulating deployments on different kinds of complex infrastructures,
we assess the flexibility of the pulverisation middleware design
as well as the effectiveness and resilience of the aggregate computing-based reconfiguration policies.

#### [Reproducible Experiments](https://github.com/nicolasfara/reconfiguration-experiments)
