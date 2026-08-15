---
layout: publication
title: "A Spike-Driven Neuromorphic Framework for Asynchronous Population-Based Optimisation"
authors: "Cruz-Duarte, J.M. & Talbi, E-G."
year: 2026
month: 8
category: publication
type: Article
venue: "IEEE Transactions on Evolutionary Computation"
doi: "10.1109/TEVC.2026.3723682"
url: "ieeexplore.ieee.org/document/11655318"
tags:
  - Neuromorphic Computing
  - Evolutionary Algorithms
  - Spiking Neural Network
  - Neuromorphic Metaheuristics
  - Neuromorphic Metaheuristics
  - Event-Driven Asynchronous Optimization
tldr: "A neuromorphic optimisation framework using spike-driven heuristics on Lava NC evaluated on continous optimisation problems."
---

## Abstract 

The growing energy footprint of computational intelligence systems calls for approaches that are both efficient and scalable. Neuromorphic Computing (NC) addresses this challenge by allowing event-driven algorithms to operate with minimal power consumption through biologically inspired spiking dynamics. We present the NeurOptimiser, a fully spike-based optimisation framework that materialises the NC-based Metaheuristic (MH) paradigm via a decentralised system. This approach comprises a population of Neuromorphic Heuristic Units, each combining dynamic and spiking perturbation heuristics to asynchronously evolve candidate solutions. The NeurOptimiser's coordination arises via spike-driven communication and best-so-far reduction over shared channels, which admits both centralised and distributed realisations on neuromorphic backends. We implement this framework on Intel's Lava platform, targeting the Loihi 2 chip, and evaluate it on the noiseless BBOB suite up to 40D. We deploy several NeurOptimiser configurations, chiefly considering dynamic systems such as the Linear and Izhikevich models for neural dynamics, as well as fixed and Differential Evolution mutation operators for spike-triggered heuristics. These instantiations serve as concrete demonstrations of the framework rather than as exhaustive enhancements to optimisers. The primary contribution is the framework itself, together with the formal foundations, implementation, and empirical validation that establish its feasibility. Results show structured population dynamics and consistent best-so-far improvements, along with upper bounds on Loihi-class power derived from per-operation energy costs.