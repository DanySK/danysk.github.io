---
title: Runtime Load-Shifting of Distributed Controllers Across Networked Devices
date: "2023-06-10"
jobDate: 2023
work: [DAIS 2023 - 23rd International Conference on Distributed Applications and Interoperable Systems]
#techs: [ protelis ]
designs: [Nicolas Farabegoli, Danilo Pianini, Roberto Casadei, Mirko Viroli]
thumbnail: 2024-fgcs-pulverization/thumb.png
projectUrl: https://doi.org/10.1016/j.future.2024.07.042
# testimonial:
#   name: John Doe
#   role: CEO @Example
#   image: sample-project/john.jpg
#   text: Prow scuttle parrel provost Sail ho shrouds spirits boom mizzenmast yardarm. Pinnace holystone mizzenmast quarter crow's nest nipperkin
---

#### Abstract

In recent years, the infrastructure supporting the execution of situated distributed computations evolved at a fast pace.
Modern collective adaptive applications – as found in the Internet of Things, swarm robotics, and social computing –
are designed to be executed on very diverse devices and to be deployed on infrastructures composed of devices ranging
from cloud servers to wearable devices,
constituting together a cloud–edge continuum.
The availability of such an infrastructure opens to better resource utilisation and performance but, at the same time,
introduces new challenges to software designers,
as applications must be conceived to be able to adapt to changing deployment domains and conditions.
In this paper, we introduce a practical framework for the development of systems based on the concept of pulverisation,
meant to neatly separate business logic and deployment concerns, allowing applications to be defined
independently of the infrastructure they will execute upon, thus supporting scalability.
The framework is based on a domain-specific language capturing, in a declarative fashion:
pulverised application components, device capabilities, resource allocation, and (runtime re-) configuration policies.
The framework, implemented in Kotlin multiplatform and available as open source,
is then evaluated in a small-scale real-world demo and in a city-scale simulated scenario,
demonstrating the feasibility of the approach and its potential benefits
in achieving better trade-offs between performance and resource utilisation.

#### [Demo](https://github.com/nicolasfara/experiments-2024-fgcs-pulverization-local-reconfiguration/)
#### [Framework](https://github.com/pulvreakt/pulvreakt)
