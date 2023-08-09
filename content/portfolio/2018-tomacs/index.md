---
title: Engineering Resilient Collective Adaptive Systems by Self-Stabilisation
date: "2018-04-01"
jobDate: 2018
work: [ACM Transactions on Modeling and Computer Simulation]
#techs: [ protelis ]
designs: [Mirko Viroli, Giorgio Audrito, Jacob Beal, Ferruccio Damiani, Danilo Pianini]
thumbnail: 2018-tomacs/thumb.png
projectUrl: https://dx.doi.org/10.1145/3177774
# testimonial:
#   name: John Doe
#   role: CEO @Example
#   image: sample-project/john.jpg
#   text: Prow scuttle parrel provost Sail ho shrouds spirits boom mizzenmast yardarm. Pinnace holystone mizzenmast quarter crow's nest nipperkin
---

Collective adaptive systems are an emerging class of networked computational systems particularly suited for application domains such as smart cities, complex sensor networks, and the Internet of Things. These systems tend to feature large-scale, heterogeneity of communication model (including opportunistic peer-to-peer wireless interaction) and require inherent self-adaptiveness properties to address unforeseen changes in operating conditions. In this context, it is extremely difficult (if not seemingly intractable) to engineer reusable pieces of distributed behaviour to make them provably correct and smoothly composable. Building on the field calculus, a computational model (and associated toolchain) capturing the notion of aggregate network-level computation, we address this problem with an engineering methodology coupling formal theory and computer simulation. On the one hand, functional properties are addressed by identifying the largest-to-date field calculus fragment generating self-stabilising behaviour, guaranteed to eventually attain a correct and stable final state despite any transient perturbation in state or topology and including highly reusable building blocks for information spreading, aggregation, and time evolution. On the other hand, dynamical properties are addressed by simulation, empirically evaluating the different performances that can be obtained by switching between implementations of building blocks with provably equivalent functional properties. Overall, our methodology sheds light on how to identify core building blocks of collective behaviour and how to select implementations that improve system performance while leaving overall system function and resiliency properties unchanged.
