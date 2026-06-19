---
layout: tool
title: NEVO Dataset
image: https://about.zenodo.org/static/img/logos/zenodo-gradient-square.svg
category: dataset
description: "Codes and experimental results for NEVO, a neuromorphic evolutionary optimiser with spike-driven Cortico-Basal-Thalamic coordination, evaluated on the BBOB benchmark suite."
version: "v2"
status: active
license: BSD 3-Clause Clear License
github: "https://github.com/jcrvz/nevo"
documentation: "https://jcrvz.github.io/nevo"
zenodo: "https://zenodo.org/records/19188034"
citation: "Cruz-Duarte, J. M., & Talbi, E.-ghazali. (2026). NEVO: A Neuromorphic EVolutionary Optimiser with Spike-Driven Cortico-Basal-Thalamic Coordination - Codes and Results [Data set]. 2026 IEEE Congress on Evolutionary Computation at the 2026 IEEE World Congress on Computational Intelligence (WCCI/CEC), Maastricht, NL. Zenodo. https://doi.org/10.5281/zenodo.19188034"
tags: [Dataset, Neuromorphic Optimisation, Evolutionary Computation, Spiking Neural Networks, Cortico-Basal-Thalamic Loop, BBOB, Nengo]
order: 5
---

This repository contains code, datasets, and analysis artefacts generated from experiments conducted with the NEVO framework.

## About This Dataset

This Zenodo repository serves exclusively for **reproducibility**, providing:

- Raw experimental data from all performed benchmark runs
- Experimental configurations and parameter files
- Scripts and processing routines used to generate the experimental figures and tables reported in the paper

The complete experiments evaluate NEVO on the **BBOB noiseless benchmark suite** (24 functions, 6 dimensions, 15 instances), with operator coordination implemented through spike-driven Cortico-Basal-Thalamic Loop (CBTL) dynamics.

## Contents

### Datasets

| File | Description |
|------|-------------|
| `exdata.zip` | Raw experimental data from full BBOB runs in CocoEx format |
| `ppdata.zip` | Postprocessed benchmark data and analysis artefacts |
| `cocoex-complementary.zip` | Complementary COCO metrics, summaries, and publication figures |
| `preliminary-figures.zip` | Preliminary visualisation outputs from the basic experiment |

### Scripts

| File | Description |
|------|-------------|
| `nevo-main.zip` | Complete NEVO implementation with core optimiser, operators, and benchmark scripts (frozen version, for reproducibility) |
| `basic_example.py` | Example script for preliminary validation figures |
| `benchmark_experiment.py` | Script used to execute full BBOB benchmark experiments |

## How to Use

The experiments can be reproduced by extracting the code package and running the benchmark script:

```bash
python benchmark_experiment.py
```

## Full Framework

The complete [NEVO](/tools/nevo-framework/) framework implementation is available and maintained at the [GitHub repository](https://github.com/jcrvz/nevo).

## Citation

```bibtex
@dataset{Cruz2026nevo-dataset,
    author       = {Cruz-Duarte, Jorge M. and Talbi, El-ghazali},
    title        = {NEVO: A Neuromorphic EVolutionary Optimiser with Spike-Driven Cortico-Basal-Thalamic Coordination - Codes and Results},
    year         = 2026,
    publisher    = {Zenodo},
    version      = {v2},
    doi          = {10.5281/zenodo.19188034},
    url          = {https://doi.org/10.5281/zenodo.19188034},
}
```