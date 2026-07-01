---
layout: publication
title: "NEVO: A Neuromorphic EVolutionary Optimiser with Spike-Driven Cortico-Basal-Thalamic Coordination"
authors: "Cruz-Duarte, J.M. & Talbi, E-G."
year: 2026
month: 6
category: presentation, publication
type: Conference Talk
venue: "IEEE World Congress on Computational Intelligence (WCCI) 2026"
location: "Maastricht, Netherlands"
slides: "/assets/slides/wcci26-paper.pdf"
tags:
  - Neuromorphic
  - Evolutionary Computing
  - Spiking Neural Network
  - Optimization
tldr: "NEVO shows that spike-driven control can steer evolutionary optimisation effectively on simpler problems, while making clear what is needed to scale to higher dimensions."
---

## Abstract 

Neuromorphic computing and evolutionary computation share key properties, including distributed state, event-driven communication, and tolerance to finite precision. Nevertheless, optimisation control is rarely implemented directly in spiking dynamics. This paper introduces the Neuromorphic EVolutionary Optimiser (NEVO), in which evolutionary operator selection is realised as spike-driven action selection within a Cortico-Basal-Thalamic Loop (CBTL), whilst candidate generation and objective evaluation remain algorithmic under a standard black-box interface. NEVO is evaluated on the noiseless BBOB suite across 2D to 40D with 15 instances per function. Results show that spike-driven coordination sustains coherent operator sequences across problem landscapes, achieving successful target attainment in 2D and 3D, whilst exposing scalability limitations beyond 10D. These findings confirm that spike-driven coordination is feasible on neuromorphic substrates and clarify how neuromorphic action selection relates to existing adaptive operator selection strategies. The analysis also identifies concrete design requirements for future implementations.