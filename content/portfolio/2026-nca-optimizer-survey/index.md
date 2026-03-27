---
title: "First-order optimization algorithms: state of the art, classification, and performance: a practitioner's guide"
date: "2026-03-26"
jobDate: 2026
work: [Neural Computing and Applications]
designs: [Ruslan Shaiakhmetov, Danilo Pianini, Angelo Filaseta, Gabriele D'Angelo, Valter Venusti]
thumbnail: 2026-nca-optimizer-survey/thumb.png
projectUrl: https://doi.org/10.1007/s00521-026-12014-1
---

#### Abstract

Driven by the rising interest in machine learning techniques,
mathematical continuous optimization algorithms have made great progress.
Among them, first-order optimization algorithms,
which rely on the first derivative (gradient) to find a function's minimum or maximum,
have gained popularity due to their efficiency and scalability.
As a result, a vast number of optimization algorithms have been developed,
each applying different techniques and offering diverse guarantees.
This variety, while beneficial, makes selecting the most appropriate algorithm
a challenging yet crucial task—choosing the wrong one may lead to sub-par accuracy or performance.

This paper explores the state of the art in continuous first-order optimization algorithms,
offering guidance for selecting the most suitable method.
We classify 23 algorithms, detailing their dependency relationships,
theoretical foundations, and optimization strategies.
The analysis includes a performance evaluation using implementations in the PyTorch framework.
Convergence, quantified by the area under the training-loss curve,
is assessed with two benchmarks:
the Rosenbrock function as a standard test
and ResNet-18 training on the CIFAR-10 dataset as a practical test.
We evaluate performance using an integral metric
and analyze robustness to hyperparameter variations, including learning rate sensitivity.
Additionally, we introduce a classification of algorithm convergence behaviors.
These experiments provide insights into algorithm performance across varying problem complexities
and highlight their stability under hyperparameter changes.
Practitioners and researchers can use this work as a guide
to identify the set of most likely good candidates as first-order optimization algorithms for their use case.
