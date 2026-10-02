# Entropy-Aware Routing for Disorder Minimization

An experimental routing framework that uses traffic disorder to make routing decisions under dynamic and adversarial network conditions.

## Overview

Traditional shortest-path routing focuses mainly on distance or hop count. This project explores whether routing can be improved by considering **traffic instability** as an additional routing factor.

The framework introduces an entropy-inspired disorder metric based on traffic variance and temporal changes, and uses it to assign weights to network edges.

The project compares:

- Traditional shortest-path routing
- Entropy-Aware Routing (EARA)

under simulated dynamic traffic and DDoS-style attack conditions.

## Key Features

- Entropy-inspired edge weighting
- Traffic variance and temporal-change analysis
- Dynamic traffic simulation
- DDoS-style attack simulation
- Attack exposure analysis
- Shortest-path vs. EARA comparison
- Longer-path analysis
- Capped vs. uncapped weighting analysis
- Multi-seed robustness testing
- Reproduction on multiple network datasets

## Results

The experiments showed that EARA can reduce routing exposure to attack-affected edges while keeping path lengths relatively close to conventional shortest-path routing.

The framework was tested on:

- Twitter social network
- Deezer Europe network

## Dataset

The experiments use publicly available network datasets.

The datasets are **not included in this repository**.

### Twitter

J. McAuley and J. Leskovec,  
*Learning to Discover Social Circles in Ego Networks*, NIPS 2012.

Dataset: https://snap.stanford.edu/data/ego-Twitter.html

### Deezer Europe

Rozemberczki and Sarkar,  
*Characteristic Functions on Graphs: Birds of a Feather, from Statistical Descriptors to Parametric Models*, 2020.

## Project Structure

```text
├── EARA (2).ipynb
├── EARA_Deezer_.ipynb
├── EARA_Deezer_results/
└── README.md
```

## Technologies

- Python
- NetworkX
- NumPy
- Pandas
- Matplotlib
- Jupyter Notebook

## Status

Research / experimental project.

The current implementation focuses on evaluating disorder-aware routing under controlled traffic and attack conditions.

## References
1. J. McAuley and J. Leskovec. Learning to Discover Social Circles in Ego Networks. NIPS, 2012.
2. Rozemberczki, B., & Sarkar, R. (2020). Characteristic functions on graphs: Birds of a feather, from statistical descriptors to parametric models. In Proceedings of the 29th ACM International Conference on Information and Knowledge Management (pp. 1325–1334). ACM. doi.org

