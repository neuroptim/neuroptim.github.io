---
layout: tool
title: "NEVO: Neuromorphic EVolutionary Optimisation"
image: /assets/images/logos/nevo-logo.png
category: framework
description: "NEVO uses a Nengo-simulated Basal Ganglia circuit to adaptively select optimisation operators at runtime, bridging neuromorphic computing with metaheuristic search."
version: "0.1.0"
status: active
license: BSD 3-Clause Clear License
github: https://github.com/jcrvz/nevo
documentation: https://jcrvz.github.io/nevo
install: "pip install nevo"
tags:
  - Nengo
  - Basal Ganglia
  - Neuromorphic
  - Optimisation
  - Evolutionary Computation
  - TD Learning
  - Python
order: 1
---

NEVO (**N**euromorphic **EV**olutionary **O**ptimisation) uses a Nengo-simulated Basal Ganglia (BG) circuit to adaptively select optimisation operators at runtime. The search loop is:

## Overview

NEVO implements adaptive heuristic-based optimisation using neuromorphic computing principles. The framework uses spiking neural networks to dynamically select and coordinate optimisation operators based on the current search state, mimicking action selection in the mammalian brain via a Winner-Take-All (WTA) via a Cortico-Basal Ganglia-Thalamic Loop (CBGTL) circuit.

## Features

- **Brain-inspired operator selection** via a Nengo Basal Ganglia and Thalamus network.
- **13 traditional operators** from well-known metaheuristics (Lévy Flight, Differential Evolution, Particle Swarm, Spiral Optimisation, Firefly, Genetic Crossover/Mutation, Simulated Annealing, Tabu Search, and more).
- **Neuromorphic operator modes**: `trad`, `nm_dual` (hard WTA with LIF ensembles), and `nm_softmix` (Beta-distribution blending).
- **Temporal Difference (TD) learning** with swappable learning rules (`SimpleTD`, `DecayingTD`, `ConservativeTD`, `AdaptiveTD`) and value models.
- **State-aware selection**: 3D feature vector (diversity, improvement rate, convergence) governs utility functions per operator.
- **Competitive memory** archive with rank-weighted centroid computation.
- **Rich probes** for time-series analysis of fitness, operator selection, and state features.
- **Loihi-compatible design**: All Nengo constructs support direct compilation to neuromorphic hardware.

## Installation

```bash
# From source (recommended)
git clone https://github.com/jcrvz/nevo.git
cd nevo
pip install -e .

# Using uv
uv pip install -e .
uv pip install -e . --extra dev   # includes dev and docs dependencies
```

> PyPI release coming soon: `pip install nevo`

**Requirements:** Python >= 3.10, `nengo >= 4.1`, `numpy >= 1.20,< 2.0`, `ioh >= 0.3.18`
