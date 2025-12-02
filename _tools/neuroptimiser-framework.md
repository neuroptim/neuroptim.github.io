---
layout: tool
title: NeurOptimiser
image: https://avatars.githubusercontent.com/u/215023069?s=400&u=3f8b7bfe3e0c69e85b0f9bc5f6bea950305e4ea3&v=4
category: framework
description: NeurOptimiser is a neuromorphic optimisation framework in which metaheuristic search emerges from asynchronous spiking dynamics.
version: "1.0.2"
license: MIT
github: https://github.com/neuroptimiser/neuroptimiser
documentation: https://neuroptimiser.github.io
pypi: https://pypi.org/project/neuroptimiser/
install: pip install neuroptimiser
tags:
  - Lava
  - Neuromorphic
  - Optimization
  - Evolutionary Computation
  - Event-Driven
  - Python
order: 2
---

NeurOptimiser is a neuromorphic optimisation framework in which metaheuristic search emerges from asynchronous spiking dynamics.

## Overview

NeurOptimiser is a neuromorphic optimisation framework in which metaheuristic search emerges from asynchronous spiking dynamics. It defines optimisation as a decentralised process executed by interconnected Neuromorphic Heuristic Units (NHUs), each embedding a spiking neuron model and a spike-triggered heuristic rule.

This framework enables fully event-driven, low-power optimisation by integrating spiking computation with local heuristic adaptation. It supports multiple neuron models, perturbation operators, and network topologies.

## Features

- Modular and extensible architecture using Intel’s Lava.
- Supports linear and Izhikevich neuron dynamics.
- Implements random, fixed, directional, and Differential Evolution operators as spike-triggered perturbations.
- Includes asynchronous neighbourhood management, tensor contraction layers, and greedy selectors.
- Compatible with BBOB (COCO) suite.
- Designed for scalability, reusability, and future deployment on Loihi-class neuromorphic hardware.

## Quick Start

```python
from neuroptimiser import NeuroOptimiser
import numpy as np

problem_function    = lambda x: np.linalg.norm(x)
problem_bounds      = np.array([[-5.0, 5.0], [-5.0, 5.0]])

optimiser = NeurOptimiser()

optimiser.solve(
    obj_func=problem_function,
    search_space=problem_bounds,
    debug_mode=True,
    num_iterations=1000,
)
```

## Benchmarking

Neuroptimiser has been validated over the BBOB suite, showing:
- Competitive convergence versus Random Search
- Consistent results across function types and dimensions
- Linear runtime scaling with number of units and problem size
