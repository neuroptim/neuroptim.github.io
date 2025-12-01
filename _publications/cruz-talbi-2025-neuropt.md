---
layout: publication
title: "NeurOptimisation: The Spiking Way to Evolve"
authors: "Cruz-Duarte, J.M. & Talbi, E-G."
year: 2025
month: 7
category: preprint
type: ArXiv Preprint
venue: "arXiv"
arxiv: "2507.08320"
tags:
  - Neuromorphic
  - Evolutionary Computing
  - Spiking Neural Network
  - Optimization
tldr: "A neuromorphic optimisation framework using spike-driven heuristics on Lava NC evaluated on continous optimisation problems."
---

## Abstract 

The increasing energy footprint of artificial intelligence systems urges alternative computational models that are both efficient and scalable. Neuromorphic Computing (NC) addresses this challenge by empowering event-driven algorithms that operate with minimal power requirements through biologically inspired spiking dynamics. We present the NeurOptimiser, a fully spike-based optimisation framework that materialises the neuromorphic-based metaheuristic paradigm through a decentralised NC system. The proposed approach comprises a population of Neuromorphic Heuristic Units (NHUs), each combining spiking neuron dynamics with spike-triggered perturbation heuristics to evolve candidate solutions asynchronously. The NeurOptimiser's coordination arises through native spiking mechanisms that support activity propagation, local information sharing, and global state updates without external orchestration. We implement this framework on Intel's Lava platform, targeting the Loihi 2 chip, and evaluate it on the noiseless BBOB suite up to 40 dimensions. We deploy several NeurOptimisers using different configurations, mainly considering dynamic systems such as linear and Izhikevich models for spiking neural dynamics, and fixed and Differential Evolution mutation rules for spike-triggered heuristics. Although these configurations are implemented as a proof of concept, we document and outline further extensions and improvements to the framework implementation. Results show that the proposed approach exhibits structured population dynamics, consistent convergence, and milliwatt-level power feasibility. They also position spike-native MHs as a viable path toward real-time, low-energy, and decentralised optimisation.