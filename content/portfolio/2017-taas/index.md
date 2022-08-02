---
title: Self-Adaptation to Device Distribution in the Internet of Things
date: "2017-09"
jobDate: 2017
work: [ACM Transactions on Autonomous and Adaptive Systems]
#techs: [ protelis ]
designs: [Mirko Viroli, Giorgio Audrito, Jacob Beal, Ferruccio Damiani, Danilo Pianini]
thumbnail: 2017-taas/thumb.png
projectUrl: https://dx.doi.org/10.1145/3105758
# testimonial:
#   name: John Doe
#   role: CEO @Example
#   image: sample-project/john.jpg
#   text: Prow scuttle parrel provost Sail ho shrouds spirits boom mizzenmast yardarm. Pinnace holystone mizzenmast quarter crow's nest nipperkin
---

A key problem when coordinating the behaviour of spatially situated networks, like those typically found in the Internet of Things (IoT), is adaptation to changes impacting network topology, density, and heterogeneity. Computational goals for such systems, however, are often dependent on geometric properties of the continuous environment in which the devices are situated rather than the particulars of how devices happen to be distributed through it. In this article, we identify a new property of distributed algorithms, eventual consistency, which guarantees that computation converges to a final state that approximates a predictable limit, based on the continuous environment, as the density and speed of devices increases. We then identify a large class of programs that are eventually consistent, building on prior results on the field calculus computational model that identify a class of self-stabilizing programs. Finally, we confirm through simulation of IoT application scenarios that eventually consistent programs from this class can provide resilient behavior where programs that are only converging fail badly.
