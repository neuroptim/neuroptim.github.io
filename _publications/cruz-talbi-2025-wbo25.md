---
layout: publication
title: "NeurOptimiser: A General Framework for Neuromorphic Optimisation"
authors: "Cruz-Duarte, J.M. & Talbi, E-G."
year: 2025
month: 8
category: presentation
type: Conference Talk
venue: "International Workshop on Big Optimization (WBO)"
location: "Catania, Italy"
slides: "/assets/slides/WBO25-lr.pdf"
tags:
  - Neuromorphic
  - Spiking Neural Network
  - Evolutionary Computing
  - Optimization
tldr: "Presentation on the NeurOptimiser framework, where spike-driven heuristics generate emergent metaheuristic search."
---

## Abstract

We present the NeurOptimiser, a spike-driven optimisation framework where metaheuristic search emerges from asynchronous neural dynamics. The architecture consists of distributed Neuromorphic Heuristic Units, each embedding a spiking neuron model with local decision rules and spike-triggered perturbation operators. Candidate solutions evolve through continuous neural states and discrete spike-induced transitions governed by fixed, random, directional, and Differential Evolution (DE) mechanisms. The framework supports linear and Izhikevich neuron models, multiple topologies, and dynamic encoding schemes. It is implemented using Intel's Lava and evaluated over the BBOB suite through three experiments addressing functionality, scalability, and runtime. Results show strong convergence, highlighting the efficacy of DE-based heuristics and demonstrating linear scaling with population size. Unlike previous methods that externalise decision-making, our approach embeds coordination and variation within the spiking substrate. It advances the recently proposed neuromorphic-based metaheuristic paradigm and provides a low-power, modular, and fully asynchronous alternative for neuromorphic optimisation.